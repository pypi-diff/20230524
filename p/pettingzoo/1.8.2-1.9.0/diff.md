# Comparing `tmp/PettingZoo-1.8.2.tar.gz` & `tmp/PettingZoo-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PettingZoo-1.8.2.tar", last modified: Fri May 14 18:31:53 2021, max compression
+gzip compressed data, was "dist/PettingZoo-1.9.0.tar", last modified: Sat Jun 12 14:54:39 2021, max compression
```

## Comparing `PettingZoo-1.8.2.tar` & `PettingZoo-1.9.0.tar`

### file list

```diff
@@ -1,308 +1,310 @@
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    14899 2021-03-26 18:52:14.000000 PettingZoo-1.8.2/LICENSE.txt
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       78 2020-11-08 00:28:29.000000 PettingZoo-1.8.2/MANIFEST.in
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3008 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/PKG-INFO
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:51.000000 PettingZoo-1.8.2/PettingZoo.egg-info/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3008 2021-05-14 18:31:50.000000 PettingZoo-1.8.2/PettingZoo.egg-info/PKG-INFO
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    11041 2021-05-14 18:31:51.000000 PettingZoo-1.8.2/PettingZoo.egg-info/SOURCES.txt
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        1 2021-05-14 18:31:50.000000 PettingZoo-1.8.2/PettingZoo.egg-info/dependency_links.txt
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      503 2021-05-14 18:31:50.000000 PettingZoo-1.8.2/PettingZoo.egg-info/requires.txt
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       11 2021-05-14 18:31:50.000000 PettingZoo-1.8.2/PettingZoo.egg-info/top_level.txt
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3952 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/README.md
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:51.000000 PettingZoo-1.8.2/pettingzoo/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    15012 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/LICENSE.txt
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      490 2021-05-14 18:31:21.000000 PettingZoo-1.8.2/pettingzoo/__init__.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/atari/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2320 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8595 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/base_atari_env.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      495 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/basketball_pong_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      316 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/boxing_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      596 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/combat_plane_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      804 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/combat_tank_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      321 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/double_dunk_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      315 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/entombed_competitive_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      315 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/entombed_cooperative_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      322 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/flag_capture_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      495 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/foozpong_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      320 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/ice_hockey_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      315 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/joust_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      320 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/mario_bros_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      988 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/maze_craze_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      317 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/othello_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1125 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/pong_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      358 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/quadrapong_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      611 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/space_invaders_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      319 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/space_war_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      318 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/surround_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      316 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/tennis_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      324 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/video_checkers_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      495 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/volleyball_pong_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      318 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/warlords_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      323 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/atari/wizard_of_wor_v2.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1427 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/__init__.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4191 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/cake_paddle.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    15978 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/cooperative_pong.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1966 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/manual_control.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       90 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong_v2.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/__init__.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      461 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/archer.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10490 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/arrow.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      493 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/knight.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3398 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/left_wall.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      483 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/mace.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1368 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch1.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1442 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch2.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1505 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch3.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1459 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch4.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3313 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/right_wall.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      483 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/zombie.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    27676 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/knights_archers_zombies.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2117 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/manual_control.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5186 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/players.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2987 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/weapons.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1289 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/zombie.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      104 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies_v7.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5856 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/background.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1840 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/manual_control.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      642 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/piston.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1197 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/piston_body.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    17933 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/pistonball.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       78 2021-03-26 18:52:15.000000 PettingZoo-1.8.2/pettingzoo/butterfly/pistonball_v4.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10831 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/background.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6972 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/background_append.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5237 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/blit_background.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3400 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/blit_background_append.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1856 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/manual_control.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    14861 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/prison.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2618 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/prisoner.png
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      792 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/alien_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      760 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/alien_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      938 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/alien_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2072 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/bunny_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2027 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/bunny_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2407 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/bunny_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1214 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/drone_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1218 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/drone_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1424 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/drone_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1323 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/glowy_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1296 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/glowy_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1407 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/glowy_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3379 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/rabbit_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3404 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/rabbit_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3525 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/rabbit_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1544 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/reptile_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1562 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/reptile_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1847 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/reptile_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2017 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/robot_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2141 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/robot_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2385 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/robot_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2567 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/tank_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2612 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/tank_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2707 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/tank_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1041 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/ufo_left.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      987 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/ufo_right.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1035 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/ufo_still.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       70 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prison_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2151 2020-12-18 03:00:30.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/constants.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5857 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bank.png
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2111 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/0.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2112 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/1.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2115 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/2.png
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      446 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/0.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      316 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/1.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      623 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/2.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      607 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/3.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      968 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/seaweed_water.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      564 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/fence_horiz_tile.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      352 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/fence_vert_tile.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      289 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/gold.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2323 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/prospector.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5686 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/river_tile.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5724 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/river_to_sand_tile.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3500 2020-11-24 22:48:02.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/sand_tile.png
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2282 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/manual_control.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    30100 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/prospector.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1025 2020-12-18 03:00:30.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector/utils.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       78 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/butterfly/prospector_v4.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2607 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/__init__.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/backgammon/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/backgammon/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    75726 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/classic/backgammon/backgammon.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5460 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/backgammon/backgammon_env.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3654 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/backgammon/bg_utils.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       52 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/backgammon_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/checkers/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    21797 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/checkers/checkers.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       44 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/checkers_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/chess/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/chess/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3753 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/chess/chess_env.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10919 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/chess/chess_utils.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2221 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/chess/test_chess.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       42 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/chess_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/connect_four/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/connect_four/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5597 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/connect_four/connect_four.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       52 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/connect_four_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       48 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/dou_dizhu_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       48 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/gin_rummy_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/go/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/go/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3387 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/go/coords.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    19782 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/go/go.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5657 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/go/go_env.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       36 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/go_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/hanabi/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/hanabi/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    13352 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/hanabi/hanabi.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       40 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/hanabi_v4.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       51 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/leduc_holdem_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       46 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/mahjong_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1959 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/dou_dizhu.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3185 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/gin_rummy.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1260 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/leduc_holdem.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1197 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/mahjong.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3659 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/rlcard_base.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1250 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/texas_holdem.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1567 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/texas_holdem_no_limit.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1828 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/uno.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/rps/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/rps/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3497 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/classic/rps/rps.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       34 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/classic/rps_v1.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/rpsls/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/rpsls/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4228 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/classic/rpsls/rpsls.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       38 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/classic/rpsls_v1.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       60 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/texas_holdem_no_limit_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       51 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/texas_holdem_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:52.000000 PettingZoo-1.8.2/pettingzoo/classic/tictactoe/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/tictactoe/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2239 2020-11-20 01:49:51.000000 PettingZoo-1.8.2/pettingzoo/classic/tictactoe/board.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5311 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/tictactoe/tictactoe.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       46 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/tictactoe_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       42 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/classic/uno_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/magent/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1145 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3366 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/adversarial_pursuit_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4436 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/battle_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4210 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/battlefield_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6556 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/combined_arms_v4.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8243 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/gather_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6597 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/magent_env.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10001 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/magent/render.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3820 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/magent/tiger_deer_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/mpe/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1354 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/__init__.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6999 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/core.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    12852 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/rendering.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      297 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/scenario.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     7780 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/secrcode.ttf
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8303 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/simple_env.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2007 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6088 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_adversary.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5991 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_crypto.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4247 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_push.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3539 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_reference.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3490 2020-12-18 03:00:30.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_speaker_listener.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3955 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_spread.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5986 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_tag.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    12191 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_world_comm.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      480 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_adversary_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      468 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_crypto_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      464 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_push_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      600 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_reference_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      488 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_speaker_listener_v3.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      600 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_spread_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      550 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_tag_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      454 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_v2.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      614 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/mpe/simple_world_comm_v2.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/sisl/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      828 2021-05-14 18:31:13.000000 PettingZoo-1.8.2/pettingzoo/sisl/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      375 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/sisl/_utils.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/sisl/multiwalker/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/sisl/multiwalker/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3856 2021-05-14 18:31:13.000000 PettingZoo-1.8.2/pettingzoo/sisl/multiwalker/multiwalker.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    28346 2021-05-14 18:31:13.000000 PettingZoo-1.8.2/pettingzoo/sisl/multiwalker/multiwalker_base.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       64 2021-05-14 18:31:13.000000 PettingZoo-1.8.2/pettingzoo/sisl/multiwalker_v7.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2487 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/manual_control.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3092 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/pursuit.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    18499 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/pursuit_base.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      364 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1992 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/agent_layer.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2802 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/agent_utils.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      605 2020-12-18 03:00:30.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/controllers.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3192 2020-11-24 22:37:46.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/discrete_agent.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3628 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/two_d_maps.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       72 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/pursuit_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/sisl/waterworld/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2020-11-20 01:49:52.000000 PettingZoo-1.8.2/pettingzoo/sisl/waterworld/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2992 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/waterworld/waterworld.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    27672 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/waterworld/waterworld_base.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       62 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/sisl/waterworld_v3.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/test/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      448 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/test/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5871 2021-05-14 18:31:13.000000 PettingZoo-1.8.2/pettingzoo/test/all_modules.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5505 2021-05-14 18:31:13.000000 PettingZoo-1.8.2/pettingzoo/test/all_parameter_combs.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)    14658 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/api_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1173 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/bombardment_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2647 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/ci_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      779 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/manual_control_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1098 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/pettingzoo/test/max_cycles_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2121 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/parallel_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1118 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/performance_benchmark.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      658 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/print_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      896 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/test/pytest_runner.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1610 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/test/render_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1123 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/save_obs_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2969 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/test/seed_test.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4205 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/test/state_test.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/utils/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      435 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1165 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/agent_selector.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1144 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/average_total_reward.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      543 2020-12-18 03:00:31.000000 PettingZoo-1.8.2/pettingzoo/utils/capture_stdout.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5758 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/conversions.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      385 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/deprecated_module.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8972 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/env.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2806 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/env_logger.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1244 2021-03-20 22:54:42.000000 PettingZoo-1.8.2/pettingzoo/utils/generate_gif.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      894 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/random_demo.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1587 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/save_observation.py
-drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      299 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/__init__.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      701 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/assert_out_of_bounds.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2322 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/base.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)      548 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/capture_stdout.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1090 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/clip_out_of_bounds.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3240 2021-03-26 18:52:16.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/order_enforcing.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1905 2021-04-24 23:57:36.000000 PettingZoo-1.8.2/pettingzoo/utils/wrappers/terminate_illegal.py
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)       38 2021-05-14 18:31:53.000000 PettingZoo-1.8.2/setup.cfg
--rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2032 2021-03-28 00:15:25.000000 PettingZoo-1.8.2/setup.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    14899 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/LICENSE.txt
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       78 2020-11-08 00:28:29.000000 PettingZoo-1.9.0/MANIFEST.in
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3008 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/PKG-INFO
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/PettingZoo.egg-info/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3008 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/PettingZoo.egg-info/PKG-INFO
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    11059 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/PettingZoo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        1 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/PettingZoo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      503 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/PettingZoo.egg-info/requires.txt
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       11 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/PettingZoo.egg-info/top_level.txt
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3952 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/README.md
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/pettingzoo/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    15012 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/LICENSE.txt
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      490 2021-06-12 14:50:20.000000 PettingZoo-1.9.0/pettingzoo/__init__.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/pettingzoo/atari/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2619 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/atari/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8595 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/base_atari_env.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      495 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/atari/basketball_pong_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      316 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/boxing_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      596 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/combat_plane_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      804 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/combat_tank_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      321 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/double_dunk_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      315 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/entombed_competitive_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      315 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/entombed_cooperative_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      322 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/flag_capture_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      495 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/atari/foozpong_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      320 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/ice_hockey_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      315 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/joust_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      320 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/mario_bros_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      988 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/maze_craze_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      317 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/othello_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1125 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/atari/pong_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      358 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/atari/quadrapong_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      611 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/space_invaders_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      319 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/space_war_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      318 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/surround_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      316 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/tennis_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      324 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/video_checkers_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      495 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/atari/volleyball_pong_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      318 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/warlords_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      323 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/atari/wizard_of_wor_v2.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/pettingzoo/butterfly/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1427 2021-05-26 21:13:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/__init__.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4191 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/cake_paddle.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    15978 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/cooperative_pong.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1966 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/manual_control.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       90 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong_v2.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:37.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/__init__.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      461 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/archer.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10490 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/arrow.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      493 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/knight.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3398 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/left_wall.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      483 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/mace.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1368 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch1.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1442 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch2.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1505 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch3.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1459 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch4.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3313 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/right_wall.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      483 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/zombie.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    27676 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/knights_archers_zombies.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2117 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/manual_control.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5186 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/players.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2987 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/weapons.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1289 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/zombie.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      104 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies_v7.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5856 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/background.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1840 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/manual_control.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      642 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/piston.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1197 2021-03-26 18:52:15.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/piston_body.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    17933 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/pistonball.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       78 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/pistonball_v4.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10831 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/background.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6972 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/background_append.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5237 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/blit_background.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3400 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/blit_background_append.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1856 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/manual_control.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    14861 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/prison.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2618 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/prisoner.png
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      792 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/alien_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      760 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/alien_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      938 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/alien_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2072 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/bunny_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2027 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/bunny_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2407 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/bunny_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1214 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/drone_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1218 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/drone_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1424 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/drone_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1323 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/glowy_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1296 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/glowy_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1407 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/glowy_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3379 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/rabbit_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3404 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/rabbit_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3525 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/rabbit_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1544 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/reptile_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1562 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/reptile_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1847 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/reptile_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2017 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/robot_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2141 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/robot_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2385 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/robot_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2567 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/tank_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2612 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/tank_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2707 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/tank_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1041 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/ufo_left.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      987 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/ufo_right.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1035 2020-11-24 22:37:46.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/ufo_still.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       70 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prison_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2151 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/constants.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5857 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bank.png
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2111 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/0.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2112 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/1.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2115 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/2.png
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      446 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/0.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      316 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/1.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      623 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/2.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      607 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/3.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      968 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/seaweed_water.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      564 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/fence_horiz_tile.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      352 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/fence_vert_tile.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      289 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/gold.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2323 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/prospector.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5686 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/river_tile.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5724 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/river_to_sand_tile.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3500 2020-11-24 22:48:02.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/sand_tile.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2282 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/manual_control.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    30100 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/prospector.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1025 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector/utils.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       78 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/butterfly/prospector_v4.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2607 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/__init__.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/backgammon/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/classic/backgammon/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    75726 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/classic/backgammon/backgammon.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5460 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/backgammon/backgammon_env.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3654 2021-05-15 13:15:43.000000 PettingZoo-1.9.0/pettingzoo/classic/backgammon/bg_utils.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       52 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/backgammon_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/checkers/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    21797 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/checkers/checkers.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       44 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/checkers_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/chess/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/chess/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3753 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/chess/chess_env.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10919 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/chess/chess_utils.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2221 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/chess/test_chess.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       42 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/chess_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     7433 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/connect_four.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/img/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      175 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/img/C4BlackPiece.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      166 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/img/C4RedPiece.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      580 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four/img/Connect4Board.png
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       52 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/connect_four_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       48 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/dou_dizhu_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       48 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/gin_rummy_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/go/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/go/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3387 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/go/coords.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    19782 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/go/go.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5657 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/go/go_env.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       36 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/go_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/hanabi/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/hanabi/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    13352 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/hanabi/hanabi.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       40 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/hanabi_v4.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       51 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/leduc_holdem_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       46 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/mahjong_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1959 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/dou_dizhu.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3185 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/gin_rummy.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1260 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/leduc_holdem.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1197 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/mahjong.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3659 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/rlcard_base.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1250 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/texas_holdem.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1567 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/texas_holdem_no_limit.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1828 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/uno.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/rps/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/rps/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4886 2021-06-07 23:22:29.000000 PettingZoo-1.9.0/pettingzoo/classic/rps/rps.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       48 2021-05-26 20:59:07.000000 PettingZoo-1.9.0/pettingzoo/classic/rps_v1.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       60 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/texas_holdem_no_limit_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       51 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/texas_holdem_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/classic/tictactoe/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/tictactoe/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2239 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/classic/tictactoe/board.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5311 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/tictactoe/tictactoe.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       46 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/tictactoe_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       42 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/classic/uno_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:38.000000 PettingZoo-1.9.0/pettingzoo/magent/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1287 2021-06-12 14:38:45.000000 PettingZoo-1.9.0/pettingzoo/magent/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3402 2021-06-12 14:37:27.000000 PettingZoo-1.9.0/pettingzoo/magent/adversarial_pursuit_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4436 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/magent/battle_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4210 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/magent/battlefield_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6555 2021-06-11 23:32:34.000000 PettingZoo-1.9.0/pettingzoo/magent/combined_arms_v5.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8243 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/magent/gather_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8649 2021-06-11 22:47:00.000000 PettingZoo-1.9.0/pettingzoo/magent/magent_env.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    10001 2021-06-11 22:47:00.000000 PettingZoo-1.9.0/pettingzoo/magent/render.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3820 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/magent/tiger_deer_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/mpe/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1354 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/__init__.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6999 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/core.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    12852 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/rendering.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      297 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/scenario.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     7780 2020-11-20 01:49:52.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/secrcode.ttf
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8717 2021-05-30 16:42:51.000000 PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/simple_env.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2007 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     6088 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_adversary.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5991 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_crypto.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4247 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_push.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3539 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_reference.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3490 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_speaker_listener.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3955 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_spread.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5986 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_tag.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    12191 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_world_comm.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      480 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_adversary_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      468 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_crypto_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      464 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_push_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      600 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_reference_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      488 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_speaker_listener_v3.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      600 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_spread_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      550 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_tag_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      454 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_v2.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      614 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/mpe/simple_world_comm_v2.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/sisl/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      828 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      375 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/_utils.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/sisl/multiwalker/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/multiwalker/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3856 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/multiwalker/multiwalker.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    28241 2021-06-07 23:22:29.000000 PettingZoo-1.9.0/pettingzoo/sisl/multiwalker/multiwalker_base.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       64 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/multiwalker_v7.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2487 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/manual_control.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3092 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/pursuit.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    18499 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/pursuit_base.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      364 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1992 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/agent_layer.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2802 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/agent_utils.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      605 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/controllers.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3192 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/discrete_agent.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3628 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/two_d_maps.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       72 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/pursuit_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/sisl/waterworld/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/waterworld/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2992 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/waterworld/waterworld.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    27672 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/waterworld/waterworld_base.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       62 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/sisl/waterworld_v3.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/test/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      448 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/test/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)    14660 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/test/api_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1173 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/test/bombardment_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      779 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/test/manual_control_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1311 2021-05-30 16:42:51.000000 PettingZoo-1.9.0/pettingzoo/test/max_cycles_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2123 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/test/parallel_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1118 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/test/performance_benchmark.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1610 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/test/render_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1123 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/test/save_obs_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2969 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/test/seed_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     4205 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/test/state_test.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/utils/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      435 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1165 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/agent_selector.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1144 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/average_total_reward.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      543 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/capture_stdout.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5758 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/conversions.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      385 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/deprecated_module.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     8832 2021-06-09 01:25:11.000000 PettingZoo-1.9.0/pettingzoo/utils/env.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2806 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/env_logger.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1244 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/generate_gif.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      894 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/random_demo.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1587 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/save_observation.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      299 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      701 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/assert_out_of_bounds.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2322 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/base.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      548 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/capture_stdout.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1090 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/clip_out_of_bounds.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     3240 2021-05-15 13:15:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/order_enforcing.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     1905 2021-05-18 00:00:44.000000 PettingZoo-1.9.0/pettingzoo/utils/wrappers/terminate_illegal.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)       38 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/setup.cfg
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2093 2021-06-12 14:54:21.000000 PettingZoo-1.9.0/setup.py
+drwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-06-12 14:54:39.000000 PettingZoo-1.9.0/test/
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)        0 2021-05-30 16:42:51.000000 PettingZoo-1.9.0/test/__init__.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5797 2021-06-12 14:37:47.000000 PettingZoo-1.9.0/test/all_modules.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     5521 2021-06-12 14:37:47.000000 PettingZoo-1.9.0/test/all_parameter_combs.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)     2704 2021-06-07 23:22:29.000000 PettingZoo-1.9.0/test/ci_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      667 2021-05-30 16:42:51.000000 PettingZoo-1.9.0/test/print_test.py
+-rwxrwxrwx   0 benblack  (1000) benblack  (1000)      952 2021-06-11 22:47:00.000000 PettingZoo-1.9.0/test/pytest_runner.py
```

### Comparing `PettingZoo-1.8.2/LICENSE.txt` & `PettingZoo-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/PKG-INFO` & `PettingZoo-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PettingZoo
-Version: 1.8.2
+Version: 1.9.0
 Summary: Gym for multi-agent reinforcement learning
 Home-page: https://github.com/PettingZoo-Team/PettingZoo
 Author: PettingZoo Team
 Author-email: justinkterry@gmail.com
 License: UNKNOWN
 Description: <p align="center">
             <img src="PettingZoo_Text.png" width="500px"/>
