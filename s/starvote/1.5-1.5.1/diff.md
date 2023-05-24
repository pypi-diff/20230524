# Comparing `tmp/starvote-1.5.tar.gz` & `tmp/starvote-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-1.5.tar` & `starvote-1.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.5/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.5/LICENSE
--rw-r--r--   0        0        0    12183 2023-05-22 07:33:51.854171 starvote-1.5/README.md
--rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.5/example.py
--rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.5/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-21 11:19:31.211412 starvote-1.5/sample_polls/README.md
--rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.5/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
--rw-r--r--   0        0        0      321 2023-05-21 14:36:07.812513 starvote-1.5/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.5/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
--rw-r--r--   0        0        0      412 2023-05-21 14:36:10.524536 starvote-1.5/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
--rw-r--r--   0        0        0      226 2023-05-21 13:55:36.270675 starvote-1.5/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.csv
--rw-r--r--   0        0        0      883 2023-05-21 14:46:04.809533 starvote-1.5/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.result.txt
--rw-r--r--   0        0        0      226 2023-05-21 13:52:36.109138 starvote-1.5/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.csv
--rw-r--r--   0        0        0      390 2023-05-21 14:45:20.721162 starvote-1.5/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.result.txt
--rw-r--r--   0        0        0     4689 2023-05-22 05:48:56.428345 starvote-1.5/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.csv
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-1.5/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.html
--rw-r--r--   0        0        0      520 2023-05-22 07:23:43.629054 starvote-1.5/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.5/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      340 2023-05-21 14:36:12.440552 starvote-1.5/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.5/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
--rw-r--r--   0        0        0      234 2023-05-21 14:36:15.004573 starvote-1.5/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
--rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.5/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
--rw-r--r--   0        0        0      267 2023-05-21 14:36:17.328593 starvote-1.5/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.5/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      374 2023-05-21 14:36:20.268617 starvote-1.5/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.5/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv
--rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.5/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf
--rw-r--r--   0        0        0     2642 2023-05-21 14:36:26.092666 starvote-1.5/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.5/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.5/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf
--rw-r--r--   0        0        0      961 2023-05-21 14:36:28.876690 starvote-1.5/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.5/sample_polls/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.5/sample_polls/starvote_ballots_best_akali_skins.result.pdf
--rw-r--r--   0        0        0      876 2023-05-21 14:36:32.040716 starvote-1.5/sample_polls/starvote_ballots_best_akali_skins.result.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.5/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.5/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf
--rw-r--r--   0        0        0     2418 2023-05-21 14:36:34.744739 starvote-1.5/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.5/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.5/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf
--rw-r--r--   0        0        0     1091 2023-05-21 14:36:37.344761 starvote-1.5/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.5/sample_polls/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.5/sample_polls/starvote_ballots_presidential_candidates.result.pdf
--rw-r--r--   0        0        0      408 2023-05-21 14:36:39.896782 starvote-1.5/sample_polls/starvote_ballots_presidential_candidates.result.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.5/sample_polls/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.5/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf
--rw-r--r--   0        0        0      419 2023-05-21 14:36:42.084801 starvote-1.5/sample_polls/starvote_ballots_presidential_poll_july_2020.result.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.5/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.5/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf
--rw-r--r--   0        0        0      961 2023-05-21 14:36:44.284819 starvote-1.5/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.5/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.5/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf
--rw-r--r--   0        0        0      377 2023-05-21 14:36:46.788840 starvote-1.5/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.txt
--rw-r--r--   0        0        0    22471 2023-05-22 07:31:28.876968 starvote-1.5/starvote/__init__.py
--rw-r--r--   0        0        0       84 2023-05-21 14:27:54.116361 starvote-1.5/starvote/__main__.py
--rw-r--r--   0        0        0     2689 2023-05-22 07:33:13.241846 starvote-1.5/tests/run_tests.py
--rw-r--r--   0        0        0    12601 1970-01-01 00:00:00.000000 starvote-1.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.5.1/LICENSE
+-rw-r--r--   0        0        0    12872 2023-05-24 18:58:45.035781 starvote-1.5.1/README.md
+-rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.5.1/example.py
+-rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-21 11:19:31.211412 starvote-1.5.1/sample_polls/README.md
+-rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
+-rw-r--r--   0        0        0      321 2023-05-21 14:36:07.812513 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
+-rw-r--r--   0        0        0      412 2023-05-21 14:36:10.524536 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0      226 2023-05-21 13:55:36.270675 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.csv
+-rw-r--r--   0        0        0      883 2023-05-21 14:46:04.809533 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.result.txt
+-rw-r--r--   0        0        0      226 2023-05-21 13:52:36.109138 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.csv
+-rw-r--r--   0        0        0      390 2023-05-21 14:45:20.721162 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0     4689 2023-05-22 05:48:56.428345 starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.csv
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.html
+-rw-r--r--   0        0        0      520 2023-05-22 07:23:43.629054 starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.5.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      340 2023-05-21 14:36:12.440552 starvote-1.5.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
+-rw-r--r--   0        0        0      234 2023-05-21 14:36:15.004573 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
+-rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
+-rw-r--r--   0        0        0      267 2023-05-21 14:36:17.328593 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      374 2023-05-21 14:36:20.268617 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv
+-rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf
+-rw-r--r--   0        0        0     2642 2023-05-21 14:36:26.092666 starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf
+-rw-r--r--   0        0        0      961 2023-05-21 14:36:28.876690 starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.pdf
+-rw-r--r--   0        0        0      876 2023-05-21 14:36:32.040716 starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf
+-rw-r--r--   0        0        0     2418 2023-05-21 14:36:34.744739 starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf
+-rw-r--r--   0        0        0     1091 2023-05-21 14:36:37.344761 starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.result.pdf
+-rw-r--r--   0        0        0      408 2023-05-21 14:36:39.896782 starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.result.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf
+-rw-r--r--   0        0        0      419 2023-05-21 14:36:42.084801 starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.result.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf
+-rw-r--r--   0        0        0      961 2023-05-21 14:36:44.284819 starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf
+-rw-r--r--   0        0        0      377 2023-05-21 14:36:46.788840 starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.txt
+-rw-r--r--   0        0        0    23647 2023-05-24 18:58:25.987616 starvote-1.5.1/starvote/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-21 14:27:54.116361 starvote-1.5.1/starvote/__main__.py
+-rw-r--r--   0        0        0     2705 2023-05-24 18:54:16.761465 starvote-1.5.1/tests/run_tests.py
+-rw-r--r--   0        0        0    13292 1970-01-01 00:00:00.000000 starvote-1.5.1/PKG-INFO
```

### Comparing `starvote-1.5/LICENSE` & `starvote-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-1.5/README.md` & `starvote-1.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,27 @@
 and avoids the worst electoral system pitfalls.  It's really great!
 
 ## A quick STAR voting primer
 
 When you vote using STAR voting, your ballot looks something like this:
 
 ```
-STAR voting ballot
-
 Amy    0 1 2 3 4 5
 Brad   0 1 2 3 4 5
 Chuck  0 1 2 3 4 5
 Darcy  0 1 2 3 4 5
 ```
 
 To vote, give every candidate a score from 0 to 5.  5 means you like
 them the most, 0 means you like them the least.  (If you don't pick one
 of the scores, that's the same as a 0.)  If you give two candidates
 the same score, that means you like them equally--you don't have a
 preference between them.
 
-To figure out who won, you apply the **STAR** methd: **S**core,
+To figure out who won, you apply the **STAR** method: **S**core,
 **T**hen **A**utomatic **R**unoff.
 
 In the first round, the score round, you add up the scores of all the
 candidates.  The top two scoring candidates automatically advance to
 the second round.
 
 In the second round, you examine every ballot to see which of the
@@ -147,15 +145,15 @@
 poll.add_ballot({'Amy': 5, 'Brian': 2, 'Chuck': 3})
 poll.add_ballot({'Amy': 4, 'Brian': 4, 'Chuck': 5})
 winner = poll.result(print=print)
 print()
 print(f"[Winner]\n{winner}")
 ```
 
-Here's what the output of this program looks like:
+When run, the above example program produces this output:
 
 ```
 [Score round]
   Chuck -- 13 (average 4.33)
   Amy   -- 10 (average 3.33)
   Brian --  9 (average 3.00)
 [Automatic runoff round]
@@ -163,15 +161,16 @@
   Amy           -- 1
   No preference -- 0
 
 [Winner]
 Chuck
 ```
 
-If the module is executed as a script, it will read a single
+If the `starvote` module is executed as a script (`python -m starvote`),
+it'll read a single
 [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values)
 in [`https://star.vote/`](https://star.vote/) format, tabulate, and print
 the result.  For example, you can run this from the root of the
 source-code repository:
 
 ```
 % python3 -m starvote sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
@@ -180,56 +179,60 @@
 to see how **starvote** handles a tie during the automatic runoff round.
 
 ## Multiple-winner elections
 
 **starvote** also implements several multi-winner electoral systems:
 
 * [Bloc STAR](https://www.starvoting.org/multi_winner),
+  a multi-winner variant of STAR voting that fills multiple
+  seats with the most *popular* candidates,
 * [Proportional STAR](https://www.starvoting.org/star-pr)
   (aka "STAR-PR", aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score)),
   a [proportional representation](https://en.wikipedia.org/wiki/Proportional_representation)
   electoral system,
 * and [Reweighted Range Voting](https://rangevoting.org/RRV.html)
   (aka "RRV"),
-  an alternative proportional electoral system.
-  Not a STAR variant per se, but the ballot and voting mechanism
+  another proportional representation electoral system.
+  RRV isn't a STAR variant per se, but the ballot and voting mechanism
   is identical to a STAR ballot.
 
 Simply
 instantiate your `Poll` object passing in the enum constant
 `starvote.Bloc_STAR`, `starvote.Proportional_STAR`,
 or `starvote.Reweighted_Range`
-for the `variant` parameter, and the number of seats in
+for the `electoral_system` parameter, and the number of seats in
 the `seats` keyword-only parameter:
 
 ```Python
-poll = starvote.Poll(variant=starvote.Bloc_STAR, seats=2)
+poll = starvote.Poll(electoral_system=starvote.Bloc_STAR, seats=2)
 ```
 
 This changes `poll.result` to return a list of winners instead
 of a single winner.
 
 You can experiment with these with the command-line version of the
-module, too.  You can specify the variant with `-v`,
+module, too.  You can specify the electoral system with `-e`,
 the number of seats with `-s`,
 and the maximum score with `-m`:
 
 ```
-% python3 -m starvote -v Reweighted_Range -s 3 -m 10 sample_polls/sample_poll_reweighted_range_3_seats.csv
+% python3 -m starvote -e Reweighted_Range -s 3 -m 10 sample_polls/sample_poll_reweighted_range_3_seats.csv
 ```
 
 ### Warning
 
-I haven't found a test corpus for either of the STAR multi-winner
-voting methods.
-I'm following the rules, as best I can, and the results I'm getting
-make sense.  But, so far, my implementations of Bloc STAR
-and Proportional STAR definitely could be wrong.
+I haven't found a single test corpus for either of the STAR
+multi-winner voting methods.
+I'm following the rules as best I can, and the results I'm getting
+make sense.  But so far I can't confirm my implementations of Bloc STAR
+and Proportional STAR are correct.  There's a very real possibility
+my code is wrong.
 
-(I do have one sample vote for )
+(I do have one sample poll for Reweighted Range voting, so I'm
+reasonably confident that implementation is fine.)
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
@@ -245,14 +248,25 @@
 The source code repository includes sample ballots downloaded from
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
+**1.5.1** - *2023/05/24*
+
+* Renamed a bunch of names in the API.
+  * Renamed `PollVariant` enum to `ElectoralSystem`.
+  * Renamed `variant` parameter to `electoral_system`.
+  * Renamed `max_score` parameter to `maximum_score`.
+* Changed command-line module options to match.
+  * Changed `-v|--variant` to `-e|--electoral-system`.
+  * Changed `-m|--max_score` to `-m|--maximum_score`.
+
+
 **1.5** - *2023/05/22*
 
 * Added support for
   [Reweighted Range Voting](https://rangevoting.org/RRV.html),
   an attractive alternative to Proportional STAR.
   Like STAR-PR, RRV is a proportional representation electoral
   system.  But RRV is simpler to understand, simpler to
```

### Comparing `starvote-1.5/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.result.txt` & `starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.csv` & `starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.html` & `starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.html`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.txt` & `starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt` & `starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt` & `starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_best_akali_skins.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_best_akali_skins.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_best_akali_skins.result.txt` & `starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt` & `starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt` & `starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_presidential_candidates.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_presidential_candidates.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt` & `starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf` & `starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5/starvote/__init__.py` & `starvote-1.5.1/starvote/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 
 __doc__ = "A simple STAR vote tabulator"
 
-__version__ = "1.5"
+__version__ = "1.5.1"
 
 __all__ = [
     'Bloc_STAR',
     'BLOC_STAR',
     'main',
     'Poll',
-    'PollVariant',
+    'ElectoralSystem',
     'Proportional_STAR',
     'Reweighted_Range',
     'RRV',
     'STAR',
     'STAR_PR',
     'UnbreakableTieError',
     ]
@@ -31,50 +31,50 @@
 class UnbreakableTieError(ValueError):
     def __init__(self, description, *candidates):
         super().__init__(description)
         self.candidates = tuple(candidates)
 
 
 @global_enum
-class PollVariant(enum.Enum):
+class ElectoralSystem(enum.Enum):
     STAR = 1
     Bloc_STAR = 2
     Proportional_STAR = 3
     Reweighted_Range = 4
 
-STAR = PollVariant.STAR
+STAR = ElectoralSystem.STAR
 # permit old capitalized name, FOR NOW
-Bloc_STAR = BLOC_STAR = PollVariant.Bloc_STAR
-Proportional_STAR = STAR_PR = PollVariant.Proportional_STAR
-Reweighted_Range = RRV = PollVariant.Reweighted_Range
+Bloc_STAR = BLOC_STAR = ElectoralSystem.Bloc_STAR
+Proportional_STAR = STAR_PR = ElectoralSystem.Proportional_STAR
+Reweighted_Range = RRV = ElectoralSystem.Reweighted_Range
 
 
 class Poll:
-    def __init__(self, variant=STAR, *, seats=1, max_score=5):
-        self.variant = variant
+    def __init__(self, electoral_system=STAR, *, seats=1, maximum_score=5):
+        self.electoral_system = electoral_system
         self.seats = seats
-        self.max_score = max_score
+        self.maximum_score = maximum_score
 
         self.candidates = {}
         self.ballots = []
 
-        if variant == STAR:
+        if electoral_system == STAR:
             if seats != 1:
-                raise ValueError("seats must be 1 when using variant STAR")
+                raise ValueError("seats must be 1 when using STAR electoral system")
         else:
             if seats == 1:
-                raise ValueError("seats must be > 1 when using variant " + str(variant).rpartition(".")[2])
+                raise ValueError("seats must be > 1 when using {str(electoral_system).rpartition('.'')[2]} electoral system")
 
     def add_candidate(self, name):
         self.candidates[name] = 0
 
     def add_ballot(self, ballot):
         for candidate, score in ballot.items():
             assert isinstance(score, int)
-            assert 0 <= score <= self.max_score, f"score {score} not in the range 0..{self.max_score}"
+            assert 0 <= score <= self.maximum_score, f"score {score} not in the range 0..{self.maximum_score}"
             if candidate not in self.candidates:
                 self.add_candidate(candidate)
             self.candidates[candidate] += score
         self.ballots.append(ballot)
 
     @staticmethod
     def compute_widths(ballots, scores):
@@ -146,15 +146,15 @@
 
     def _rrv(self, ballots, candidates, *, print=None):
         # Suggested by Tim Peters as an alternative to Proportional STAR;
         # a score-based proportional electoral system that doesn't throw away ballots.
         # https://rangevoting.org/RRV.html
         # https://rangevoting.org/RRVr.html
 
-        C = self.max_score
+        C = self.maximum_score
         weight = 1.0 # aka C/C
         weighted_ballots = [ [b, C, weight] for b in ballots ]
         winners = []
 
         for polling_round in range(1, self.seats + 1):
             if print:
                 print(f"[Reweighted Range {polling_round}]")
@@ -322,47 +322,47 @@
         winners = []
         candidates = self.candidates
         ballots = self.ballots
 
         if not candidates:
             raise ValueError("no candidates")
 
-        if self.variant == STAR:
+        if self.electoral_system == STAR:
             if print:
                 print("[STAR]")
             if len(candidates) == 1:
                 winners = list(candidates)
                 winner = winners[0]
                 if print:
                     print("  Only one candidate, returning winner {winner}!")
                 return winner
             round_text_format = ""
         else:
             if print:
-                if self.variant == BLOC_STAR:
+                if self.electoral_system == BLOC_STAR:
                     print("[BLOC STAR]")
-                elif self.variant == Proportional_STAR:
+                elif self.electoral_system == Proportional_STAR:
                     print("[Proportional STAR]")
                 else:
                     print("[Reweighted Range]")
                 print(f"  {self.seats} seats.")
             if len(candidates) <= self.seats:
                 raise ValueError(f"not enough candidates, need {self.seats}, have {len(candidates)}")
             if len(candidates) == self.seats:
                 print(f"  Have exactly {self.seats} candidates, all candidates are winners!")
                 return list(candidates)
             # we're gonna modify ballots, so, make copies
             ballots = [dict(b) for b in ballots]
             candidates = dict(candidates)
             round_text_format = " {polling_round}"
 
-        if self.variant == Proportional_STAR:
+        if self.electoral_system == Proportional_STAR:
             return self._proportional_result(ballots, candidates, print=print)
 
-        if self.variant == Reweighted_Range:
+        if self.electoral_system == Reweighted_Range:
             return self._rrv(ballots, candidates, print=print)
 
         for polling_round in range(1, self.seats+1):
             candidates_count = len(candidates)
             ballots_count = len(ballots)
             assert candidates_count
 
@@ -422,15 +422,15 @@
             if self.seats > 1:
                 for b in ballots:
                     if winner in b:
                         del b[winner]
                 assert winner in candidates
                 del candidates[winner]
 
-        if self.variant == STAR:
+        if self.electoral_system == STAR:
             assert len(winners) == 1
             return winner
 
         assert len(winners) == self.seats
         return winners
 
 
@@ -438,32 +438,40 @@
     import csv
     import os.path
 
     text = []
     if print is None:
         def print(*a, sep=" "):
             text.append(sep.join(str(o) for o in a))
+        def flush_print():
+            t = "\n".join(text)
+            builtins.print(t)
+    else:
+        def flush_print(): pass
 
     def usage(s=None):
         if s:
             print(s)
             print()
-        print("usage: starvote.py [-v|--variant variant] [-s|--seats seats] ballot.csv")
+        print("usage: starvote.py [-e|--electoral-system system] [-m|--maximum-score score] [-s|--seats seats] ballot.csv")
         print()
-        print("-v|--variant specifies STAR variant.  supported variants are STAR (default) and BLOC_STAR.")
-        print("-s|--seats specifies number of seats, default 1.")
+        print("Options:")
+        print("  -e|--electoral-system specifies electoral system.  Supported systems are STAR (default), BLOC, STAR-PR, and RRV.")
+        print("  -m|--maximum-score specifies the maximum score per vote, default 5.")
+        print("  -s|--seats specifies number of seats, default 1.")
         print()
-        print("ballot is assumed to be in https://start.vote CSV format.")
+        print("ballot.csv is assumed to be in https://start.vote CSV format.")
         print()
+        flush_print()
         return -1
 
     if not argv:
-        usage()
+        return usage()
 
-    variant_map = {
+    electoral_system_map = {
         "STAR": STAR,
         None: STAR,
 
         "Bloc_STAR": Bloc_STAR,
         "Bloc": Bloc_STAR,
         # permit old capitalized names, FOR NOW
         "BLOC_STAR": Bloc_STAR,
@@ -472,103 +480,113 @@
         "Proportional_STAR": Proportional_STAR,
         "STAR-PR": Proportional_STAR,
 
         "Reweighted_Range": Reweighted_Range,
         "RRV": Reweighted_Range,
     }
 
-    variant = None
+    electoral_system = None
     seats = None
-    max_score = None
+    maximum_score = None
 
     csv_file = None
 
     value_waiting_for_oparg = None
     extraneous_args = []
 
+    allow_options = True
+
     for arg in argv:
 
         if value_waiting_for_oparg:
             option, name = value_waiting_for_oparg
-            if name == "variant":
-                variant = variant_map.get(arg)
-                if variant is None:
-                    usage(f"unknown variant {arg}")
+            if name == "electoral_system":
+                electoral_system = electoral_system_map.get(arg)
+                if electoral_system is None:
+                    return usage(f"unknown electoral system {arg}")
             elif name == "seats":
                 seats = int(arg)
-            elif name == "max_score":
-                max_score = int(arg)
+            elif name == "maximum_score":
+                maximum_score = int(arg)
             else:
-                raise RuntimeError(f"unknown value waiting for oparg {variant!r}")
+                raise RuntimeError(f"unknown value waiting for oparg {value_waiting_for_oparg!r}")
             value_waiting_for_oparg = None
             continue
 
-        if arg.startswith("-v=") or arg.startswith("--variant="):
-            if variant is not None:
-                usage("variant specified twice")
-            v = arg.partition('=')[2]
-            variant = variant_map.get(v, None)
-            if variant is None:
-                usage(f"unknown variant {v}")
-            continue
-        if arg in ("-v", "--variant"):
-            if variant is not None:
-                usage("variant specified twice")
-            value_waiting_for_oparg = (arg, "variant")
-            continue
+        if allow_options:
+            if arg.startswith("-e=") or arg.startswith("--electoral-system="):
+                if electoral_system is not None:
+                    return usage("electoral system specified twice")
+                e = arg.partition('=')[2]
+                electoral_system = electoral_system_map.get(e, None)
+                if electoral_system is None:
+                    return usage(f"unknown electoral system {e}")
+                continue
+            if arg in ("-e", "--electoral-system"):
+                if electoral_system is not None:
+                    return usage("electoral system specified twice")
+                value_waiting_for_oparg = (arg, "electoral_system")
+                continue
 
-        if arg.startswith("-s=") or arg.startswith("--seats="):
-            if seats is not None:
-                usage("seats specified twice")
-            seats = int(arg.partition('='))
-            continue
-        if arg in ("-s", "--seats"):
-            if seats is not None:
-                usage("seats specified twice")
-            value_waiting_for_oparg = (arg, "seats")
-            continue
+            if arg.startswith("-s=") or arg.startswith("--seats="):
+                if seats is not None:
+                    return usage("seats specified twice")
+                seats = int(arg.partition('='))
+                continue
+            if arg in ("-s", "--seats"):
+                if seats is not None:
+                    return usage("seats specified twice")
+                value_waiting_for_oparg = (arg, "seats")
+                continue
 
-        if arg.startswith("-m=") or arg.startswith("--max-score="):
-            if max_score is not None:
-                usage("max-score specified twice")
-            max_score = int(arg.partition('='))
-            continue
-        if arg in ("-m", "--max-score"):
-            if max_score is not None:
-                usage("max-score specified twice")
-            value_waiting_for_oparg = (arg, "max_score")
-            continue
+            if arg.startswith("-m=") or arg.startswith("--maximum-score="):
+                if maximum_score is not None:
+                    return usage("maximum score specified twice")
+                maximum_score = int(arg.partition('='))
+                continue
+            if arg in ("-m", "--maximum-score"):
+                if maximum_score is not None:
+                    return usage("maximum score specified twice")
+                value_waiting_for_oparg = (arg, "maximum_score")
+                continue
+
+            if arg == "--":
+                allow_options = False
+                continue
+
+            if arg.startswith('-'):
+                return usage(f"unknown option {arg}")
 
         if csv_file is None:
             csv_file = arg
             continue
         extraneous_args.append(arg)
 
     if extraneous_args:
-        usage("too many arguments: " + " ".join(extraneous_args))
+        return usage("too many arguments: " + " ".join(extraneous_args))
     if value_waiting_for_oparg:
         option, name = value_waiting_for_oparg
-        usage(f"no argument specified for {option}")
+        return usage(f"no argument specified for {option}")
 
     args = []
     kwargs = {}
 
-    if variant is not None:
-        args.append(variant)
+    if electoral_system is not None:
+        args.append(electoral_system)
 
     if seats is not None:
         kwargs["seats"] = seats
 
-    if max_score is not None:
-        kwargs["max_score"] = max_score
+    if maximum_score is not None:
+        kwargs["maximum_score"] = maximum_score
 
     if csv_file is None:
-        usage("no CSV file specified.")
+        return usage("no CSV file specified.")
     if not os.path.isfile(csv_file):
-        usage("invalid CSV file specified.")
+        return usage("invalid CSV file specified.")
 
     poll = Poll(*args, **kwargs)
     with open(csv_file, "rt") as f:
         reader = csv.reader(f)
         candidates = None
         for row in reader:
             # clip off voterid, date, and pollid
@@ -602,11 +620,10 @@
         print(f"  {winner}")
     else:
         print("[Winners]")
         for w in winner:
             print(f"  {w}")
 
     if text:
-        t = "\n".join(text)
-        builtins.print(t)
+        flush_print()
 
     return 0
```

### Comparing `starvote-1.5/tests/run_tests.py` & `starvote-1.5.1/tests/run_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,45 +37,45 @@
     return output
 def flush_text():
     builtins.print(get_text())
 
 verbose = ("-v" in sys.argv) or ("--verbose" in sys.argv)
 
 seats_re = re.compile("_(\d+)_seats_")
-max_score_re = re.compile("_max-score_(\d+)[_.]")
+maximum_score_re = re.compile("_max-score_(\d+)[_.]")
 
 tests_run = 0
 for csv in sorted(glob.glob("sample_polls/*.csv")):
     expected_file = csv.replace(".csv", ".result.txt")
     if not os.path.isfile(expected_file):
         builtins.print("skipping", csv)
         continue
     text.clear()
     args = []
     multi_winner = False
     if "_proportional_star_" in csv:
-        args.extend(("-v", "Proportional_STAR"))
+        args.extend(("-e", "Proportional_STAR"))
         multi_winner = True
     elif "_bloc_star_" in csv:
-        args.extend(("-v", "Bloc_STAR"))
+        args.extend(("-e", "Bloc_STAR"))
         multi_winner = True
     elif "_reweighted_range_" in csv:
-        args.extend(("-v", "Reweighted_Range"))
+        args.extend(("-e", "Reweighted_Range"))
         multi_winner = True
 
     if multi_winner:
         match = seats_re.search(csv)
         assert match
         seats = match.group(1)
         args.extend(("-s", seats))
 
-        match = max_score_re.search(csv)
+        match = maximum_score_re.search(csv)
         if match:
-            max_score = match.group(1)
-            args.extend(("-m", max_score))
+            maximum_score = match.group(1)
+            args.extend(("-m", maximum_score))
 
     args.append(csv)
     if verbose:
         print(args)
         flush_text()
     starvote.main(args, print=print)
     got = get_text().strip().split("\n")
```

### Comparing `starvote-1.5/PKG-INFO` & `starvote-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 1.5
+Version: 1.5.1
 Summary: A simple STAR vote tabulator
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,29 +23,27 @@
 and avoids the worst electoral system pitfalls.  It's really great!
 
 ## A quick STAR voting primer
 
 When you vote using STAR voting, your ballot looks something like this:
 
 ```
-STAR voting ballot
-
 Amy    0 1 2 3 4 5
 Brad   0 1 2 3 4 5
 Chuck  0 1 2 3 4 5
 Darcy  0 1 2 3 4 5
 ```
 
 To vote, give every candidate a score from 0 to 5.  5 means you like
 them the most, 0 means you like them the least.  (If you don't pick one
 of the scores, that's the same as a 0.)  If you give two candidates
 the same score, that means you like them equally--you don't have a
 preference between them.
 
-To figure out who won, you apply the **STAR** methd: **S**core,
+To figure out who won, you apply the **STAR** method: **S**core,
 **T**hen **A**utomatic **R**unoff.
 
 In the first round, the score round, you add up the scores of all the
 candidates.  The top two scoring candidates automatically advance to
 the second round.
 
 In the second round, you examine every ballot to see which of the
@@ -159,15 +157,15 @@
 poll.add_ballot({'Amy': 5, 'Brian': 2, 'Chuck': 3})
 poll.add_ballot({'Amy': 4, 'Brian': 4, 'Chuck': 5})
 winner = poll.result(print=print)
 print()
 print(f"[Winner]\n{winner}")
 ```
 
-Here's what the output of this program looks like:
+When run, the above example program produces this output:
 
 ```
 [Score round]
   Chuck -- 13 (average 4.33)
   Amy   -- 10 (average 3.33)
   Brian --  9 (average 3.00)
 [Automatic runoff round]
@@ -175,15 +173,16 @@
   Amy           -- 1
   No preference -- 0
 
 [Winner]
 Chuck
 ```
 
-If the module is executed as a script, it will read a single
+If the `starvote` module is executed as a script (`python -m starvote`),
+it'll read a single
 [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values)
 in [`https://star.vote/`](https://star.vote/) format, tabulate, and print
 the result.  For example, you can run this from the root of the
 source-code repository:
 
 ```
 % python3 -m starvote sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
@@ -192,56 +191,60 @@
 to see how **starvote** handles a tie during the automatic runoff round.
 
 ## Multiple-winner elections
 
 **starvote** also implements several multi-winner electoral systems:
 
 * [Bloc STAR](https://www.starvoting.org/multi_winner),
+  a multi-winner variant of STAR voting that fills multiple
+  seats with the most *popular* candidates,
 * [Proportional STAR](https://www.starvoting.org/star-pr)
   (aka "STAR-PR", aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score)),
   a [proportional representation](https://en.wikipedia.org/wiki/Proportional_representation)
   electoral system,
 * and [Reweighted Range Voting](https://rangevoting.org/RRV.html)
   (aka "RRV"),
-  an alternative proportional electoral system.
-  Not a STAR variant per se, but the ballot and voting mechanism
+  another proportional representation electoral system.
+  RRV isn't a STAR variant per se, but the ballot and voting mechanism
   is identical to a STAR ballot.
 
 Simply
 instantiate your `Poll` object passing in the enum constant
 `starvote.Bloc_STAR`, `starvote.Proportional_STAR`,
 or `starvote.Reweighted_Range`
-for the `variant` parameter, and the number of seats in
+for the `electoral_system` parameter, and the number of seats in
 the `seats` keyword-only parameter:
 
 ```Python
-poll = starvote.Poll(variant=starvote.Bloc_STAR, seats=2)
+poll = starvote.Poll(electoral_system=starvote.Bloc_STAR, seats=2)
 ```
 
 This changes `poll.result` to return a list of winners instead
 of a single winner.
 
 You can experiment with these with the command-line version of the
-module, too.  You can specify the variant with `-v`,
+module, too.  You can specify the electoral system with `-e`,
 the number of seats with `-s`,
 and the maximum score with `-m`:
 
 ```
-% python3 -m starvote -v Reweighted_Range -s 3 -m 10 sample_polls/sample_poll_reweighted_range_3_seats.csv
+% python3 -m starvote -e Reweighted_Range -s 3 -m 10 sample_polls/sample_poll_reweighted_range_3_seats.csv
 ```
 
 ### Warning
 
-I haven't found a test corpus for either of the STAR multi-winner
-voting methods.
-I'm following the rules, as best I can, and the results I'm getting
-make sense.  But, so far, my implementations of Bloc STAR
-and Proportional STAR definitely could be wrong.
+I haven't found a single test corpus for either of the STAR
+multi-winner voting methods.
+I'm following the rules as best I can, and the results I'm getting
+make sense.  But so far I can't confirm my implementations of Bloc STAR
+and Proportional STAR are correct.  There's a very real possibility
+my code is wrong.
 
-(I do have one sample vote for )
+(I do have one sample poll for Reweighted Range voting, so I'm
+reasonably confident that implementation is fine.)
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
@@ -257,14 +260,25 @@
 The source code repository includes sample ballots downloaded from
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
+**1.5.1** - *2023/05/24*
+
+* Renamed a bunch of names in the API.
+  * Renamed `PollVariant` enum to `ElectoralSystem`.
+  * Renamed `variant` parameter to `electoral_system`.
+  * Renamed `max_score` parameter to `maximum_score`.
+* Changed command-line module options to match.
+  * Changed `-v|--variant` to `-e|--electoral-system`.
+  * Changed `-m|--max_score` to `-m|--maximum_score`.
+
+
 **1.5** - *2023/05/22*
 
 * Added support for
   [Reweighted Range Voting](https://rangevoting.org/RRV.html),
   an attractive alternative to Proportional STAR.
   Like STAR-PR, RRV is a proportional representation electoral
   system.  But RRV is simpler to understand, simpler to
```