```

### Comparing `PettingZoo-1.8.2/PettingZoo.egg-info/PKG-INFO` & `PettingZoo-1.9.0/PettingZoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PettingZoo
-Version: 1.8.2
+Version: 1.9.0
 Summary: Gym for multi-agent reinforcement learning
 Home-page: https://github.com/PettingZoo-Team/PettingZoo
 Author: PettingZoo Team
 Author-email: justinkterry@gmail.com
 License: UNKNOWN
 Description: <p align="center">
             <img src="PettingZoo_Text.png" width="500px"/>
```

### Comparing `PettingZoo-1.8.2/PettingZoo.egg-info/SOURCES.txt` & `PettingZoo-1.9.0/PettingZoo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 PettingZoo.egg-info/dependency_links.txt
 PettingZoo.egg-info/requires.txt
 PettingZoo.egg-info/top_level.txt
 pettingzoo/LICENSE.txt
 pettingzoo/__init__.py
 pettingzoo/atari/__init__.py
 pettingzoo/atari/base_atari_env.py
-pettingzoo/atari/basketball_pong_v1.py
+pettingzoo/atari/basketball_pong_v2.py
 pettingzoo/atari/boxing_v1.py
 pettingzoo/atari/combat_plane_v1.py
 pettingzoo/atari/combat_tank_v1.py
 pettingzoo/atari/double_dunk_v2.py
 pettingzoo/atari/entombed_competitive_v2.py
 pettingzoo/atari/entombed_cooperative_v2.py
 pettingzoo/atari/flag_capture_v1.py
-pettingzoo/atari/foozpong_v1.py
+pettingzoo/atari/foozpong_v2.py
 pettingzoo/atari/ice_hockey_v1.py
 pettingzoo/atari/joust_v2.py
 pettingzoo/atari/mario_bros_v2.py
 pettingzoo/atari/maze_craze_v2.py
 pettingzoo/atari/othello_v2.py
-pettingzoo/atari/pong_v1.py
-pettingzoo/atari/quadrapong_v2.py
+pettingzoo/atari/pong_v2.py
+pettingzoo/atari/quadrapong_v3.py
 pettingzoo/atari/space_invaders_v1.py
 pettingzoo/atari/space_war_v1.py
 pettingzoo/atari/surround_v1.py
 pettingzoo/atari/tennis_v2.py
 pettingzoo/atari/video_checkers_v3.py
-pettingzoo/atari/volleyball_pong_v1.py
+pettingzoo/atari/volleyball_pong_v2.py
 pettingzoo/atari/warlords_v2.py
 pettingzoo/atari/wizard_of_wor_v2.py
 pettingzoo/butterfly/__init__.py
 pettingzoo/butterfly/cooperative_pong_v2.py
 pettingzoo/butterfly/knights_archers_zombies_v7.py
 pettingzoo/butterfly/pistonball_v4.py
 pettingzoo/butterfly/prison_v3.py
@@ -133,15 +133,14 @@
 pettingzoo/classic/dou_dizhu_v3.py
 pettingzoo/classic/gin_rummy_v3.py
 pettingzoo/classic/go_v3.py
 pettingzoo/classic/hanabi_v4.py
 pettingzoo/classic/leduc_holdem_v3.py
 pettingzoo/classic/mahjong_v3.py
 pettingzoo/classic/rps_v1.py
-pettingzoo/classic/rpsls_v1.py
 pettingzoo/classic/texas_holdem_no_limit_v3.py
 pettingzoo/classic/texas_holdem_v3.py
 pettingzoo/classic/tictactoe_v3.py
 pettingzoo/classic/uno_v3.py
 pettingzoo/classic/backgammon/__init__.py
 pettingzoo/classic/backgammon/backgammon.py
 pettingzoo/classic/backgammon/backgammon_env.py
@@ -149,14 +148,17 @@
 pettingzoo/classic/checkers/checkers.py
 pettingzoo/classic/chess/__init__.py
 pettingzoo/classic/chess/chess_env.py
 pettingzoo/classic/chess/chess_utils.py
 pettingzoo/classic/chess/test_chess.py
 pettingzoo/classic/connect_four/__init__.py
 pettingzoo/classic/connect_four/connect_four.py
+pettingzoo/classic/connect_four/img/C4BlackPiece.png
+pettingzoo/classic/connect_four/img/C4RedPiece.png
+pettingzoo/classic/connect_four/img/Connect4Board.png
 pettingzoo/classic/go/__init__.py
 pettingzoo/classic/go/coords.py
 pettingzoo/classic/go/go.py
 pettingzoo/classic/go/go_env.py
 pettingzoo/classic/hanabi/__init__.py
 pettingzoo/classic/hanabi/hanabi.py
 pettingzoo/classic/rlcard_envs/__init__.py
@@ -166,24 +168,22 @@
 pettingzoo/classic/rlcard_envs/mahjong.py
 pettingzoo/classic/rlcard_envs/rlcard_base.py
 pettingzoo/classic/rlcard_envs/texas_holdem.py
 pettingzoo/classic/rlcard_envs/texas_holdem_no_limit.py
 pettingzoo/classic/rlcard_envs/uno.py
 pettingzoo/classic/rps/__init__.py
 pettingzoo/classic/rps/rps.py
-pettingzoo/classic/rpsls/__init__.py
-pettingzoo/classic/rpsls/rpsls.py
 pettingzoo/classic/tictactoe/__init__.py
 pettingzoo/classic/tictactoe/board.py
 pettingzoo/classic/tictactoe/tictactoe.py
 pettingzoo/magent/__init__.py
-pettingzoo/magent/adversarial_pursuit_v2.py
+pettingzoo/magent/adversarial_pursuit_v3.py
 pettingzoo/magent/battle_v3.py
 pettingzoo/magent/battlefield_v3.py
-pettingzoo/magent/combined_arms_v4.py
+pettingzoo/magent/combined_arms_v5.py
 pettingzoo/magent/gather_v3.py
 pettingzoo/magent/magent_env.py
 pettingzoo/magent/render.py
 pettingzoo/magent/tiger_deer_v3.py
 pettingzoo/mpe/__init__.py
 pettingzoo/mpe/simple_adversary_v2.py
 pettingzoo/mpe/simple_crypto_v2.py
@@ -228,25 +228,20 @@
 pettingzoo/sisl/pursuit/utils/controllers.py
 pettingzoo/sisl/pursuit/utils/discrete_agent.py
 pettingzoo/sisl/pursuit/utils/two_d_maps.py
 pettingzoo/sisl/waterworld/__init__.py
 pettingzoo/sisl/waterworld/waterworld.py
 pettingzoo/sisl/waterworld/waterworld_base.py
 pettingzoo/test/__init__.py
-pettingzoo/test/all_modules.py
-pettingzoo/test/all_parameter_combs.py
 pettingzoo/test/api_test.py
 pettingzoo/test/bombardment_test.py
-pettingzoo/test/ci_test.py
 pettingzoo/test/manual_control_test.py
 pettingzoo/test/max_cycles_test.py
 pettingzoo/test/parallel_test.py
 pettingzoo/test/performance_benchmark.py
-pettingzoo/test/print_test.py
-pettingzoo/test/pytest_runner.py
 pettingzoo/test/render_test.py
 pettingzoo/test/save_obs_test.py
 pettingzoo/test/seed_test.py
 pettingzoo/test/state_test.py
 pettingzoo/utils/__init__.py
 pettingzoo/utils/agent_selector.py
 pettingzoo/utils/average_total_reward.py
@@ -260,8 +255,14 @@
 pettingzoo/utils/save_observation.py
 pettingzoo/utils/wrappers/__init__.py
 pettingzoo/utils/wrappers/assert_out_of_bounds.py
 pettingzoo/utils/wrappers/base.py
 pettingzoo/utils/wrappers/capture_stdout.py
 pettingzoo/utils/wrappers/clip_out_of_bounds.py
 pettingzoo/utils/wrappers/order_enforcing.py
-pettingzoo/utils/wrappers/terminate_illegal.py
+pettingzoo/utils/wrappers/terminate_illegal.py
+test/__init__.py
+test/all_modules.py
+test/all_parameter_combs.py
+test/ci_test.py
+test/print_test.py
+test/pytest_runner.py
```

### Comparing `PettingZoo-1.8.2/README.md` & `PettingZoo-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/LICENSE.txt` & `PettingZoo-1.9.0/pettingzoo/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/__init__.py` & `PettingZoo-1.9.0/pettingzoo/atari/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 from pettingzoo.utils.deprecated_module import DeprecatedModule
 
-basketball_pong_v0 = DeprecatedModule("basketball_pong", "v0", "v1")
+basketball_pong_v0 = DeprecatedModule("basketball_pong", "v0", "v2")
+basketball_pong_v1 = DeprecatedModule("basketball_pong", "v1", "v2")
 boxing_v0 = DeprecatedModule("boxing", "v0", "v1")
 combat_plane_v0 = DeprecatedModule("combat_plane", "v0", "v1")
 combat_tank_v0 = DeprecatedModule("combat_tank", "v0", "v1")
 double_dunk_v0 = DeprecatedModule("double_dunk", "v0", "v2")
 double_dunk_v1 = DeprecatedModule("double_dunk", "v1", "v2")
 entombed_competitive_v0 = DeprecatedModule("entombed_competitive", "v0", "v2")
 entombed_competitive_v1 = DeprecatedModule("entombed_competitive", "v1", "v2")
 entombed_cooperative_v0 = DeprecatedModule("entombed_cooperative", "v0", "v2")
 entombed_cooperative_v1 = DeprecatedModule("entombed_cooperative", "v1", "v2")
 flag_capture_v0 = DeprecatedModule("flag_capture", "v0", "v1")
-foozpong_v0 = DeprecatedModule("foozpong", "v0", "v1")
+foozpong_v0 = DeprecatedModule("foozpong", "v0", "v2")
+foozpong_v1 = DeprecatedModule("foozpong", "v1", "v2")
 ice_hockey_v0 = DeprecatedModule("ice_hockey", "v0", "v1")
 joust_v0 = DeprecatedModule("joust", "v0", "v2")
 joust_v1 = DeprecatedModule("joust", "v1", "v2")
 mario_bros_v0 = DeprecatedModule("mario_bros", "v0", "v2")
 mario_bros_v1 = DeprecatedModule("mario_bros", "v1", "v2")
 maze_craze_v0 = DeprecatedModule("maze_craze", "v0", "v2")
 maze_craze_v1 = DeprecatedModule("maze_craze", "v1", "v2")
 othello_v0 = DeprecatedModule("othello", "v0", "v2")
 othello_v1 = DeprecatedModule("othello", "v1", "v2")
-pong_v0 = DeprecatedModule("pong", "v0", "v1")
-quadrapong_v0 = DeprecatedModule("quadrapong", "v0", "v2")
-quadrapong_v1 = DeprecatedModule("quadrapong", "v1", "v2")
+pong_v0 = DeprecatedModule("pong", "v0", "v2")
+pong_v1 = DeprecatedModule("pong", "v1", "v2")
+quadrapong_v0 = DeprecatedModule("quadrapong", "v0", "v3")
+quadrapong_v1 = DeprecatedModule("quadrapong", "v1", "v3")
+quadrapong_v2 = DeprecatedModule("quadrapong", "v2", "v3")
 space_invaders_v0 = DeprecatedModule("space_invaders", "v0", "v1")
 space_war_v0 = DeprecatedModule("space_war", "v0", "v1")
 surround_v0 = DeprecatedModule("surround", "v0", "v1")
 tennis_v0 = DeprecatedModule("tennis", "v0", "v2")
 tennis_v1 = DeprecatedModule("tennis", "v1", "v2")
 video_checkers_v0 = DeprecatedModule("video_checkers", "v0", "v3")
 video_checkers_v1 = DeprecatedModule("video_checkers", "v1", "v3")
 video_checkers_v2 = DeprecatedModule("video_checkers", "v2", "v3")
-volleyball_pong_v0 = DeprecatedModule("volleyball_pong", "v0", "v1")
+volleyball_pong_v0 = DeprecatedModule("volleyball_pong", "v0", "v2")
+volleyball_pong_v1 = DeprecatedModule("volleyball_pong", "v1", "v2")
 warlords_v0 = DeprecatedModule("warlords", "v0", "v2")
 warlords_v1 = DeprecatedModule("warlords", "v1", "v2")
 wizard_of_wor_v0 = DeprecatedModule("wizard_of_wor", "v0", "v2")
 wizard_of_wor_v1 = DeprecatedModule("wizard_of_wor", "v1", "v2")
```

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/base_atari_env.py` & `PettingZoo-1.9.0/pettingzoo/atari/base_atari_env.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/combat_plane_v1.py` & `PettingZoo-1.9.0/pettingzoo/atari/combat_plane_v1.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/combat_tank_v1.py` & `PettingZoo-1.9.0/pettingzoo/atari/combat_tank_v1.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/maze_craze_v2.py` & `PettingZoo-1.9.0/pettingzoo/atari/maze_craze_v2.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/pong_v1.py` & `PettingZoo-1.9.0/pettingzoo/atari/pong_v2.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/atari/space_invaders_v1.py` & `PettingZoo-1.9.0/pettingzoo/atari/space_invaders_v1.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/__init__.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/__init__.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/cake_paddle.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/cake_paddle.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/cooperative_pong.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/cooperative_pong.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/cooperative_pong/manual_control.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/cooperative_pong/manual_control.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/arrow.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/arrow.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/left_wall.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/left_wall.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch1.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch1.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch2.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch2.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch3.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch3.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/patch4.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/patch4.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/img/right_wall.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/img/right_wall.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/knights_archers_zombies.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/knights_archers_zombies.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/manual_control.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/manual_control.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/players.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/players.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/weapons.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/weapons.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/knights_archers_zombies/src/zombie.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/knights_archers_zombies/src/zombie.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/background.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/background.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/manual_control.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/manual_control.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/piston.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/piston.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/piston_body.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/piston_body.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/pistonball/pistonball.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/pistonball/pistonball.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/background.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/background.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/background_append.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/background_append.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/blit_background.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/blit_background.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/blit_background_append.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/blit_background_append.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/manual_control.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/manual_control.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/prison.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/prison.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/prisoner.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/prisoner.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/alien_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/alien_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/alien_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/alien_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/alien_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/alien_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/bunny_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/bunny_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/bunny_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/bunny_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/bunny_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/bunny_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/drone_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/drone_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/drone_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/drone_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/drone_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/drone_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/glowy_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/glowy_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/glowy_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/glowy_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/glowy_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/glowy_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/rabbit_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/rabbit_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/rabbit_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/rabbit_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/rabbit_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/rabbit_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/reptile_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/reptile_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/reptile_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/reptile_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/reptile_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/reptile_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/robot_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/robot_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/robot_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/robot_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/robot_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/robot_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/tank_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/tank_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/tank_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/tank_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/tank_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/tank_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/ufo_left.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/ufo_left.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/ufo_right.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/ufo_right.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prison/sprites/ufo_still.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prison/sprites/ufo_still.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/constants.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/constants.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bank.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bank.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/0.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/0.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/1.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/1.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/bankers/2.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/bankers/2.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/2.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/2.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/3.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/3.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/debris/seaweed_water.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/debris/seaweed_water.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/fence_horiz_tile.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/fence_horiz_tile.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/prospector.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/prospector.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/river_tile.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/river_tile.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/river_to_sand_tile.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/river_to_sand_tile.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/data/sand_tile.png` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/data/sand_tile.png`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/manual_control.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/manual_control.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/prospector.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/prospector.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/butterfly/prospector/utils.py` & `PettingZoo-1.9.0/pettingzoo/butterfly/prospector/utils.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/__init__.py` & `PettingZoo-1.9.0/pettingzoo/classic/__init__.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/backgammon/backgammon.py` & `PettingZoo-1.9.0/pettingzoo/classic/backgammon/backgammon.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/backgammon/backgammon_env.py` & `PettingZoo-1.9.0/pettingzoo/classic/backgammon/backgammon_env.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/backgammon/bg_utils.py` & `PettingZoo-1.9.0/pettingzoo/classic/backgammon/bg_utils.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/checkers/checkers.py` & `PettingZoo-1.9.0/pettingzoo/classic/checkers/checkers.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/chess/chess_env.py` & `PettingZoo-1.9.0/pettingzoo/classic/chess/chess_env.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/chess/chess_utils.py` & `PettingZoo-1.9.0/pettingzoo/classic/chess/chess_utils.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/chess/test_chess.py` & `PettingZoo-1.9.0/pettingzoo/classic/chess/test_chess.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/connect_four/connect_four.py` & `PettingZoo-1.9.0/pettingzoo/classic/connect_four/connect_four.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from pettingzoo import AECEnv
 from gym import spaces
 import numpy as np
 import warnings
+import os
+
 
 from pettingzoo.utils import wrappers
 from pettingzoo.utils.agent_selector import agent_selector
 
 
+def get_image(path):
+    import pygame
+    from os import path as os_path
+    cwd = os_path.dirname(__file__)
+    image = pygame.image.load(cwd + '/' + path)
+    return image
+
+
 def env():
     env = raw_env()
-    env = wrappers.CaptureStdoutWrapper(env)
     env = wrappers.TerminateIllegalWrapper(env, illegal_reward=-1)
     env = wrappers.AssertOutOfBoundsWrapper(env)
     env = wrappers.OrderEnforcingWrapper(env)
     return env
 
 
 class raw_env(AECEnv):
-    metadata = {'render.modes': ['human'], "name": "connect_four_v3"}
+    metadata = {'render.modes': ['human', "rgb_array"], "name": "connect_four_v3"}
 
     def __init__(self):
         super().__init__()
         # 6 rows x 7 columns
         # blank space = 0
         # agent 0 -- 1
         # agent 1 -- 2
         # flat representation in row major order
+        self.screen = None
+
         self.board = [0] * (6 * 7)
 
         self.agents = ['player_0', 'player_1']
         self.possible_agents = self.agents[:]
 
         self.action_spaces = {i: spaces.Discrete(7) for i in self.agents}
         self.observation_spaces = {i: spaces.Dict({
@@ -113,19 +124,55 @@
         self.infos = {i: {} for i in self.agents}
 
         self._agent_selector = agent_selector(self.agents)
 
         self.agent_selection = self._agent_selector.reset()
 
     def render(self, mode='human'):
-        print("{}'s turn'".format(self.agent_selection))
-        print(str(np.array(self.board).reshape(6, 7)))
+        screen_width = 1287
+        screen_height = 1118
+        if mode == "human":
+            import pygame
+
+            if self.screen is None:
+                pygame.init()
+                self.screen = pygame.display.set_mode((screen_width, screen_height))
+
+            # Load and scale all of the necessary images
+            tile_size = (screen_width * (91 / 99)) / 7
+
+            red_chip = get_image(os.path.join('img', 'C4RedPiece.png'))
+            red_chip = pygame.transform.scale(red_chip, (int(tile_size * (9 / 13)), int(tile_size * (9 / 13))))
+
+            black_chip = get_image(os.path.join('img', 'C4BlackPiece.png'))
+            black_chip = pygame.transform.scale(black_chip, (int(tile_size * (9 / 13)), int(tile_size * (9 / 13))))
+
+            board_img = get_image(os.path.join('img', 'Connect4Board.png'))
+            board_img = pygame.transform.scale(board_img, ((int(screen_width)), int(screen_height)))
+
+            self.screen.blit(board_img, (0, 0))
+
+            # Blit the necessary chips and their positions
+            for i in range(0, 42):
+                if self.board[i] == 1:
+                    self.screen.blit(red_chip, ((i % 7) * (tile_size) + (tile_size * (6 / 13)), int((i / 7)) * (tile_size) + (tile_size * (6 / 13))))
+                elif self.board[i] == 2:
+                    self.screen.blit(black_chip, ((i % 7) * (tile_size) + (tile_size * (6 / 13)), int((i / 7)) * (tile_size) + (tile_size * (6 / 13))))
+
+            pygame.display.update()
+
+        observation = np.array(pygame.surfarray.pixels3d(self.screen))
+
+        return np.transpose(observation, axes=(1, 0, 2)) if mode == "rgb_array" else None
 
     def close(self):
-        pass
+        if self.screen is not None:
+            import pygame
+            pygame.quit()
+            self.screen = None
 
     def check_for_winner(self):
         board = np.array(self.board).reshape(6, 7)
         piece = self.agents.index(self.agent_selection) + 1
 
         # Check horizontal locations for win
         column_count = 7
@@ -138,20 +185,20 @@
 
         # Check vertical locations for win
         for c in range(column_count):
             for r in range(row_count - 3):
                 if board[r][c] == piece and board[r + 1][c] == piece and board[r + 2][c] == piece and board[r + 3][c] == piece:
                     return True
 
-        # Check positively sloped diaganols
+        # Check positively sloped diagonals
         for c in range(column_count - 3):
             for r in range(row_count - 3):
                 if board[r][c] == piece and board[r + 1][c + 1] == piece and board[r + 2][c + 2] == piece and board[r + 3][c + 3] == piece:
                     return True
 
-        # Check negatively sloped diaganols
+        # Check negatively sloped diagonals
         for c in range(column_count - 3):
             for r in range(3, row_count):
                 if board[r][c] == piece and board[r - 1][c + 1] == piece and board[r - 2][c + 2] == piece and board[r - 3][c + 3] == piece:
                     return True
 
         return False
```

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/go/coords.py` & `PettingZoo-1.9.0/pettingzoo/classic/go/coords.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/go/go.py` & `PettingZoo-1.9.0/pettingzoo/classic/go/go.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/go/go_env.py` & `PettingZoo-1.9.0/pettingzoo/classic/go/go_env.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/hanabi/hanabi.py` & `PettingZoo-1.9.0/pettingzoo/classic/hanabi/hanabi.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/dou_dizhu.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/dou_dizhu.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/gin_rummy.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/gin_rummy.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/leduc_holdem.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/mahjong.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/mahjong.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/rlcard_base.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/rlcard_base.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/texas_holdem.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/texas_holdem.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/texas_holdem_no_limit.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/texas_holdem_no_limit.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rlcard_envs/uno.py` & `PettingZoo-1.9.0/pettingzoo/classic/rlcard_envs/uno.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rps/rps.py` & `PettingZoo-1.9.0/pettingzoo/sisl/waterworld/waterworld.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,84 @@
-from gym.spaces import Discrete
-import numpy as np
+from .waterworld_base import MAWaterWorld as _env
 from pettingzoo import AECEnv
 from pettingzoo.utils import agent_selector
 from pettingzoo.utils import wrappers
-
-ROCK = 0
-PAPER = 1
-SCISSORS = 2
-NONE = 3
-MOVES = ["ROCK", "PAPER", "SCISSORS", "None"]
-NUM_ITERS = 100
+import numpy as np
+from pettingzoo.utils.conversions import parallel_wrapper_fn
 
 
-def env():
-    env = raw_env()
-    env = wrappers.CaptureStdoutWrapper(env)
-    env = wrappers.AssertOutOfBoundsWrapper(env)
+def env(**kwargs):
+    env = raw_env(**kwargs)
+    env = wrappers.ClipOutOfBoundsWrapper(env)
     env = wrappers.OrderEnforcingWrapper(env)
     return env
 
 
+parallel_env = parallel_wrapper_fn(env)
+
+
 class raw_env(AECEnv):
-    """Two-player environment for rock paper scissors.
-    The observation is simply the last opponent action."""
 
-    metadata = {'render.modes': ['human'], "name": "rps_v1"}
+    metadata = {'render.modes': ['human', "rgb_array"], 'name': 'waterworld_v3'}
 
-    def __init__(self):
-        self.agents = ["player_" + str(r) for r in range(2)]
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        self.env = _env(*args, **kwargs)
+
+        self.agents = ["pursuer_" + str(r) for r in range(self.env.num_agents)]
         self.possible_agents = self.agents[:]
         self.agent_name_mapping = dict(zip(self.agents, list(range(self.num_agents))))
+        self._agent_selector = agent_selector(self.agents)
+        # spaces
+        self.action_spaces = dict(zip(self.agents, self.env.action_space))
+        self.observation_spaces = dict(
+            zip(self.agents, self.env.observation_space))
+        self.has_reset = False
 
-        self.action_spaces = {agent: Discrete(3) for agent in self.agents}
-        self.observation_spaces = {agent: Discrete(4) for agent in self.agents}
+    def seed(self, seed=None):
+        self.env.seed(seed)
 
-        self.reinit()
+    def convert_to_dict(self, list_of_list):
+        return dict(zip(self.agents, list_of_list))
 
-    def reinit(self):
+    def reset(self):
+        self.has_reset = True
+        self.env.reset()
         self.agents = self.possible_agents[:]
-        self._agent_selector = agent_selector(self.agents)
+        self._agent_selector.reinit(self.agents)
         self.agent_selection = self._agent_selector.next()
-        self.rewards = {agent: 0 for agent in self.agents}
-        self._cumulative_rewards = {agent: 0 for agent in self.agents}
-        self.dones = {agent: False for agent in self.agents}
-        self.infos = {agent: {} for agent in self.agents}
-        self.state = {agent: NONE for agent in self.agents}
-        self.observations = {agent: NONE for agent in self.agents}
-        self.num_moves = 0
-
-    def render(self, mode="human"):
-        string = ("Current state: Agent1: {} , Agent2: {}".format(MOVES[self.state[self.agents[0]]], MOVES[self.state[self.agents[1]]]))
-        print(string)
-        return string
-
-    def observe(self, agent):
-        # observation of one agent is the previous state of the other
-        return np.array(self.observations[agent])
+        self.rewards = dict(zip(self.agents, [(0) for _ in self.agents]))
+        self._cumulative_rewards = dict(zip(self.agents, [(0) for _ in self.agents]))
+        self.dones = dict(zip(self.agents, [False for _ in self.agents]))
+        self.infos = dict(zip(self.agents, [{} for _ in self.agents]))
 
     def close(self):
-        pass
+        if self.has_reset:
+            self.env.close()
 
-    def reset(self):
-        self.reinit()
+    def render(self, mode="human"):
+        return self.env.render(mode)
 
     def step(self, action):
         if self.dones[self.agent_selection]:
             return self._was_done_step(action)
         agent = self.agent_selection
 
-        self.state[self.agent_selection] = action
+        is_last = self._agent_selector.is_last()
+        self.env.step(action, self.agent_name_mapping[agent], is_last)
 
-        # collect reward if it is the last agent to act
-        if self._agent_selector.is_last():
-            self.rewards[self.agents[0]], self.rewards[self.agents[1]] = {
-                (ROCK, ROCK): (0, 0),
-                (ROCK, PAPER): (-1, 1),
-                (ROCK, SCISSORS): (1, -1),
-                (PAPER, ROCK): (1, -1),
-                (PAPER, PAPER): (0, 0),
-                (PAPER, SCISSORS): (-1, 1),
-                (SCISSORS, ROCK): (-1, 1),
-                (SCISSORS, PAPER): (1, -1),
-                (SCISSORS, SCISSORS): (0, 0),
-            }[(self.state[self.agents[0]], self.state[self.agents[1]])]
-
-            self.num_moves += 1
-            self.dones = {agent: self.num_moves >= NUM_ITERS for agent in self.agents}
-
-            # observe the current state
-            for i in self.agents:
-                self.observations[i] = self.state[self.agents[1 - self.agent_name_mapping[i]]]
-        else:
-            self.state[self.agents[1 - self.agent_name_mapping[agent]]] = NONE
-            self._clear_rewards()
+        for r in self.rewards:
+            self.rewards[r] = self.env.control_rewards[self.agent_name_mapping[r]]
+        if is_last:
+            for r in self.rewards:
+                self.rewards[r] += self.env.last_rewards[self.agent_name_mapping[r]]
 
+        if self.env.frames >= self.env.max_cycles:
+            self.dones = dict(zip(self.agents, [True for _ in self.agents]))
+        else:
+            self.dones = dict(zip(self.agents, self.env.last_dones))
         self._cumulative_rewards[self.agent_selection] = 0
         self.agent_selection = self._agent_selector.next()
         self._accumulate_rewards()
+
+    def observe(self, agent):
+        return self.env.observe(self.agent_name_mapping[agent])
```

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/rpsls/rpsls.py` & `PettingZoo-1.9.0/pettingzoo/classic/rps/rps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 from gym.spaces import Discrete
 import numpy as np
 from pettingzoo import AECEnv
 from pettingzoo.utils import agent_selector
 from pettingzoo.utils import wrappers
+from pettingzoo.utils.conversions import parallel_wrapper_fn
 
-ROCK = 0
-PAPER = 1
-SCISSORS = 2
-LIZARD = 3
-SPOCK = 4
-NONE = 5
-MOVES = ["ROCK", "PAPER", "SCISSORS", "LIZARD", "SPOCK", "None"]
-NUM_ITERS = 100
 
-
-def env():
-    env = raw_env()
+def env(**kwargs):
+    env = raw_env(**kwargs)
     env = wrappers.CaptureStdoutWrapper(env)
     env = wrappers.AssertOutOfBoundsWrapper(env)
     env = wrappers.OrderEnforcingWrapper(env)
     return env
 
 
+parallel_env = parallel_wrapper_fn(env)
+
+
 class raw_env(AECEnv):
-    """Two-player environment for rock paper scissors lizard spock.
+    """Two-player environment for rock paper scissors.
+    Expandable environment to rock paper scissors lizard spock action_6 action_7 ...
     The observation is simply the last opponent action."""
 
-    metadata = {'render.modes': ['human'], "name": "rpsls_v1"}
+    metadata = {'render.modes': ['human'], "name": "rps_v1"}
+
+    def __init__(self, num_actions=3, max_cycles=15):
+        self.max_cycles = max_cycles
+
+        # number of actions must be odd and greater than 3
+        assert num_actions > 2, "The number of actions must be equal or greater than 3."
+        assert num_actions % 2 != 0, "The number of actions must be an odd number."
+        self._moves = ["ROCK", "PAPER", "SCISSORS"]
+        if num_actions > 3:
+            # expand to lizard, spock for first extra action pair
+            self._moves.extend(("SPOCK", "LIZARD"))
+            for action in range(num_actions - 5):
+                self._moves.append("ACTION_"f'{action + 6}')
+        # none is last possible action, to satisfy discrete action space
+        self._moves.append("None")
+        self._none = num_actions
 
-    def __init__(self):
         self.agents = ["player_" + str(r) for r in range(2)]
         self.possible_agents = self.agents[:]
         self.agent_name_mapping = dict(zip(self.agents, list(range(self.num_agents))))
-
-        self.action_spaces = {agent: Discrete(5) for agent in self.agents}
-        self.observation_spaces = {agent: Discrete(6) for agent in self.agents}
+        self.action_spaces = {agent: Discrete(num_actions) for agent in self.agents}
+        self.observation_spaces = {agent: Discrete(1 + num_actions) for agent in self.agents}
 
         self.reinit()
 
     def reinit(self):
         self.agents = self.possible_agents[:]
         self._agent_selector = agent_selector(self.agents)
         self.agent_selection = self._agent_selector.next()
         self.rewards = {agent: 0 for agent in self.agents}
         self._cumulative_rewards = {agent: 0 for agent in self.agents}
         self.dones = {agent: False for agent in self.agents}
         self.infos = {agent: {} for agent in self.agents}
-        self.state = {agent: NONE for agent in self.agents}
-        self.observations = {agent: NONE for agent in self.agents}
+
+        self.state = {agent: self._none for agent in self.agents}
+        self.observations = {agent: self._none for agent in self.agents}
+
         self.num_moves = 0
 
     def render(self, mode="human"):
-        string = ("Current state: Agent1: {} , Agent2: {}".format(MOVES[self.state[self.agents[0]]], MOVES[self.state[self.agents[1]]]))
+        if len(self.agents) > 1:
+            string = ("Current state: Agent1: {} , Agent2: {}".format(self._moves[self.state[self.agents[0]]], self._moves[self.state[self.agents[1]]]))
+        else:
+            string = ("Max number of cycles reached. Episode done.")
         print(string)
         return string
 
     def observe(self, agent):
         # observation of one agent is the previous state of the other
         return np.array(self.observations[agent])
 
@@ -70,52 +85,41 @@
             return self._was_done_step(action)
         agent = self.agent_selection
 
         self.state[self.agent_selection] = action
 
         # collect reward if it is the last agent to act
         if self._agent_selector.is_last():
-            self.rewards[self.agents[0]], self.rewards[self.agents[1]] = {
-                (ROCK, ROCK): (0, 0),
-                (ROCK, PAPER): (-1, 1),
-                (ROCK, SCISSORS): (1, -1),
-                (ROCK, LIZARD): (1, -1),
-                (ROCK, SPOCK): (-1, 1),
-
-                (PAPER, ROCK): (1, -1),
-                (PAPER, PAPER): (0, 0),
-                (PAPER, SCISSORS): (-1, 1),
-                (PAPER, LIZARD): (-1, 1),
-                (PAPER, SPOCK): (1, -1),
-
-                (SCISSORS, ROCK): (-1, 1),
-                (SCISSORS, PAPER): (1, -1),
-                (SCISSORS, SCISSORS): (0, 0),
-                (SCISSORS, LIZARD): (1, -1),
-                (SCISSORS, SPOCK): (-1, 1),
-
-                (LIZARD, ROCK): (-1, 1),
-                (LIZARD, PAPER): (1, -1),
-                (LIZARD, SCISSORS): (-1, 1),
-                (LIZARD, LIZARD): (0, 0),
-                (LIZARD, SPOCK): (1, -1),
-
-                (SPOCK, ROCK): (1, -1),
-                (SPOCK, PAPER): (-1, 1),
-                (SPOCK, SCISSORS): (1, -1),
-                (SPOCK, LIZARD): (-1, 1),
-                (SPOCK, SPOCK): (0, 0),
-            }[(self.state[self.agents[0]], self.state[self.agents[1]])]
+
+            # same action => 0 reward each agent
+            if self.state[self.agents[0]] == self.state[self.agents[1]]:
+                rewards = (0, 0)
+            else:
+                # same action parity => lower action number wins
+                if (self.state[self.agents[0]] + self.state[self.agents[1]]) % 2 == 0:
+                    if self.state[self.agents[0]] > self.state[self.agents[1]]:
+                        rewards = (-1, 1)
+                    else:
+                        rewards = (1, -1)
+                # different action parity => higher action number wins
+                else:
+                    if self.state[self.agents[0]] > self.state[self.agents[1]]:
+                        rewards = (1, -1)
+                    else:
+                        rewards = (-1, 1)
+            self.rewards[self.agents[0]], self.rewards[self.agents[1]] = rewards
 
             self.num_moves += 1
-            self.dones = {agent: self.num_moves >= NUM_ITERS for agent in self.agents}
+
+            self.dones = {agent: self.num_moves >= self.max_cycles for agent in self.agents}
 
             # observe the current state
             for i in self.agents:
                 self.observations[i] = self.state[self.agents[1 - self.agent_name_mapping[i]]]
         else:
-            self.state[self.agents[1 - self.agent_name_mapping[agent]]] = NONE
+            self.state[self.agents[1 - self.agent_name_mapping[agent]]] = self._none
+
             self._clear_rewards()
 
         self._cumulative_rewards[self.agent_selection] = 0
         self.agent_selection = self._agent_selector.next()
         self._accumulate_rewards()
```

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/tictactoe/board.py` & `PettingZoo-1.9.0/pettingzoo/classic/tictactoe/board.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/classic/tictactoe/tictactoe.py` & `PettingZoo-1.9.0/pettingzoo/classic/tictactoe/tictactoe.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/__init__.py` & `PettingZoo-1.9.0/pettingzoo/magent/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from pettingzoo.utils.deprecated_module import DeprecatedModule
 
-adversarial_pursuit_v0 = DeprecatedModule("adversarial_pursuit", "v0", "v2")
-adversarial_pursuit_v1 = DeprecatedModule("adversarial_pursuit", "v1", "v2")
+adversarial_pursuit_v0 = DeprecatedModule("adversarial_pursuit", "v0", "v3")
+adversarial_pursuit_v1 = DeprecatedModule("adversarial_pursuit", "v1", "v3")
+adversarial_pursuit_v2 = DeprecatedModule("adversarial_pursuit", "v2", "v3")
 battle_v0 = DeprecatedModule("battle", "v0", "v3")
 battle_v1 = DeprecatedModule("battle", "v1", "v3")
 battle_v2 = DeprecatedModule("battle", "v2", "v3")
 battlefield_v0 = DeprecatedModule("battlefield", "v0", "v3")
 battlefield_v1 = DeprecatedModule("battlefield", "v1", "v3")
 battlefield_v2 = DeprecatedModule("battlefield", "v2", "v3")
-combined_arms_v0 = DeprecatedModule("combined_arms", "v0", "v4")
-combined_arms_v1 = DeprecatedModule("combined_arms", "v1", "v4")
-combined_arms_v2 = DeprecatedModule("combined_arms", "v2", "v4")
-combined_arms_v3 = DeprecatedModule("combined_arms", "v3", "v4")
+combined_arms_v0 = DeprecatedModule("combined_arms", "v0", "v5")
+combined_arms_v1 = DeprecatedModule("combined_arms", "v1", "v5")
+combined_arms_v2 = DeprecatedModule("combined_arms", "v2", "v5")
+combined_arms_v3 = DeprecatedModule("combined_arms", "v3", "v5")
+combined_arms_v4 = DeprecatedModule("combined_arms", "v4", "v5")
 gather_v0 = DeprecatedModule("gather", "v0", "v3")
 gather_v1 = DeprecatedModule("gather", "v1", "v3")
 gather_v2 = DeprecatedModule("gather", "v2", "v3")
 tiger_deer_v0 = DeprecatedModule("tiger_deer", "v0", "v3")
 tiger_deer_v1 = DeprecatedModule("tiger_deer", "v1", "v3")
 tiger_deer_v2 = DeprecatedModule("tiger_deer", "v2", "v3")
```

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/adversarial_pursuit_v2.py` & `PettingZoo-1.9.0/pettingzoo/magent/adversarial_pursuit_v3.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 def get_config(map_size, minimap_mode, tag_penalty):
     gw = magent.gridworld
     cfg = gw.Config()
 
     cfg.set({"map_width": map_size, "map_height": map_size})
     cfg.set({"minimap_mode": minimap_mode})
+    cfg.set({"embedding_size": 10})
 
     options = {
         'width': 2, 'length': 2, 'hp': 1, 'speed': 1,
         'view_range': gw.CircleRange(5), 'attack_range': gw.CircleRange(2),
         'attack_penalty': tag_penalty
     }
     predator = cfg.register_agent_type(
@@ -65,15 +66,15 @@
 
     cfg.add_reward_rule(gw.Event(a, 'attack', b), receiver=[a, b], value=[1, -1])
 
     return cfg
 
 
 class _parallel_env(magent_parallel_env, EzPickle):
-    metadata = {'render.modes': ['human', 'rgb_array'], 'name': "adversarial_pursuit_v2"}
+    metadata = {'render.modes': ['human', 'rgb_array'], 'name': "adversarial_pursuit_v3"}
 
     def __init__(self, map_size, minimap_mode, reward_args, max_cycles, extra_features):
         EzPickle.__init__(self, map_size, minimap_mode, reward_args, max_cycles, extra_features)
         assert map_size >= 7, "size of map must be at least 7"
         env = magent.GridWorld(get_config(map_size, minimap_mode, **reward_args), map_size=map_size)
 
         handles = env.get_handles()
```

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/battle_v3.py` & `PettingZoo-1.9.0/pettingzoo/magent/battle_v3.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/battlefield_v3.py` & `PettingZoo-1.9.0/pettingzoo/magent/battlefield_v3.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/combined_arms_v4.py` & `PettingZoo-1.9.0/pettingzoo/magent/combined_arms_v5.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pettingzoo.magent.render import Renderer
 from pettingzoo.utils import agent_selector
 from .magent_env import magent_parallel_env, make_env
 from pettingzoo.utils.conversions import from_parallel_wrapper
 from pettingzoo.utils.conversions import parallel_wrapper_fn
 from gym.utils import EzPickle
 
-
 default_map_size = 45
 max_cycles_default = 1000
 KILL_REWARD = 5
 minimap_mode_default = False
 default_reward_args = dict(step_reward=-0.005, dead_penalty=-0.1, attack_penalty=-0.1, attack_opponent_reward=0.2)
 
 
@@ -140,15 +139,15 @@
         if not (0 < x < width - 1 and 0 < y < height - 1):
             assert False
     env.add_agents(handles[2], method="custom", pos=pos[0])
     env.add_agents(handles[3], method="custom", pos=pos[1])
 
 
 class _parallel_env(magent_parallel_env, EzPickle):
-    metadata = {'render.modes': ['human', 'rgb_array'], 'name': "combined_arms_v4"}
+    metadata = {'render.modes': ['human', 'rgb_array'], 'name': "combined_arms_v5"}
 
     def __init__(self, map_size, minimap_mode, reward_args, max_cycles, extra_features):
         EzPickle.__init__(self, map_size, minimap_mode, reward_args, max_cycles, extra_features)
         assert map_size >= 16, "size of map must be at least 16"
         env = magent.GridWorld(load_config(map_size, minimap_mode, **reward_args))
         reward_vals = np.array([KILL_REWARD] + list(reward_args.values()))
         reward_range = [np.minimum(reward_vals, 0).sum(), np.maximum(reward_vals, 0).sum()]
```

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/gather_v3.py` & `PettingZoo-1.9.0/pettingzoo/magent/gather_v3.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/magent_env.py` & `PettingZoo-1.9.0/pettingzoo/magent/magent_env.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,36 +23,48 @@
     def __init__(self, env, active_handles, names, map_size, max_cycles, reward_range, minimap_mode, extra_features):
         self.map_size = map_size
         self.max_cycles = max_cycles
         self.minimap_mode = minimap_mode
         self.extra_features = extra_features
         self.env = env
         self.handles = active_handles
+        self._all_handles = self.env.get_handles()
         env.reset()
         self.generate_map()
-
         self.team_sizes = team_sizes = [env.get_num(handle) for handle in self.handles]
         self.agents = [f"{names[j]}_{i}" for j in range(len(team_sizes)) for i in range(team_sizes[j])]
         self.possible_agents = self.agents[:]
 
         num_actions = [env.get_action_space(handle)[0] for handle in self.handles]
         action_spaces_list = [Discrete(num_actions[j]) for j in range(len(team_sizes)) for i in range(team_sizes[j])]
         # may change depending on environment config? Not sure.
         team_obs_shapes = self._calc_obs_shapes()
+        state_shape = self._calc_state_shape()
         observation_space_list = [Box(low=0., high=2., shape=team_obs_shapes[j], dtype=np.float32) for j in range(len(team_sizes)) for i in range(team_sizes[j])]
+
+        self.state_space = Box(low=0., high=2., shape=state_shape, dtype=np.float32)
         reward_low, reward_high = reward_range
+
         if extra_features:
             for space in observation_space_list:
                 idx = space.shape[2] - 3 if minimap_mode else space.shape[2] - 1
                 space.low[:, :, idx] = reward_low
                 space.high[:, :, idx] = reward_high
+            idx_state = self.state_space.shape[2] - 3 if minimap_mode else self.state_space.shape[2] - 1
+            self.state_space.low[:, :, idx_state] = reward_low
+            self.state_space.high[:, :, idx_state] = reward_high
 
         self.action_spaces = {agent: space for agent, space in zip(self.agents, action_spaces_list)}
         self.observation_spaces = {agent: space for agent, space in zip(self.agents, observation_space_list)}
+
         self._zero_obs = {agent: np.zeros_like(space.low) for agent, space in self.observation_spaces.items()}
+        self.base_state = np.zeros(self.state_space.shape)
+        walls = self.env._get_walls_info()
+        wall_x, wall_y = zip(*walls)
+        self.base_state[wall_x, wall_y, 0] = 1
         self._renderer = None
         self.frames = 0
 
     def seed(self, seed=None):
         if seed is None:
             seed = seeding.create_seed(seed, max_bytes=4)
         self.env.set_seed(seed)
@@ -65,14 +77,22 @@
         feat_size = [[fs[0]] for fs in feature_spaces]
         for feature_space in feat_size:
             if not self.extra_features:
                 feature_space[0] = 2 if self.minimap_mode else 0
         obs_spaces = [(view_space[:2] + (view_space[2] + feature_space[0],)) for view_space, feature_space in zip(view_spaces, feat_size)]
         return obs_spaces
 
+    def _calc_state_shape(self):
+        feature_spaces = [self.env.get_feature_space(handle) for handle in self._all_handles]
+
+        # map channel and agent pair channel. Remove global agent position when minimap mode and extra features
+        state_depth = (max(feature_spaces)[0] - 2) * self.extra_features + 1 + len(self._all_handles) * 2
+
+        return (self.map_size, self.map_size, state_depth)
+
     def render(self, mode="human"):
         if self._renderer is None:
             self._renderer = Renderer(self.env, self.map_size, mode)
         assert mode == self._renderer.mode, "mode must be consistent across render calls"
         return self._renderer.render(mode)
 
     def close(self):
@@ -92,22 +112,20 @@
         observes = [None] * self.max_num_agents
         for handle in self.handles:
             ids = self.env.get_agent_id(handle)
             view, features = self.env.get_observation(handle)
 
             if self.minimap_mode and not self.extra_features:
                 features = features[:, -2:]
-
             if self.minimap_mode or self.extra_features:
                 feat_reshape = np.expand_dims(np.expand_dims(features, 1), 1)
                 feat_img = np.tile(feat_reshape, (1, view.shape[1], view.shape[2], 1))
                 fin_obs = np.concatenate([view, feat_img], axis=-1)
             else:
                 fin_obs = np.copy(view)
-
             for id, obs in zip(ids, fin_obs):
                 observes[id] = obs
 
         ret_agents = set(self.agents)
         return {agent: obs if obs is not None else self._zero_obs[agent] for agent, obs in zip(self.possible_agents, observes) if agent in ret_agents}
 
     def _all_rewards(self):
@@ -123,14 +141,40 @@
         if not step_done:
             for handle in self.handles:
                 ids = self.env.get_agent_id(handle)
                 dones[ids] = ~self.env.get_alive(handle)
         ret_agents = set(self.agents)
         return {agent: bool(done) for agent, done in zip(self.possible_agents, dones) if agent in ret_agents}
 
+    def state(self):
+        '''
+        Returns an observation of the global environment
+        '''
+        state = np.copy(self.base_state)
+
+        for handle in self._all_handles:
+            view, features = self.env.get_observation(handle)
+
+            pos = self.env.get_pos(handle)
+            pos_x, pos_y = zip(*pos)
+            state[pos_x, pos_y, 1 + handle.value * 2] = 1
+            state[pos_x, pos_y, 2 + handle.value * 2] = view[:, view.shape[1] // 2, view.shape[2] // 2, 2]
+
+            if self.extra_features:
+                add_zeros = np.zeros((features.shape[0], state.shape[2] - (1 + len(self.team_sizes) * 2 + features.shape[1])))
+
+                rewards = features[:, -1]
+                actions = features[:, :-1]
+                actions = np.concatenate((actions, add_zeros), axis=1)
+                rewards = rewards.reshape(len(rewards), 1)
+                state_features = np.hstack((actions, rewards))
+
+                state[pos_x, pos_y, 1 + len(self.team_sizes) * 2:] = state_features
+        return state
+
     def step(self, all_actions):
         action_list = [0] * self.max_num_agents
         self.agents = [agent for agent in self.agents if not self.all_dones[agent]]
         self.env.clear_dead()
         for i, agent in enumerate(self.possible_agents):
             if agent in all_actions:
                 action_list[i] = all_actions[agent]
```

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/render.py` & `PettingZoo-1.9.0/pettingzoo/magent/render.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 
 class Renderer:
     def __init__(self, env, map_size, mode):
         import pygame
         self.env = env
         self.mode = mode
         self.handles = self.env.get_handles()
-
         base_resolution = (map_size * 8, map_size * 8 + 15)
         if mode == "human":
             pygame.init()
             pygame.display.init()
             infoObject = pygame.display.Info()
             screen_size = (infoObject.current_w - 50, infoObject.current_h - 50)
             self.resolution = resolution = np.min([screen_size, base_resolution], axis=0)
@@ -133,14 +132,15 @@
         env = self.env
         self.groups = env._get_groups_info()
         resolution = self.resolution
 
         grid_map = np.zeros((resolution[0], resolution[1], 3), dtype=np.int16)
         view_position = [self.map_size[0] / 2 * grid_size - resolution[0] / 2,
                          self.map_size[1] / 2 * grid_size - resolution[1] / 2]
+
         groups = self.groups
         banner_formatter = self.banner_formatter
         status = True
         triggered = False
         # x_range: which vertical gridlines should be shown on the display
         # y_range: which horizontal gridlines should be shown on the display
         x_range = (
```

### Comparing `PettingZoo-1.8.2/pettingzoo/magent/tiger_deer_v3.py` & `PettingZoo-1.9.0/pettingzoo/magent/tiger_deer_v3.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/__init__.py` & `PettingZoo-1.9.0/pettingzoo/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/core.py` & `PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/core.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/rendering.py` & `PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/rendering.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/secrcode.ttf` & `PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/secrcode.ttf`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/_mpe_utils/simple_env.py` & `PettingZoo-1.9.0/pettingzoo/mpe/_mpe_utils/simple_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,37 +35,45 @@
         self._index_map = {agent.name: idx for idx, agent in enumerate(self.world.agents)}
 
         self._agent_selector = agent_selector(self.agents)
 
         # set spaces
         self.action_spaces = dict()
         self.observation_spaces = dict()
+        state_dim = 0
         for agent in self.world.agents:
             space_dim = 1
             if agent.movable:
                 space_dim *= self.world.dim_p * 2 + 1
             if not agent.silent:
                 space_dim *= self.world.dim_c
 
             obs_dim = len(self.scenario.observation(agent, self.world))
+            state_dim += obs_dim
             self.action_spaces[agent.name] = spaces.Discrete(space_dim)
             self.observation_spaces[agent.name] = spaces.Box(low=-np.float32(np.inf), high=+np.float32(np.inf), shape=(obs_dim,), dtype=np.float32)
 
+        self.state_space = spaces.Box(low=-np.float32(np.inf), high=+np.float32(np.inf), shape=(state_dim,), dtype=np.float32)
+
         self.steps = 0
 
         self.current_actions = [None] * self.num_agents
 
         self.viewer = None
 
     def seed(self, seed=None):
         self.np_random, seed = seeding.np_random(seed)
 
     def observe(self, agent):
         return self.scenario.observation(self.world.agents[self._index_map[agent]], self.world).astype(np.float32)
 
+    def state(self):
+        states = tuple([self.scenario.observation(self.world.agents[self._index_map[agent]], self.world).astype(np.float32) for agent in self.possible_agents])
+        return np.concatenate(states, axis=None)
+
     def reset(self):
         self.scenario.reset_world(self.world, self.np_random)
 
         self.agents = self.possible_agents[:]
         self.rewards = {name: 0. for name in self.agents}
         self._cumulative_rewards = {name: 0. for name in self.agents}
         self.dones = {name: False for name in self.agents}
```

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_adversary.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_adversary.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_crypto.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_crypto.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_push.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_push.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_reference.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_reference.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_speaker_listener.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_speaker_listener.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_spread.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_spread.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_tag.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_tag.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/scenarios/simple_world_comm.py` & `PettingZoo-1.9.0/pettingzoo/mpe/scenarios/simple_world_comm.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/simple_reference_v2.py` & `PettingZoo-1.9.0/pettingzoo/mpe/simple_reference_v2.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/simple_spread_v2.py` & `PettingZoo-1.9.0/pettingzoo/mpe/simple_spread_v2.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/simple_tag_v2.py` & `PettingZoo-1.9.0/pettingzoo/mpe/simple_tag_v2.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/mpe/simple_world_comm_v2.py` & `PettingZoo-1.9.0/pettingzoo/mpe/simple_world_comm_v2.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/__init__.py` & `PettingZoo-1.9.0/pettingzoo/sisl/__init__.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/multiwalker/multiwalker.py` & `PettingZoo-1.9.0/pettingzoo/sisl/multiwalker/multiwalker.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/multiwalker/multiwalker_base.py` & `PettingZoo-1.9.0/pettingzoo/sisl/multiwalker/multiwalker_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     def __init__(self, world, init_x=TERRAIN_STEP * TERRAIN_STARTPAD / 2,
                  init_y=TERRAIN_HEIGHT + 2 * LEG_H, n_walkers=2, seed=None):
         self.world = world
         self._n_walkers = n_walkers
         self.hull = None
         self.init_x = init_x
         self.init_y = init_y
+        self.walker_id = -int(self.init_x)
         self._seed(seed)
 
     def _destroy(self):
         if not self.hull:
             return
         self.world.DestroyBody(self.hull)
         self.hull = None
@@ -104,26 +105,24 @@
 
     def _seed(self, seed=None):
         self.np_random, seed = seeding.np_random(seed)
         return [seed]
 
     def _reset(self):
         self._destroy()
-
         init_x = self.init_x
         init_y = self.init_y
         self.hull = self.world.CreateDynamicBody(
             position=(init_x, init_y),
             fixtures=fixtureDef(
                 shape=polygonShape(
                     vertices=[(x / SCALE, y / SCALE) for x, y in HULL_POLY]),
                 density=5.0,
                 friction=0.1,
-                categoryBits=0x002,
-                # maskBits=(0x001 & 0x002),  # collide only with ground
+                groupIndex=self.walker_id,
                 restitution=0.0)  # 0.99 bouncy
         )
         self.hull.color1 = (0.5, 0.4, 0.9)
         self.hull.color2 = (0.3, 0.3, 0.5)
         self.hull.ApplyForceToCenter((self.np_random.uniform(-INITIAL_RANDOM, INITIAL_RANDOM), 0),
                                      True)
 
@@ -133,16 +132,15 @@
             leg = self.world.CreateDynamicBody(
                 position=(init_x, init_y - LEG_H / 2 - LEG_DOWN),
                 angle=(i * 0.05),
                 fixtures=fixtureDef(
                     shape=polygonShape(box=(LEG_W / 2, LEG_H / 2)),
                     density=1.0,
                     restitution=0.0,
-                    categoryBits=0x002,
-                    maskBits=0x001
+                    groupIndex=self.walker_id,
                 )  # collide with ground only
             )
             leg.color1 = (0.6 - i / 10., 0.3 - i / 10., 0.5 - i / 10.)
             leg.color2 = (0.4 - i / 10., 0.2 - i / 10., 0.3 - i / 10.)
             rjd = revoluteJointDef(
                 bodyA=self.hull,
                 bodyB=leg,
@@ -161,16 +159,15 @@
             lower = self.world.CreateDynamicBody(
                 position=(init_x, init_y - LEG_H * 3 / 2 - LEG_DOWN),
                 angle=(i * 0.05),
                 fixtures=fixtureDef(
                     shape=polygonShape(box=(0.8 * LEG_W / 2, LEG_H / 2)),
                     density=1.0,
                     restitution=0.0,
-                    categoryBits=0x0020,
-                    maskBits=0x001
+                    groupIndex=self.walker_id,
                 )
             )
             lower.color1 = (0.6 - i / 10., 0.3 - i / 10., 0.5 - i / 10.)
             lower.color2 = (0.4 - i / 10., 0.2 - i / 10., 0.3 - i / 10.)
             rjd = revoluteJointDef(
                 bodyA=leg,
                 bodyB=lower,
@@ -681,16 +678,16 @@
 
         self.terrain_poly = []
         for i in range(self.terrain_length - 1):
             poly = [(self.terrain_x[i], self.terrain_y[i]),
                     (self.terrain_x[i + 1], self.terrain_y[i + 1])]
             t = self.world.CreateStaticBody(fixtures=fixtureDef(
                 shape=edgeShape(vertices=poly),
-                friction=FRICTION,
-                categoryBits=0x0001,))
+                friction=FRICTION
+            ))
             color = (0.3, 1.0 if i % 2 == 0 else 0.8, 0.3)
             t.color1 = color
             t.color2 = color
             self.terrain.append(t)
             color = (0.4, 0.6, 0.3)
             poly += [(poly[1][0], 0), (poly[0][0], 0)]
             self.terrain_poly.append((poly, color))
```

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/manual_control.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/manual_control.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/pursuit.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/pursuit.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/pursuit_base.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/pursuit_base.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/agent_layer.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/agent_layer.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/agent_utils.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/agent_utils.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/controllers.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/discrete_agent.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/discrete_agent.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/pursuit/utils/two_d_maps.py` & `PettingZoo-1.9.0/pettingzoo/sisl/pursuit/utils/two_d_maps.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/sisl/waterworld/waterworld_base.py` & `PettingZoo-1.9.0/pettingzoo/sisl/waterworld/waterworld_base.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/all_modules.py` & `PettingZoo-1.9.0/test/all_modules.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from pettingzoo.atari import basketball_pong_v1
+from pettingzoo.atari import basketball_pong_v2
 from pettingzoo.atari import boxing_v1
 from pettingzoo.atari import combat_plane_v1
 from pettingzoo.atari import combat_tank_v1
 from pettingzoo.atari import double_dunk_v2
 from pettingzoo.atari import entombed_competitive_v2
 from pettingzoo.atari import entombed_cooperative_v2
 from pettingzoo.atari import flag_capture_v1
-from pettingzoo.atari import foozpong_v1
+from pettingzoo.atari import foozpong_v2
 from pettingzoo.atari import ice_hockey_v1
 from pettingzoo.atari import joust_v2
 from pettingzoo.atari import mario_bros_v2
 from pettingzoo.atari import maze_craze_v2
 from pettingzoo.atari import othello_v2
-from pettingzoo.atari import pong_v1
-from pettingzoo.atari import quadrapong_v2
+from pettingzoo.atari import pong_v2
+from pettingzoo.atari import quadrapong_v3
 from pettingzoo.atari import space_invaders_v1
 from pettingzoo.atari import space_war_v1
 from pettingzoo.atari import surround_v1
 from pettingzoo.atari import tennis_v2
 from pettingzoo.atari import video_checkers_v3
-from pettingzoo.atari import volleyball_pong_v1
+from pettingzoo.atari import volleyball_pong_v2
 from pettingzoo.atari import wizard_of_wor_v2
 from pettingzoo.atari import warlords_v2
 
 from pettingzoo.classic import chess_v3
 from pettingzoo.classic import checkers_v3
 from pettingzoo.classic import rps_v1
-from pettingzoo.classic import rpsls_v1
 from pettingzoo.classic import connect_four_v3
 from pettingzoo.classic import tictactoe_v3
 from pettingzoo.classic import leduc_holdem_v3
 from pettingzoo.classic import mahjong_v3
 from pettingzoo.classic import texas_holdem_v3
 from pettingzoo.classic import texas_holdem_no_limit_v3
 from pettingzoo.classic import uno_v3
@@ -43,17 +42,17 @@
 from pettingzoo.butterfly import knights_archers_zombies_v7
 from pettingzoo.butterfly import pistonball_v4
 from pettingzoo.butterfly import cooperative_pong_v2
 from pettingzoo.butterfly import prison_v3
 from pettingzoo.butterfly import prospector_v4
 
 from pettingzoo.magent import battle_v3
-from pettingzoo.magent import adversarial_pursuit_v2
+from pettingzoo.magent import adversarial_pursuit_v3
 from pettingzoo.magent import gather_v3
-from pettingzoo.magent import combined_arms_v4
+from pettingzoo.magent import combined_arms_v5
 from pettingzoo.magent import tiger_deer_v3
 from pettingzoo.magent import battlefield_v3
 
 from pettingzoo.mpe import simple_adversary_v2
 from pettingzoo.mpe import simple_crypto_v2
 from pettingzoo.mpe import simple_push_v2
 from pettingzoo.mpe import simple_reference_v2
@@ -75,43 +74,42 @@
     "butterfly/cooperative_pong",
     "butterfly/prison",
     "butterfly/prospector",
     "sisl/pursuit"
 }
 
 all_environments = {
-    "atari/basketball_pong_v1": basketball_pong_v1,
+    "atari/basketball_pong_v2": basketball_pong_v2,
     "atari/boxing_v1": boxing_v1,
     "atari/combat_tank_v1": combat_tank_v1,
     "atari/combat_plane_v1": combat_plane_v1,
     "atari/double_dunk_v2": double_dunk_v2,
     "atari/entombed_cooperative_v2": entombed_cooperative_v2,
     "atari/entombed_competitive_v2": entombed_competitive_v2,
     "atari/flag_capture_v1": flag_capture_v1,
-    "atari/foozpong_v1": foozpong_v1,
+    "atari/foozpong_v2": foozpong_v2,
     "atari/joust_v2": joust_v2,
     "atari/ice_hockey_v1": ice_hockey_v1,
     "atari/maze_craze_v2": maze_craze_v2,
     "atari/mario_bros_v2": mario_bros_v2,
     "atari/othello_v2": othello_v2,
-    "atari/pong_v1": pong_v1,
-    "atari/quadrapong_v2": quadrapong_v2,
+    "atari/pong_v2": pong_v2,
+    "atari/quadrapong_v3": quadrapong_v3,
     "atari/space_invaders_v1": space_invaders_v1,
     "atari/space_war_v1": space_war_v1,
     "atari/surround_v1": surround_v1,
     "atari/tennis_v2": tennis_v2,
     "atari/video_checkers_v3": video_checkers_v3,
-    "atari/volleyball_pong_v1": volleyball_pong_v1,
+    "atari/volleyball_pong_v2": volleyball_pong_v2,
     "atari/wizard_of_wor_v2": wizard_of_wor_v2,
     "atari/warlords_v2": warlords_v2,
 
     "classic/chess_v3": chess_v3,
     "classic/checkers_v3": checkers_v3,
     "classic/rps_v1": rps_v1,
-    "classic/rpsls_v1": rpsls_v1,
     "classic/connect_four_v3": connect_four_v3,
     "classic/tictactoe_v3": tictactoe_v3,
     "classic/leduc_holdem_v3": leduc_holdem_v3,
     "classic/mahjong_v3": mahjong_v3,
     "classic/texas_holdem_v3": texas_holdem_v3,
     "classic/texas_holdem_no_limit_v3": texas_holdem_no_limit_v3,
     "classic/uno_v3": uno_v3,
@@ -123,18 +121,18 @@
 
     "butterfly/knights_archers_zombies_v7": knights_archers_zombies_v7,
     "butterfly/pistonball_v4": pistonball_v4,
     "butterfly/cooperative_pong_v2": cooperative_pong_v2,
     "butterfly/prison_v3": prison_v3,
     "butterfly/prospector_v4": prospector_v4,
 
-    "magent/adversarial_pursuit_v2": adversarial_pursuit_v2,
+    "magent/adversarial_pursuit_v3": adversarial_pursuit_v3,
     "magent/battle_v3": battle_v3,
     "magent/battlefield_v3": battlefield_v3,
-    "magent/combined_arms_v4": combined_arms_v4,
+    "magent/combined_arms_v5": combined_arms_v5,
     "magent/gather_v3": gather_v3,
     "magent/tiger_deer_v3": tiger_deer_v3,
 
     "mpe/simple_adversary_v2": simple_adversary_v2,
     "mpe/simple_crypto_v2": simple_crypto_v2,
     "mpe/simple_push_v2": simple_push_v2,
     "mpe/simple_reference_v2": simple_reference_v2,
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/all_parameter_combs.py` & `PettingZoo-1.9.0/test/all_parameter_combs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .all_modules import *  # noqa: F403
 
 import pytest
 from .all_modules import all_environments
-from.api_test import api_test
+from pettingzoo.test.api_test import api_test
 
 
 parameterized_envs = [
     (boxing_v1.env, dict(obs_type="grayscale_image")),
     (boxing_v1.env, dict(obs_type="ram")),
     (boxing_v1.env, dict(full_action_space=False)),
 
@@ -74,18 +74,18 @@
     # Commented out due to rare segfault
     (tiger_deer_v3.env, dict(minimap_mode=True)),
     (battle_v3.env, dict(minimap_mode=False)),
     (battlefield_v3.env, dict(minimap_mode=False, extra_features=False)),
     (battlefield_v3.env, dict(minimap_mode=False, extra_features=True)),
     (battlefield_v3.env, dict(minimap_mode=True, extra_features=False)),
     (battlefield_v3.env, dict(minimap_mode=True, extra_features=True)),
-    (adversarial_pursuit_v2.env, dict(map_size=15)),
+    (adversarial_pursuit_v3.env, dict(map_size=15)),
     (battle_v3.env, dict(map_size=15)),
     (battlefield_v3.env, dict(map_size=46)),
-    (combined_arms_v4.env, dict(map_size=16)),
+    (combined_arms_v5.env, dict(map_size=16)),
     (tiger_deer_v3.env, dict(map_size=15)),
 
     (simple_adversary_v2.env, dict(N=4)),
     (simple_reference_v2.env, dict(local_ratio=0.2)),
     (simple_spread_v2.env, dict(N=5)),
     (simple_tag_v2.env, dict(num_good=5, num_adversaries=10, num_obstacles=4)),
     (simple_tag_v2.env, dict(num_good=1, num_adversaries=1, num_obstacles=1)),
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/api_test.py` & `PettingZoo-1.9.0/pettingzoo/test/api_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         assert set(env.dones.keys()) == (set(env.agents)), "agents should not be given a done if they were done last turn"
         assert set(env.infos.keys()) == (set(env.agents)), "agents should not be given an info if they were done last turn"
         assert set(env.agents).issubset(set(env.possible_agents)), "possible agents should always include all agents"
         if done:
             live_agents.remove(agent)
             has_finished.add(agent)
         assert env.agents == live_agents, "environment must delete agents as the game continues"
-        if env.env_done:
+        if not env.agents:
             assert has_finished == set(env.possible_agents), "not all agents finished, some were skipped over"
             break
 
         if isinstance(env.observation_spaces[agent], gym.spaces.Box):
             assert env.observation_spaces[agent].dtype == prev_observe.dtype
         if not env.observation_spaces[agent].contains(prev_observe):
             print("Out of bounds observation: ", prev_observe)
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/bombardment_test.py` & `PettingZoo-1.9.0/pettingzoo/test/bombardment_test.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/ci_test.py` & `PettingZoo-1.9.0/test/ci_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import sys
-from .api_test import api_test
-from .performance_benchmark import performance_benchmark
-from .manual_control_test import manual_control_test
-from .all_modules import all_environments, manual_environments
-from .all_modules import all_prefixes
-from .render_test import render_test
-from .seed_test import seed_test
-from .save_obs_test import test_save_obs
-from .max_cycles_test import max_cycles_test
-from .parallel_test import parallel_api_test
+from pettingzoo.test.api_test import api_test
+from pettingzoo.test.performance_benchmark import performance_benchmark
+from pettingzoo.test.manual_control_test import manual_control_test
+from .all_modules import all_environments, manual_environments, all_prefixes
+from pettingzoo.test.render_test import render_test
+from pettingzoo.test.seed_test import seed_test
+from pettingzoo.test.save_obs_test import test_save_obs
+from pettingzoo.test.max_cycles_test import max_cycles_test
+from pettingzoo.test.parallel_test import parallel_api_test
 
 assert len(sys.argv) == 7, "ci_test expects 5 arguments: env_id, num_cycles, render, manual_control, performance, save_obs"
 
 num_cycles = int(sys.argv[2])
 render = sys.argv[3] == 'True'
 manual_control = sys.argv[4] == 'True'
 performance = sys.argv[5] == 'True'
@@ -31,16 +30,15 @@
         api_test(_env, num_cycles=num_cycles, render=render, verbose_progress=True)
     except Exception as e:
         error_collected.append("API Test: " + str(e))
 
     if "classic/" not in env_id:
         parallel_api_test(env_module.parallel_env(), num_cycles=num_cycles)
 
-    if "prospector" not in env_id:
-        seed_test(env_module.env, num_cycles)
+    seed_test(env_module.env, num_cycles)
 
     if "classic/" not in env_id:
         max_cycles_test(env_module)
 
     # error_test(env_module.env())
 
     if save_obs:
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/manual_control_test.py` & `PettingZoo-1.9.0/pettingzoo/test/manual_control_test.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/parallel_test.py` & `PettingZoo-1.9.0/pettingzoo/test/parallel_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
             assert set(done.keys()) == (set(par_env.agents)), "agents should not be given a done if they were done last turn"
             assert set(info.keys()) == (set(par_env.agents)), "agents should not be given a info if they were done last turn"
             assert set(par_env.agents).issubset(set(par_env.possible_agents)), "possible agents should include all agents always"
             for agent, d in done.items():
                 if d:
                     live_agents.remove(agent)
             has_finished |= {agent for agent, d in done.items() if d}
-            if par_env.env_done:
+            if not par_env.agents:
                 assert has_finished == set(par_env.possible_agents), "not all agents finished, some were skipped over"
                 break
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/performance_benchmark.py` & `PettingZoo-1.9.0/pettingzoo/test/performance_benchmark.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/print_test.py` & `PettingZoo-1.9.0/test/print_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-dir_names = ["butterfly", "sisl", "magent", "mpe"]
+dir_names = ["butterfly", "sisl", "magent", "mpe", "atari"]
 
 had_error = False
 
 for name in dir_names:
     root_dir = os.path.join("pettingzoo", name)
 
     for _dir, subdirs, files in os.walk(root_dir):
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/pytest_runner.py` & `PettingZoo-1.9.0/test/pytest_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import pytest
 import pickle
 from .all_modules import all_environments
-from .api_test import api_test
-from .seed_test import seed_test
-from .parallel_test import parallel_api_test
-from .max_cycles_test import max_cycles_test
-from .state_test import state_test
+from pettingzoo.test.api_test import api_test
+from pettingzoo.test.seed_test import seed_test
+from pettingzoo.test.parallel_test import parallel_api_test
+from pettingzoo.test.max_cycles_test import max_cycles_test
+from pettingzoo.test.state_test import state_test
 import os
 
 
 @pytest.mark.parametrize(("name", "env_module"), list(all_environments.items()))
 def test_module(name, env_module):
     _env = env_module.env()
     assert str(_env) == os.path.basename(name)
     api_test(_env)
     if "classic/" not in name:
         parallel_api_test(env_module.parallel_env())
 
-    test_kept_state = "prospector" not in name
-    seed_test(env_module.env, 50, test_kept_state)
+    seed_test(env_module.env, 50)
 
     if "classic/" not in name:
         max_cycles_test(env_module)
 
-    if "butterfly/" in name:
+    if ("butterfly/" in name) or ("mpe/" in name) or ("magent/" in name):
         state_test(_env, env_module.parallel_env())
 
     recreated_env = pickle.loads(pickle.dumps(_env))
     api_test(recreated_env)
```

### Comparing `PettingZoo-1.8.2/pettingzoo/test/render_test.py` & `PettingZoo-1.9.0/pettingzoo/test/render_test.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/save_obs_test.py` & `PettingZoo-1.9.0/pettingzoo/test/save_obs_test.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/seed_test.py` & `PettingZoo-1.9.0/pettingzoo/test/seed_test.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/test/state_test.py` & `PettingZoo-1.9.0/pettingzoo/test/state_test.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/agent_selector.py` & `PettingZoo-1.9.0/pettingzoo/utils/agent_selector.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/average_total_reward.py` & `PettingZoo-1.9.0/pettingzoo/utils/average_total_reward.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/capture_stdout.py` & `PettingZoo-1.9.0/pettingzoo/utils/capture_stdout.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/conversions.py` & `PettingZoo-1.9.0/pettingzoo/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/env.py` & `PettingZoo-1.9.0/pettingzoo/utils/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,14 @@
     def num_agents(self):
         return len(self.agents)
 
     @property
     def max_num_agents(self):
         return len(self.possible_agents)
 
-    @property
-    def env_done(self):
-        return not self.agents
-
     def _dones_step_first(self):
         '''
         Makes .agent_selection point to first done agent. Stores old value of agent_selection
         so that _was_done_step can restore the variable after the done agent steps.
         '''
         _dones_order = [agent for agent in self.agents if self.dones[agent]]
         if _dones_order:
@@ -248,18 +244,14 @@
     def num_agents(self):
         return len(self.agents)
 
     @property
     def max_num_agents(self):
         return len(self.possible_agents)
 
-    @property
-    def env_done(self):
-        return not self.agents
-
     def __str__(self):
         '''
         returns a name which looks like: "space_invaders_v1" by default
         '''
         if hasattr(self, 'metadata'):
             return self.metadata.get('name', self.__class__.__name__)
         else:
```

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/env_logger.py` & `PettingZoo-1.9.0/pettingzoo/utils/env_logger.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/generate_gif.py` & `PettingZoo-1.9.0/pettingzoo/utils/generate_gif.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/random_demo.py` & `PettingZoo-1.9.0/pettingzoo/utils/random_demo.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/save_observation.py` & `PettingZoo-1.9.0/pettingzoo/utils/save_observation.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/wrappers/assert_out_of_bounds.py` & `PettingZoo-1.9.0/pettingzoo/utils/wrappers/assert_out_of_bounds.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/wrappers/base.py` & `PettingZoo-1.9.0/pettingzoo/utils/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/wrappers/capture_stdout.py` & `PettingZoo-1.9.0/pettingzoo/utils/wrappers/capture_stdout.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/wrappers/clip_out_of_bounds.py` & `PettingZoo-1.9.0/pettingzoo/utils/wrappers/clip_out_of_bounds.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/wrappers/order_enforcing.py` & `PettingZoo-1.9.0/pettingzoo/utils/wrappers/order_enforcing.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/pettingzoo/utils/wrappers/terminate_illegal.py` & `PettingZoo-1.9.0/pettingzoo/utils/wrappers/terminate_illegal.py`

 * *Files identical despite different names*

### Comparing `PettingZoo-1.8.2/setup.py` & `PettingZoo-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from setuptools import find_packages, setup
-
 with open("README.md", "r") as fh:
     long_description = ""
     header_count = 0
     for line in fh:
         if line.startswith("##"):
             header_count += 1
         if header_count < 2:
@@ -20,18 +19,18 @@
     for line in lines:
         if line.startswith("__version__"):
             return line.strip().split()[-1].strip().strip('"')
     raise RuntimeError("bad version data in __init__.py")
 
 
 extras = {
-    "atari": ["multi_agent_ale_py==0.1.10", "pygame==2.0.0"],
+    "atari": ["multi_agent_ale_py==0.1.11", "pygame==2.0.0"],
     "classic": ["python-chess==0.31.4", "rlcard==0.2.8", "hanabi_learning_environment==0.0.1"],
     "butterfly": ["pygame==2.0.0", "pymunk==6.0.0"],
-    "magent": ["magent==0.1.13"],
+    "magent": ["magent==0.1.14"],
     "mpe": ["pyglet>=1.4.0"],
     "sisl": ["pygame==2.0.0", "box2d-py==2.3.5"],
     "tests": ["pynput"]
 }
 
 extras["all"] = extras["atari"]+extras["classic"]+extras["butterfly"]+extras["magent"]+extras["mpe"]+extras["sisl"]
 
@@ -43,15 +42,15 @@
     author_email="justinkterry@gmail.com",
     description="Gym for multi-agent reinforcement learning",
     url='https://github.com/PettingZoo-Team/PettingZoo',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["Reinforcement Learning", "game", "RL", "AI", "gym"],
     python_requires=">=3.6, <3.10",
-    packages=find_packages(),
+    packages=["pettingzoo"] + ["pettingzoo." + pkg for pkg in find_packages("pettingzoo")],
     include_package_data=True,
     install_requires=[
         "numpy>=1.18.0",
         "gym>=0.18.0"
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

