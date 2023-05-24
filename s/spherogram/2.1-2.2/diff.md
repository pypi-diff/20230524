# Comparing `tmp/spherogram-2.1.tar.gz` & `tmp/spherogram-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spherogram-2.1.tar", last modified: Fri Nov  5 15:02:20 2021, max compression
+gzip compressed data, was "spherogram-2.2.tar", last modified: Tue May 23 20:01:39 2023, max compression
```

## Comparing `spherogram-2.1.tar` & `spherogram-2.2.tar`

### file list

```diff
@@ -1,130 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.801681 spherogram-2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-11-05 15:02:09.000000 spherogram-2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-11-05 15:02:20.801681 spherogram-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2021-11-05 15:02:09.000000 spherogram-2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.785681 spherogram-2.1/dev/
--rw-r--r--   0 runner    (1001) docker     (121)    32012 2021-11-05 15:02:09.000000 spherogram-2.1/dev/DTcodes.py
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-05 15:02:09.000000 spherogram-2.1/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-11-05 15:02:09.000000 spherogram-2.1/dev/conventions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.785681 spherogram-2.1/dev/dev_jennet/
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dev_jennet/AlexanderKauffman.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dev_jennet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dev_jennet/bridge_finding.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dev_jennet/spanning_trees.py
--rw-r--r--   0 runner    (1001) docker     (121)    10782 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dev_jennet/test_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dt_issue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-11-05 15:02:09.000000 spherogram-2.1/dev/dt_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-11-05 15:02:09.000000 spherogram-2.1/dev/sage_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-11-05 15:02:09.000000 spherogram-2.1/dev/sage_link_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     4468 2021-11-05 15:02:09.000000 spherogram-2.1/dev/signature.py
--rw-r--r--   0 runner    (1001) docker     (121)    21865 2021-11-05 15:02:09.000000 spherogram-2.1/dev/tangle_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.789681 spherogram-2.1/planarity_src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.793681 spherogram-2.1/planarity_src/c/
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/appconst.h
--rw-r--r--   0 runner    (1001) docker     (121)     6676 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graph.h
--rw-r--r--   0 runner    (1001) docker     (121)    16505 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphColorVertices.c
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphColorVertices.h
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphColorVertices.private.h
--rw-r--r--   0 runner    (1001) docker     (121)    23963 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphColorVertices_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (121)    18687 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphDFSUtils.c
--rw-r--r--   0 runner    (1001) docker     (121)    43741 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphDrawPlanar.c
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphDrawPlanar.h
--rw-r--r--   0 runner    (1001) docker     (121)     5452 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphDrawPlanar.private.h
--rw-r--r--   0 runner    (1001) docker     (121)    27468 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphDrawPlanar_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (121)    63389 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphEmbed.c
--rw-r--r--   0 runner    (1001) docker     (121)    23976 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphExtensions.c
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphExtensions.h
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphExtensions.private.h
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphFunctionTable.h
--rw-r--r--   0 runner    (1001) docker     (121)    28630 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphIO.c
--rw-r--r--   0 runner    (1001) docker     (121)    32754 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphIsolator.c
--rw-r--r--   0 runner    (1001) docker     (121)    11995 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK23Search.c
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK23Search.h
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK23Search.private.h
--rw-r--r--   0 runner    (1001) docker     (121)    11194 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK23Search_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (121)    84775 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK33Search.c
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK33Search.h
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK33Search.private.h
--rw-r--r--   0 runner    (1001) docker     (121)    29971 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK33Search_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (121)    60582 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK4Search.c
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK4Search.h
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK4Search.private.h
--rw-r--r--   0 runner    (1001) docker     (121)    19913 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphK4Search_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (121)    31173 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphNonplanar.c
--rw-r--r--   0 runner    (1001) docker     (121)     9689 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphOuterplanarObstruction.c
--rw-r--r--   0 runner    (1001) docker     (121)    38887 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphStructures.h
--rw-r--r--   0 runner    (1001) docker     (121)    39125 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphTests.c
--rw-r--r--   0 runner    (1001) docker     (121)    91710 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/graphUtils.c
--rw-r--r--   0 runner    (1001) docker     (121)    11972 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/listcoll.c
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/listcoll.h
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/planarity.h
--rw-r--r--   0 runner    (1001) docker     (121)     3996 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/platformTime.h
--rw-r--r--   0 runner    (1001) docker     (121)     6293 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/stack.c
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/c/stack.h
--rw-r--r--   0 runner    (1001) docker     (121)   151505 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/planarity.c
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2021-11-05 15:02:09.000000 spherogram-2.1/planarity_src/planarity.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.793681 spherogram-2.1/planarmap_src/
--rw-r--r--   0 runner    (1001) docker     (121)   166851 2021-11-05 15:02:10.000000 spherogram-2.1/planarmap_src/planarmap.c
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/planarmap.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.797681 spherogram-2.1/planarmap_src/src/
--rw-r--r--   0 runner    (1001) docker     (121)    15553 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMconjugation.c
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMconjugation.h
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMdef.c
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMdef.h
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMdisplay.h
--rw-r--r--   0 runner    (1001) docker     (121)     6519 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMenlight.c
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMenlight.h
--rw-r--r--   0 runner    (1001) docker     (121)    15985 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMextract.c
--rw-r--r--   0 runner    (1001) docker     (121)      977 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMextract.h
--rw-r--r--   0 runner    (1001) docker     (121)    12608 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMplanmap.c
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/PMplanmap.h
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/interface.h
--rw-r--r--   0 runner    (1001) docker     (121)     6579 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/stats.c
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-11-05 15:02:09.000000 spherogram-2.1/planarmap_src/src/stats.h
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-05 15:02:20.801681 spherogram-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7483 2021-11-05 15:02:09.000000 spherogram-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.797681 spherogram-2.1/spherogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-11-05 15:02:20.000000 spherogram-2.1/spherogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2021-11-05 15:02:20.000000 spherogram-2.1/spherogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-05 15:02:20.000000 spherogram-2.1/spherogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-05 15:02:20.000000 spherogram-2.1/spherogram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-11-05 15:02:20.000000 spherogram-2.1/spherogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-05 15:02:20.000000 spherogram-2.1/spherogram.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.797681 spherogram-2.1/spherogram_src/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.797681 spherogram-2.1/spherogram_src/codecs/
--rw-r--r--   0 runner    (1001) docker     (121)     7491 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/codecs/Base64LikeDT.py
--rw-r--r--   0 runner    (1001) docker     (121)    36149 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/codecs/DT.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37831 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.801681 spherogram-2.1/spherogram_src/links/
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8192 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/alexander.py
--rw-r--r--   0 runner    (1001) docker     (121)   100850 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/doc.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/draw.py
--rw-r--r--   0 runner    (1001) docker     (121)    14852 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/exhaust.py
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/extra_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    29543 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/invariants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/jones.py
--rw-r--r--   0 runner    (1001) docker     (121)     9085 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/jones_old.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/links.py
--rw-r--r--   0 runner    (1001) docker     (121)    49763 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/links_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14497 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/morse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    26240 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/orthogonal.py
--rw-r--r--   0 runner    (1001) docker     (121)    10666 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/planar_isotopy.py
--rw-r--r--   0 runner    (1001) docker     (121)     8447 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/random_links.py
--rw-r--r--   0 runner    (1001) docker     (121)    13122 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/seifert.py
--rw-r--r--   0 runner    (1001) docker     (121)    22766 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/simplify.py
--rw-r--r--   0 runner    (1001) docker     (121)     8184 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/tangles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 15:02:20.801681 spherogram-2.1/spherogram_src/links/test/
--rw-r--r--   0 runner    (1001) docker     (121)    12504 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/test/old_testing_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     5787 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/test/test_montesinos.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/torus.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/links/twist.py
--rw-r--r--   0 runner    (1001) docker     (121)    18495 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/presentations.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/sage_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-05 15:02:09.000000 spherogram-2.1/spherogram_src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.922453 spherogram-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-23 20:01:24.000000 spherogram-2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 20:01:39.918453 spherogram-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-23 20:01:24.000000 spherogram-2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.906452 spherogram-2.2/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)    31967 2023-05-23 20:01:24.000000 spherogram-2.2/dev/DTcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 20:01:24.000000 spherogram-2.2/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-23 20:01:24.000000 spherogram-2.2/dev/conventions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.906452 spherogram-2.2/dev/dev_jennet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/AlexanderKauffman.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/bridge_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/spanning_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dt_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dt_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 20:01:24.000000 spherogram-2.2/dev/hard_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-23 20:01:24.000000 spherogram-2.2/dev/issue_35.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-23 20:01:24.000000 spherogram-2.2/dev/other_link_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 20:01:24.000000 spherogram-2.2/dev/sage_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-23 20:01:24.000000 spherogram-2.2/dev/sage_link_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-23 20:01:24.000000 spherogram-2.2/dev/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21769 2023-05-23 20:01:24.000000 spherogram-2.2/dev/tangle_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.906452 spherogram-2.2/planarity_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/planarity_src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/appconst.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices.private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices_Extensions.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDFSUtils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43741 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar.private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar_Extensions.c
+-rw-r--r--   0 runner    (1001) docker     (123)    63389 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphEmbed.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphExtensions.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphExtensions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphExtensions.private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphFunctionTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28630 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphIO.c
+-rw-r--r--   0 runner    (1001) docker     (123)    32754 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphIsolator.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search.private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search_Extensions.c
+-rw-r--r--   0 runner    (1001) docker     (123)    84775 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search.private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29971 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search_Extensions.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search.private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19913 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search_Extensions.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphNonplanar.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphOuterplanarObstruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38887 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphStructures.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39125 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphTests.c
+-rw-r--r--   0 runner    (1001) docker     (123)    91710 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphUtils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/listcoll.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/listcoll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/planarity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/platformTime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/stack.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/stack.h
+-rw-r--r--   0 runner    (1001) docker     (123)   158817 2023-05-23 20:01:25.000000 spherogram-2.2/planarity_src/planarity.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/planarity.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/planarmap_src/
+-rw-r--r--   0 runner    (1001) docker     (123)   174385 2023-05-23 20:01:25.000000 spherogram-2.2/planarmap_src/planarmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/planarmap.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/planarmap_src/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMconjugation.c
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMconjugation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMdef.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMdef.h
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMdisplay.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMenlight.c
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMenlight.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMextract.c
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMextract.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMplanmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMplanmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 20:01:24.000000 spherogram-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:01:39.922453 spherogram-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-23 20:01:24.000000 spherogram-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/spherogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/codecs/Base64LikeDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35378 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/codecs/DT.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/links/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/alexander.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100850 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/doc.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/exhaust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/extra_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29484 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/jones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/jones_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55123 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/links_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/morse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26248 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/orthogonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/planar_isotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/random_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/seifert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24336 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/tangles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/links/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/test/old_testing_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/test/test_montesinos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/twist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/presentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/sage_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/version.py
```

### Comparing `spherogram-2.1/PKG-INFO` & `spherogram-2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: spherogram
-Version: 2.1
+Version: 2.2
 Summary: Spherical diagrams for 3-manifold topology
 Home-page: https://github.com/3-manifolds/Spherogram
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@marc-culler.info, nathan@dunfield.info
 License: GPLv2+
 Keywords: knot,link,SnapPy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -21,9 +20,7 @@
 Spherogram is a Python module for dealing with the kind of planar
 diagrams that arise in 3-dimensional topology, such as link and
 Heegaard diagrams. It a component of the larger
 `SnapPy <https://snappy.computop.org>`_ project.  For some basic
 examples of using Spherogram to build links, 
 `see here <https://snappy.computop.org/spherogram.html>`_.  You can
 browse the `source code <https://github.com/3-manifolds/Spherogram>`_.
-
-
```

### Comparing `spherogram-2.1/README.rst` & `spherogram-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/dev/DTcodes.py` & `spherogram-2.2/dev/DTcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def char_to_int(x):
     n = ord(x)
     if 96 < n < 123:
         return n - 96
     if 64 < n < 91:
-        return 64 - n  
+        return 64 - n
     raise ValueError('Not an ascii letter.')
 
 
 def string_to_ints(s):
     return [char_to_int(x) for x in s]
 
 
@@ -44,15 +44,15 @@
 # leaves at North; the second time it enters at East and leaves at
 # West.
 #
 #        N
 #        ^
 #        |
 #        |
-# W <--------- E second         Initial vertex orientation 
+# W <--------- E second         Initial vertex orientation
 #        |
 #        |
 #        S
 #      first
 #
 # This arbitrary choice determines some embedding of each crossing
 # into the oriented plane.  During the process of constructing a
@@ -114,15 +114,15 @@
             return first-1 if first%2 == 0 else second-1
 
     def upper_pair(self):
         first, second, even_over = self
         return (0,2) if bool(first%2) ^ even_over else (1,3)
 
 
-class DTPath(object):
+class DTPath():
     """
     An iterator which starts at a FatEdge and walks around the
     link component containing that edge.  A DTPath raises
     StopIteration when it returns to its starting edge.
     """
     def __init__(self, edge, graph, forward=True):
         self.first_edge = edge
@@ -140,15 +140,15 @@
             if self.next_edge == self.first_edge:
                 raise StopIteration
         except AttributeError:
             self.next_edge = self.first_edge
         return self.next_edge
 
     __next__ = next
-    
+
 class DTFatEdge(FatEdge):
     """
     A fat edge which can be marked and belongs to a link component.
     """
     def __init__(self, x, y, twists=0, component=0):
         FatEdge.__init__(self, x, y, twists)
         self.marked = False
@@ -220,15 +220,15 @@
         """
         # Ignore the first push -- the first arc always is ambiguous
         # but the choice is irrelevant, up to reflecting the plane.
         if not self.pushed:
             self.pushed = True
             return
         #print 'pushing %s'%flips
-        self.stack.append( 
+        self.stack.append(
             [flips,
              [ ( (e[0], e.slots[0]), (e[1], e.slots[1]), e.component )
                for e in self.edges if e.marked],
              [ ( (e[0], e.slots[0]), (e[1], e.slots[1]), e.component )
                for e in self.edges if not e.marked]
              ]
             )
@@ -259,15 +259,15 @@
 
     def path(self, vertex, edge):
         """
         Return an iteratator which iterates through the edges of a
         component, starting at the given edge, in the direction
         determined by the vertex.
         """
-        if not vertex in edge:
+        if vertex not in edge:
             raise ValueError('That vertex is not an endpoint of the edge.')
         forward = True if vertex == edge[0] else False
         return DTPath(edge, self, forward)
 
     def marked_arc(self, vertex):
         """
         Given a vertex with marked valence 2, find the maximal marked
@@ -295,15 +295,15 @@
                 if len(edges) > 1:
                     break
                 else:
                     vertices.add(V)
                     edge = edges.pop()
         left_path.reverse()
         return left_path + right_path
-                
+
     def unmarked_arc(self, vertex):
         """
         Starting at this vertex, find an unmarked edge and follow its
         component until we run into a vertex with at least one marked
         edge.  Remove loops to get an embedded arc. Return the list
         of edges traversed by the embedded arc.
         """
@@ -364,16 +364,16 @@
             # the vertex_set gets expanded to include vertices visited
             # by the bridge path.
             vertex = start_vertex
             vertex_set = set(vertex_list)
             edge_path, vertex_path, seen_edges = [], [], set()
             while True:
                 edges = [e for e in self(vertex) if
-                         not e.marked 
-                         and e not in seen_edges 
+                         not e.marked
+                         and e not in seen_edges
                          and e(vertex) not in vertex_set]
                 try:
                     new_edge = edges.pop()
                     vertex = new_edge(vertex)
                     edge_path.append(new_edge)
                     if ( self.marked_valence(vertex) > 0 ):
                         return start_vertex, vertex, edge_path
@@ -402,24 +402,24 @@
         extend the embedding over an unmarked arc, the ending slots of
         both ends of the arc must lie on the same boundary curve.
         Flipping may be needed to arrange this.)
         """
         if not edge.marked:
             raise ValueError('Must begin at a marked edge.')
         result = set()
-        first_vertex = vertex = edge[1] 
+        first_vertex = vertex = edge[1]
         while True:
             end = 0 if edge[0] is vertex else 1
             slot = edge.slots[end]
             for k in range(3):
                 slot += side
                 interior_edge = self(vertex)[slot]
                 if not interior_edge.marked:
                     # For lookups, slot values must be in 0,1,2,3
-                    yield vertex, slot%4  
+                    yield vertex, slot%4
                 else:
                     break
             if k == 0:
                 yield (vertex, None)
             if edge is interior_edge:
                 raise ValueError('Marked subgraph has a dead end.')
             edge = interior_edge
@@ -434,15 +434,15 @@
         return set(self._boundary_slots(edge, side=-1))
 
     def right_slots(self, edge):
         """
         Return the (vertex, slot) pairs on the right boundary curve.
         """
         return set(self._boundary_slots(edge, side=1))
-        
+
     def flip(self, vertex):
         """
         Move the edge at the North slot to the South slot, and
         move the edge in the South  slot to the North slot.
         """
         #print 'flipping %s'%vertex
         if self.marked_valences[vertex] > 2:
@@ -460,15 +460,15 @@
         n = edgelist.index(vertex.first_under())
         return edgelist[n:] + edgelist[:n]
 
     def flipped(self, vertex):
         """
         Has this vertex been flipped?
         """
-        return bool(len([e for e in self(vertex) 
+        return bool(len([e for e in self(vertex)
                          if e[1] is vertex and e.slots[1] in (2,3)])%2)
 
     def sign(self, vertex):
         """
         The sign of the crossing corresponding to this vertex.
         See the documentation for Spherogram.link.
         """
@@ -480,39 +480,42 @@
         """
         Return the SnapPea KLP strand name for the given edge at the
         end opposite to the vertex.
         """
         W = edge(vertex)
         slot = edge.slot(W)
         return 'X' if (slot==0 or slot==2) ^ self.flipped(W) else 'Y'
-    
+
     def KLP_dict(self, vertex, indices):
         """
         Return a dict describing this vertex and its neighbors
-        in KLP terminology.  The translation from our convention is
-        as follows:
-                  Y                    Y
-                  3                    0
-                  ^                    ^
-                  |                    |
-           0 -----+----> 2 X     1 ----+---> 3 X   
-                  |                    |
-                  |                    |
-                  1                    2
-              not flipped           flipped
+        in KLP terminology.
+
+        The translation from our convention is as follows::
+
+                    Y                    Y
+                    3                    0
+                    ^                    ^
+                    |                    |
+             0 -----+----> 2 X     1 ----+---> 3 X
+                    |                    |
+                    |                    |
+                    1                    2
+                not flipped           flipped
+
         The indices argument is a dict that assigns an integer
         index to each vertex of the graph.
         """
         KLP = {}
         flipped = self.flipped(vertex)
         edges = self(vertex)
         neighbors = self[vertex]
         strands = [self.KLP_strand(vertex, edge) for edge in edges]
         ids = [ indices[v] for v in neighbors ]
-        
+
         KLP['sign'] = 'R' if self.sign(vertex) == 1 else 'L'
         slot = 1 if flipped else 0
         KLP['Xbackward_neighbor'] = ids[slot]
         KLP['Xbackward_strand'] = strands[slot]
         slot = 3 if flipped else 2
         KLP['Xforward_neighbor']  = ids[slot]
         KLP['Xforward_strand'] = strands[slot]
@@ -522,18 +525,19 @@
         KLP['Ybackward_strand'] = strands[slot]
         slot = 0 if flipped else 3
         KLP['Yforward_neighbor'] = ids[slot]
         KLP['Yforward_strand'] = strands[slot]
         KLP['Ycomponent'] = edges[slot].component
         return KLP
 
+
 # This assumes that the diagram has no loops, and that each component
 # meets the next one (so in particular the diagram is connected.
 
-class DTcodec(object):
+class DTcodec():
     """
     Codec for DT codes of a link projection.
     """
 
     def __init__(self, input, flips=None):
         if isinstance(input, (bytes, str, list)):
             self.decode(input, flips)
@@ -581,15 +585,15 @@
             self.code = dt
         code = self.code
         overcrossings = [sign(x) for comp in code for x in comp]
         evens = [abs(x) for comp in code for x in comp]
         self.size = size = 2*len(evens)
         pairs = zip(range(1, size, 2), evens)
         # Build a lookup table for the vertices.
-        # (DT codes are 1-based; we just waste the 0 entry.) 
+        # (DT codes are 1-based; we just waste the 0 entry.)
         self.lookup = lookup = [None for n in range(1+size)]
         for pair, overcrossing in zip(pairs, overcrossings):
             V = DTvertex(pair, overcrossing)
             m, n = pair
             lookup[m] = lookup[n] = V
         # Now build the fatgraph determined by the DT code.
         self.fat_graph = G = DTFatGraph()
@@ -719,15 +723,15 @@
         an arc from v to w starting with the v_edge and ending with
         the w_edge.  If flips are needed, make them.  If the embedding
         cannot be extended raise an exception.
         """
         G = self.fat_graph
         vslot = G(v).index(v_edge)
         wslot = G(w).index(w_edge)
-        #print 'do_flips: %s[%s] %s[%s]'%(v, vslot, w, wslot) 
+        #print 'do_flips: %s[%s] %s[%s]'%(v, vslot, w, wslot)
         not_unique = ( G.marked_valences[v] == G.marked_valences[w] == 2 )
         # starting from the v_edge, go ccw to a marked edge
         for k in range(1,3):
             ccw_edge = G(v)[vslot+k]
             if ccw_edge.marked:
                 break
         if not ccw_edge.marked:
```

### Comparing `spherogram-2.1/dev/conventions.py` & `spherogram-2.2/dev/conventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,7 @@
 
 import snappy
 from spherogram import Crossing, Link, RationalTangle
 import doctest
 from sage.all import gap
 
 print(doctest.testmod())
-
```

### Comparing `spherogram-2.1/dev/dev_jennet/AlexanderKauffman.py` & `spherogram-2.2/dev/dev_jennet/AlexanderKauffman.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,38 +34,39 @@
         if c in black_faces[i]:
             edge.append(verts[i])
     edge.append(c)
     if len(edge) != 3:
         raise Exception("Did not find two faces incident to c="+repr(c))
     return tuple(edge)
 
-def _dual_spanning_tree(K,T):
+
+def _dual_spanning_tree(K, T):
     "Returns the spanning tree for the white graph dual to the spanning tree T for the black graph. Here, dual means the edges do not intersect, i.e., no common crossings."
-    edges = list()
     G = K.white_graph()
     crossings_to_ignore = [e[2] for e in T.edges()]
-    crossings_to_use = [c for c in K.crossings if not c in crossings_to_ignore]
-    return Graph([K._crossing_to_edge(G,c) for c in crossings_to_use])
+    crossings_to_use = [c for c in K.crossings if c not in crossings_to_ignore]
+    return Graph([K._crossing_to_edge(G, c) for c in crossings_to_use])
+
 
 def Kauffman_states(K):
     "Returns the set of Kauffman states for the Alexander polynomial, corresponding to the spanning trees in the black graph. Returns a list of dictionaries, with keys crossings and values faces in the knot projection."
     G = K.black_graph()
     trees = G.spanning_trees()
     marked_edge = ((K.crossings[0],0), K.crossings[0].adjacent[0]) #We (arbitrarily) mark an edge in K.
     states = list()
     for T in trees:
-        #Find the root of T. 
+        #Find the root of T.
         for v in T.vertices():
             if marked_edge[0] in v:
                 root = v
         #Orient T out from the root.
         oT = orient_tree(T,root)
         #Find the planar dual spanning tree for the white graph
         dT = _dual_spanning_tree(K,T)
-        #Find the root of dT. 
+        #Find the root of dT.
         for v in dT.vertices():
             if marked_edge[0] in v:
                 droot = v
         odT = orient_tree(dT,droot)
         state = dict()
         for e in oT.edges():
             state[e[2]] = e[1]
```

### Comparing `spherogram-2.1/dev/dev_jennet/bridge_finding.py` & `spherogram-2.2/dev/dev_jennet/bridge_finding.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def find_bridges(G):
     global cnt
     global low # low[v] is the lowest preorder number of any vertex connected to v
     global preorder
     global bridges
 
-    cnt = 0    
+    cnt = 0
     low = dict()
     pre = dict()
     bridges = []
 
     verts = G.vertices()
     low = dict([(v,-1) for v in verts])
     preorder = dict([(v,-1) for v in verts])
@@ -45,8 +45,7 @@
         # if there are multiple edges from u to v, ignore only one
         elif (u != w or connections(G,u,v) > 1):
             low[v] = min(low[v], preorder[w])
 
 
 def connections(G, a, b):
     return len([x for x in G.edges() if x[0] == a and x[1] == b] + [x for x in G.edges() if x[0] == b and x[1] == a])
-
```

### Comparing `spherogram-2.1/dev/dev_jennet/spanning_trees.py` & `spherogram-2.2/dev/dev_jennet/spanning_trees.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     if len(G.edges()) == len(part_G.edges()):
         trees +=[part_G.copy()]
     else:
 
         # let e be an edge not in part_G
         X = G.edges()
-  
+
         for y in part_G.edges():
             X.remove(y)
         e = X[0]
 
         # add e to part_G
         part_G.add_edge(e)
         B = get_B(part_G,G)
@@ -56,43 +56,42 @@
 
         # delete e from part_G and from G
         G.delete_edge(e)
         part_G.delete_edge(e)
 
         # let C be the set of bridges which are not tree edges
         C = bridge_finding.find_bridges(G)
- 
+
         for x in part_G.edges():
             if x in C:
                 C.remove(x)
- 
+
         # add all edges in C to part_G
         part_G.add_edges(C)
 
         # rec
-        trees += rec(part_G, G)        
+        trees += rec(part_G, G)
         part_G.delete_edges(C)
         G.add_edge(e)
 
     return trees
 
 def get_B(part_G,G):
-    """ 
+    """
     Returns the set of edges not in part_G joining vertices already connected in part_G
     """
     B = []
     comps = part_G.connected_components()
     vc_dict = dict()
     for i in range(len(comps)):
         for v in comps[i]:
             vc_dict[v] = i
-    
+
     X = G.edges()
-    for y in part_G.edges(): 
+    for y in part_G.edges():
         X.remove(y)
-    
+
     for e in X:
         if vc_dict[e[0]] == vc_dict[e[1]]:
             B.append(e)
-  
-    return B
 
+    return B
```

### Comparing `spherogram-2.1/dev/dev_jennet/test_links.py` & `spherogram-2.2/dev/dev_jennet/test_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import spherogram
 import unittest
 from random import randrange
 
 class TestLinkFunctions(unittest.TestCase):
-    
+
     def setUp(self):
         # Trefoil
         a = spherogram.Crossing('a')
         b = spherogram.Crossing('b')
         c = spherogram.Crossing('c')
         a[2] = b[1]
         b[3] = c[0]
@@ -19,51 +19,51 @@
 
         self.K3_1 = spherogram.Link('3_1')
         self.K7_2 = spherogram.Link('7_2')
         self.K8_3 = spherogram.Link('8_3')
         self.K8_13 = spherogram.Link('8_13')
 
         # Hopf Link
-        a = spherogram.Crossing('a') 
-        b = spherogram.Crossing('b') 
-        a[0]=b[1] 
-        a[1]=b[0] 
-        a[2]=b[3] 
-        a[3]=b[2] 
+        a = spherogram.Crossing('a')
+        b = spherogram.Crossing('b')
+        a[0]=b[1]
+        a[1]=b[0]
+        a[2]=b[3]
+        a[3]=b[2]
         self.L2a1 = spherogram.Link([a,b])
 
-        #Borromean Link (3) 
-        a = spherogram.Crossing('a') 
-        b = spherogram.Crossing('b') 
-        c = spherogram.Crossing('c') 
-        d = spherogram.Crossing('d') 
-        e = spherogram.Crossing('e') 
-        f = spherogram.Crossing('f') 
+        #Borromean Link (3)
+        a = spherogram.Crossing('a')
+        b = spherogram.Crossing('b')
+        c = spherogram.Crossing('c')
+        d = spherogram.Crossing('d')
+        e = spherogram.Crossing('e')
+        f = spherogram.Crossing('f')
         a[2] = f[1]
-        a[3] = e[0] 
-        b[1] = a[0] 
-        b[2] = e[3] 
-        c[0] = a[1] 
-        c[1] = b[0] 
-        d[3] = c[2] 
-        d[0] = b[3] 
-        e[2] = d[1] 
-        e[1] = f[0] 
-        f[2] = c[3] 
-        f[3] = d[2] 
+        a[3] = e[0]
+        b[1] = a[0]
+        b[2] = e[3]
+        c[0] = a[1]
+        c[1] = b[0]
+        d[3] = c[2]
+        d[0] = b[3]
+        e[2] = d[1]
+        e[1] = f[0]
+        f[2] = c[3]
+        f[3] = d[2]
         self.Borr = spherogram.Link([a,b,c,d,e,f])
-        
+
         self.L6a2 = spherogram.Link('L6a2')
         self.L6a4 = spherogram.Link('L6a4')
         self.L7a3 = spherogram.Link('L7a3')
 
         self.knots = [self.K3_1, self.K7_2, self.K8_3, self.K8_13]
         self.links = [self.L2a1, self.L6a4, self.L6a2, self.L7a3]
         self.all_links = self.knots + self.links
-               
+
     def random_knot(self):
         random_index = randrange(0,len(self.knots))
         return self.knots[random_index]
 
     def random_link(self):
         random_index = randrange(0,len(self.links))
         return self.links[random_index]
@@ -107,16 +107,16 @@
 
     def testKnotGroup(self):
         # Correct number of generators? abelian invariants?
         for k in self.all_links:
             self.assertEqual(len(k.knot_group().generators()),             len(k.crossings))
             self.assertEqual(k.knot_group().abelian_invariants()[0],       0)
             self.assertEqual(len(k.knot_group().abelian_invariants()),     len(k.link_components))
-       
-    def testAlexanderPoly(self): 
+
+    def testAlexanderPoly(self):
         t = var('t')
         a = var('a')
 
         # method = 'wirt'
         self.assertEqual(self.Tref.alexander_poly(),       t - 1 + t**-1)
         self.assertEqual(self.K3_1.alexander_poly(),       t - 1 + t**-1)
         self.assertEqual(self.K7_2.alexander_poly(),       3*t - 5 + 3*t**-1)
@@ -128,15 +128,15 @@
 
         # method = 'snappy'
         self.assertEqual(self.Tref.alexander_poly(method='snappy'),       a**2 - a + 1)
         self.assertEqual(self.K3_1.alexander_poly(method='snappy'), a**2 - a + 1)
         self.assertEqual(self.K7_2.alexander_poly(method='snappy'),       3*a**2 - 5*a + 3)
         self.assertEqual(self.K8_3.alexander_poly(method='snappy'),       4*a**2 - 9*a + 4)
         self.assertEqual(self.K8_13.alexander_poly(method='snappy'),      2*a**4 - 7*a**3 + 11*a**2 - 7*a + 2)
-        
+
     def testConnectedSum(self):
         repeat = 3
         while repeat > 0:
             k1 = self.random_knot()
             k2 = self.random_knot()
             Sum = k1.connected_sum(k2)
             self.assertEqual(Sum.alexander_poly(), k1.alexander_poly()*k2.alexander_poly())
@@ -181,28 +181,28 @@
         repeat = 3
         while repeat > 0:
             k1 = self.random_knot()
             k1_prime = k1.mirror()
             self.assert_(k1.signature() == -1*k1_prime.signature(), msg="knot signature failed for "+ repr(k1))
             self.assert_(k1.writhe() == -1*k1_prime.writhe(), msg="knot writhe failed for "+repr(k1))
             repeat-=1
-            
+
         repeat = 3
         while repeat > 0:
             k2 = self.random_link()
             k2_prime = k2.mirror()
             self.assert_(k2.signature() == -1*k2_prime.signature(), msg="link signature failed for " + repr(k2))
             self.assert_(k2.writhe() == -1*k2_prime.writhe(), msg="link writhe failed for " + repr(k2))
             repeat-=1
 
     def testDet(self):
         self.assertEqual(self.K3_1.determinant(),                 3)
         self.assertEqual(self.K3_1.determinant(method='color'),   3)
         self.assertEqual(self.K3_1.determinant(method='goeritz'), 3)
-        
+
         self.assertEqual(self.Tref.determinant(),                 3)
         self.assertEqual(self.Tref.determinant(method='color'),   3)
         self.assertEqual(self.Tref.determinant(method='goeritz'), 3)
 
         self.assertEqual(self.K7_2.determinant(),                 11)
         self.assertEqual(self.K7_2.determinant(method='color'),   11)
         self.assertEqual(self.K7_2.determinant(method='goeritz'), 11)
```

### Comparing `spherogram-2.1/dev/dt_issue.py` & `spherogram-2.2/dev/dt_issue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import snappy, spherogram
+import snappy
+import spherogram
 import spherogram.links.orthogonal
 from nsnappytools import appears_hyperbolic
 from sage.all import *
 
 
 links = snappy.HTLinkExteriors()
 for i in range(1):
@@ -32,15 +33,15 @@
     n = len(cusp_perm)
     return cusp_perm == range(n) and cusp_maps == (n*[Id])
 
 def manifolds_match(M0, M1):
     isoms = M0.is_isometric_to(M1, True)
     assert len(isoms) == 1
     return matches_peripheral_data(isoms[0])
-            
+
 def test_DT(dt, M2=None):
     if M2 is None:
         M2 = snappy.Manifold()
     dtc = spherogram.DTcodec(dt)
     L = dtc.link()
     M0, M1 = dtc.exterior(), L.exterior()
     L.view(M2.LE)
```

### Comparing `spherogram-2.1/dev/dt_tests.py` & `spherogram-2.2/dev/dt_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     v = e[0]
     w = e[1]
     for i in range(50000):
         v == w
     return v
 
 
-class TestObject(object):
+class TestObject():
     pass
 
 
 def test5():
     D = dict([(TestObject(), i) for i in range(10)])
     k = D.keys()[0]
     for i in range(10000000):
```

### Comparing `spherogram-2.1/dev/sage_link_compare.py` & `spherogram-2.2/dev/sage_link_compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-import spherogram, snappy
+import spherogram
+import snappy
 from sage.all import Link as SageLink
 from sage.all import LaurentPolynomialRing, PolynomialRing, ZZ, var
 from sage.symbolic.ring import SymbolicRing
 
+
 def alexander_poly_of_sage(knot):
     p = knot.alexander_polynomial()
     ans = p.polynomial_construction()[0]
     if ans.leading_coefficient() < 0:
         ans = -ans
     return ans
 
+
 def jones_polynomial_of_sage(knot):
     """
     To match our conventions (which seem to agree with KnotAtlas), we
     need to swap q and 1/q.
     """
     q = LaurentPolynomialRing(ZZ, 'q').gen()
     p = knot.jones_polynomial(skein_normalization=True)
     exps = p.exponents()
     assert all(e % 4 == 0 for e in exps)
     return sum(c*q**(-e//4) for c, e in zip(p.coefficients(), exps))
 
+
 def test_knot(snappy_manifold):
     M = snappy_manifold
     assert M.num_cusps() == 1
 
     U = M.link()
     T = U.sage_link()
 
@@ -33,18 +37,15 @@
     assert U.signature() == T.signature()
     assert U.jones_polynomial() == jones_polynomial_of_sage(T)
 
     T_alt = SageLink(U.braid_word(as_sage_braid=True))
     assert U.signature() == T_alt.signature()
     U_alt = spherogram.Link(T.braid())
     assert U.signature() == U_alt.signature()
-    
-    
+
     #q = var('q')
     #print (SR(K_us.jones_poly()) - K_them.jones_polynomial(variab='q').subs(q=1/q)).simplify()
     #print K_us.signature(), K_them.signature()
 
 
-    
 M = snappy.Manifold('K11n42')
 knot_manifolds = snappy.HTLinkExteriors(cusps=1)
-
```

### Comparing `spherogram-2.1/dev/signature.py` & `spherogram-2.2/dev/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Given a palindromic polynomial p(x) of degree 2n, return a
     polynomial g so that p(x) = x^n g(x + 1/x).
     """
     assert is_palindromic(p) and p.degree() % 2 == 0
     R = p.parent()
     x = R.gen()
     f, g = p, R(0)
-    
+
     while f != 0:
         c = f.leading_coefficient()
         assert f.degree() % 2 == 0
         d = f.degree()//2
         g += c*x**d
         f = (f - c*(x**2 + 1)**d)
         if f != 0:
@@ -75,17 +75,16 @@
 def signature_via_numpy(A):
     CC = ComplexField(53)
     A = A.change_ring(CC).numpy()
     assert np.linalg.norm(A - A.conjugate().transpose()) < 10e-10
     eigs = np.linalg.eigh(A)[0]
     smallest = min(np.abs(eigs))
     assert smallest > 1e-5
-    return np.sum(eigs > 0) - np.sum(eigs < 0) 
+    return np.sum(eigs > 0) - np.sum(eigs < 0)
 
-    
 
 def signature_function_of_integral_matrix(V, prec=53):
     """
     Computes the signature function sigma of V via numerical methods.
     Returns two lists, the first representing a partition of [0, 1]:
 
          x_0 = 0 < x_1 < x_2 < ... < x_n = 1
@@ -99,36 +98,36 @@
     CC = ComplexField(prec)
     pi = RR.pi()
     I = CC.gen()
     partition = [RR(0)] + [a for a, e in roots_on_unit_circle(poly, prec)] + [RR(1)]
     n = len(partition) - 1
     values = []
     for i in range(n):
-         omega = exp((2*pi*I)*(partition[i] + partition[i + 1])/2)
-         A = (1 - omega)*V + (1 - omega.conjugate())*V.transpose()
-         values.append(signature_via_numpy(A))
+        omega = exp((2*pi*I)*(partition[i] + partition[i + 1])/2)
+        A = (1 - omega)*V + (1 - omega.conjugate())*V.transpose()
+        values.append(signature_via_numpy(A))
 
     assert list(reversed(values)) == values
     return partition, values
 
+
 def signature_function(L, prec=53):
     """
     Computes the signature function sigma of K via numerical methods.
     Returns two lists, the first representing a partition of [0, 1]:
 
          x_0 = 0 < x_1 < x_2 < ... < x_n = 1
 
     and the second list consisting of the values [v_0, ... , v_(n-1)]
     of sigma on the interval (x_i, x_(i+1)).  Currently, the value of
     sigma *at* x_i is not computed.
     """
     V = L.seifert_matrix()
     return signature_function_of_integral_matrix(V)
-        
-    
+
 
 def basic_knot_test():
     # All passed!
     for M in snappy.HTLinkExteriors(cusps=1):
         print(M.name())
         R = PolynomialRing(ZZ, 't')
         K = M.link()
@@ -138,14 +137,13 @@
         p2 = alexander_poly_from_seifert(V)
         assert p0 == p1 == p2
         partition, values = signature_function_of_integral_matrix(V)
         n = len(values)
         assert n % 2 == 1
         m = (n - 1)//2
         assert K.signature() == values[m]
-    
-    
+
 
 if __name__ == '__main__':
     K = spherogram.Link('K12n123')
     V = matrix(ZZ, K.seifert_matrix())
     basic_knot_test()
```

### Comparing `spherogram-2.1/dev/tangle_patch.py` & `spherogram-2.2/dev/tangle_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import spherogram
 from spherogram.links.tangles import Tangle, OneTangle, MinusOneTangle
 import networkx as nx
 from random import randint,choice,sample
 from spherogram.links.random_links import map_to_link, random_map
 
 """
-This file contains some unfinished code to work with tangles, including 
+This file contains some unfinished code to work with tangles, including
 getting tangles out of link diagrams, as well as some Conway mutation.
 """
 
 def rotate_list(L, s):
     n = len(L)
     return [ L[(i + s) % n] for i in range(n) ]
 
@@ -36,107 +36,107 @@
     new_crossing = spherogram.Crossing(label)
     old_position = randint(0,len(adj)-1)
     old_crossing, old_strand = adj.pop(old_position)
     new_strand = randint(0,3)
     old_crossing[old_strand]=new_crossing[new_strand]
     for i in range(1,4):
         adj.insert(old_position,(new_crossing,(new_strand-i)%4))
-    adj[len(adj)/2:] = reversed(adj[len(adj)/2:])    
+    adj[len(adj)/2:] = reversed(adj[len(adj)/2:])
     tangle_copy.crossings.append(new_crossing)
     tangle_copy.n = self.n+1
     return tangle_copy
 
+
 def random_tree(size):
     """
     Repeatedly splits crossings, starting with a single crossing, resulting
     in a random 4-valent tree of crossings.
     """
-
     T = OneTangle()
     T.crossings[0].label = 0
-    for i in range(1,size):
+    for i in range(1, size):
         T = T.add_random_crossing(i)
     return T
 
+
 def random_tree_link(size):
     """
     Generate two random tree tangles and glues together.  Gives a link of size
     2*size
     """
-
-    return random_tree(size).circular_sum(random_tree(size),0)
+    return random_tree(size).circular_sum(random_tree(size), 0)
 
 
-def random_tree_knot(size,simplify=None,prime_decomp = False):
+def random_tree_knot(size, simplify=None, prime_decomp=False):
     found_nontrivial = False
     while not found_nontrivial:
         link = random_tree_link(size)
-        knot = link.sublink(max(link.link_components,key=len))
+        knot = link.sublink(max(link.link_components, key=len))
         knot.simplify(mode=simplify)
         if len(knot) > 0:
-            found_nontrivial=True
-    
+            found_nontrivial = True
+
     if prime_decomp:
         cant_deconnect = False
         while cant_deconnect:
             ds = knot.deconnect_sum()
-            knot = max(ds,key=len)
-            cant_deconnect = (len(ds)>1)
+            knot = max(ds, key=len)
+            cant_deconnect = (len(ds) > 1)
     return knot
 
-def all_circular_sums(self,other):
+
+def all_circular_sums(self, other):
     """
     All possible tangle sums as above
     """
 
     if len(self.adjacent) != len(other.adjacent):
         raise Exception("Tangles do not have the same number of strands")
-    return [self.circular_sum(other,n) for n in range(len(other.adjacent))]
-
+    return [self.circular_sum(other, n) for n in range(len(other.adjacent))]
 
 
 def random_root(self):
     return choice(choice(self.crossings).crossing_strands())
 
 
 def isosig_with_gluings(self, gluings, root=None):
-    return (self.isosig(root = root),tuple(gluings))
+    return (self.isosig(root=root), tuple(gluings))
+
 
-def min_isosig_with_gluings(self, gluings, root = None):
-    if root != None:
+def min_isosig_with_gluings(self, gluings, root=None):
+    if root is not None:
         cs_name = cslabel(root)
     isosigs = []
     for i in range(self.n*2):
         rotated_tangle = self.circular_rotate(i)
-        if root != None:
+        if root is not None:
             rotated_root = crossing_strand_from_name(rotated_tangle,cs_name)
         else:
             rotated_root = None
         #permuting the indices in the gluings
         perm = range(len(self.adjacent))
         perm[len(perm)/2:] = reversed(perm[len(perm)/2:])
         perm = rotate_list(perm,i)
         perm[len(perm)/2:] = reversed(perm[len(perm)/2:])
         rotated_gluings = []
         for g in gluings:
             new_g = [perm[g[0]],perm[g[1]]]
             new_g.sort()
             rotated_gluings.append(tuple(new_g))
         rotated_gluings.sort()
-        isosigs.append(rotated_tangle.isosig_with_gluings(rotated_gluings,root=rotated_root))        
-
+        isosigs.append(rotated_tangle.isosig_with_gluings(rotated_gluings,root=rotated_root))
 
     return min(isosigs)
 
 Tangle.all_circular_sums = all_circular_sums
 Tangle.add_random_crossing = add_random_crossing
 
 def cycle_basis(G):
     """
-    Uses networkx's cycle basis function on dual graph and converts to 
+    Uses networkx's cycle basis function on dual graph and converts to
     form with spherogram objects
     """
 
     Gx = G.to_networkx()
     vert_cycles = nx.cycle_basis(Gx)
     return [edge_cycle(vert_cycle,G) for vert_cycle in vert_cycles]
 
@@ -224,15 +224,15 @@
                 break
         if not seen_before:
             four_cycles_no_duplicates.append(fc)
     return four_cycles_no_duplicates
 
 def edge_cycle(vert_list,G):
     """
-    Converts from list of vertices of dual graph to list of edges.  
+    Converts from list of vertices of dual graph to list of edges.
     If multiple edges, just chooses one.
     """
     edges = list(G.edges)
     cycle = []
     for i in range(len(vert_list)-1):
         face_pair = [vert_list[i],vert_list[i+1]]
         for edge in edges:
@@ -296,15 +296,14 @@
             if i > 100:
                 raise Exception()
         cs = cs.rotate(1)
         boundary_comp.append(cs)
     boundary_comp.pop(-1) #code aboves adds the start_cs twice
     return boundary_comp
 
-    
 
 def tangle_neighborhood(link,crossing,radius,return_gluings=True,hull=False):
     """
     Splits a link into two tangles along a ball around a crossing of the given
     radius.  Destroys original link.  This might not generate an actual tangle;
     the graph metric ball will usually have multiple boundary components.
     """
@@ -332,15 +331,15 @@
         comps.remove(largest_comp) #remove largest component
         for comp in comps:
             print('crossings: ' +str(crossings))
             print('filling in comp:'+str(comp))
             print('adjacent: '+str(adjacent))
             c = comp.pop()
             cs = choice(c.crossing_strands())
-            
+
             print('cs: ' + str(cs))
             exit_strand = meander(cs,sides)[1] #meander until you hit boundary
             exit_strand = exit_strand[0].crossing_strands()[exit_strand[1]]
             print('exit_strand: ' +str(exit_strand))
             bound_comp = trace_boundary_component(exit_strand,adjacent)
             print('traced component: ' + str(bound_comp))
             if exit_strand not in main_boundary_comp:
@@ -403,15 +402,15 @@
         if str(new_edge) == str(edge):
             return new_edge
 
 def tangle_cut(link, cycle):
     """
     Creates two Tangle objects from a given cycle (with no self intersections)
     in the dual graph of a link (inside and outside).  Cycle is given
-    as a list of (oriented) edges in the dual graph. Make sure crossings 
+    as a list of (oriented) edges in the dual graph. Make sure crossings
     are uniquely labeled. Destroys original link.
     """
 
     sides = {} #keeps track of which side each crossing strand is as dictionary
     sides[cslabel(cycle[0].interface[0])] = 0 #start by assigning to first pair
     sides[cslabel(cycle[0].interface[1])] = 1 #sides
     side0 = [cycle[0].interface[0]]
@@ -443,26 +442,26 @@
                 sides[cslabel(edge2_cs1)] = edge1_cs2_side
                 sides[cslabel(edge2_cs2)] = edge1_cs1_side
                 if edge1_cs2_side == 1:
                     side1.append(edge2_cs1)
                     side0.append(edge2_cs2)
                 else:
                     side0.append(edge2_cs1)
-                    side1.append(edge2_cs2)                    
+                    side1.append(edge2_cs2)
 #                print('case 1')
                 break
             if edge1_cs1 == edge2_cs2:
                 sides[cslabel(edge2_cs1)] = edge1_cs1_side
                 sides[cslabel(edge2_cs2)] = edge1_cs2_side
                 if edge1_cs2_side == 1:
                     side0.append(edge2_cs1)
                     side1.append(edge2_cs2)
                 else:
                     side1.append(edge2_cs1)
-                    side0.append(edge2_cs2)                    
+                    side0.append(edge2_cs2)
 #                print('case 2')
                 break
             if edge1_cs1.opposite() == edge1_cs2: #returned without seeing them
                 wrong_face = True
 #                print('case 3')
                 break
 
@@ -476,37 +475,37 @@
                 sides[cslabel(edge2_cs1)] = edge1_cs1_side
                 sides[cslabel(edge2_cs2)] = edge1_cs2_side
                 if edge1_cs2_side == 1:
                     side0.append(edge2_cs1)
                     side1.append(edge2_cs2)
                 else:
                     side1.append(edge2_cs1)
-                    side0.append(edge2_cs2)                    
+                    side0.append(edge2_cs2)
                 break
             if edge1_cs2 == edge2_cs2:
  #               print('case 5')
                 sides[cslabel(edge2_cs1)] = edge1_cs2_side
                 sides[cslabel(edge2_cs2)] = edge1_cs1_side
                 if edge1_cs2_side == 1:
                     side1.append(edge2_cs1)
                     side0.append(edge2_cs2)
                 else:
                     side0.append(edge2_cs1)
                     side1.append(edge2_cs2)
                 break
             if edge1_cs2.opposite() == edge1_cs1: #returned without seeing them again, must be error
                 raise Exception("Neither side worked")
-    
+
     crossing_sides = fill_in_crossings(link,sides)
     n = len(cycle)
     side0[n/2:] = reversed(side0[n/2:]) #flip to use as adjacent in tangle
     side1[n/2:] = reversed(side1[n/2:])
     crossings0 = [crossing_from_name(link,c) for c in crossing_sides if crossing_sides[c] == 0]
     crossings1 = [crossing_from_name(link,c) for c in crossing_sides if crossing_sides[c] == 1]
-    
+
     #clear crossing info
     clear_orientations(crossings0)
     clear_orientations(crossings1)
 
     #One of the tangles is the 'outside', and needs to be flipped
     #Just check side0
     side0_needs_flip = False
@@ -563,15 +562,15 @@
     while True:
         cs = cs.opposite().rotate(randint(1,3))
         if cslabel(cs) in sides: # hit the side
             end_side = sides[cslabel(cs)]
             break
         crossings_encountered.append(cs.crossing)
     return set(crossings_encountered),end_side
-    
+
 def cslabel(cs):
     """
     Label of crossing strand, without frills
     """
     return (cs[0].label,cs[1])
 
 def crossing_strand_from_name(link,csname):
@@ -586,15 +585,14 @@
 def crossing_from_name(link,crossname):
     for c in link.crossings:
         if c.label == crossname:
             return c
     raise Exception("Crossing not found")
 
 
-
 def crossing_by_label(label,link):
     for c in link.crossings:
         if c.label == label:
             return c
 
 def all_neighborhoods(link,radius):
     nhds = []
```

### Comparing `spherogram-2.1/planarity_src/c/appconst.h` & `spherogram-2.2/planarity_src/c/appconst.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graph.h` & `spherogram-2.2/planarity_src/c/graph.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphColorVertices.c` & `spherogram-2.2/planarity_src/c/graphColorVertices.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphColorVertices.h` & `spherogram-2.2/planarity_src/c/graphColorVertices.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphColorVertices.private.h` & `spherogram-2.2/planarity_src/c/graphColorVertices.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphColorVertices_Extensions.c` & `spherogram-2.2/planarity_src/c/graphColorVertices_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphDFSUtils.c` & `spherogram-2.2/planarity_src/c/graphDFSUtils.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphDrawPlanar.c` & `spherogram-2.2/planarity_src/c/graphDrawPlanar.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphDrawPlanar.h` & `spherogram-2.2/planarity_src/c/graphDrawPlanar.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphDrawPlanar.private.h` & `spherogram-2.2/planarity_src/c/graphDrawPlanar.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphDrawPlanar_Extensions.c` & `spherogram-2.2/planarity_src/c/graphDrawPlanar_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphEmbed.c` & `spherogram-2.2/planarity_src/c/graphEmbed.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphExtensions.c` & `spherogram-2.2/planarity_src/c/graphExtensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphExtensions.h` & `spherogram-2.2/planarity_src/c/graphExtensions.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphExtensions.private.h` & `spherogram-2.2/planarity_src/c/graphExtensions.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphFunctionTable.h` & `spherogram-2.2/planarity_src/c/graphFunctionTable.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphIO.c` & `spherogram-2.2/planarity_src/c/graphIO.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphIsolator.c` & `spherogram-2.2/planarity_src/c/graphIsolator.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK23Search.c` & `spherogram-2.2/planarity_src/c/graphK23Search.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK23Search.h` & `spherogram-2.2/planarity_src/c/graphK23Search.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK23Search.private.h` & `spherogram-2.2/planarity_src/c/graphK23Search.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK23Search_Extensions.c` & `spherogram-2.2/planarity_src/c/graphK23Search_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK33Search.c` & `spherogram-2.2/planarity_src/c/graphK33Search.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK33Search.h` & `spherogram-2.2/planarity_src/c/graphK33Search.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK33Search.private.h` & `spherogram-2.2/planarity_src/c/graphK33Search.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK33Search_Extensions.c` & `spherogram-2.2/planarity_src/c/graphK33Search_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK4Search.c` & `spherogram-2.2/planarity_src/c/graphK4Search.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK4Search.h` & `spherogram-2.2/planarity_src/c/graphK4Search.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK4Search.private.h` & `spherogram-2.2/planarity_src/c/graphK4Search.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphK4Search_Extensions.c` & `spherogram-2.2/planarity_src/c/graphK4Search_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphNonplanar.c` & `spherogram-2.2/planarity_src/c/graphNonplanar.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphOuterplanarObstruction.c` & `spherogram-2.2/planarity_src/c/graphOuterplanarObstruction.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphStructures.h` & `spherogram-2.2/planarity_src/c/graphStructures.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphTests.c` & `spherogram-2.2/planarity_src/c/graphTests.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/graphUtils.c` & `spherogram-2.2/planarity_src/c/graphUtils.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/listcoll.c` & `spherogram-2.2/planarity_src/c/listcoll.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/listcoll.h` & `spherogram-2.2/planarity_src/c/listcoll.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/planarity.h` & `spherogram-2.2/planarity_src/c/planarity.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/platformTime.h` & `spherogram-2.2/planarity_src/c/platformTime.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/stack.c` & `spherogram-2.2/planarity_src/c/stack.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/c/stack.h` & `spherogram-2.2/planarity_src/c/stack.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarity_src/planarity.c` & `spherogram-2.2/planarity_src/planarity.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "planarity_src/c/graph.h"
         ],
@@ -23,16 +23,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -63,14 +63,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -99,18 +100,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -140,18 +145,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -163,61 +217,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
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
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
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
@@ -326,17 +391,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
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
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -442,35 +566,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -566,18 +690,18 @@
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
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -594,16 +718,18 @@
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
@@ -726,14 +852,15 @@
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
@@ -1977,15 +2104,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyList_Type_index.type = (PyObject*)&PyList_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -2213,15 +2340,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_planarity) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2520,28 +2647,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -2596,18 +2723,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* UnpackUnboundCMethod */
 static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
     PyObject *method;
     method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
     if (unlikely(!method))
@@ -2630,19 +2755,19 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
     if (likely(cfunc->func)) {
         int flag = cfunc->flag;
         if (flag == METH_O) {
             return (*(cfunc->func))(self, arg);
         } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
+            #if PY_VERSION_HEX >= 0x030700A0
                 return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
+            #else
                 return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
+            #endif
         } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
             return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
         }
     }
     return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
 }
 #endif
@@ -2789,15 +2914,15 @@
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -2819,15 +2944,15 @@
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
@@ -2913,41 +3038,48 @@
     Py_INCREF(code_object);
 }
 
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
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -2958,34 +3090,49 @@
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
@@ -3586,19 +3733,41 @@
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
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -3848,14 +4017,31 @@
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
```

### Comparing `spherogram-2.1/planarity_src/planarity.pyx` & `spherogram-2.2/planarity_src/planarity.pyx`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/planarmap.c` & `spherogram-2.2/planarmap_src/planarmap.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "planarmap",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,14 +58,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -94,18 +95,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -135,18 +140,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -158,61 +212,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
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
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
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
@@ -321,17 +386,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
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
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -437,35 +561,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -561,18 +685,18 @@
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
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -589,16 +713,18 @@
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
@@ -725,14 +851,15 @@
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
@@ -952,26 +1079,26 @@
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
 
@@ -992,21 +1119,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -2038,15 +2173,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -2276,15 +2411,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_planarmap) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2894,17 +3029,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -3204,28 +3337,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -3293,15 +3426,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -3323,15 +3456,15 @@
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
@@ -3417,41 +3550,48 @@
     Py_INCREF(code_object);
 }
 
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
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -3462,34 +3602,49 @@
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
@@ -4090,19 +4245,41 @@
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
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -4352,14 +4529,31 @@
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
```

### Comparing `spherogram-2.1/planarmap_src/planarmap.pyx` & `spherogram-2.2/planarmap_src/planarmap.pyx`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMconjugation.c` & `spherogram-2.2/planarmap_src/src/PMconjugation.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMconjugation.h` & `spherogram-2.2/planarmap_src/src/PMconjugation.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMdef.c` & `spherogram-2.2/planarmap_src/src/PMdef.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMdef.h` & `spherogram-2.2/planarmap_src/src/PMdef.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMenlight.c` & `spherogram-2.2/planarmap_src/src/PMenlight.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMextract.c` & `spherogram-2.2/planarmap_src/src/PMextract.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMextract.h` & `spherogram-2.2/planarmap_src/src/PMextract.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/PMplanmap.c` & `spherogram-2.2/planarmap_src/src/PMplanmap.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/planarmap_src/src/stats.c` & `spherogram-2.2/planarmap_src/src/stats.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/setup.py` & `spherogram-2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,100 @@
-import os, shutil, sys, sysconfig, subprocess
+import os
+import shutil
+import sys
+import sysconfig
+import subprocess
 from glob import glob
 from setuptools import setup, Command, Extension
 
 
 # Defensive linker flags for Linux:
 if sys.platform.startswith('linux'):
     extra_link_args=['-Wl,-Bsymbolic-functions', '-Wl,-Bsymbolic']
 else:
     extra_link_args=[]
 
+# Install a custpom build environ for MSVC, if necessary.
+if sys.platform == 'win32':
+    try:
+        # To customize your msvc environment create msvc_env.py
+        # and define the dict dev_env to be a copy of the os.environ
+        # that you have when you run python in the Command Prompt for
+        # your installation of Visual Studio.
+        from msvc_env import dev_env
+        os.environ.update(dev_env)
+        MSVC_extra_objects = []    
+    except:
+        pass
 
 # The planarity extension
 
 try:
     import sage.libs
     ext_modules = []
-except ImportError:    
+except ImportError:
     planarity_dir = 'planarity_src/c/'
     planarity_ui_sources = glob(planarity_dir + 'planarity*.c')
     planarity_sources = [file for file in glob('planarity_src/c/*.c')
-                         if not file in planarity_ui_sources]
+                         if file not in planarity_ui_sources]
 
     if sys.platform.startswith('win'):
-        extra_compile_args = ['-D_CRT_SECURE_NO_WARNINGS']
+        extra_compile_args = [
+            '-D_CRT_SECURE_NO_WARNINGS',
+            r'-IC:\Program Files (x86)\Windows Kits\10\Include\10.0.17134.0\ucrt',
+            r'-IC:\Program Files (x86)\Windows Kits\10\Include\10.0.17134.0\shared'
+        ]
+        extra_link_args = [
+            r'/LIBPATH:C:\Program Files (x86)\Windows Kits\10\Lib\10.0.17134.0\um\x64',
+            r'/LIBPATH:C:\Program Files (x86)\Windows Kits\10\Lib\10.0.17134.0\ucrt\x64',
+        ]
     else:
         extra_compile_args = []
-    
+        extra_link_args = []
+
     Planarity = Extension(
         name = 'spherogram.planarity',
-        sources = ['planarity_src/planarity.c'] + planarity_sources, 
+        sources = ['planarity_src/planarity.c'] + planarity_sources,
         include_dirs = [planarity_dir],
         extra_compile_args = extra_compile_args,
         extra_link_args = extra_link_args
         )
 
     ext_modules = [Planarity]
 
 # A real clean
 
 class SpherogramClean(Command):
     user_options = []
     def initialize_options(self):
-        pass 
+        pass
     def finalize_options(self):
         pass
     def run(self):
         junkdirs = (glob('build/lib*') +
                     glob('build/bdist*') +
                     glob('snappy*.egg-info') +
                     ['__pycache__', os.path.join('python', 'doc')]
         )
         for dir in junkdirs:
             try:
                 shutil.rmtree(dir)
             except OSError:
                 pass
-        junkfiles = glob('*/*.so*') + glob('*/*.pyc') + glob('*/*.c') 
+        junkfiles = glob('*/*.so*') + glob('*/*.pyc') + glob('*/*.c')
         for file in junkfiles:
             try:
                 os.remove(file)
             except OSError:
                 pass
-        
+
 class SpherogramTest(Command):
     user_options = []
     def initialize_options(self):
-        pass 
+        pass
     def finalize_options(self):
         pass
     def run(self):
         build_lib_dir = os.path.join(
             'build',
             'lib.{platform}-{version_info[0]}.{version_info[1]}'.format(
                 platform=sysconfig.get_platform(),
@@ -82,15 +107,15 @@
 def check_call(args):
     try:
         subprocess.check_call(args)
     except subprocess.CalledProcessError:
         executable = args[0]
         command = [a for a in args if not a.startswith('-')][-1]
         raise RuntimeError(command + ' failed for ' + executable)
-        
+
 class SpherogramRelease(Command):
     user_options = [('install', 'i', 'install the release into each Python')]
     def initialize_options(self):
         self.install = False
     def finalize_options(self):
         pass
     def run(self):
@@ -142,15 +167,15 @@
 pmap_src_dir = pmap_dir + '/src/'
 pmap_src_files = [pmap_src_dir + file for file in
                   ['PMdef.c', 'PMplanmap.c', 'PMenlight.c',
                    'PMconjugation.c', 'PMextract.c', 'stats.c']]
 
 Planarmap = Extension(
     name = 'spherogram.planarmap',
-    sources =  [pmap_dir + 'planarmap.c'] + pmap_src_files, 
+    sources =  [pmap_dir + 'planarmap.c'] + pmap_src_files,
     include_dirs = [pmap_src_dir],
     extra_link_args = extra_link_args
     )
 
 ext_modules.append(Planarmap)
 
 
@@ -174,35 +199,35 @@
 
 # Get long description from README
 long_description = open('README.rst').read()
 long_description = long_description.split('==\n')[1]
 long_description = long_description.split('\nDeveloped')[0]
 
 install_requires = ['decorator', 'networkx',
-                    'snappy_manifolds>=1.1', 'knot_floer_homology>=1.1']
+                    'snappy_manifolds>=1.1.2', 'knot_floer_homology>=1.2']
 
 setup( name = 'spherogram',
        version = version,
        install_requires = install_requires,
        python_requires = '>=3',
        dependency_links = [],
        packages = ['spherogram', 'spherogram.links',
                    'spherogram.links.test', 'spherogram.codecs',
                    'spherogram.dev', 'spherogram.dev.dev_jennet'],
        package_dir = {'spherogram' : 'spherogram_src', 'spherogram.dev':'dev'},
-       package_data = {'spherogram.links'  :  ['doc.pdf']}, 
+       package_data = {'spherogram.links'  :  ['doc.pdf']},
        ext_modules = ext_modules,
        cmdclass =  {'clean': SpherogramClean,
                     'test': SpherogramTest,
                     'release': SpherogramRelease,
                     'pip_install':SpherogramPipInstall,
        },
        zip_safe = False,
 
-       description= 'Spherical diagrams for 3-manifold topology', 
+       description= 'Spherical diagrams for 3-manifold topology',
        long_description = long_description,
        author = 'Marc Culler and Nathan M. Dunfield',
        author_email = 'culler@marc-culler.info, nathan@dunfield.info',
        license='GPLv2+',
        url = 'https://github.com/3-manifolds/Spherogram',
        classifiers = [
            'Development Status :: 5 - Production/Stable',
@@ -211,8 +236,7 @@
            'Operating System :: OS Independent',
            'Programming Language :: C',
            'Programming Language :: Python',
            'Topic :: Scientific/Engineering :: Mathematics',
         ],
         keywords = 'knot, link, SnapPy',
 )
-
```

### Comparing `spherogram-2.1/spherogram.egg-info/PKG-INFO` & `spherogram-2.2/spherogram.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: spherogram
-Version: 2.1
+Version: 2.2
 Summary: Spherical diagrams for 3-manifold topology
 Home-page: https://github.com/3-manifolds/Spherogram
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@marc-culler.info, nathan@dunfield.info
 License: GPLv2+
 Keywords: knot,link,SnapPy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -21,9 +20,7 @@
 Spherogram is a Python module for dealing with the kind of planar
 diagrams that arise in 3-dimensional topology, such as link and
 Heegaard diagrams. It a component of the larger
 `SnapPy <https://snappy.computop.org>`_ project.  For some basic
 examples of using Spherogram to build links, 
 `see here <https://snappy.computop.org/spherogram.html>`_.  You can
 browse the `source code <https://github.com/3-manifolds/Spherogram>`_.
-
-
```

### Comparing `spherogram-2.1/spherogram.egg-info/SOURCES.txt` & `spherogram-2.2/spherogram.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 dev/DTcodes.py
 dev/__init__.py
 dev/conventions.py
 dev/dt_issue.py
 dev/dt_tests.py
+dev/hard_links.py
+dev/issue_35.py
+dev/other_link_formats.py
 dev/sage_graph.py
 dev/sage_link_compare.py
 dev/signature.py
 dev/tangle_patch.py
 dev/dev_jennet/AlexanderKauffman.py
 dev/dev_jennet/__init__.py
 dev/dev_jennet/bridge_finding.py
```

### Comparing `spherogram-2.1/spherogram_src/codecs/Base64LikeDT.py` & `spherogram-2.2/spherogram_src/codecs/Base64LikeDT.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 are numbered, run the command Link('DT:[(6,-8),(-10,12),(-2,4)]').view()
 in SnapPy and select the "Info->DT Labels" menu item from the PLink window.)
 
 Associated to a DT code are the flips, which contain information about the signs
 of the crossings.  The flips can be deduced from the DT code, but the algorithm
 for laying out a link projection from a DT code runs faster if the flips are
 known in advance. Here, the associated flips are::
-  
+
    >>> from spherogram import DTcodec
    >>> flips = DTcodec(code).flips
    >>> flips
    [False, True, False, True, True, False]
 
 To use the base64-like encoding (without or with flips)::
 
@@ -59,42 +59,43 @@
 If there are flips, they are simply stored as bit fields following the encoding
 of the last component.
 """
 
 _base64LikeEncoding = (
     'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789+-')
 
+
 def _unsigned_int_to_char(i):
     """
     Convert an integer 0-63 to ASCII character.
     """
     return _base64LikeEncoding[i]
 
+
 def _char_to_unsigned_int(char):
     """
     Convert an ASCII character to an integer 0-63
     """
-
     i = ord(char)
-    if i >= 97 and i <= 122:  # a z
+    if 97 <= i <= 122:  # a z
         return i - 97
-    if i >= 65 and i <= 90: # A Z
+    if 65 <= i <= 90:  # A Z
         return i - 39
-    if i >= 48 and i <= 57: # 0 9
+    if 48 <= i <= 57:  # 0 9
         return i + 4
     if i == 43:
         return 62
     return 63
 
+
 def _chars_to_int(chars):
     """
     Take a string of ASCII characters and convert it to integer using the
     base64-like scheme described above.
     """
-    
     value = 0
 
     for pos, char in enumerate(chars):
         i = _char_to_unsigned_int(char)
         if pos == 0:
             # The very first bit gives the sign
             if i & (1 << 5):
@@ -102,14 +103,15 @@
             else:
                 sign = +1
             i = i & 31
         value = (value << 6) + i
 
     return sign * value
 
+
 def _consume_int_and_advance(chars, pos, num_chars):
     """
     Read the num_chars characters from the string chars and interpret it as
     base64-like encoded integer. Also return the end of that integer. This
     is supposed to be in a pattern like this::
 
         >>> chars = "abcdef"
@@ -118,137 +120,139 @@
         >>> second_integer, pos = _consume_int_and_advance(chars, pos, 2)
         >>> third_integer,  pos = _consume_int_and_advance(chars, pos, 2)
     """
 
     end = pos + num_chars
     return _chars_to_int(chars[pos:end]), end
 
+
 def _int_to_chars(value, num_chars):
     """
     Encode the given integer using base64-like encoding with num_chars
     characters.
     """
-    
+
     abs_value = abs(value)
 
     chars = ""
     for pos in range(num_chars):
         if pos == num_chars - 1:
             if value < 0:
                 abs_value |= (1 << 5)
 
         chars = _unsigned_int_to_char(abs_value & 63) + chars
         abs_value >>= 6
 
     return chars
 
+
 def _get_num_chars(code):
     """
     Given a DT code, determine the minimal number of characters to encode
     each integer so that the code fits.
     """
-    max_number = max([
-            max([abs(crossing) for crossing in comp])
-            for comp in code])
+    max_number = max(abs(crossing) for comp in code for crossing in comp)
     num_chars = 1
     while max_number > 31:
         num_chars += 1
         max_number >>= 6
     return num_chars
 
+
 def _encode_DT_code(code):
     """
     Given a DT code, convert to base64-like encoding.
     """
     num_chars = _get_num_chars(code)
-    
     # 1 -> "1", 2 -> "2", ...
-    chars  = _unsigned_int_to_char(num_chars + 52)
-
+    chars = _unsigned_int_to_char(num_chars + 52)
     chars += _int_to_chars(len(code), num_chars)
     for comp in code:
         chars += _int_to_chars(len(comp), num_chars)
         for crossing in comp:
             chars += _int_to_chars(crossing, num_chars)
-        
     return chars
 
+
 def _boolean_to_int(b):
-    return 1 if b else 0
+    return 1 if b else 0  # int(b)
+
 
 def _encode_flips(flips):
     """
     Given flips, encode as bit field.
     """
     chars = ""
 
-    padded_flips = flips + 5 * [ 0 ]
+    padded_flips = flips + 5 * [0]
 
     for pos in range(len(padded_flips) // 6):
         val = 0
         for i in range(6):
             val |= _boolean_to_int(padded_flips[6 * pos + i]) << i
         chars += _unsigned_int_to_char(val)
 
     return chars
 
-def encode_base64_like_DT_code(code, flips = None):
+
+def encode_base64_like_DT_code(code, flips=None):
     """
     Given a DT code and optionally flips, convert to base64-like encoding.
     """
     if flips:
         return _encode_DT_code(code) + _encode_flips(flips)
     else:
         return _encode_DT_code(code)
 
+
 def _decode_DT_code(chars):
     """
     Given a base64-like encoding, return the DT code and the position where
     the remaining characters not consumed yet start.
     """
     code = []
 
     # "1" -> 1, "2" -> 2
     num_chars = _char_to_unsigned_int(chars[0]) - 52
 
     num_components, pos = _consume_int_and_advance(chars, 1, num_chars)
-    
+
     for i in range(num_components):
         component = []
-        
+
         num_crossings, pos = _consume_int_and_advance(chars, pos, num_chars)
         for j in range(num_crossings):
             crossing, pos = _consume_int_and_advance(chars, pos, num_chars)
             component.append(crossing)
 
         code.append(tuple(component))
 
     return code, pos
 
+
 def _decode_flips(chars):
     """
     Read a bit field from base64-like encoding.
     """
     flips = []
     for char in chars:
         val = _char_to_unsigned_int(char)
         for j in range(6):
             flips.append(bool((val >> j) & 1))
     return flips
 
+
 def _empty_to_none(l):
-    if not l:
-        return None
-    return l
+    return l if l else None
+
 
 def decode_base64_like_DT_code(chars):
     """
     Given a base64-like encoding, return the DT code and, if present in the
     encoding as well, return the flips, otherwise None.
     """
     code, pos = _decode_DT_code(chars)
 
-    num_crossings = sum([len(component) for component in code])
+    num_crossings = sum(len(component) for component in code)
     flips = _decode_flips(chars[pos:])[:num_crossings]
 
     return code, _empty_to_none(flips)
-
```

### Comparing `spherogram-2.1/spherogram_src/codecs/DT.py` & `spherogram-2.2/spherogram_src/codecs/DT.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 
 def char_to_int(x):
     n = ord(x)
     if 96 < n < 123:
         return n - 96
     if 64 < n < 91:
-        return 64 - n  
+        return 64 - n
     raise ValueError('Not an ascii letter.')
 
 
 def string_to_ints(s):
     return [char_to_int(x) for x in s]
 
 
 def partition_list(L, parts):
     assert sum(parts) == len(L)
     ans = []
     k = 0
     for p in parts:
-        ans.append(tuple(L[k:k+p]))
+        ans.append(tuple(L[k:k + p]))
         k += p
     return ans
 
 
 DT_alphabet = '_abcdefghijklmnopqrstuvwxyzZYXWVUTSRQPONMLKJIHGFEDCBA'
 
 # To reconstruct a knot projection from a DT code we first construct
@@ -47,15 +47,15 @@
 # leaves at North; the second time it enters at East and leaves at
 # West.
 #
 #        N
 #        ^
 #        |
 #        |
-# W <--------- E second         Initial vertex orientation 
+# W <--------- E second         Initial vertex orientation
 #        |
 #        |
 #        S
 #      first
 #
 # This arbitrary choice determines some embedding of each crossing
 # into the oriented plane.  During the process of constructing a
@@ -86,15 +86,15 @@
     """
     # In keeping with the philosophy of Spherogram.graphs, vertices
     # should never be changed by graph methods.  The DTcodec can
     # do whatever it wants with them, but in this implementation
     # it never changes vertices either.
 
     def __new__(self, pair, overcrossing=1):
-        even_over = True if overcrossing == -1 else False
+        even_over = bool(overcrossing == -1)
         return tuple.__new__(self, (min(pair), max(pair), even_over))
 
     def __repr__(self):
         return str((self[0], self[1]))
 
     def entry_slot(self, N):
         if N == self[0]:
@@ -113,15 +113,15 @@
             raise ValueError('%d is not a label of %s' % (N, self))
 
     def upper_pair(self):
         first, second, even_over = self
         return (0, 2) if bool(first % 2) ^ even_over else (1, 3)
 
 
-class DTPath(object):
+class DTPath():
     """
     An iterator which starts at a FatEdge and walks around the
     link component containing that edge.  A DTPath raises
     StopIteration when it returns to its starting edge.
     """
     def __init__(self, edge, graph, forward=True):
         self.first_edge = edge
@@ -139,15 +139,15 @@
             if self.next_edge == self.first_edge:
                 raise StopIteration
         except AttributeError:
             self.next_edge = self.first_edge
         return self.next_edge
 
     __next__ = next
-    
+
 
 class DTFatEdge(FatEdge):
     """
     A fat edge which can be marked and belongs to a link component.
     """
     def __init__(self, x, y, twists=0, component=0):
         FatEdge.__init__(self, x, y, twists)
@@ -172,15 +172,15 @@
     edge_class = DTFatEdge
 
     def __init__(self):
         self.vertices = OrderedSet()
         self.edges = OrderedSet()
         self.incidence_dict = {}
         self.Edge = self.__class__.edge_class
-        self.marked_valences = dict( (v,0) for v in self.vertices )
+        self.marked_valences = {v: 0 for v in self.vertices}
         self.stack = []
         self.pushed = False
 
     def add_edge(self, x, y):
         # Adds keys to the marked_valences dict as vertices are added.
         # This will cause trouble if edges are added while edges are marked!
         edge = FatGraph.add_edge(self, x, y)
@@ -211,69 +211,64 @@
 
     def clear(self):
         """
         Remove all edge markings.
         """
         for e in self.edges:
             e.marked = False
-        self.marked_valences = dict( (v,0) for v in self.vertices )
+        self.marked_valences = {v: 0 for v in self.vertices}
 
     def push(self, flips):
         """
         Save the state of this DTFatGraph before doing the flips.
         The flips will be done by the pop.
         """
         # Ignore the first push -- the first arc always is ambiguous
         # but the choice is irrelevant, up to reflecting the plane.
         if not self.pushed:
             self.pushed = True
             return
-        #print 'pushing %s'%flips
-        self.stack.append( 
+        self.stack.append(
             [flips,
-             [ ( (e[0], e.slots[0]), (e[1], e.slots[1]), e.component )
-               for e in self.edges if e.marked],
-             [ ( (e[0], e.slots[0]), (e[1], e.slots[1]), e.component )
-               for e in self.edges if not e.marked]
-             ]
-            )
+             [((e[0], e.slots[0]), (e[1], e.slots[1]), e.component)
+              for e in self.edges if e.marked],
+             [((e[0], e.slots[0]), (e[1], e.slots[1]), e.component)
+              for e in self.edges if not e.marked]])
 
     def pop(self):
         """
         Restore the state of this DTFatGraph and perform the saved flips.
         """
         self.edges = set()
         flips, marked, unmarked = self.stack.pop()
         for x, y, component in marked:
             edge = self.add_edge(x, y)
             edge.component = component
             edge.marked = True
         for x, y, component in unmarked:
             edge = self.add_edge(x, y)
             edge.component = component
-        #print 'popped %s[%s]'%(vertex, flips)
-        #print 'stack size: %d'%len(self.stack)
         return flips
 
     def clear_stack(self):
         """
         Reset the state stack.
         """
         self.stack = []
         self.pushed = False
 
     def path(self, vertex, edge):
         """
-        Return an iteratator which iterates through the edges of a
+        Return an iterator which iterates through the edges of a
         component, starting at the given edge, in the direction
         determined by the vertex.
         """
         if vertex not in edge:
             raise ValueError('That vertex is not an endpoint of the edge.')
-        forward = True if vertex == edge[0] else False
+        forward = bool(vertex == edge[0])
         return DTPath(edge, self, forward)
 
     def marked_arc(self, vertex):
         """
         Given a vertex with marked valence 2, find the maximal marked
         arc containing the vertex for which all interior edges have
         marked valence 2.  If the marked subgraph is a circle, or a
@@ -291,23 +286,23 @@
             while True:
                 path.append(edge)
                 V = edge(V)
                 if V == vertex:
                     raise ValueError('Marked graph is a circle')
                 edges = [e for e in self(V) if e.marked and e != edge]
                 if len(edges) == 0:
-                    raise ValueError('Marked graph has a dead end at %s.'%V)
+                    raise ValueError('Marked graph has a dead end at %s.' % V)
                 if len(edges) > 1:
                     break
                 else:
                     vertices.add(V)
                     edge = edges.pop()
         left_path.reverse()
         return left_path + right_path
-                
+
     def unmarked_arc(self, vertex):
         """
         Starting at this vertex, find an unmarked edge and follow its
         component until we run into a vertex with at least one marked
         edge.  Remove loops to get an embedded arc. Return the list
         of edges traversed by the embedded arc.
         """
@@ -324,16 +319,16 @@
             edges.append(edge)
             vertex = edge(vertex)
             if self.marked_valence(vertex) > 0:
                 break
             # Remove loops as they appear
             if vertex in seen:
                 n = vertices.index(vertex)
-                edges = edges[:n+1]
-                vertices = vertices[:n+1]
+                edges = edges[:n + 1]
+                vertices = vertices[:n + 1]
                 seen = set(vertices)
             else:
                 vertices.append(vertex)
                 seen.add(vertex)
         return edges, vertex
 
     def bridge(self, marked_arc):
@@ -358,37 +353,34 @@
         # Find the interior vertices on the arc.
         e0, e1 = marked_arc[:2]
         v = e0[0] if e0[1] in e1 else e0[1]
         vertex_list = []
         for edge in marked_arc[:-1]:
             v = edge(v)
             vertex_list.append(v)
-        #print 'bridge:', marked_arc
-        #print 'avoiding:', vertex_list
         for start_vertex in vertex_list:
             # the vertex_set gets expanded to include vertices visited
             # by the bridge path.
             vertex = start_vertex
             vertex_set = set(vertex_list)
             edge_path, vertex_path, seen_edges = [], [], set()
             while True:
-                edges = [e for e in self(vertex) if
-                         not e.marked 
-                         and e not in seen_edges 
+                edges = [e for e in self(vertex) if not e.marked
+                         and e not in seen_edges
                          and e(vertex) not in vertex_set]
                 try:
                     new_edge = edges.pop()
                     vertex = new_edge(vertex)
                     edge_path.append(new_edge)
-                    if ( self.marked_valence(vertex) > 0 ):
+                    if self.marked_valence(vertex) > 0:
                         return start_vertex, vertex, edge_path
                     seen_edges.add(new_edge)
                     vertex_path.append(vertex)
                     vertex_set.add(vertex)
-                except IndexError: # Cannot continue: back up.
+                except IndexError:  # Cannot continue: back up.
                     if len(edge_path) == 0:
                         break
                     edge_path.pop()
                     vertex_set.remove(vertex_path.pop())
                     try:
                         vertex = vertex_path[-1]
                     except IndexError:
@@ -437,31 +429,30 @@
         return set(self._boundary_slots(edge, side=-1))
 
     def right_slots(self, edge):
         """
         Return the (vertex, slot) pairs on the right boundary curve.
         """
         return set(self._boundary_slots(edge, side=1))
-        
+
     def flip(self, vertex, force=False):
         """
         Move the edge at the North slot to the South slot, and
         move the edge in the South  slot to the North slot.
         """
-        #print 'flipping %s'%vertex
         if not force and self.marked_valences[vertex] > 2:
-            msg = 'Cannot flip %s with marked valence %d.'%(
+            msg = 'Cannot flip %s with marked valence %d.' % (
                 vertex, self.marked_valences[vertex])
             raise FlippingError(msg)
         self.reorder(vertex, (North, East, South, West))
 
     def incoming_under(self, vertex):
         first, second, even_over = vertex
         incoming = [e.PD_index() for e in self(vertex) if e[1] is vertex]
-        incoming.sort(key = lambda x : x%2)
+        incoming.sort(key=lambda x: x % 2)
         return incoming[0] if even_over else incoming[1]
 
     def PD_tuple(self, vertex):
         """
         Return the PD labels of the incident edges in order, starting
         with the incoming undercrossing as required for PD codes.
         """
@@ -469,59 +460,62 @@
         n = edgelist.index(self.incoming_under(vertex))
         return tuple(edgelist[n:] + edgelist[:n])
 
     def flipped(self, vertex):
         """
         Has this vertex been flipped?
         """
-        return bool(len([e for e in self(vertex) 
-                         if e[1] is vertex and e.slots[1] in (2,3)])%2)
+        return bool(len([e for e in self(vertex)
+                         if e[1] is vertex and e.slots[1] in (2, 3)]) % 2)
 
     def sign(self, vertex):
         """
         The sign of the crossing corresponding to this vertex.
         See the documentation for Spherogram.link.
         """
         flipped = self.flipped(vertex)
-        even_first = bool(vertex[0] %2 == 0)
+        even_first = bool(vertex[0] % 2 == 0)
         return -1 if (flipped ^ vertex[2] ^ even_first) else 1
 
     def KLP_strand(self, vertex, edge):
         """
         Return the SnapPea KLP strand name for the given edge at the
         end opposite to the vertex.
         """
         W = edge(vertex)
         slot = edge.slot(W)
-        return 'X' if (slot==0 or slot==2) ^ self.flipped(W) else 'Y'
-    
+        return 'X' if (slot == 0 or slot == 2) ^ self.flipped(W) else 'Y'
+
     def KLP_dict(self, vertex, indices):
         """
         Return a dict describing this vertex and its neighbors
-        in KLP terminology.  The translation from our convention is
-        as follows:
-                  Y                    Y
-                  3                    0
-                  ^                    ^
-                  |                    |
-           0 -----+----> 2 X     1 ----+---> 3 X   
-                  |                    |
-                  |                    |
-                  1                    2
-              not flipped           flipped
+        in KLP terminology.
+
+        The translation from our convention is as follows::
+
+                    Y                    Y
+                    3                    0
+                    ^                    ^
+                    |                    |
+             0 -----+----> 2 X     1 ----+---> 3 X
+                    |                    |
+                    |                    |
+                    1                    2
+               not flipped           flipped
+
         The indices argument is a dict that assigns an integer
         index to each vertex of the graph.
         """
         KLP = {}
         flipped = self.flipped(vertex)
         edges = self(vertex)
         neighbors = self[vertex]
         strands = [self.KLP_strand(vertex, edge) for edge in edges]
-        ids = [ indices[v] for v in neighbors ]
-        
+        ids = [indices[v] for v in neighbors]
+
         KLP['sign'] = 'R' if self.sign(vertex) == 1 else 'L'
         slot = 1 if flipped else 0
         KLP['Xbackward_neighbor'] = ids[slot]
         KLP['Xbackward_strand'] = strands[slot]
         slot = 3 if flipped else 2
         KLP['Xforward_neighbor'] = ids[slot]
         KLP['Xforward_strand'] = strands[slot]
@@ -535,15 +529,15 @@
         KLP['Ycomponent'] = edges[slot].component
         return KLP
 
 # This assumes that the diagram has no loops, and that each component
 # meets the next one (so in particular the diagram is connected.
 
 
-class DTcodec(object):
+class DTcodec():
     """
     Codec for DT codes of a link projection.
     """
 
     def __init__(self, input, flips=None):
         if isinstance(input, (bytes, str, list)):
             self.decode(input, flips)
@@ -573,65 +567,65 @@
         This method constructs a planar FatGraph from its input data.
         """
         if flips is not None:
             flips = [bool(flip) for flip in flips]
         self.flips = flips
         if isinstance(dt, (str,)):
             if dt[:2] == '0x':
-                dt_bytes = [int(dt[n:n+2], 16) for n in range(2,len(dt),2)]
+                dt_bytes = [int(dt[n:n + 2], 16) for n in range(2, len(dt), 2)]
                 self.code, self.flips = self.unpack_signed_DT(dt_bytes)
-            elif ord(dt[-1]) & 1<<7:
+            elif ord(dt[-1]) & 1 << 7:
                 dt_bytes = bytearray(dt)
                 self.code, self.flips = self.unpack_signed_DT(dt)
             elif dt[0] in '123456789':
                 self.code, self.flips = decode_base64_like_DT_code(dt)
             else:
                 parts = dt.split('.')
                 self.code = self.convert_alpha(parts[0])
                 if len(parts) > 1:
-                    self.flips = [False if d == '0' else True for d in parts[1]]
+                    self.flips = [d != '0' for d in parts[1]]
         elif isinstance(dt, bytes):
             self.code, self.flips = self.unpack_signed_DT(dt)
         else:
             self.code = dt
         code = self.code
-        overcrossings = [sign(x) for comp in code for x in comp]
+        overcrossings = (sign(x) for comp in code for x in comp)
         evens = [abs(x) for comp in code for x in comp]
-        self.size = size = 2*len(evens)
+        self.size = size = 2 * len(evens)
         pairs = zip(range(1, size, 2), evens)
         # Build a lookup table for the vertices.
-        # (DT codes are 1-based; we just waste the 0 entry.) 
-        self.lookup = lookup = [None for n in range(1+size)]
+        # (DT codes are 1-based; we just waste the 0 entry.)
+        self.lookup = lookup = [None for n in range(1 + size)]
         for pair, overcrossing in zip(pairs, overcrossings):
             V = DTvertex(pair, overcrossing)
             m, n = pair
             lookup[m] = lookup[n] = V
         # Now build the fatgraph determined by the DT code.
         self.fat_graph = G = DTFatGraph()
         N = start = 1
         last_odd = -1
         for c, component in enumerate(code):
             if len(component) == 0:
                 continue
-            last_odd += 2*len(component)
+            last_odd += 2 * len(component)
             V = self[N]
             # Walk around this component, adding edges.
             while N <= last_odd:
                 W = self[N + 1]
-                edge = G.add_edge( (V, V.exit_slot(N)),
-                                   (W, W.entry_slot(N+1)) )
+                edge = G.add_edge((V, V.exit_slot(N)),
+                                  (W, W.entry_slot(N + 1)))
                 edge.component = c
                 N += 1
                 V = W
             # Close up this component and go to the next one.
             S = self[start]
-            edge = G.add_edge( (V, V.exit_slot(N)),
-                               (S, S.entry_slot(start)) )
+            edge = G.add_edge((V, V.exit_slot(N)),
+                              (S, S.entry_slot(start)))
             edge.component = c
-            start = N = N+1
+            start = N = N + 1
         # Now build the planar embedding
         labels = [abs(N) for component in code for N in component]
         if self.flips is None:
             self.embed()
             # Our convention is that the first crossing is positive.
             if G.sign(self[1]) != 1:
                 for label in labels:
@@ -643,32 +637,32 @@
                     G.flip(self[label])
 
     def unpack_signed_DT(self, signed_dt):
         dt = []
         component = []
         flips = []
         for byte in bytearray(signed_dt):
-            flips.append(bool(byte & 1<<6))
-            label = (1 + byte & 0x1f)<<1
-            if byte & 1<<5:
+            flips.append(bool(byte & 1 << 6))
+            label = (1 + byte & 0x1f) << 1
+            if byte & 1 << 5:
                 label = -label
             component.append(label)
-            if byte & 1<<7:
+            if byte & 1 << 7:
                 dt.append(tuple(component))
                 component = []
         return dt, flips
 
     def convert_alpha(self, code):
         code = string_to_ints(code)
         num_crossings, components = code[:2]
-        comp_lengths = code[2:2+components]
-        crossings = [x<<1 for x in code[2+components:]]
+        comp_lengths = code[2:2 + components]
+        crossings = [x << 1 for x in code[2 + components:]]
         assert len(crossings) == num_crossings
         return partition_list(crossings, comp_lengths)
-        
+
     def encode(self, header=True, alphabetical=True, flips=True):
         """
         Returns a string describing the DT code.  Options control
         whether to include the 'DT:' header, whether to use the
         numerical or alphabetical format, and whether to use the
         extended form, which adds flip information for each crossing.
         If flips is set to "auto", only include flips in large links
@@ -700,44 +694,42 @@
                     result += encode_base64_like_DT_code(code, self.flips)
                 else:
                     result += encode_base64_like_DT_code(code)
             else:
                 prefix_ints = [num_crossings, len(code)]
                 prefix_ints += chunks
                 code_ints = [x for component in code for x in component]
-                alphacode = ''.join(tuple([DT_alphabet[n>>1]
-                                           for n in code_ints]))
-                prefix = ''.join(tuple([DT_alphabet[n] for n in prefix_ints]))
+                alphacode = ''.join(DT_alphabet[n >> 1]
+                                    for n in code_ints)
+                prefix = ''.join(DT_alphabet[n] for n in prefix_ints)
                 if flips:
-                    alphacode += '.' + ''.join([str(int(f)) for f in self.flips])
+                    alphacode += '.' + ''.join(str(int(f)) for f in self.flips)
                 result += (prefix + alphacode)
         else:
             result += str(code)
             if flips:
-                result += ',  %s'%[int(f) for f in self.flips]
-            result = result.replace(', ',',')
+                result += ',  %s' % [int(f) for f in self.flips]
+            result = result.replace(', ', ',')
         return result
 
     def embed(self, edge=None):
         """
         Try to flip crossings in the FatGraph until it becomes planar.
         """
         G = self.fat_graph
         # Add the marked_valence cache
-        if edge is None: # OK. No problem. Just pick one at random.
+        if edge is None:  # OK. No problem. Just pick one at random.
             for edge in G.edges:
                 break
         # Find a circle and embed it.
         vertices, circle_edges = self.find_circle(edge)
         G.mark(circle_edges)
-        #print 'circle', circle_edges
         # Add one arc, to get a theta graph.
         # The first arc needs to be bridge!
         first, last, arc_edges = G.bridge(circle_edges[:2])
-        #print 'first_arc', arc_edges
         self.do_flips(first, arc_edges[0], last, arc_edges[-1])
         G.mark(arc_edges)
         # Keep adding arcs until the whole graph is embedded.
         while True:
             try:
                 if not self.embed_arc():
                     break
@@ -775,15 +767,15 @@
     def get_incomplete_vertex(self):
         """
         Return a vertex with some marked and some unmarked edges.
         If there are any, return a vertex with marked valence 3.
         """
         G = self.fat_graph
         vertices = [v for v in G.vertices if 0 < G.marked_valences[v] < 4]
-        vertices.sort( key=lambda v : G.marked_valences[v] )
+        vertices.sort(key=lambda v: G.marked_valences[v])
         try:
             return vertices.pop()
         except IndexError:
             return None
 
     def do_flips(self, v, v_edge, w, w_edge):
         """
@@ -806,24 +798,24 @@
         left_slots = G.left_slots(ccw_edge)
         right_slots = G.right_slots(ccw_edge)
         v_valence, w_valence = G.marked_valences[v], G.marked_valences[w]
         if (v, vslot) in left_slots:
             v_slot_side, v_other_side = left_slots, right_slots
         else:
             v_slot_side, v_other_side = right_slots, left_slots
-        w_on_slot_side = w in [ x[0] for x in v_slot_side ]
-        w_on_other_side = w in [ x[0] for x in v_other_side ]
+        w_on_slot_side = w in [x[0] for x in v_slot_side]
+        w_on_other_side = w in [x[0] for x in v_other_side]
         if not w_on_slot_side and not w_on_other_side:
             raise EmbeddingError('Embedding does not extend.')
         if (w, wslot) in v_slot_side:
             if v_valence == w_valence == 2:
                 # This is an ambiguous situation.  We could either do
                 # nothing or flip both vertices.  Push our state with
                 # instructions to flip both vertices if we pop.
-                G.push( [v,w] )
+                G.push([v, w])
             return
         if w_valence != 2:
             G.flip(v)
             return
         elif v_valence != 2:
             G.flip(w)
             return
@@ -848,27 +840,24 @@
         v = self.get_incomplete_vertex()
         if v is None:
             return False
         if G.marked_valences[v] == 2:
             # This should work for any vertex if the diagram is prime.
             try:
                 first, last, arc_edges = G.bridge(G.marked_arc(v))
-                #print 'adding bridge', arc_edges
             except ValueError:
                 # If we can't find a bridge it means that the diagram
                 # has a separating pair of edges.  We just take any
                 # arc we can get, and see if we can find our way by
                 # pushing and popping.
-                #print 'Diagram is not prime!'
                 arc_edges, last = G.unmarked_arc(v)
                 first = v
             self.do_flips(first, arc_edges[0], last, arc_edges[-1])
         else:
             arc_edges, last_vertex = G.unmarked_arc(v)
-            #print 'adding arc', arc_edges
             # Since v has 3 marked edges, we put it second here.
             self.do_flips(last_vertex, arc_edges[-1], v, arc_edges[0])
         G.mark(arc_edges)
         return True
 
     def signed_DT(self):
         """
@@ -876,75 +865,71 @@
 
         >>> d = DTcodec([(-6,-8,-2,-4)])
         >>> d2 = DTcodec(d.signed_DT())
         >>> d2.code
         [(-6, -8, -2, -4)]
         """
         code_bytes = bytearray()
-        try:
-            next_flip = self.flips.__iter__().next
-        except AttributeError: # Python 3
-            next_flip = self.flips.__iter__().__next__
+        it = iter(self.flips)
         for component in self.code:
             for label in component:
                 byte = abs(label)
-                byte = (byte>>1) - 1
+                byte = (byte >> 1) - 1
                 if label < 0:
-                    byte |= 1<<5
-                if next_flip():
-                    byte |= 1<<6
+                    byte |= 1 << 5
+                if next(it):
+                    byte |= 1 << 6
                 code_bytes.append(byte)
-            code_bytes[-1] |= 1<<7
+            code_bytes[-1] |= 1 << 7
         return bytes(code_bytes)
 
     def hex_signed_DT(self):
         """
         Return the hex encoding of the signed DT byte sequence.
 
         >>> d = DTcodec([(-6,-8,-2,-4)])
         >>> d2 = DTcodec(d.hex_signed_DT())
         >>> d2.code
         [(-6, -8, -2, -4)]
         """
-        return '0x'+''.join(['%.2x'%b for b in bytearray(self.signed_DT())])
+        return '0x' + ''.join('%.2x' % b for b in bytearray(self.signed_DT()))
 
     def PD_code(self, KnotTheory=False):
         """
         Return a PD code for the projection described by this DT code,
         as a list of lists of 4 integers.  If KnotTheory is set to
         True, return a string that can be used as input to the Knot
         Theory package.
-       
+
         >>> d = DTcodec([(-6,-8,-2,-4)], [0,1,1,0])
         >>> sorted(d.PD_code())
         [(2, 8, 3, 7), (4, 1, 5, 2), (6, 4, 7, 3), (8, 5, 1, 6)]
         """
         G = self.fat_graph
-        PD = [ G.PD_tuple(v) for v in G.vertices ]
+        PD = [G.PD_tuple(v) for v in G.vertices]
         if KnotTheory:
-            return 'PD[%s]'%', '.join(['X%s'%repr(list(t)) for t in PD])
-        else:
-            return PD
+            return 'PD[%s]' % ', '.join('X%s' % repr(list(t)) for t in PD)
+        return PD
 
     def link(self):
         G = self.fat_graph
         crossing_dict, slot_dict = {}, {}
         for v in G.vertices:
             c = Crossing(v[0])
             c.make_tail(0)
             if G.sign(v) == 1:
                 c.make_tail(3)
             else:
                 c.make_tail(1)
             c.orient()
             crossing_dict[v] = c
-            if v.upper_pair() == (0,2):
-                slot_dict[v] = (3,0,1,2)
+            if v.upper_pair() == (0, 2):
+                slot_dict[v] = (3, 0, 1, 2)
             else:
-                slot_dict[v] = (2,3,0,1) if G.flipped(v) else (0,1,2,3)            
+                slot_dict[v] = (2, 3, 0, 1) if G.flipped(v) else (0, 1, 2, 3)
         for edge in G.edges:
             v0, v1 = edge
             s0, s1 = edge.slots
             a0, a1 = slot_dict[v0][s0], slot_dict[v1][s1]
             c0, c1 = crossing_dict[v0], crossing_dict[v1]
             c0[a0] = c1[a1]
         link = Link(list(crossing_dict.values()), check_planarity=False, build=False)
@@ -953,17 +938,17 @@
         i = 1
         for comp in self.code:
             c = self[i]
             if i == c[0]:
                 e = slot_dict[c][2] if G.flipped(c) else slot_dict[c][0]
             else:
                 e = slot_dict[c][1]
-            ce = CrossingEntryPoint(crossing_dict[c],e)
+            ce = CrossingEntryPoint(crossing_dict[c], e)
             component_starts.append(ce)
-            i += 2*len(comp)
+            i += 2 * len(comp)
         link._build_components(component_starts)
         if not link.is_planar():
             raise ValueError('DT code does not seem to define a *planar* diagram')
         return link
 
     def KLPProjection(self):
         """
```

### Comparing `spherogram-2.1/spherogram_src/graphs.py` & `spherogram-2.2/spherogram_src/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,50 +31,54 @@
 
 for x, y in G.edges:
   ...
 
 where x and y will be the two endpoints of the edge (ordered as
 tail, head in the case of directed edges).
 """
+from collections import deque
 
-_within_sage = False
 try:
     import sage.all
     import sage.graphs.graph
     _within_sage = True
 except ImportError:
+    _within_sage = False
+
+if not _within_sage:
     try:
         from .planarity import planar
         from spherogram.planarity import planar
-    except ValueError: # Allow importing from source directory
+    except ValueError:  # Allow importing from source directory
         pass
 
-from collections import deque, defaultdict
-
 
 class CyclicList(list):
     def __getitem__(self, n):
         if isinstance(n, int):
-            return list.__getitem__(self, n%len(self))
+            return list.__getitem__(self, n % len(self))
         elif isinstance(n, slice):
             # Python3 only: in python2, __getslice__ gets called instead.
             return list.__getitem__(self, n)
+
     def succ(self, x):
-        return self[(self.index(x)+1)%len(self)]
+        return self[(self.index(x) + 1) % len(self)]
+
     def pred(self, x):
-        return self[(self.index(x)-1)%len(self)]
+        return self[(self.index(x) - 1) % len(self)]
+
 
 class BaseEdge(tuple):
     """
     Base class for edges: a 2-tuple of vertices with extra methods.
     Calling a BaseEdge with one of its vertices returns the other one.
     """
 
     def __new__(cls, x, y, **kwargs):
-        return tuple.__new__(cls, (x,y))
+        return tuple.__new__(cls, (x, y))
 
     def __call__(self, end):
         """
         Calling an edge with one endpoint returns the other one.
         """
         if end is self[0]:
             return self[1]
@@ -88,55 +92,58 @@
 
     def incident_to(self):
         return list(self)
 
     def is_loop(self):
         return self[0] is self[1]
 
+
 class Edge(BaseEdge):
     """
     An undirected edge.  We allow multiple Edges between the same
     vertices, so the __eq__ operator is overloaded.
     """
 
     def __repr__(self):
-        return '%s --- %s'%self
+        return '%s --- %s' % self
 
     def __hash__(self):
         return id(self)
 
     def __eq__(self, other):
         return self is other
 
+
 class MultiEdge(BaseEdge):
     """
     An undirected edge.  MultiEdges are equal if they have the
     same vertices.  The multiplicity is initialized to 1.
     """
 
     def __init__(self, x, y):
         self.multiplicity = 1
 
     def __repr__(self):
-        return '%s --%d-- %s'%(self[0], self.multiplicity, self[1])
+        return '%s --%d-- %s' % (self[0], self.multiplicity, self[1])
 
     def __hash__(self):
         return id(self)
 
     def __eq__(self, other):
         return set(self) == set(other)
 
+
 class DirectedEdge(BaseEdge):
     """
     An Edge with a tail and a head.  The two vertices can be accessed as
     E.tail and E.head
     """
 
     def __repr__(self):
-        return '%s --> %s'%self
+        return '%s --> %s' % self
 
     def __hash__(self):
         return id(self)
 
     def __eq__(self, other):
         return self is other
 
@@ -144,51 +151,53 @@
     def head(self):
         return self[1]
 
     @property
     def tail(self):
         return self[0]
 
+
 class DirectedMultiEdge(DirectedEdge):
     """
     A DirectedEdge with multiplicity.  DirectedMultiEdges are equal if
     they have the same head and tail.  The multiplicity is initialized to 1.
     """
 
     def __init__(self, v, w):
         self.multiplicity = 1
 
     def __repr__(self):
-        return '%s --%d-> %s'%(self[0], self.multiplicity, self[1])
+        return '%s --%d-> %s' % (self[0], self.multiplicity, self[1])
 
     def __hash__(self):
         return id(self)
 
     def __eq__(self, other):
         return tuple(self) == tuple(other)
 
+
 class FatEdge(Edge):
     """
     An Edge that knows its place among the edges incident to each
     of its vertices.  Initialize with two pairs (v,n) and (w,m) meaning
     that this edge joins v to w and has index n at v and m at w.
     The parity of the optional integer argument twists determines
     whether the edge is twisted or not.
     """
     def __new__(cls, x, y, twists=0):
-        return tuple.__new__(cls, (x[0],y[0]))
+        return tuple.__new__(cls, (x[0], y[0]))
 
     def __init__(self, x, y, twists=0):
-        self.slots = [x[1],y[1]]
-        self.twisted = True if twists%2 != 0 else False
+        self.slots = [x[1], y[1]]
+        self.twisted = bool(twists % 2)
 
     def __repr__(self):
-        return '%s[%d] -%s- %s[%d]'%(self[0], self.slots[0],
-                                     'x' if self.twisted else '-',
-                                     self[1], self.slots[1])
+        return '%s[%d] -%s- %s[%d]' % (self[0], self.slots[0],
+                                       'x' if self.twisted else '-',
+                                       self[1], self.slots[1])
 
     def __hash__(self):
         return id(self)
 
     def slot(self, vertex):
         try:
             return self.slots[self.index(vertex)]
@@ -197,15 +206,16 @@
 
     def set_slot(self, vertex, n):
         try:
             self.slots[self.index(vertex)] = n
         except ValueError:
             raise ValueError('Vertex is not an end of this edge.')
 
-class Graph(object):
+
+class Graph():
     """
     A set of vertices and a set of edges joining pairs of vertices.
     Vertices are arbitrary hashable objects and should not be
     modified by Graph methods.
     """
     edge_class = Edge
 
@@ -220,17 +230,17 @@
             self.add_vertex(vertex)
         self._validate()
 
     def _validate(self):
         pass
 
     def __repr__(self):
-        V = 'Vertices:\n  ' + '\n  '.join([str(v) for v in self.vertices])
-        E = 'Edges:\n  ' + '\n  '.join([str(e) for e in self.edges])
-        return '%s\n%s'%(V,E)
+        V = 'Vertices:\n  ' + '\n  '.join(str(v) for v in self.vertices)
+        E = 'Edges:\n  ' + '\n  '.join(str(e) for e in self.edges)
+        return '%s\n%s' % (V, E)
 
     def __call__(self, vertex):
         """
         Return a list of incident edges, including loops, which appear
         twice.
         """
         return self.incidence_dict[vertex]
@@ -243,15 +253,15 @@
 
     def incident(self, vertex):
         """
         Return the set of non-loops incident to the vertex.
         """
         return set(e for e in self.incidence_dict[vertex] if not e.is_loop())
 
-    def edges_between(self,vertex1,vertex2):
+    def edges_between(self, vertex1, vertex2):
         return self.incident(vertex1).intersection(self.incident(vertex2))
 
     # Allow flows to go in either direction across an edge.
     flow_incident = incident
 
     def children(self, vertex):
         """
@@ -327,23 +337,23 @@
         extending paths.  For example, Digraphs set flow_incident =
         outgoing.
         """
         incident = self.flow_incident if for_flow else self.incident
         initial = incident(source) - forbidden
         seen = forbidden | initial
         # Use a deque since we need to popleft.
-        fifo = deque([ (None, source, e) for e in initial ])
+        fifo = deque([(None, source, e) for e in initial])
         while fifo:
             parent, vertex, child = fifo.popleft()
             new_edges = incident(child(vertex)) - seen
             seen |= new_edges
             fifo.extend([(child, child(vertex), edge) for edge in new_edges])
             yield parent, vertex, child
 
-    def next(self):  #For Python 2 compatibility
+    def next(self):  # For Python 2 compatibility
         return self.__next__()
 
     def components(self, deleted_vertices=[]):
         """
         Return the vertex sets of the connected components of the
         graph obtained by removing the deleted_vertices and any edges
         incident to them.
@@ -426,62 +436,62 @@
         if capacity is None:
             residual = dict.fromkeys(self.edges, 1)
         else:
             residual = dict.copy(capacity)
             for e in self.edges:
                 if e not in residual:
                     residual[e] = float('inf')
-        full_edges = set([e for e in self.edges if residual[e] == 0])
+        full_edges = set(e for e in self.edges if residual[e] == 0)
         children = {}
         for vertex in self.vertices:
             children[vertex] = set()
         cut_set = set()
         path_list = []
         while True:
             # Try to find a new path from source to sink
             parents, cut_set, reached_sink = {}, set([source]), False
             generator = self.breadth_first_edges(
                 source=source,
                 forbidden=full_edges,
                 for_flow=True)
             for parent, vertex, child in generator:
-                 parents[child] = (parent, vertex)
-                 cut_set.add(child(vertex))
-                 if child(vertex) == sink:
-                     reached_sink = True
-                     break
+                parents[child] = (parent, vertex)
+                cut_set.add(child(vertex))
+                if child(vertex) == sink:
+                    reached_sink = True
+                    break
             # If we did not get to the sink, we visited every vertex
             # reachable from the source, thereby providing the cut
             # set.
             if not reached_sink:
                 break
             # If we got to the sink, do the bookkeeping and continue.
             path = deque()
             flow = residual[child]
             while True:
-                path.appendleft( (vertex, child) )
+                path.appendleft((vertex, child))
                 children[vertex].add(child)
                 if vertex == source:
                     break
                 child = parent
                 parent, vertex = parents[child]
                 flow = min(flow, residual[child])
             for vertex, edge in path:
                 residual[edge] -= flow
                 if residual[edge] == 0:
                     full_edges.add(edge)
-            path_list.append( (flow, path) )
+            path_list.append((flow, path))
         # Find the cut edges.
         cut_edges = set()
         for vertex in cut_set:
-            cut_edges |= set([edge for edge in self.edges
-                              if vertex in edge
-                              and edge(vertex) not in cut_set])
+            cut_edges |= set(edge for edge in self.edges
+                             if vertex in edge
+                             and edge(vertex) not in cut_set)
         # Find the unsaturated edges.
-        unsaturated = [ e for e in self.edges if residual[e] > 0 ]
+        unsaturated = [e for e in self.edges if residual[e] > 0]
         flow_dict = dict.fromkeys(self.edges, 0)
         # Compute the flow.
         for flow, edges in path_list:
             for vertex, edge in edges:
                 if vertex == edge[0]:
                     flow_dict[edge] += flow
                 else:
@@ -508,98 +518,95 @@
 
         >>> G = Graph([(0,1),(1,2),(2,0)]).mergeable()
         >>> F = lambda x: frozenset([x])
         >>> G.merge(F(1),F(2))
         >>> set(G.vertices) == {frozenset([1, 2]), frozenset([0])}
         True
         """
-        new_vertex = V1|V2
+        new_vertex = V1 | V2
         if new_vertex in self.vertices:
             raise ValueError('Merged vertex already exists!')
-        self.edges -= set([e for e in self.edges if V1 in e and V2 in e])
+        self.edges -= set(e for e in self.edges if V1 in e and V2 in e)
         self.vertices.remove(V1)
         self.vertices.remove(V2)
         old_vertices = (V1, V2)
         self.vertices.add(new_vertex)
         for edge in [e for e in self.edges if V1 in e or V2 in e]:
             self.edges.remove(edge)
             x, y = edge
             if x in old_vertices:
-                self.edges.add( self.Edge(new_vertex, y) )
+                self.edges.add(self.Edge(new_vertex, y))
             if y in old_vertices:
-                self.edges.add( self.Edge(x, new_vertex) )
+                self.edges.add(self.Edge(x, new_vertex))
 
     def mergeable(self):
         """
         Return a new graph whose vertices are singleton frozensets,
         each containing a vertex of this graph, and with edges
         corresponding to those of this graph.  The new graph
         will support merging vertices.
         """
         V = [frozenset([v]) for v in self.vertices]
         E = [self.Edge(frozenset([x]), frozenset([y])) for x, y in self.edges]
-        return self.__class__(E,V)
+        return self.__class__(E, V)
 
     def to_networkx(self):
         """
         Return a copy of the graph in the networkx format
         """
         G = nx.Graph()
         G.add_nodes_from(self.vertices)
         G.add_edges_from(self.edges)
         return G
 
+
 class ReducedGraph(Graph):
     """
     A graph with at most one edge between any two vertices,
     but having edges with multiplicities.
     """
     edge_class = MultiEdge
 
     def __init__(self, pairs=[], singles=[]):
         self.Edge = self.__class__.edge_class
         self.find_edge = dict()
         Graph.__init__(self, pairs, singles)
 
     def add_edge(self, x, y):
-        if (x,y) in self.find_edge:
+        if (x, y) in self.find_edge:
             edge = self.find_edge[(x, y)]
             edge.multiplicity += 1
         else:
             edge = self.Edge(x, y)
-            self.vertices.update([x,y])
+            self.vertices.update([x, y])
             self.edges.add(edge)
-            self.find_edge[(x,y)] = edge
+            self.find_edge[(x, y)] = edge
             for v in edge:
                 try:
                     self.incidence_dict[v].append(edge)
                 except KeyError:
                     self.incidence_dict[v] = [edge]
         return edge
 
     def multi_valence(self, vertex):
         """
         Return the valence of a vertex, counting edge multiplicities.
         """
-        valence = 0
-        for e in self.incidence_dict[vertex]:
-                valence += e.multiplicity
-        return valence
+        return sum(e.multiplicity for e in self.incidence_dict[vertex])
 
     def is_planar(self):
         """
         Return the planarity.
         """
-
         verts_with_loops = set()
         non_loop_edges = set()
         for e in self.edges:
             v, w = e
             if v != w:
-                non_loop_edges.add( (v, w) )
+                non_loop_edges.add((v, w))
             else:
                 verts_with_loops.add(v)
 
         sans_loops = ReducedGraph(non_loop_edges)
         if _within_sage:
             S = sans_loops.sage(loops=False, multiedges=False)
             is_planar = S.is_planar(set_embedding=True)
@@ -615,31 +622,31 @@
         return is_planar
 
     def embedding(self):
         if self.is_planar():
             return self._embedding
 
     def one_min_cut(self, source, sink):
-        capacity = dict((e, e.multiplicity) for e in self.edges)
+        capacity = {e: e.multiplicity for e in self.edges}
         cut = Graph.one_min_cut(self, source, sink, capacity)
-        cut['size'] = sum([e.multiplicity for e in cut['edges'] ])
+        cut['size'] = sum(e.multiplicity for e in cut['edges'])
         return cut
 
     def cut_pairs(self):
         """
         Return a list of cut_pairs.  The graph is assumed to be
         connected and to have no cut vertices.
         """
         pairs = []
         majors = [v for v in self.vertices if self.valence(v) > 2]
         if len(majors) == 2:
             v, V = majors
             if self.valence(v) == 3:
                 return []
-            edge = self.find_edge[(v,V)]
+            edge = self.find_edge[(v, V)]
             if not edge or edge.multiplicity < 2:
                 return []
             return majors
         major_set = set(majors)
         for n in range(1, len(majors)):
             for v in majors[:n]:
                 pair = (v, majors[n])
@@ -687,61 +694,59 @@
         self.edges.add(edge)
         self.vertices.update(edge)
         for v in edge:
             # the values of incidence_dict should be objects that keep
             # themselves sorted.
             if v in incidences:
                 incidences[v].append(edge)
-                incidences[v].sort(key=lambda e : e.slot(v))
+                incidences[v].sort(key=lambda e: e.slot(v))
             else:
                 incidences[v] = CyclicList([edge])
         return edge
 
     def _validate(self):
         for v in self.vertices:
             slots = [e.slot(v) for e in self(v)]
             assert slots == range(len(slots))
 
     def reorder(self, vertex, cyclist):
         for e, n in zip(self(vertex), cyclist):
             e.set_slot(vertex, n)
-        self.incidence_dict[vertex].sort(key=lambda e : e.slot(vertex))
+        self.incidence_dict[vertex].sort(key=lambda e: e.slot(vertex))
 
     def boundary_cycles(self):
-        left  = [(e[0], e, 'L') for e in self.edges]
+        left = [(e[0], e, 'L') for e in self.edges]
         right = [(e[0], e, 'R') for e in self.edges]
         sides = left + right
         cycles = []
         while sides:
             cycle = []
             v, e, s = start = sides.pop()
-            #print('start:', start)
             while True:
                 cycle.append(e)
                 # cross the edge
                 v = e(v)
-                if (
-                    ( e.twisted and s=='L') or
-                    ( not e.twisted and (s=='L')==(v==e[0]) )
-                    ): # go counter-clockwise
+                if ((e.twisted and s == 'L') or
+                        (not e.twisted and (s == 'L') == (v == e[0]))):
+                    # go counter-clockwise
                     e = self(v).succ(e)
                     s = 'R' if e.twisted or v == e[0] else 'L'
-                else: # go clockwise
+                else:  # go clockwise
                     e = self(v).pred(e)
                     s = 'L' if e.twisted or v == e[0] else 'R'
-                if (e[0],e,s) == start:
+                if (e[0], e, s) == start:
                     cycles.append(cycle)
                     break
-                #print('next', (e[0],e,s))
-                sides.remove( (e[0],e,s) )
+                sides.remove((e[0], e, s))
         return cycles
 
     def filled_euler(self):
         return len(self.vertices) - len(self.edges) + len(self.boundary_cycles())
 
+
 class Digraph(Graph):
     """
     A directed graph.  This subclass adds methods for finding incoming
     and outgoing edges, indegree and outdegree, and deals with all
     three notions of connectedness for digraphs.
 
     >>> G = Digraph([(0,1),(1,2),(2,3),(3,1),(4,2)])
@@ -767,25 +772,25 @@
     edge_class = DirectedEdge
 
     def outgoing(self, vertex):
         """
         Return the set of non-loop edges which *begin* at the vertex.
         """
         return set(e for e in self(vertex)
-                     if e.tail is vertex and not e.head is vertex)
+                   if e.tail is vertex and e.head is not vertex)
 
     # Force flows to go in the direction of the edge.
     flow_incident = outgoing
 
     def incoming(self, vertex):
         """
         Return the set of non-loop edges which *end* at the vertex.
         """
         return set(e for e in self(vertex)
-                     if e.head is vertex and not e.tail is vertex)
+                   if e.head is vertex and e.tail is not vertex)
 
     def children(self, vertex):
         """
         Return the set of distinct vertices which are endpoints of
         outgoing non-loop edges.
         """
         return set(e(vertex) for e in self.outgoing(vertex))
@@ -818,19 +823,16 @@
         strong component DAG be a linear order.  Note that
         reachability is not a symmetric relation, so there is no
         associated notion of a connected component.
         """
         DAG = self.component_DAG()
         if not DAG.is_weakly_connected():
             return False
-        elif [v for v in DAG.vertices
-              if DAG.indegree(v)>1 or DAG.outdegree(v)>1]:
-            return False
-        else:
-            return True
+        return all(DAG.indegree(v) <= 1 and DAG.outdegree(v) <= 1
+                   for v in DAG.vertices)
 
     def strong_components(self):
         """
         Return the vertex sets of the strongly connected components.
 
         >>> G = Digraph([(0,1),(0,2),(1,2),(2,3),(3,1)])
         >>> G.strong_components() == [frozenset([1, 2, 3]), frozenset([0])]
@@ -861,15 +863,16 @@
         >>> sorted(C.vertices) == [frozenset([1, 2, 3]), frozenset([0])]
         True
         >>> [tuple(e) for e in C.edges] == [(frozenset([0]), frozenset([1, 2, 3]))]
         True
         """
         return StrongConnector(self).DAG()
 
-class StrongConnector(object):
+
+class StrongConnector():
     """
     Finds strong components of a digraph using Tarjan's algorithm;
     see http://en.wikipedia.org/wiki/Tarjan%27s_strongly_connected_components_algorithm
     """
     def __init__(self, digraph):
         self.digraph = digraph
         self.seen = []
@@ -917,125 +920,147 @@
         joining two components if and only if there is an edge of the
         underlying digraph having an endpoint in each component.
         Using self.links, rather than self.digraph.edges, is a slight
         optimization.
         """
         edges = set()
         for tail, head in self.links:
-            dag_tail= self.which_component[tail]
+            dag_tail = self.which_component[tail]
             dag_head = self.which_component[head]
             if dag_head != dag_tail:
-                edges.add( (dag_tail, dag_head) )
+                edges.add((dag_tail, dag_head))
         return Digraph(edges, self.components)
 
 
 class Poset(set):
     """
     A partially ordered set, generated from a directed acyclic graph.
-    Instantiate with a Digraph.  A ValueError exception is raised if the
+
+    Instantiate with a Digraph.  A ``ValueError`` exception is raised if the
     Digraph contains a cycle.
     """
     def __init__(self, digraph):
         self.elements = set(digraph.vertices)
-        self.larger = {}
-        self.smaller = {}
-        self.successors = {}
+        self.larger = {vertex: set() for vertex in self}
+        self.smaller = {vertex: set() for vertex in self}
+        self.successors = {vertex: set(digraph[vertex]) for vertex in self}
         self.closed = set()
-        for vertex in self:
-            self.larger[vertex] = set()
-            self.smaller[vertex] = set()
-            self.successors[vertex] = set(digraph[vertex])
-        seen = []
+        seen = set()
         for vertex in self:
             if vertex not in seen:
                 self.search(vertex, seen, digraph)
 
     def __iter__(self):
         return self.elements.__iter__()
 
     def __len__(self):
         return len(self.elements)
 
     def search(self, vertex, seen, digraph):
-        seen.append(vertex)
+        seen.add(vertex)
         for child in digraph.children(vertex):
             if child in self.smaller[vertex]:
                 raise ValueError('Digraph is not acyclic.')
             self.smaller[child].add(vertex)
             self.smaller[child] |= self.smaller[vertex]
             self.search(child, seen, digraph)
             self.larger[vertex].add(child)
             self.larger[vertex] |= self.larger[child]
 
     def compare(self, x, y):
         if x == y:
             return 0
-        elif x in self.smaller[y]:
+        if x in self.smaller[y]:
             return 1
-        elif y in self.smaller[x]:
+        if y in self.smaller[x]:
             return -1
-        else:
-            return None
+        return None
 
     def incomparable(self, x):
         """
         Return the elements which are not comparable to x.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> sorted(P.incomparable(3))
+        [1, 2]
         """
         return self.elements - self.smaller[x] - self.larger[x] - set([x])
 
     def smallest(self):
         """
         Return the subset of minimal elements.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> sorted(P.smallest())
+        [0]
         """
         return frozenset([x for x in self if not self.smaller[x]])
 
     def largest(self):
         """
         Return the subset of maximal elements.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> sorted(P.largest())
+        [4]
         """
-        return frozenset( [ x for x in self if not self.larger[x] ] )
+        return frozenset([x for x in self if not self.larger[x]])
 
     def closure(self, A):
         """
         Return the smallest set X containing A which is is closed
         under < , i.e. such that (x in X and y < x) => y in X.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> sorted(P.closure([1, 3]))
+        [0, 1, 3]
         """
         result = frozenset(A)
         for a in A:
             result |= self.smaller[a]
-        if len(result) == len(A):
-            return result
-        else:
-            return self.closure(result)
+        return result
 
     def XXclosed_subsets(self, start=None):
         """
         Generator for all transitively closed subsets.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> len(list(P.XXclosed_subsets()))
+        7
         """
         if start is None:
             if self.closed:
                 for subset in self.closed:
                     yield subset
                 return
             else:
                 start = self.smallest()
         complement = self.elements - start
         if start not in self.closed:
             self.closed.add(start)
             yield start
         for element in complement:
-            # print( 'adding ', element)
             extended = self.closure(start | set([element]))
             for subset in self.XXclosed_subsets(extended):
                 yield subset
 
     def XXXclosed_subsets(self, start=None):
         """
         Generator for all transitively closed subsets.  The subsets
         are computed once, then cached for use in subsequent calls.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> len(list(P.XXXclosed_subsets()))
+        7
         """
         if start is None:
             if self.closed:
                 for subset in self.closed:
                     yield subset
                 return
             else:
@@ -1050,48 +1075,59 @@
             extended = self.closure(start | set([child]))
             for subset in self.XXXclosed_subsets(extended):
                 yield subset
 
     def closed_subsets(self):
         """
         Generator for all nonempty transitively closed subsets.
+
+        >>> G = Digraph([(0,1),(1,2),(2,4),(0,3),(3,4)])
+        >>> P = Poset(G)
+        >>> len(list(P.closed_subsets()))
+        7
         """
         # A closed subset is the closure of its set of maximal
         # elements, which is an arbitrary subset of pairwise
         # incomparable elements.  For the empty relation, every subset
         # is pairwise incomparable.  So, in general, this can easily
         # generate exponentially many subsets.
         #
         # This is used for finding level transformations of group
         # presentations.  We should think about taking advantage of
         # the special features of that situation.  For now, though, we
         # just iterate through all subsets and check each one.
 
         for X in powerset(self.elements):
-            if 0 < len(X):
-                pairwise_incomparable = True
-                for x in X:
-                    if ( X.intersection(self.smaller[x]) or
-                         X.intersection(self.larger[x]) ):
-                        pairwise_incomparable = False
-                        break
-                if pairwise_incomparable:
-                    yield self.closure(X)
+            if not X:
+                continue
+            pairwise_incomparable = True
+            for x in X:
+                if any(y in self.smaller[x] or y in self.larger[x]
+                       for y in X):
+                    pairwise_incomparable = False
+                    break
+            if pairwise_incomparable:
+                yield self.closure(X)
 
 
 def powerset(S):
-    """Recursive generator for all subsets of a set."""
+    """
+    Recursive generator for all subsets of a set.
+
+    >>> [len(u) for u in powerset({2,3,5})]
+    [2, 2, 1, 2, 1, 1, 0]
+    """
     X = S.copy()
     while X:
         for x in X:
             break
         X.remove(x)
         singleton = set([x])
         for Y in powerset(X):
-            yield(singleton | Y)
+            yield (singleton | Y)
         yield X
 
 
 if _within_sage:
     def _to_sage(self, loops=True, multiedges=True):
         S = sage.graphs.graph.Graph(loops=loops, multiedges=multiedges)
         S.add_vertices(self.vertices)
```

### Comparing `spherogram-2.1/spherogram_src/links/__init__.py` & `spherogram-2.2/spherogram_src/links/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from .links import Crossing, Strand, Link, ClosedBraid
+import os
+import sys
 
-from .tangles import Tangle, RationalTangle, ZeroTangle, InfinityTangle, IdentityBraid, join_strands
+from .links import Crossing, Strand, Link, ClosedBraid
+from .tangles import Tangle, CapTangle, CupTangle, RationalTangle, ZeroTangle, InfinityTangle, MinusOneTangle, OneTangle, IntegerTangle, IdentityBraid, ComponentTangle, join_strands
 from . import orthogonal
-Link.view = orthogonal.orthogonal_draw
-import os, sys
 from .random_links import random_link
 
+Link.view = orthogonal.orthogonal_draw
+
+
 def pdf_docs():
     "Open the PDF docs for links and tangles using the default application"
     file = __path__[0] + os.sep + "doc.pdf"
     if sys.platform.startswith('darwin'):
         command = 'open'
     elif sys.platform.startswith('win'):
         command = 'start'
     else:
         command = 'xdg-open'
     os.system(command + ' ' + file)
 
-__all__ = ['Crossing', 'Strand', 'Link', 'ClosedBraid', 'Tangle', 'RationalTangle',
-    'ZeroTangle', 'InfinityTangle', 'IdentityBraid', 'join_strands',
-    'pdf_docs', 'random_link']
+
+__all__ = ['Crossing', 'Strand', 'Link', 'ClosedBraid',
+           'Tangle', 'CapTangle', 'CupTangle', 'RationalTangle',
+           'ZeroTangle', 'InfinityTangle', 'MinusOneTangle', 'OneTangle', 'IntegerTangle',
+           'IdentityBraid', 'join_strands',
+           'pdf_docs', 'random_link']
```

### Comparing `spherogram-2.1/spherogram_src/links/alexander.py` & `spherogram-2.2/spherogram_src/links/alexander.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     The two entry points of a crossing with Dror's convention that the
     overcrossing ("a") is first and the undercrossing ("b") is second.
     """
     verts = [1, 0] if crossing.sign == -1 else [3, 0]
     return [CrossingEntryPoint(crossing, v) for v in verts]
 
 
-class StrandIndices(object):
+class StrandIndices():
     """
     A map from the crossings strands of a link L onto range(n).
     """
     def __init__(self, link, ordered_crossings=None):
         indices = dict()
         if ordered_crossings is None:
             ordered_crossings = link.crossings
@@ -86,19 +86,19 @@
     """
     assert a != b
     alpha, beta = A[a, a], A[a, b]
     gamma, delta = A[b, a], A[b, b]
     mu = 1 - beta
     theta, epsilon = A.row(a), A.row(b)
     phi, psi = A.column(a), A.column(b)
-    A = A + matrix(psi).transpose()*matrix(theta)/mu
+    A = A + matrix(psi).transpose() * matrix(theta) / mu
     i, j = min(a, b), max(a, b)
-    A[i] = epsilon + delta*theta/mu
-    A[:, i] = phi + alpha*psi/mu
-    A[i, i] = gamma + alpha*delta/mu
+    A[i] = epsilon + delta * theta / mu
+    A[:, i] = phi + alpha * psi / mu
+    A[i, i] = gamma + alpha * delta / mu
     A = A.delete_rows([j])
     A = A.delete_columns([j])
     return A
 
 
 def test_meta_associativity():
     """
@@ -107,24 +107,22 @@
     def eval_merges(merges):
         R = PolynomialRing(QQ, 'x', 49).fraction_field()
         A = matrix(7, 7, R.gens())
         for a, b in merges:
             A = strand_matrix_merge(A, a, b)
         return A
 
-    associative_merges = [
-        ([(0,1), (0,1)], [(1,2), (0,1)]),
-        ([(0,1), (0,2)], [(1,3), (0,1)]),
-        ([(2,5), (2,3)], [(5,3), (2,3)])
-        ]
+    associative_merges = [([(0, 1), (0, 1)], [(1, 2), (0, 1)]),
+                          ([(0, 1), (0, 2)], [(1, 3), (0, 1)]),
+                          ([(2, 5), (2, 3)], [(5, 3), (2, 3)])]
     for m1, m2 in associative_merges:
         assert eval_merges(m1) == eval_merges(m2)
 
 
-class DrorDatum(object):
+class DrorDatum():
     """
     The (omega, A) pair which is the invariant defined in the first column of
     http://www.math.toronto.edu/drorbn/Talks/Aarhus-1507/
     """
     def __init__(self, link, ordered_crossings):
         self.strand_indices = StrandIndices(link, ordered_crossings)
         self.ring = R = PolynomialRing(ZZ, 't').fraction_field()
@@ -149,19 +147,19 @@
         mu = 1 - A[a, b]
         self.omega *= mu
         self.A = strand_matrix_merge(A, a, b)
         indices.merge(cs_a, cs_b)
 
 
 def num_overlap(crossing, frontier):
-    neighbor_strands = set([cs.opposite() for cs in crossing.crossing_strands()])
+    neighbor_strands = set(cs.opposite() for cs in crossing.crossing_strands())
     return len(neighbor_strands.intersection(frontier))
 
 
-class Exhaustion(object):
+class Exhaustion():
     """
     An exhaustion of a link where crossings are added in one-by-one
     so that the resulting tangle is connected at every stage.
 
     Starting at the given crossing, it uses a greedy algorithm to try
     to minimize the sizes of the frontiers of the intermediate tangles.
 
@@ -172,30 +170,30 @@
             crossing = random.choice(link.crossings)
         crossings = [crossing]
         gluings = [[]]
         frontier = set(crossing.crossing_strands())
         frontier_lengths = [4]
         while len(crossings) < len(link.crossings):
             choices = [(num_overlap(cs.opposite()[0], frontier), cs) for cs in frontier]
-            overlap, cs = max(choices, key=lambda x:x[0])
+            overlap, cs = max(choices, key=lambda x: x[0])
             C = cs.opposite().crossing
             assert C not in crossings
             crossings.append(C)
             C_gluings = []
             for cs in C.crossing_strands():
                 opp = cs.opposite()
                 if opp in frontier:
                     frontier.discard(opp)
                     b = cs.oriented()
                     a = b.opposite()
                     C_gluings.append((a, b))
                 else:
                     frontier.add(cs)
 
-            assert frontier_lengths[-1] + 4 - 2*overlap == len(frontier)
+            assert frontier_lengths[-1] + 4 - 2 * overlap == len(frontier)
             frontier_lengths.append(len(frontier))
             gluings.append(C_gluings)
 
         self.link = link
         self.crossings = crossings
         self.frontier_lengths = frontier_lengths
         self.gluings = gluings
```

### Comparing `spherogram-2.1/spherogram_src/links/doc.pdf` & `spherogram-2.2/spherogram_src/links/doc.pdf`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/spherogram_src/links/draw.py` & `spherogram-2.2/spherogram_src/links/draw.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.1/spherogram_src/links/exhaust.py` & `spherogram-2.2/spherogram_src/links/exhaust.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if a < i:
             ans[a] = v
         if a > i + 1:
             ans[a - 2] = v
     return ans
 
 
-class Event(object):
+class Event():
     """
     There are three kinds of events:
 
     * ('cup', a, b, c=None): Introduce a new oriented strand with
       endpoints a and b oriented from a to b.  The optional argument c
       is the index of the link component in the final link.
 
@@ -55,15 +55,15 @@
     def __repr__(self):
         ans = (self.kind, self.a, self.b)
         if self.c is not None:
             ans += (self.c,)
         return repr(ans)
 
 
-class MorseEncoding(object):
+class MorseEncoding():
     """
     A MorseEncoding is a concrete encoding of a Morse diagram of an
     oriented link in the sprit of:
 
     http://katlas.org/wiki/MorseLink_Presentations
 
     as a sequence of events.  At each stage, there are n active strand
@@ -76,18 +76,18 @@
     >>> me = MorseEncoding(events)
     >>> me.events[1:3]
     [('cup', 0, 1), ('cross', 1, 2)]
     >>> me.width
     4
     >>> me_copy = MorseEncoding(me.events)
     >>> L = me.link()
-    >>> L.exterior().identify()[0]
+    >>> L.exterior().identify()[0]  #doctest: +SNAPPY
     m004(0,0)
     >>> U = MorseEncoding([('cup', 0, 1), ('cap', 0, 1)]).link()
-    >>> U.exterior().fundamental_group().num_generators()
+    >>> U.exterior().fundamental_group().num_generators()  #doctest: +SNAPPY
     1
     """
 
     def __init__(self, events):
         self.events = []
         for event in events:
             if not isinstance(event, Event):
@@ -142,15 +142,15 @@
                     active[event.b] = C[1]
         return Link(crossings)
 
     def __iter__(self):
         return self.events.__iter__()
 
 
-class BiDict(object):
+class BiDict():
     """
     A bijective mapping from range(n) to a set of hashable non-integers.
 
     >>> bd = BiDict({0:'a', 1:'b', 2:'c', 3:'d'})
     >>> bd[0], bd['b']
     ('a', 1)
     >>> bd._check()
@@ -176,15 +176,15 @@
     BiDict({0: 'u', 1: 'v', 2: 'a', 3: 'x', 4: 'y', 5: 'd', 6: 'f'})
     >>> sorted(bd.values())
     ['a', 'd', 'f', 'u', 'v', 'x', 'y']
     """
 
     def __init__(self, int_to_set_dict):
         self.n = n = len(int_to_set_dict)
-        assert sorted(int_to_set_dict.keys()) == list(range(n))
+        assert sorted(int_to_set_dict) == list(range(n))
         self.int_to_set = int_to_set_dict
         self.set_to_int = {v: k for k, v in int_to_set_dict.items()}
 
     def __getitem__(self, index):
         if isinstance(index, int):
             return self.int_to_set[index]
         elif index in self.set_to_int:
@@ -241,23 +241,23 @@
         self.set_to_int = {k: shift(v) for k, v in self.set_to_int.items()}
 
     def values(self):
         return self.int_to_set.values()
 
     def __repr__(self):
         itos = self.int_to_set
-        keys = sorted(itos.keys())
+        keys = sorted(itos)
         items = ['%d: %s' % (k, repr(itos[k])) for k in keys]
         return 'BiDict({' + ', '.join(items) + '})'
 
     def __len__(self):
         return len(self.int_to_set)
 
     def _check(self):
-        return sorted(self.int_to_set.keys()) == list(range(self.n))
+        return sorted(self.int_to_set) == list(range(self.n))
 
 
 def is_range(L):
     """
     >>> is_range([2, 3, 4]), is_range([2, 3, 5])
     (True, False)
     """
@@ -287,15 +287,15 @@
             if is_range(overlap):
                 possible.append((len(overlap), min(overlap), crossing))
         max_overlap = max(possible)[0]
         good_choices = [pos for pos in possible if pos[0] == max_overlap]
         return random.choice(good_choices)
 
 
-class MorseExhaustion(object):
+class MorseExhaustion():
     """
     An exhaustion of a link where crossings are added in one-by-one
     so that the resulting tangle is connected at every stage.
 
     Starting at the given crossing, it uses a greedy algorithm to try
     to minimize the sizes of the frontiers of the intermediate tangles.
 
@@ -305,27 +305,37 @@
     If no initial crossing is specified, one is chosen at random.
 
     >>> L = Link('L2a1')
     >>> mexhaust = MorseExhaustion(L, L.crossings[0])
     >>> mexhaust
     [('cup', 0, 1), ('cup', 0, 1), ('cross', 1, 2), ('cross', 1, 2), ('cap', 0, 1), ('cap', 0, 1)]
     >>> me = MorseEncoding(mexhaust)
-    >>> me.link().exterior().fundamental_group().relators()
+    >>> me.link().exterior().fundamental_group().relators() #doctest: +SNAPPY
     ['abAB']
-    """
 
+    >>> K = Link([[0, 0, 1, 1]])  # Unknot
+    >>> MorseExhaustion(K)
+    [('cup', 0, 1), ('cup', 0, 1), ('cross', 1, 2), ('cap', 0, 1), ('cap', 0, 1)]
+    """
     def __init__(self, link, crossing=None):
         events = []
-        if crossing is None:
-            crossing = random.choice(link.crossings)
-        crossings = [crossing]
-        events = [('cup', 0, 1), ('cup', 0, 1), ('cross', 1, 2)]
-        css = crossing.crossing_strands()
-        frontier = Frontier({0: css[3], 1: css[2], 2: css[1], 3: css[0]})
-        frontier_lengths = [4]
+        if link.crossings:
+            if crossing is None:
+                crossing = random.choice(link.crossings)
+            crossings = [crossing]
+            events = [('cup', 0, 1), ('cup', 0, 1), ('cross', 1, 2)]
+            css = crossing.crossing_strands()
+            frontier = Frontier({0: css[3], 1: css[2], 2: css[1], 3: css[0]})
+            frontier_lengths = [4]
+            if len(link.crossings) == 1:
+                events += [('cap', 0, 1), ('cap', 0, 1)]
+        else: # Only unlinked unknotted components
+            crossings = []
+            frontier_lengths = []
+
         while len(crossings) < len(link.crossings):
             overlap, i, C = frontier.biggest_all_consecutive_overlap()
             cs = frontier[i]
             cs_opp = cs.opposite()
             assert C not in crossings
             crossings.append(C)
             if overlap == 1:
@@ -363,14 +373,18 @@
                 events += 2 * [('cap', i, i + 1)]
                 for a in range(4):
                     frontier.pop(i)
             assert frontier_lengths[-1] + 4 - 2 * overlap == len(frontier)
             assert frontier._check()
             frontier_lengths.append(len(frontier))
 
+        c = link.unlinked_unknot_components
+        events += c*[('cup', 0, 1), ('cap', 0, 1)]
+        frontier_lengths += c*[2, 0]
+
         self.link = link
         self.crossings = crossings
         self.frontier_lengths = frontier_lengths
         self.events = events
         self.width = max(frontier_lengths) // 2
 
     def __repr__(self):
```

### Comparing `spherogram-2.1/spherogram_src/links/extra_tests.py` & `spherogram-2.2/spherogram_src/links/extra_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,88 @@
+import sys
 from . import links, tangles
+
 Crossing, Link, RationalTangle, IdentityBraid = links.Crossing, links.Link, tangles.RationalTangle, tangles.IdentityBraid
-import os
-import sys
-import re
 
 # ----- Some basic tests, constructing links by hand -------
 
+
 def figure8():
     a, b, c, d = [Crossing(x) for x in 'abcd']
     a[0] = c[1]
     a[1] = d[0]
     a[2] = b[1]
     a[3] = b[0]
     b[2] = d[3]
     b[3] = c[2]
     c[3] = d[2]
     c[0] = d[1]
-    return Link([a,b,c,d])
+    return Link([a, b, c, d])
+
 
 def punct_torus():
     a = Crossing('a')
     a[0] = a[2]
     a[1] = a[3]
     return Link([a], check_planarity=False)
 
+
 def whitehead():
-    a, b, c, d, e =  crossings = [Crossing(x) for x in 'abcde']
+    a, b, c, d, e = crossings = [Crossing(x) for x in 'abcde']
     a[0] = b[3]
     a[1] = d[0]
     a[2] = d[3]
     a[3] = c[0]
     b[0] = c[3]
     b[1] = e[2]
     b[2] = e[1]
     c[1] = d[2]
     c[2] = e[3]
     d[1] = e[0]
     return Link(crossings)
- 
+
+
 def basic_test():
-    K, W, T = figure8(), whitehead(), punct_torus()
-    print( K.is_planar(), W.is_planar(), punct_torus().is_planar() )
-    print( K.PD_code(True) )
-    print( K.DT_code(True) , K.peer_code())
-    print( W.PD_code(True) )
-    print( W.DT_code(True) , K.peer_code())
+    K, W, _ = figure8(), whitehead(), punct_torus()
+    print(K.is_planar(), W.is_planar(), punct_torus().is_planar())
+    print(K.PD_code(True))
+    print(K.DT_code(True), K.peer_code())
+    print(W.PD_code(True))
+    print(W.DT_code(True), K.peer_code())
 
 
 # ----- checking the SnapPy link exterior code ------------
 
 def knot(fractions):
     if len(fractions) == 1:
         return RationalTangle(*fractions[0]).denominator_closure()
     else:
         A, B, C = [RationalTangle(*f) for f in fractions]
         T = A + B + C
         return T.numerator_closure()
 
+
 def some_knots():
-    from . import hyperbolic_montesinos 
-    return [ (K, knot(fractions)) for K, fractions in hyperbolic_montesinos.knots] 
+    from . import hyperbolic_montesinos
+    return [(K, knot(fractions))
+            for K, fractions in hyperbolic_montesinos.knots]
+
 
 def exterior_test():
     try:
         import snappy
     except ImportError:
         print("SnapPy not installed, skipping link exterior test.")
 
     print(figure8().exterior().volume(), whitehead().exterior().volume())
 
     C, Id = RationalTangle(1), IdentityBraid(1)
     x = C | Id
     y = Id | (-C)
-    print((x*y*x*y).denominator_closure().exterior().volume())
+    print((x * y * x * y).denominator_closure().exterior().volume())
 
     for name, K in some_knots():
         M0, M1 = K.exterior(), snappy.Manifold(K.DT_code(True))
         N0 = snappy.LinkExteriors.identify(M0)
         N1 = snappy.LinkExteriors.identify(M1)
         assert N0.name() == name and N1.name() == name
 
@@ -85,43 +91,43 @@
 
 def alexander_polynomial_test():
     """
     Export a bunch of Montesinos knots as PD diagrams and
     compute the Alexander polynomials via KnotTheory and
     also Sage.  Make sure they match.
     """
-    
     try:
         sys.path.append('/Users/dunfield/work/python')
         import nsagetools
     except ImportError:
         print("Skipping this test as you're not within Sage and/or are not Nathan.")
-        return 
+        return
 
     from sage.all import mathematica, PolynomialRing, ZZ
 
     mathematica.execute('AppendTo[$Path, "/pkgs"]')
     mathematica.execute('<<KnotTheory`')
     mathematica.execute('Off[KnotTheory::loading]')
     mathematica.execute('Off[KnotTheory::credits]')
     mathematica.execute('MyAlex[L_] := CoefficientList[t^100*Alexander[L][t], t]')
 
     def alex_by_KnotTheory(L):
         p = mathematica.MyAlex(L.PD_code(True)).sage()
-        i = min( [i for i,c in enumerate(p) if c != 0])
+        i = next(iter(i for i, c in enumerate(p) if c != 0))
         R = PolynomialRing(ZZ, 'a')
         return R(p[i:])
 
     def alex_match(L):
         p1 = alex_by_KnotTheory(L)
         p2 = nsagetools.alexander_polynomial(L.exterior())
         return 0 in [p1 - p2, p1 + p2]
 
     for name, K in some_knots():
         assert alex_match(K)
 
     print("Checked Alexander polynomials via KnotTheory for these 167 knots.")
 
+
 if __name__ == '__main__':
     basic_test()
     exterior_test()
     alexander_polynomial_test()
```

### Comparing `spherogram-2.1/spherogram_src/links/invariants.py` & `spherogram-2.2/spherogram_src/links/invariants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,140 +1,145 @@
 """
 When used within Sage, the Link class gains many methods to compute
 standard invariants.  Much of this code was contributed by Robert Lipshitz
 and Jennet Dickinson.
 """
 
 from . import links_base, alexander
-from .links_base import Crossing, Strand, CrossingStrand
-from ..sage_helper import _within_sage, sage_method
+from .links_base import CrossingStrand, Crossing
+from ..sage_helper import _within_sage, sage_method, sage_pd_clockwise
 
 deprecation_warnings_issued = set()
 
 if _within_sage:
-    import sage.all
-    import sage.graphs.graph
     from sage.matrix.constructor import matrix
-    from sage.symbolic.ring import SR
     from sage.groups.free_group import FreeGroup
     import sage.graphs.graph as graph
-    from sage.symbolic.ring import var
     from sage.groups.braid import Braid, BraidGroup
-    from sage.all import ZZ, QQ
+    from sage.rings.rational_field import QQ
     from sage.rings.polynomial.laurent_polynomial_ring import LaurentPolynomialRing
-    from sage.graphs.graph import Graph
     from sage.quadratic_forms.quadratic_form import QuadraticForm
     try:
         from sage.knots.knot import Knot as SageKnot
         from sage.knots.link import Link as SageLink
     except ImportError:  # Sage older than 7.2
         SageKnot, SageLink = type(None), type(None)
     import functools
 else:
     pass
 
-def normalize_alex_poly(p,t):
+
+def normalize_alex_poly(p, t):
     """
     Normalize the sign of the leading coefficient and make all
     exponents positive, then return as an ordinary rather than Laurent
     polynomial.
     """
-
     if len(t) == 1:
-        p = p*(t[0]**(-min(p.exponents())))
-        if p.coefficients()[-1]<0:
+        p = p * (t[0]**(-min(p.exponents())))
+        if p.coefficients()[-1] < 0:
             p = -p
         p, e = p.polynomial_construction()
         assert e == 0
         return p
 
-
-    max_degree = max([sum(x) for x in p.exponents()])
-    highest_monomial_exps = [x for x in p.exponents() if sum(x)==max_degree]
+    max_degree = max(sum(x) for x in p.exponents())
+    highest_monomial_exps = [x for x in p.exponents() if sum(x) == max_degree]
     leading_exponents = max(highest_monomial_exps)
-    leading_monomial = functools.reduce(lambda x,y: x*y,[t[i]**(leading_exponents[i]) for i in range(len(t))])
+    leading_monomial = functools.reduce(lambda x, y: x * y,
+                                        [t[i]**(leading_exponents[i])
+                                         for i in range(len(t))])
     l = p.monomial_coefficient(leading_monomial)
 
     if l < 0:
         p = -p
 
-    for i in range(len(t)):
-        exps = map(lambda x: x[i], p.exponents())
-        min_exp = min(exps)
-        p = p*(t[i]**(-min_exp))
+    for i, ti in enumerate(t):
+        min_exp = min(x[i] for x in p.exponents())
+        p = p * (ti**(-min_exp))
 
     R = p.parent()
     p = R.polynomial_ring()(p)
     return p
 
 
 def sage_braid_as_int_word(braid):
+    """
+    Convert a Sage Braid to a word.
+    """
+    # Could simplify using braid.Tietze().
+
     G = braid.parent()
-    gen_idx = dict([(g, i + 1) for i, g in enumerate(G.gens())])
+    gen_idx = {g: i + 1 for i, g in enumerate(G.gens())}
     ans = []
     for g, e in braid.syllables():
         if e > 0:
-            ans += e*[gen_idx[g]]
+            ans += e * [gen_idx[g]]
         else:
-            ans += abs(e)*[-gen_idx[g]]
+            ans += abs(e) * [-gen_idx[g]]
 
     n = G.ngens()
-    if max([abs(a) for a in ans]) < n:
+    if max(abs(a) for a in ans) < n:
         ans += [n, -n]
     return ans
 
 
 extra_docstring = """
     You can also convert to and from SageMath braid and link types,
     see the documentation for the "sage_link" method for details.
 """
 
+
 class Link(links_base.Link):
-    __doc__ = links_base.Link.__doc__  + extra_docstring
+    __doc__ = links_base.Link.__doc__ + extra_docstring
 
     def __init__(self, crossings=None, braid_closure=None, check_planarity=True, build=True):
         if _within_sage:
             if isinstance(crossings, Braid):
                 assert braid_closure is None
                 braid_closure = crossings
                 crossings = None
             if isinstance(braid_closure, Braid):
                 braid_closure = sage_braid_as_int_word(braid_closure)
             if crossings is not None and isinstance(crossings, (SageKnot, SageLink)):
+                # Sage's PD_code lists strands *clockwise* not our
+                # *anticlockwise* prior to Sage 10.1.
                 crossings = crossings.pd_code()
+                if sage_pd_clockwise:
+                    crossings = [[x[0], x[3], x[2], x[1]] for x in crossings]
 
         links_base.Link.__init__(self, crossings, braid_closure, check_planarity, build)
 
     @sage_method
     def linking_matrix(self):
         """
         Calculates the linking number for each pair of link components.
 
         Returns a linking matrix, in which the (i,j)th component is the
         linking number of the ith and jth link components.
         """
-        matrix = [ [0 for i in range(len(self.link_components)) ] for j in range(len(self.link_components)) ]
+        mat = [[0 for i in range(len(self.link_components))]
+               for j in range(len(self.link_components))]
         for n1, comp1 in enumerate(self.link_components):
             for n2, comp2 in enumerate(self.link_components):
-                tally = [ [0 for m in range(len(self.crossings)) ] for n in range(2) ]
-                if not (comp1 == comp2):
+                tally = [[0 for m in range(len(self.crossings))]
+                         for n in range(2)]
+                if comp1 != comp2:
                     for i, c in enumerate(self.crossings):
                         for x1 in comp1:
                             if x1[0] == c:
                                 tally[0][i] += 1
                         for x2 in comp2:
                             if x2[0] == c:
                                 tally[1][i] += 1
                 for k, c in enumerate(self.crossings):
                     if (tally[0][k] == 1 and tally[1][k] == 1):
-                        matrix[n1][n2] += 0.5 * (c.sign)
-        for i1, m1 in enumerate(matrix):
-            for i2, m2 in enumerate(m1):
-                matrix[i1][i2] = int(matrix[i1][i2])
-        return matrix
+                        mat[n1][n2] += 0.5 * (c.sign)
+                mat[n1][n2] = int(mat[n1][n2])
+        return mat
 
     @sage_method
     def knot_group(self):
         """
         Computes the knot group using the Wirtinger presentation.
 
         Returns a finitely presented group::
@@ -142,15 +147,14 @@
            sage: K = Link('3_1')
            sage: G = K.knot_group()
            sage: type(G)
            <class 'sage.groups.finitely_presented.FinitelyPresentedGroup_with_category'>
         """
         n = len(self.crossings)
         F = FreeGroup(n)
-        g = list(F.gens())
         rels = []
         pieces = self._pieces()
 
         for z in self.crossings:
             for m, p in enumerate(pieces):
                 for t, q in enumerate(p):
                     if q[0] == z:
@@ -160,17 +164,17 @@
                             i = m
                         else:
                             k = m
             i += 1
             j += 1
             k += 1
             if z.sign > 0:
-                r = F([-k,i,k,-j])
+                r = F([-k, i, k, -j])
             if z.sign < 0:
-                r = F([k,i,-k,-j])
+                r = F([k, i, -k, -j])
             rels.append(r)
 
         return F / rels
 
     @sage_method
     def alexander_matrix(self, mv=True):
         """
@@ -192,49 +196,52 @@
         comp = len(self.link_components)
         if comp < 2:
             mv = False
 
         G = self.knot_group()
         num_gens = len(G.gens())
 
-        L_g = LaurentPolynomialRing(QQ,['g%d' % (i+1) for i in range(num_gens)])
+        L_g = LaurentPolynomialRing(QQ, [f'g{i+1}' for i in range(num_gens)])
         g = list(L_g.gens())
 
-        if(mv):
-            L_t = LaurentPolynomialRing(QQ,['t%d' % (i+1) for i in range(comp)])
+        if mv:
+            L_t = LaurentPolynomialRing(QQ, [f't{i+1}' for i in range(comp)])
             t = list(L_t.gens())
 
-            #determine the component to which each variable corresponds
+            # determine the component to which each variable corresponds
             g_component = [c.strand_components[2] for c in self.crossings]
-            for i in range(len(g)):
-                g[i] = t[g_component[i]]
+            for i, gci in enumerate(g_component):
+                g[i] = t[gci]
 
         else:
-            L_t = LaurentPolynomialRing(QQ,'t')
+            L_t = LaurentPolynomialRing(QQ, 't')
             t = L_t.gen()
-            g = [t]*len(g)
+            g = [t] * len(g)
 
         B = G.alexander_matrix(g)
 
-        return (B,g)
+        return (B, g)
 
     @sage_method
     def alexander_poly(self, *args, **kwargs):
         """
         Please use the "alexander_polynomial" method instead.
         """
         if 'alexander_poly' not in deprecation_warnings_issued:
             deprecation_warnings_issued.add('alexander_poly')
             print('Deprecation Warning: use "alexander_polynomial" instead of "alexander_poly".')
         return self.alexander_polynomial(*args, **kwargs)
 
     @sage_method
-    def alexander_polynomial(self, multivar=True, v='no', method='default', norm = True, factored = False):
+    def alexander_polynomial(self, multivar=True, v='no', method='default',
+                             norm=True, factored=False):
         """
-        Calculates the Alexander polynomial of the link. For links with one component,
+        Calculates the Alexander polynomial of the link.
+
+        For links with one component,
         can evaluate the alexander polynomial at v::
 
             sage: K = Link('4_1')
             sage: K.alexander_polynomial()
             t^2 - 3*t + 1
             sage: K.alexander_polynomial(v=[4])
             5
@@ -247,70 +254,69 @@
         tangle-based algorithm.  For links, we apply Fox calculus to a
         Wirtinger presentation for the link::
 
             sage: L = Link('K13n123')
             sage: L.alexander_polynomial() == L.alexander_polynomial(method='wirtinger')
             True
         """
-
         # sign normalization still missing, but when "norm=True" the
         # leading coefficient with respect to the first variable is made
         # positive.
         if method == 'snappy':
             try:
                 return self.exterior().alexander_polynomial()
             except ImportError:
-                raise RuntimeError('this method for alexander_polynomial '+no_snappy_msg)
-        else:
-            comp = len(self.link_components)
-            if comp < 2:
-                multivar = False
-
-            # If single variable, use the super-fast method of Bar-Natan.
-            if comp == 1 and method == 'default' and norm:
-                p = alexander.alexander(self)
-            else: # Use a simple method based on the Wirtinger presentation.
-                if method not in ['default', 'wirtinger']:
-                    raise ValueError("Available methods are 'default' and 'wirtinger'")
-
-                if(multivar):
-                    L = LaurentPolynomialRing(QQ,['t%d' % (i+1) for i in range(comp)])
-                    t = list(L.gens())
-                else:
-                    L = LaurentPolynomialRing(QQ,'t')
-                    t = [L.gen()]
-
-                M = self.alexander_matrix(mv=multivar)
-                C = M[0]
-                m = C.nrows()
-                n = C.ncols()
-                if n>m:
-                    k = m-1
-                else:
-                    k = n-1
-
-                subMatrix = C[0:k,0:k]
-                p = subMatrix.determinant()
-                if p == 0:
-                    return 0
-                if multivar:
-                    t_i = M[1][-1]
-                    p = (p.factor())/(t_i-1)
-                    p = p.expand()
+                raise RuntimeError('the method "snappy" for '
+                                   'alexander_polynomial requires SnapPy')
 
-                if(norm):
-                    p = normalize_alex_poly(p,t)
+        comp = len(self.link_components)
+        if comp < 2:
+            multivar = False
 
-            if v != 'no':
-                return p(*v)
+        # If single variable, use the super-fast method of Bar-Natan.
+        if comp == 1 and method == 'default' and norm:
+            p = alexander.alexander(self)
+        else:  # Use a simple method based on the Wirtinger presentation.
+            if method not in ['default', 'wirtinger']:
+                raise ValueError("Available methods are 'default' and 'wirtinger'")
+
+            if multivar:
+                L = LaurentPolynomialRing(QQ, [f't{i+1}' for i in range(comp)])
+                t = list(L.gens())
+            else:
+                L = LaurentPolynomialRing(QQ, 't')
+                t = [L.gen()]
 
-            if multivar and factored: # it's easier to view this way
-                return p.factor()
+            M = self.alexander_matrix(mv=multivar)
+            C = M[0]
+            m = C.nrows()
+            n = C.ncols()
+            if n > m:
+                k = m - 1
             else:
-                return p
+                k = n - 1
+
+            subMatrix = C[0: k, 0: k]
+            p = subMatrix.determinant()
+            if p == 0:
+                return 0
+            if multivar:
+                t_i = M[1][-1]
+                p = (p.factor()) / (t_i - 1)
+                p = p.expand()
+
+            if norm:
+                p = normalize_alex_poly(p, t)
+
+        if v != 'no':
+            return p(*v)
+
+        if multivar and factored:  # it's easier to view this way
+            return p.factor()
+        return p
 
     def knot_floer_homology(self, prime=2, complex=False):
         """
         Uses Zoltán Szabó's HFK Calculator to compute the knot Floer
         homology.  This also gives the Seifert genus, whether the knot
         fibers, etc:
 
@@ -373,71 +379,64 @@
 
         sage: from sage.all import matrix, GF
         sage: M = matrix(GF(31991), len(gens), len(gens), vert, sparse=True)
         sage: M*M == 0
         True
         sage: M.right_kernel().rank() - M.rank()
         1
-
         """
         import knot_floer_homology
         if len(self.link_components) + self.unlinked_unknot_components > 1:
             raise ValueError('Only works for knots, this has more components')
         if len(self.link_components) == 0 and self.unlinked_unknot_components == 1:
             return Link(braid_closure=[1, 1, -1]).knot_floer_homology()
         return knot_floer_homology.pd_to_hfk(self, prime=prime, complex=complex)
 
-    def _edge_sign(K, edge):
-        "Returns the sign (+/- 1) associated to given edge in the black graph."
-        crossing = edge[2]
-        if set(((crossing,0),(crossing,1))).issubset(set(edge[0])) or set(((crossing,0),(crossing,1))).issubset(set(edge[1])):
-            return +1
-        return -1
-
     @sage_method
     def black_graph(self):
         """
-        Returns the black graph of K. If the black graph is disconnected
-        (which can only happen for a split link diagram), returns one
-        connected component. The edges are labeled by the crossings
-        they correspond to.  Example::
+        Returns the black graph of K.
+
+        If the black graph is disconnected (which can only happen for
+        a split link diagram), returns one connected component. The
+        edges are labeled by the crossings they correspond to.
+
+        Example::
 
             sage: K=Link('5_1')
             sage: K.black_graph()
             Subgraph of (): Multi-graph on 2 vertices
 
         WARNING: While there is also a "white_graph" method, it need
         not be the case that these two graphs are complementary in the
         expected way.
         """
-
         faces = []
         for x in self.faces():
             l = []
             for y in x:
-                l.append((y[0],y[1]))
-                l.append((y[0],(y[1]+1)%4))
+                l.append((y[0], y[1]))
+                l.append((y[0], (y[1] + 1) % 4))
             faces.append(l)
 
-        coords=list()
-        for i in range(len(faces)-1):
-            for j in range (i+1, len(faces)):
-                a=set(faces[i])
-                b=set(faces[j])
-                s=a.union(b)
+        coords = list()
+        for i in range(len(faces) - 1):
+            for j in range(i + 1, len(faces)):
+                a = set(faces[i])
+                b = set(faces[j])
+                s = a.union(b)
                 for x in range(len(self.crossings)):
-                    crossings=[self.crossings[x][0],self.crossings[x][1],self.crossings[x][2],self.crossings[x][3]]
-                    total=set(crossings)
+                    total = set(self.crossings[x][i] for i in range(4))
                     if total.issubset(s):
-                        coords.append((tuple(faces[i]),tuple(faces[j]),self.crossings[x])) #label by the crossing.
+                        coords.append((tuple(faces[i]), tuple(faces[j]),
+                                       self.crossings[x]))  # label by the crossing.
 
-        G=graph.Graph(coords, multiedges=True)
-        component=G.connected_components(sort=False)[1]
-        G=G.subgraph(component)
-        return G
+        G = graph.Graph(coords, multiedges=True)
+        component = G.connected_components(sort=False)[1]
+        return G.subgraph(component)
 
     @sage_method
     def white_graph(self):
         """
         Return the white graph of a non-split link projection.
 
         This method generates a multigraph whose vertices correspond
@@ -469,23 +468,26 @@
             Subgraph of (): Multi-graph on 2 vertices
 
         WARNING: While there is also a "black_graph" method, it need
         not be the case that these two graphs are complementary in the
         expected way.
         """
         # Map corners (i.e. CrossingStrands) to faces.
-        face_of = dict((corner, n) for n, face in enumerate(self.faces()) for corner in face)
+        face_of = {corner: n for n, face in enumerate(self.faces())
+                   for corner in face}
 
         # Create the edges, labeled with crossing and sign.
         edges = []
         for c in self.crossings:
-            edges.append((face_of[CrossingStrand(c, 0)], face_of[CrossingStrand(c, 2)],
-                          {'crossing':c, 'sign':1}))
-            edges.append((face_of[CrossingStrand(c, 1)], face_of[CrossingStrand(c, 3)],
-                          {'crossing':c, 'sign':-1}))
+            edges.append((face_of[CrossingStrand(c, 0)],
+                          face_of[CrossingStrand(c, 2)],
+                          {'crossing': c, 'sign': 1}))
+            edges.append((face_of[CrossingStrand(c, 1)],
+                          face_of[CrossingStrand(c, 3)],
+                          {'crossing': c, 'sign': -1}))
 
         # Build the graph.
         G = graph.Graph(edges, multiedges=True)
         components = G.connected_components()
         if len(components) > 2:
             raise ValueError('The link diagram is split.')
         return G.subgraph(components[1])
@@ -497,28 +499,25 @@
         If the return_graph flag is set, also return the graph::
 
             sage: K=Link('4_1')
             sage: abs(K.goeritz_matrix().det())
             5
         """
         G = self.white_graph()
-        V = G.vertices()
+        V = G.vertices(sort=True)
         N = len(V)
-        m = matrix(N,N)
-        vertex = dict((v, n) for n, v in enumerate(V))
+        m = matrix(N, N)
+        vertex = {v: n for n, v in enumerate(V)}
         for e in G.edges(sort=False):
             i, j = vertex[e[0]], vertex[e[1]]
-            m[(i,j)] = m[(j,i)] = m[(i,j)] + e[2]['sign']
+            m[(i, j)] = m[(j, i)] = m[(i, j)] + e[2]['sign']
         for i in range(N):
-            m[(i,i)] = -sum(m.column(i))
+            m[(i, i)] = -sum(m.column(i))
         m = m.delete_rows([0]).delete_columns([0])
-        if return_graph:
-            return m, G
-        else:
-            return m
+        return (m, G) if return_graph else m
 
     @sage_method
     def signature(self, new_convention=True):
         """
         Returns the signature of the link, computed from the Goeritz matrix using
         the algorithm of Gordon and Litherland::
 
@@ -538,39 +537,37 @@
         recover the previous default by::
 
           sage: L = Link('3a1')
           sage: L.signature()
           -2
           sage: L.signature(new_convention=False)
           2
-
-
         """
         m, G = self.goeritz_matrix(return_graph=True)
-        correction = sum([e[2]['sign'] for e in G.edges(sort=False)
-                          if e[2]['sign'] == e[2]['crossing'].sign])
+        correction = sum(e['sign'] for _, _, e in G.edges(sort=False)
+                         if e['sign'] == e['crossing'].sign)
         ans = QuadraticForm(QQ, m).signature() + correction
         if new_convention:
             ans = -ans
         return ans
 
     @sage_method
     def _colorability_matrix(self):
         """Auxiliary function used by determinant."""
         edges = self._pieces()
-        m=matrix(len(self.crossings), len(edges))
+        m = matrix(len(self.crossings), len(edges))
         for c in self.crossings:
             for i in range(4):
                 for s in edges:
-                    if (c,i) in s:
-                        ind=edges.index(s)
-                        if i==1 or i==3:
-                            m[(self.crossings.index(c),ind)]+=1
-                        if i==2 or i==0:
-                            m[(self.crossings.index(c),ind)]-=1
+                    if (c, i) in s:
+                        ind = edges.index(s)
+                        if i % 2:
+                            m[(self.crossings.index(c), ind)] += 1
+                        else:
+                            m[(self.crossings.index(c), ind)] -= 1
                         break
         return m
 
     @sage_method
     def determinant(self, method='goeritz'):
         """
         Returns the determinant of the link, a non-negative integer.
@@ -579,26 +576,25 @@
         using the Goeritz matrix, and 'color', using the 'colorability matrix', or
         anything else, to compute the Alexander polynomial at -1.  Example::
 
             sage: K = Link( [(4,1,5,2),(6,4,7,3),(8,5,1,6),(2,8,3,7)] )  # Figure 8 knot
             sage: K.determinant()
             5
         """
-        if method=='color':
+        if method == 'color':
             M = self._colorability_matrix()
-            size = len(self.crossings)-1
+            size = len(self.crossings) - 1
             N = matrix(size, size)
             for i in range(size):
                 for j in range(size):
-                    N[(i,j)]=M[(i+1,j+1)]
+                    N[(i, j)] = M[(i + 1, j + 1)]
             return abs(N.determinant())
-        elif method=='goeritz':
+        if method == 'goeritz':
             return abs(self.goeritz_matrix().determinant())
-        else:
-            return abs(self.alexander_polynomial(multivar=False, v=[-1], norm = False))
+        return abs(self.alexander_polynomial(multivar=False, v=[-1], norm=False))
 
     @sage_method
     def morse_number(self, solver='GLPK'):
         """
         The *Morse number* of a planar link diagram D is
 
             m(D) = min { # of maxima of h on D }
@@ -644,15 +640,15 @@
         conventions of https://arxiv.org/abs/math/0201043
 
         In particular, it obeys the oriented skein relation::
 
           q^2 V(L-) - q^-2 V(L+) = (q - q^-1) V(L0)
 
         and V(n-component unlink) = (q + q^-1)^(n-1).
-        
+
         WARNING: The default conventions changed in SnapPy 3.0.  You
         can recover the old conventions as illustrated below::
 
           sage: L = Link('8_5')
           sage: J = L.jones_polynomial(); J
           1 - q^2 + 3*q^4 - 3*q^6 + 3*q^8 - 4*q^10 + 3*q^12 - 2*q^14 + q^16
           sage: Jold = L.jones_polynomial(new_convention=False); Jold
@@ -679,16 +675,16 @@
         else:
             if len(self.link_components) != 1:
                 J = jones_old.Jones_poly(self, new_convention=False)
             else:
                 J = jones.jones_polynomial(self, normalized=True)
                 R = J.parent()
                 q = R.gen()
-                terms = [J[e]*q**(e//2) for e in J.exponents()]
-                J = sum(terms , R(0))
+                terms = [J[e] * q**(e // 2) for e in J.exponents()]
+                J = sum(terms, R(0))
 
         if variable is not None:
             J = J(variable)
         return J
 
     def seifert_matrix(self):
         """
@@ -739,15 +735,15 @@
         braids, a new algorithm".
         """
         from . import seifert
         word = seifert.braid_word(self)
         if as_sage_braid:
             if not _within_sage:
                 raise ValueError('Requested Sage braid outside of Sage.')
-            n = max([abs(a) for a in word]) + 1
+            n = max(abs(a) for a in word) + 1
             word = BraidGroup(n)(word)
         return word
 
     @sage_method
     def sage_link(self):
         """
         Convert to a SageMath Knot or Link::
@@ -758,14 +754,21 @@
            sage: L.alexander_polynomial()/K.alexander_polynomial()  # Agree up to units
            -t^3
            sage: L.signature(), K.signature()
            (-4, -4)
 
         Can also go the other way::
 
+           sage: L = Link('K11n11')
+           sage: M = Link(L.sage_link())
+           sage: L.signature(), M.signature()
+           (-2, -2)
+
+        Can also take a braid group perspective.
+
             sage: B = BraidGroup(4)
             sage: a, b, c = B.gens()
             sage: Link(braid_closure=(a**-3) * (b**4) * (c**2) * a * b * c )
             <Link: 2 comp; 12 cross>
             sage: L = Link(a * b * c); L
             <Link: 1 comp; 3 cross>
             sage: S = L.sage_link(); S
@@ -787,14 +790,15 @@
 
             sage: L = Link('K13n100')
             sage: L._sage_()
             Knot represented by 13 crossings
         """
         return self.sage_link()
 
+
 class ClosedBraid(Link):
     """
     This is a convenience class for constructing closed braids.
 
     The constructor accepts either a single argument, which should be a list of
     integers to be passed to the Link constructor as the braid_closure
     parameter, or one or more integer arguments which will be packaged as a list
@@ -814,8 +818,8 @@
                 args = ()
             elif isinstance(args[0], int):
                 self.braid_word = kwargs['braid_closure'] = args
                 args = ()
         Link.__init__(self, *args, **kwargs)
 
     def __repr__(self):
-        return 'ClosedBraid%s'%str(self.braid_word)
+        return 'ClosedBraid%s' % str(self.braid_word)
```

### Comparing `spherogram-2.1/spherogram_src/links/jones.py` & `spherogram-2.2/spherogram_src/links/jones.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,112 @@
 """
 
 Computing the Jones polynomial following the conventions of Jake
-Rasmussen's lectures at PCMI, Summer 2019.
+Rasmussen's lectures at PCMI, Summer 2019:
 
+https://www.dpmms.cam.ac.uk/~jar60/PCMINotes.pdf
 https://www.youtube.com/watch?v=--l-XOhDXOU
 https://www.youtube.com/watch?v=3VwcGHycyAE
 
 
+
+
 """
 
-from sage.all import ZZ, LaurentPolynomialRing, PerfectMatchings, PerfectMatching
+from ..sage_helper import _within_sage
 from . import exhaust
+from .links_base import Link
+
+if _within_sage:
+    from sage.all import ZZ, LaurentPolynomialRing, PerfectMatchings, PerfectMatching
+    R = LaurentPolynomialRing(ZZ, 'q')
+    q = R.gen()
+else:
+    pass
 
-R = LaurentPolynomialRing(ZZ, 'q')
-q = R.gen()
 
 def num_Pn(n):
     """
     An element of Jake's P_{0, n} of planar tangles from 0 points to n
     points will be a PerfectMatching of [0,..,n-1] where
     is_noncrossing is True.
     """
     return len([m for m in PerfectMatchings(n) if m.is_noncrossing()])
 
+
 def insert_cup(matching, i):
     """
     Insert a new adjacent matching which joins i and i + 1.
 
-    >>> m = PerfectMatching([(0, 1), (2, 5), (3, 4)])
-    >>> insert_cup(m, 0)
+    sage: m = PerfectMatching([(0, 1), (2, 5), (3, 4)])
+    sage: insert_cup(m, 0)
     [(0, 1), (2, 3), (4, 7), (5, 6)]
-    >>> insert_cup(m, 1)
+    sage: insert_cup(m, 1)
     [(0, 3), (1, 2), (4, 7), (5, 6)]
-    >>> insert_cup(m, 6)
+    sage: insert_cup(m, 6)
     [(0, 1), (2, 5), (3, 4), (6, 7)]
     """
     assert len(matching.base_set()) >= i
+
     def shift(pair):
         return [a if a < i else a + 2 for a in pair]
     return PerfectMatching([shift(pair) for pair in matching] + [(i, i + 1)])
 
+
 def cap_off(matching, i):
     """
     Merge i and i + 1 with a cap.  Returns a new matching and whether
     or not a circle was created.
 
-    >>> m = PerfectMatching([(0, 5), (1, 4), (2, 3)])
-    >>> cap_off(m, 2)
+    sage: m = PerfectMatching([(0, 5), (1, 4), (2, 3)])
+    sage: cap_off(m, 2)
     ([(0, 3), (1, 2)], True)
-    >>> cap_off(m, 3)
+    sage: cap_off(m, 3)
     ([(0, 3), (1, 2)], False)
     """
     def shift(a):
         return a if a < i else a - 2
+
     def follow(a):
         b = matching.partner(a)
         if b == i:
             b = matching.partner(i + 1)
         elif b == i + 1:
             b = matching.partner(i)
         return b
 
     n = len(matching.base_set())
     circle = matching.partner(i) == i + 1
     new_match = set()
     for a in range(n):
-        if not a in {i, i + 1}:
+        if a not in {i, i + 1}:
             u, v = shift(a), shift(follow(a))
             if u > v:
                 u, v = v, u
             new_match.add((u, v))
     return PerfectMatching(new_match), circle
 
-class VElement(object):
+
+class VElement():
     """
     An element of some V_{0, n} which is the free R-module on P_{0, n}
 
-    >>> m = PerfectMatching([(0, 1), (3, 4), (2, 5)])
-    >>> v1 = VElement(m)
-    >>> v1
+    sage: m = PerfectMatching([(0, 1), (3, 4), (2, 5)])
+    sage: v1 = VElement(m)
+    sage: v1
     (1)*[(0, 1), (2, 5), (3, 4)]
-    >>> v2 = (q + q**-1)*v1
-    >>> v2
+    sage: v2 = (q + q**-1)*v1
+    sage: v2
     (q^-1 + q)*[(0, 1), (2, 5), (3, 4)]
-    >>> v3 = q* VElement(PerfectMatching([(5, 0), (4, 3), (1, 2)]))
-    >>> v1 + v2 + v3
+    sage: v3 = q* VElement(PerfectMatching([(5, 0), (4, 3), (1, 2)]))
+    sage: v1 + v2 + v3
     (q^-1 + 1 + q)*[(0, 1), (2, 5), (3, 4)] + (q)*[(0, 5), (1, 2), (3, 4)]
-    >>> v2.insert_cup(6)
+    sage: v2.insert_cup(6)
     (q^-1 + q)*[(0, 1), (2, 5), (3, 4), (6, 7)]
-    >>> (v1 + v2 + v3).cap_off(1)
+    sage: (v1 + v2 + v3).cap_off(1)
     (q^-1 + 2 + q + q^2)*[(0, 3), (1, 2)]
     """
     def __init__(self, spec=None):
         self.dict = dict()
         if spec is None:
             spec = PerfectMatching([])
         if isinstance(spec, dict):
@@ -100,65 +114,74 @@
         if isinstance(spec, PerfectMatching):
             assert spec.is_noncrossing()
             self.dict[spec] = R.one()
 
     def __rmul__(self, other):
         if other in R:
             other = R(other)
-            return VElement({m:other*c for m, c in self.dict.items()})
+            return VElement({m: other * c for m, c in self.dict.items()})
 
     def __add__(self, other):
         if isinstance(other, VElement):
             ans_dict = self.dict.copy()
             for matching, coeff in other.dict.items():
                 cur_coeff = self.dict.get(matching, R.zero())
                 ans_dict[matching] = cur_coeff + coeff
         return VElement(ans_dict)
 
     def __repr__(self):
-        matchings = sorted(self.dict.keys())
+        matchings = sorted(self.dict)
         terms = ['(%s)*%s' % (self.dict[m], m) for m in matchings]
         if len(terms) == 0:
             return '0'
         return ' + '.join(terms)
 
     def insert_cup(self, i):
         """
         Insert an new matching at (i, i + 1)
         """
-        return VElement({insert_cup(m, i):c for m, c in self.dict.items()})
+        return VElement({insert_cup(m, i): c for m, c in self.dict.items()})
 
     def cap_off(self, i):
         ans_dict = dict()
         for matching, coeff in self.dict.items():
             new_matching, has_circle = cap_off(matching, i)
             cur_coeff = ans_dict.get(new_matching, R.zero())
             if has_circle:
-                coeff = (q + q**-1)*coeff
+                coeff = (q + q**-1) * coeff
             ans_dict[new_matching] = cur_coeff + coeff
         return VElement(ans_dict)
 
     def cap_then_cup(self, i):
         return self.cap_off(i).insert_cup(i)
 
     def add_positive_crossing(self, i):
-        return self + (-q)*self.cap_then_cup(i)
+        return self + (-q) * self.cap_then_cup(i)
 
     def add_negative_crossing(self, i):
-        return self.cap_then_cup(i) + (-q)*self
+        return self.cap_then_cup(i) + (-q) * self
 
     def is_multiple_of_empty_pairing(self):
         return len(self.dict) == 1 and (PerfectMatching([]) in self.dict)
 
 
 def kauffman_bracket(link):
     """
-    >>> L = Link('T(2, 3)')
-    >>> kauffman_bracket(L)
+    sage: L = Link('T(2, 3)')
+    sage: kauffman_bracket(L)
     q^-2 + 1 + q^2 - q^6
+
+    sage: U4 = Link(braid_closure=[1, -1, 2, -2, 3, -3])
+    sage: kauffman_bracket(U4)
+    -q^-1 - 4*q - 6*q^3 - 4*q^5 - q^7
+
+    sage: U3 = Link([])
+    sage: U3.unlinked_unknot_components = 3
+    sage: kauffman_bracket(U3) == (q + q**-1)**3
+    True
     """
     ans = VElement()
     if isinstance(link, exhaust.MorseEncoding):
         encoded = link
     else:
         exhaustion = exhaust.MorseExhaustion(link)
         encoded = exhaust.MorseEncoding(exhaustion)
@@ -172,35 +195,33 @@
             if event.a < event.b:
                 ans = ans.add_positive_crossing(event.min)
             else:
                 ans = ans.add_negative_crossing(event.min)
     assert ans.is_multiple_of_empty_pairing()
     return ans.dict[PerfectMatching([])]
 
+
 def jones_polynomial(link, normalized=True):
     bracket = kauffman_bracket(link)
     if normalized:
         factor = q + q**-1
         norm_bracket = bracket // factor
-        assert norm_bracket*factor == bracket
+        assert norm_bracket * factor == bracket
     else:
         norm_bracket = bracket
 
     signs = [c.sign for c in link.crossings]
     n_minus, n_plus = signs.count(-1), signs.count(1)
-    return (-1)**n_minus * q**(n_plus - 2*n_minus) * norm_bracket
+    return (-1)**n_minus * q**(n_plus - 2 * n_minus) * norm_bracket
 
-def test_one_link(link):
-    new_poly = jones_polynomial(link)
-    old_poly = link.jones_polynomial(new_convention=True)
-    return new_poly - old_poly == 0
 
 def test_links(N):
     import snappy
     for i in range(N):
         M = snappy.HTLinkExteriors.random()
         L = M.link()
         print(M.name(), test_one_link(L))
 
+
 if __name__ == '__main__':
     import doctest
     print(doctest.testmod())
```

### Comparing `spherogram-2.1/spherogram_src/links/jones_old.py` & `spherogram-2.2/spherogram_src/links/jones_old.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,123 +16,129 @@
     --A graph G.
     --A spanning tree T for G
     --And edge e of T
 
     Cutting T along e separates T into two components.
     Returns: The list of edges in G - e connecting the two different components of T-e."""
     if not T.has_edge(*e):
-        raise Exception("e must be an edge of T.")
-    H = G.copy()
+        raise ValueError("e must be an edge of T.")
     S = T.copy()
     S.delete_edge(e)
     (C1, C2) = S.connected_components()
     answer = list()
     for f in G.edges(sort=True, key=edge_index):
         if (f[0] in C1 and f[1] in C2) or (f[0] in C2 and f[1] in C1):
             if f != e:
                 answer.append(f)
     return answer
 
+
 def is_internally_active(G, T, e):
     """
     Input:
     --A graph G.
     --A spanning tree T for G
     --And edge e of G
 
     Returns: True if e is in T and e is internally active for T, False otherwise. Uses the ordering on G.edges()."""
     if not T.has_edge(*e):
         return False
-    for f in cut(G,T,e):
+    for f in cut(G, T, e):
         if edge_index(f) < edge_index(e):
             return False
     return True
 
-def cyc(G,T,e):
+
+def cyc(G, T, e):
     """
     Input:
     --A graph G.
     --A spanning tree T for G
     --And edge e of G not in T
 
     Adjoining e to T creates a cycle.
     Returns: this cycle."""
     if not G.has_edge(*e):
-        raise Exception("e must be an edge of G.")
+        raise ValueError("e must be an edge of G.")
     if T.has_edge(*e):
-        raise Exception("e must not be an edge of T.")
-    #First thing: catch exceptional case that e is a multiple for an edge in T (giving a 2-cycle).
+        raise ValueError("e must not be an edge of T.")
+    # First thing: catch exceptional case that e is a multiple for an edge in T (giving a 2-cycle).
     try:
-        l = T.edge_label(e[0],e[1])
-        if isinstance(l,list):
-            l = l[0] #For multigraphs, edge_label returns a list. In this case, it's a list with one element...
-        if (e[0],e[1], l) in T.edges(sort=True, key=edge_index):
-            return [(e[0],e[1],l),e]
-        return [(e[1],e[0],l),e]
+        l = T.edge_label(e[0], e[1])
+        if isinstance(l, list):
+            l = l[0]  # For multigraphs, edge_label returns a list. In this case, it's a list with one element...
+        if (e[0], e[1], l) in T.edges(sort=True, key=edge_index):
+            return [(e[0], e[1], l), e]
+        return [(e[1], e[0], l), e]
     except Exception:
         pass
 
-    #Now the typical case.  First, need to turn T into a Graph which
-    #doesn't allow multiedges and also make a copy since we will
-    #modify it.
+    # Now the typical case.  First, need to turn T into a Graph which
+    # doesn't allow multiedges and also make a copy since we will
+    # modify it.
     S = graph.Graph(T.edges(sort=True, key=edge_index))
     S.add_edge(e)
     cb = S.cycle_basis()[0]
     answer = list()
     for i in range(len(cb)):
-        l = S.edge_label(cb[i],cb[(i+1)%len(cb)])
-        if S.has_edge(cb[i],cb[(i+1)%len(cb)],l):
-            answer.append((cb[i],cb[(i+1)%len(cb)],l))
+        l = S.edge_label(cb[i], cb[(i + 1) % len(cb)])
+        if S.has_edge(cb[i], cb[(i + 1) % len(cb)], l):
+            answer.append((cb[i], cb[(i + 1) % len(cb)], l))
         else:
-            answer.append((cb[(i+1)%len(cb)],cb[i],l))
+            answer.append((cb[(i + 1) % len(cb)], cb[i], l))
     return answer
 
-def is_externally_active(G,T,e):
+
+def is_externally_active(G, T, e):
     """
     Input:
     --A graph G.
     --A spanning tree T for G
     --And edge e of G
 
     Returns: True is e is not in T and e is externally active for T, False otherwise. Uses the ordering on G.edges()."""
     if T.has_edge(*e):
         return False
-    for f in cyc(G,T,e):
+    for f in cyc(G, T, e):
         if edge_index(f) < edge_index(e):
             return False
     return True
 
+
 def _edge_sign(K, edge):
     "Returns the sign (+/- 1) associated to given edge in the black graph."
     crossing = edge[2]
-    if set(((crossing,0),(crossing,1))).issubset(set(edge[0])) or set(((crossing,0),(crossing,1))).issubset(set(edge[1])):
+    if set(((crossing, 0), (crossing, 1))).issubset(set(edge[0])) or set(((crossing, 0), (crossing, 1))).issubset(set(edge[1])):
         return +1
     return -1
 
+
 def _Jones_contrib_edge(K, G, T, e, A):
     "Returns the contribution to the Jones polynomial of the specified tree T and edge e."
-    #Need to also take crossing sign into account -- A -> 1/A in negative case.
+    # Need to also take crossing sign into account -- A -> 1/A in negative case.
     s = e[2]['sign']
-    if is_internally_active(G,T,e):
-        return -A**(-3*s)
-    if T.has_edge(*e) and (not is_internally_active(G,T,e)):
+    if is_internally_active(G, T, e):
+        return -A**(-3 * s)
+    if T.has_edge(*e) and (not is_internally_active(G, T, e)):
         return A**s
-    if is_externally_active(G,T,e):
-        return -A**(3*s)
-    if (not T.has_edge(*e)) and (not is_externally_active(G,T,e)):
-        return A**(-1*s)
+    if is_externally_active(G, T, e):
+        return -A**(3 * s)
+    if (not T.has_edge(*e)) and (not is_externally_active(G, T, e)):
+        return A**(-1 * s)
+
 
 def _Jones_contrib(K, G, T, A):
     "Returns the contribution to the Jones polynomial of the tree T. G should be self.black_graph()."
     answer = 1
     # 2 loops, edges in T and edges not in T
     for e in G.edges(sort=True, key=edge_index):
-        answer = answer*_Jones_contrib_edge(K,G,T,e,A)
+        answer = answer * _Jones_contrib_edge(K, G, T, e, A)
     return answer
 
+
 def Jones_poly(K, variable=None, new_convention=False):
     """
     The old convention should really have powers of q^(1/2) for links
     with an odd number of components, but it just multiplies the
     answer by q^(1/2) to get rid of them.  Moroever, the choice of
     value for the unlink is a little screwy, essentially::
 
@@ -140,38 +146,39 @@
 
     In the new convention, powers of q^(1/2) never appear, i.e. the
     new q is the old q^(1/2) and moreover the value for an n-component
     unlink is (q + 1/q)^(n - 1).  This should match Bar-Natan's paper
     on Khovanov homology.
     """
     if not variable:
-        L = LaurentPolynomialRing(QQ,'q')
+        L = LaurentPolynomialRing(QQ, 'q')
         variable = L.gen()
     answer = 0
-    L_A = LaurentPolynomialRing(QQ,'A')
+    L_A = LaurentPolynomialRing(QQ, 'A')
     A = L_A.gen()
     G = K.white_graph()
     for i, labels in enumerate(G.edge_labels()):
         labels['edge_index'] = i
     writhe = K.writhe()
     for T in spanning_trees(G):
-        answer = answer + _Jones_contrib(K,G,T,A)
-    answer = answer * (-A)**(3*writhe)
+        answer = answer + _Jones_contrib(K, G, T, A)
+    answer = answer * (-A)**(3 * writhe)
     ans = 0
     for i in range(len(answer.coefficients())):
         coeff = answer.coefficients()[i]
         exp = answer.exponents()[i]
         if new_convention:
             # Now do the substitution A = i q^(1/2) so A^2 = -q
             assert exp % 2 == 0
-            ans = ans + coeff*((-variable)**(exp//2))
+            ans = ans + coeff * ((-variable)**(exp // 2))
         else:
-            ans = ans + coeff*(variable**(exp//4))
+            ans = ans + coeff * (variable**(exp // 4))
     return ans
 
+
 def spanning_trees(G):
     """
     NOTE: This code was essentially merged into SageMath proper
     in 2014.  However, because of sorting-related changes needed to
     support Python 3, the *other* code in this file will not work with
     SageMath's version of Graph.spanning_trees.  Hence we retain our
     original version, somewhat modified to work around the Python 3
@@ -218,18 +225,18 @@
          Graph on 6 vertices,
          Graph on 6 vertices]
 
     REFERENCES:
 
     .. [RT75] Read, R. C. and Tarjan, R. E.
       Bounds on Backtrack Algorithms for Listing Cycles, Paths, and Spanning Trees
-      Networks, Volume 5 (1975), numer 3, pages 237-252.
+      Networks, Volume 5 (1975), number 3, pages 237-252.
     """
 
-    def _recursive_spanning_trees(G,forest):
+    def _recursive_spanning_trees(G, forest):
         """
         Returns all the spanning trees of G containing forest
         """
         if not G.is_connected():
             return []
 
         if G.size() == forest.size():
@@ -238,37 +245,38 @@
             # Pick an edge e from G-forest
             for e in G.edges(sort=True, key=edge_index):
                 if not forest.has_edge(e):
                     break
 
             # 1) Recursive call with e removed from G
             G.delete_edge(e)
-            trees = _recursive_spanning_trees(G,forest)
+            trees = _recursive_spanning_trees(G, forest)
             G.add_edge(e)
 
             # 2) Recursive call with e include in forest
             #
             # e=xy links the CC (connected component) of forest containing x
             # with the CC containing y. Any other edge which does that
             # cannot be added to forest anymore, and B is the list of them
             c1 = forest.connected_component_containing_vertex(e[0])
             c2 = forest.connected_component_containing_vertex(e[1])
             G.delete_edge(e)
-            B = G.edge_boundary(c1,c2,sort=False)
+            B = G.edge_boundary(c1, c2, sort=False)
             G.add_edge(e)
 
             # Actual call
             forest.add_edge(e)
             G.delete_edges(B)
-            trees.extend(_recursive_spanning_trees(G,forest))
+            trees.extend(_recursive_spanning_trees(G, forest))
             G.add_edges(B)
             forest.delete_edge(e)
 
             return trees
 
     if G.is_connected() and len(G):
         forest = graph.Graph()
-        forest.add_vertices(G.vertices())
+        forest.add_vertices(G.vertices(sort=True))
         forest.add_edges(G.bridges())
-        return _recursive_spanning_trees(graph.Graph(G,immutable=False,loops=False), forest)
+        return _recursive_spanning_trees(graph.Graph(G, immutable=False, loops=False),
+                                         forest)
     else:
         return []
```

### Comparing `spherogram-2.1/spherogram_src/links/links_base.py` & `spherogram-2.2/spherogram_src/links/links_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,23 @@
   http://katlas.org/wiki/Planar_Diagrams
 
 See the file "doc.pdf" for the conventions, and the file
 "test.py" for some examples of creating links.
 """
 from .. import graphs
 from .ordered_set import OrderedSet
-CyclicList = graphs.CyclicList
+
+
+class CyclicList4(list):
+    def __init__(self):
+        return list.__init__(self, [None, None, None, None])
+
+    def __getitem__(self, n):
+        return list.__getitem__(self, n % 4)
+
 
 is_int_DT_exterior = re.compile(
     r'DT[:]? *(\[[0-9, \-\(\)]+\](?: *, *\[[01, ]+\])?)$')
 is_alpha_DT_exterior = re.compile(r'DT[:\[] *([a-zA-Z]+(?:\.[01]+)?)[\]]?$')
 
 # Helper function.
 
@@ -56,50 +64,51 @@
     for table in DT_tables:
         try:
             return str(table[name])
         except IndexError:
             continue
 
 
-class Crossing(object):
+class Crossing():
     """
     See "doc.pdf" for the conventions.  The sign of a crossing can be in {0,
     +1, -1}.  In the first case, the strands at the crossings can have
     any orientations, but crossings with sign +/-1 must be oriented as
     shown in "doc.pdf".
 
     Roles of some of the other attributes:
 
     * label: Arbitrary name used for printing the crossing.
 
     * directions: store the orientations of the link components passing
-    through the crossing.  For a +1 crossing this is { (0, 2), (3, 1) }.
-    Set with calls to make_tail.
+      through the crossing.  For a +1 crossing this is { (0, 2), (3, 1) }.
+      Set with calls to make_tail.
 
     * adjacent: The other Crossings that this Crossing is attached to.
 
     * strand_labels: Numbering of the strands, used for DT codes and
-    such.
+      such.
 
     * strand_components: Which element of the parent
-    Link.link_components each input's strand belongs to.
+      Link.link_components each input's strand belongs to.
     """
 
     def __init__(self, label=None):
         self.label = label
-        self.adjacent = CyclicList([None, None, None, None])
+        self.adjacent = CyclicList4()
         self._clear()
+        self._adjacent_len = 4
 
     def _clear(self):
         self.sign, self.directions = 0, set()
         self._clear_strand_info()
 
     def _clear_strand_info(self):
-        self.strand_labels = CyclicList([None, None, None, None])
-        self.strand_components = CyclicList([None, None, None, None])
+        self.strand_labels = CyclicList4()
+        self.strand_components = CyclicList4()
 
     def make_tail(self, a):
         """
         Orients the strand joining input "a" to input" a+2" to start at "a" and end at
         "a+2".
         """
         b = (a, (a + 2) % 4)
@@ -109,38 +118,46 @@
 
     def rotate(self, s):
         """
         Rotate the incoming connections by 90*s degrees anticlockwise.
         """
         def rotate(v):
             return (v + s) % 4
-        new_adjacent = CyclicList(self.adjacent[s:] + self.adjacent[:s])
+        new_adjacent = [self.adjacent[rotate(i)] for i in range(4)]
         for i, (o, j) in enumerate(new_adjacent):
             if o != self:
                 o.adjacent[j] = (self, i)
                 self.adjacent[i] = (o, j)
             else:
                 self.adjacent[i] = (self, (j - s) % 4)
 
-        self.directions = set([(rotate(a), rotate(b))
-                               for a, b in self.directions])
+        self.directions = set((rotate(a), rotate(b))
+                              for a, b in self.directions)
 
     def rotate_by_90(self):
         "Effectively switches the crossing"
         self.rotate(1)
 
     def rotate_by_180(self):
         "Effective reverses directions of the strands"
         self.rotate(2)
 
     def orient(self):
         if (2, 0) in self.directions:
             self.rotate_by_180()
         self.sign = 1 if (3, 1) in self.directions else -1
 
+    def is_incoming(self, i):
+        if self.sign == 1:
+            return i in (0, 3)
+        elif self.sign == -1:
+            return i in (0, 1)
+        else:
+            raise ValueError('Crossing not oriented')
+
     def __getitem__(self, i):
         return (self, i % 4)
 
     def entry_points(self):
         verts = [0, 1] if self.sign == -1 else [0, 3]
         return [CrossingEntryPoint(self, v) for v in verts]
 
@@ -195,31 +212,36 @@
     One of the four strands of a crossing.
     """
 
     def rotate(self, s=1):
         """
         The CrossingStrand *counter-clockwise* from self.
         """
-        return CrossingStrand(self.crossing, (self.strand_index + s) % len(self.crossing.adjacent))
+        c, e = self.crossing, self.strand_index
+        return CrossingStrand(c, (e + s) % c._adjacent_len)
 
     def opposite(self):
         """
         The CrossingStrand at the other end of the edge from self
         """
         return CrossingStrand(* self.crossing.adjacent[self.strand_index])
 
     def next(self):
         """
         The CrossingStrand obtained by moving in the direction of self for
         one crossing
         """
-        return self.rotate(2).opposite()
+        # Equivalent to: return self.rotate(2).opposite()
+        c, e = self.crossing, self.strand_index
+        return CrossingStrand(*c.adjacent[(e + 2) % c._adjacent_len])
 
     def next_corner(self):
-        return self.rotate().opposite()
+        # Equivalent to: return self.rotate().opposite()
+        c, e = self.crossing, self.strand_index
+        return CrossingStrand(*c.adjacent[(e + 1) % c._adjacent_len])
 
     def previous_corner(self):
         return self.opposite().rotate(-1)
 
     def strand_label(self):
         return self.crossing.strand_labels[self.strand_index]
 
@@ -240,19 +262,19 @@
 class CrossingEntryPoint(CrossingStrand):
     """
     One of the two entry points of an oriented crossing
     """
 
     def next(self):
         c, e = self.crossing, self.strand_index
-        s = 1 if isinstance(c, Strand) else 2
+        s = c._adjacent_len // 2
         return CrossingEntryPoint(*c.adjacent[(e + s) % (2 * s)])
 
     def previous(self):
-        s = 1 if isinstance(self.crossing, Strand) else 2
+        s = self.crossing._adjacent_len // 2
         return CrossingEntryPoint(*self.opposite().rotate(s))
 
     def other(self):
         nonzero_entry_point = 1 if self.crossing.sign == -1 else 3
         other = nonzero_entry_point if self.strand_index == 0 else 0
         return CrossingEntryPoint(self.crossing, other)
 
@@ -294,24 +316,26 @@
 
 
 class Labels(OrderedDict):
     def add(self, x):
         self[x] = len(self)
 
 
-class Strand(object):
+class Strand():
     """
     When constructing links, it's convenient to have strands as well
     as crossings.  These are stripped by the Link class when it
     pieces things together.
     """
 
-    def __init__(self, label=None):
+    def __init__(self, label=None, component_idx=None):
         self.label = label
         self.adjacent = [None, None]
+        self._adjacent_len = 2
+        self.component_idx = component_idx
 
     def fuse(self):
         """
         Joins the incoming and outgoing strands and removes
         self from the picture.
         """
         (a, i), (b, j) = self.adjacent
@@ -343,15 +367,15 @@
     ans = []
     for L in lists:
         ans.append([n + i for i, x in enumerate(L) if filter(n + i)])
         n += len(L)
     return ans
 
 
-class Link(object):
+class Link():
     """
     Links are made from Crossings.  The general model is that of the PD
     diagrams used in `KnotTheory <http://katlas.org/wiki/Planar_Diagrams>`_.
 
     See the file "doc.pdf" for the conventions, which can be accessed
     via "spherogram.pdf_docs()", and the `Spherogram tutorial
     <http://www.math.uic.edu/t3m/SnapPy/spherogram.html>`_
@@ -399,14 +423,15 @@
     """
 
     def __init__(self, crossings=None, braid_closure=None, check_planarity=True, build=True):
         self.name = None
 
         component_starts = None
         start_orientations = None
+        component_spec = None  # either None or a list of (CrossingStrand, int) pairs
 
         if crossings is not None and braid_closure is not None:
             raise ValueError('Specified *both* crossings and braid_closure')
 
         if crossings is not None:
             if isinstance(crossings, str):
                 crossings = self._crossings_from_string(crossings)
@@ -418,33 +443,94 @@
                 start_orientations = component_starts[:]
         elif braid_closure is not None:
             crossings = self._crossings_from_braid_closure(braid_closure)
         else:
             crossings = []  # empty link
 
         # Make sure everything is tied up.
-        if True in [None in c.adjacent for c in crossings]:
-            raise ValueError('No loose strands allowed')
+        if any(None in c.adjacent for c in crossings):
+            raise ValueError('no loose strands allowed')
 
         # Fuse the strands.  If there any components made up
         # only of strands, these are thrown out here.
+        # We also construct component_spec from these which will
+        # be used to permute the components of the link.
 
         self.unlinked_unknot_components = 0
+        component_strands = []
         for s in crossings:
             if isinstance(s, Strand):
-                if s.is_loop():
+                if s.component_idx is not None:
+                    # defer fusing
+                    component_strands.append(s)
+                elif s.is_loop():
                     self.unlinked_unknot_components += 1
+                else:
+                    s.fuse()
+        if component_starts and component_strands:
+            raise Exception("Strands cannot have component indices if the"
+                            " link already has component_starts")
+        # check component strands are incident only to crossings
+        for s in component_strands:
+            if not all(isinstance(c, Crossing) for c, _ in s.adjacent):
+                raise ValueError("Strands with a component index must be in the same"
+                                 " component as a crossing")
+        # Go through the component strands to construct component_starts
+        if component_strands:
+            component_spec = []
+            for s in component_strands:
+                c, i = s.adjacent[0]
+                assert isinstance(c, Crossing)
+                component_spec.append((CrossingStrand(c, i), s.component_idx))
+                assert not s.is_loop()  # at this point it is impossible to be a loop
                 s.fuse()
+
+        # Finally remove all the Strand objects from the crossing list
         self.crossings = [c for c in crossings if not isinstance(c, Strand)]
 
         if build:
             self._build(start_orientations, component_starts)
             if check_planarity and not self.is_planar():
                 raise ValueError("Link isn't planar")
 
+            if component_spec:
+                # Assemble a permutation of the link components
+                component_perm = [None] * len(self.link_components)
+                unused_comps = OrderedSet(reversed(range(len(self.link_components))))
+                for cs, idx in component_spec:
+                    # orient the crossing strand as a CrossingEntryPoint
+                    cs = cs.crossing.entry_points()[cs.strand_index % 2]
+                    # Locate the link component that contains this cs
+                    for i, comp in enumerate(self.link_components):
+                        if cs in comp:
+                            if component_perm[idx] == i:
+                                # This is a second Strand in the same component
+                                # with the same component_idx, which is OK
+                                break
+                            elif component_perm[idx] is None:
+                                if i not in unused_comps:
+                                    raise ValueError("Two Strand objects in the same component"
+                                                     " have different component_idx values")
+                                component_perm[idx] = i
+                                unused_comps.remove(i)
+                                break
+                            else:
+                                raise ValueError("Two Strand objects in different components"
+                                                 " have the same component_idx values")
+                    else:
+                        raise Exception()  # This should not happen
+                for i in range(len(self.link_components)):
+                    if component_perm[i] is None:
+                        # This is why unused_comps is initialized with reversed order
+                        component_perm[i] = unused_comps.pop()
+                assert len(unused_comps) == 0
+
+                component_starts = [self.link_components[i][0] for i in component_perm]
+                self._build_components(component_starts=component_starts)
+
         # If the crossings aren't labeled then label them for
         # debugging purposes.
         if all(X.label is None for X in self.crossings):
             for c, X in enumerate(self.crossings):
                 X.label = c
 
     def _crossings_from_string(self, spec):
@@ -501,15 +587,15 @@
         for c, X in enumerate(code):
             for i, x in enumerate(X):
                 if x in gluings:
                     gluings[x].append((c, i))
                 else:
                     gluings[x] = [(c, i)]
 
-        if set([len(v) for v in gluings.values()]) != set([2]):
+        if set(len(v) for v in gluings.values()) != set([2]):
             raise ValueError("PD code isn't consistent")
 
         component_starts = self._component_starts_from_PD(
             code, labels, gluings)
 
         crossings = [Crossing(i) for i, d in enumerate(code)]
         for (c, i), (d, j) in gluings.values():
@@ -554,19 +640,29 @@
                 if l1 < l2:
                     next_label = l1
                     direction = (c1, j1)
                 elif l2 < l1:
                     next_label = l2
                     direction = (c2, j2)
                 else:
-                    # have a component of length 2, so now rely on the
-                    # convention that the first position at a PD
-                    # crossing is a directed entry point.
+                    # We have a component of length 2, so now rely on
+                    # the convention that the first position at a PD
+                    # crossing is a directed entry point. (If both
+                    # crossings are over or both under, the
+                    # orientation is arbitrary anyway.)
                     next_label = l1
-                    direction = (c2, j2) if j2 % 2 == 1 else (c1, j1)
+
+                    # The strand labeled m is oriented c2 --> c1 if
+                    # and only if either l1 = l2 is the incoming
+                    # understrand of c2 or m is incoming understrand
+                    # at c1.
+                    if code[c2][0] == l1 or code[c1][0] == m:
+                        direction = (c1, j1)
+                    else:
+                        direction = (c2, j2)
 
                 starts.append(direction)
             while next_label != m:
                 labels.remove(next_label)
                 g = gluings[next_label]
                 other_direction = g[1 - g.index(direction)]
                 direction = (other_direction[0], (other_direction[1] + 2) % 4)
@@ -591,15 +687,15 @@
         then sigma_i corresponds to the rational tangle -1 in our
         conventions.
 
         The components of the resulting link are will be oriented
         consistently with the braid.
         """
         if num_strands is None:
-            num_strands = max([abs(a) for a in word]) + 1
+            num_strands = max(abs(a) for a in word) + 1
 
         strands = [Strand('s' + repr(i)) for i in range(num_strands)]
         current = [(x, 1) for x in strands]
         crossings = []
 
         for i, a in enumerate(word):
             C = Crossing('x' + repr(i))
@@ -639,14 +735,28 @@
             c._clear()
         if same_components_and_orientations:
             self._build(start_orientations=start_css,
                         component_starts=start_css)
         else:
             self._build()
 
+    def _check_crossing_orientations(self):
+        for C in self.crossings:
+            if C.sign == 1:
+                assert C.directions == {(0, 2), (3, 1)}
+            elif C.sign == -1:
+                assert C.directions == {(0, 2), (1, 3)}
+            else:
+                assert False
+            for (a, b) in C.directions:
+                D, d = C.adjacent[b]
+                assert d in {x for x, y in D.directions}
+                D, d = C.adjacent[a]
+                assert d in {y for x, y in D.directions}
+
     def _orient_crossings(self, start_orientations=None):
         if self.all_crossings_oriented():
             return
         if start_orientations is None:
             start_orientations = list()
         remaining = OrderedSet(
             [(c, i) for c in self.crossings for i in range(4) if c.sign == 0])
@@ -715,14 +825,16 @@
         >>> L.DT_code()
         [(18, 10, 16, 14), (2, 4, 6, 12, 20, 8)]
         >>> L._build_components([C0[-1], C1[0]])
         >>> L.DT_code()
         [(20, 12, 18, 16), (8, 2, 4, 6, 14, 10)]
         """
         if component_starts is not None:
+            # Take all CrossingStrand and CrossingEntryPoint objects
+            # and turn them into CrossingEntryPoints
             component_starts = [cs.crossing.entry_points()[cs.strand_index % 2]
                                 for cs in component_starts]
         remaining, components = OrderedSet(
             self.crossing_entries()), LinkComponents()
         other_crossing_entries = []
         self.labels = labels = Labels()
         for c in self.crossings:
@@ -871,18 +983,22 @@
         Alternatively, the sequence of CrossingStrands can be regarded
         as the *heads* of the oriented edges of the face.
         """
         corners = OrderedSet([CrossingStrand(c, i)
                               for c in self.crossings for i in range(4)])
         faces = []
         while len(corners):
-            face = [corners.pop()]
+            cs0 = corners.pop()
+            face = [cs0]
+            next = cs0
             while True:
-                next = face[-1].next_corner()
-                if next == face[0]:
+                # Next two lines equiv to: next = next.next_corner()
+                c, e = next.crossing, next.strand_index
+                next = CrossingStrand(*c.adjacent[(e + 1) % 4])
+                if next == cs0:
                     faces.append(face)
                     break
                 else:
                     corners.remove(next)
                     face.append(next)
 
         return faces
@@ -1025,15 +1141,15 @@
                 try:
                     self.link_components[c]
                 except IndexError:
                     raise ValueError('No component of that index')
             indices.append(c)
 
         def keep(C):
-            return set([i in indices for i in C.strand_components]) == set([True])
+            return all(i in indices for i in C.strand_components)
 
         L = self.copy()
         final_crossings = []
         for C in L.crossings:
             if keep(C):
                 final_crossings.append(C)
             else:
@@ -1061,15 +1177,15 @@
         >>> L_copy = Link(L.PD_code())
         >>> [len(c) for c in L_copy.link_components]
         [4, 4, 4, 6, 8]
         """
         PD = []
 
         for c in self.crossings:
-            PD.append([s + min_strand_index for s in c.strand_labels[:]])
+            PD.append([s + min_strand_index for s in c.strand_labels])
         if KnotTheory:
             PD = "PD" + repr(PD).replace('[', 'X[')[1:]
         else:
             PD = [tuple(x) for x in PD]
         return PD
 
     def _oriented_PD_code(self, KnotTheory=False, min_strand_index=0):
@@ -1105,42 +1221,42 @@
         'a' being 2, 'A' being -2, etc.
         """
         DT_info = [c.DT_info() for c in self.crossings]
         first_to_second = {first: second for first, second, _ in DT_info}
         first_to_flip = {first: flip for first, _, flip in DT_info}
         odd_labels = enumerate_lists(
             self.link_components, n=1, filter=lambda x: x % 2 == 1)
-        DT = [tuple([first_to_second[x] for x in component])
+        DT = [tuple(first_to_second[x] for x in component)
               for component in odd_labels]
-        the_flips = [first_to_flip[x] for x in sum(odd_labels, [])]
+        the_flips = (first_to_flip[x] for x in sum(odd_labels, []))
 
         if DT_alpha:
             if len(self) > 52:
                 raise ValueError("Too many crossing for alphabetic DT code")
             DT_alphabet = '_abcdefghijklmnopqrstuvwxyzZYXWVUTSRQPONMLKJIHGFEDCBA'
             init_data = [len(self), len(DT)] + [len(c) for c in DT]
             DT = ''.join([DT_alphabet[x] for x in init_data] +
                          [DT_alphabet[x >> 1] for x in sum(DT, tuple())])
             if flips:
-                DT += '.' + ''.join([repr(flip) for flip in the_flips])
-            return "DT[" + DT + "]"
+                DT += '.' + ''.join(repr(flip) for flip in the_flips)
+            return f"DT[{DT}]"
         else:
             if flips:
-                return DT, the_flips
+                return DT, list(the_flips)
             else:
                 return DT
 
     def peer_code(self):
-        peer = dict([c.peer_info() for c in self.crossings])
+        peer = dict(c.peer_info() for c in self.crossings)
         even_labels = enumerate_lists(
             self.link_components, n=0, filter=lambda x: x % 2 == 0)
-        ans = '[' + ','.join([repr([peer[c][0] for c in comp])
-                              [1:-1].replace(',', '') for comp in even_labels])
-        ans += '] / ' + ' '.join([['_', '+', '-'][peer[c][1]]
-                                  for c in sum(even_labels, [])])
+        ans = '[' + ','.join(repr([peer[c][0] for c in comp])
+                             [1:-1].replace(',', '') for comp in even_labels)
+        ans += '] / ' + ' '.join(['_', '+', '-'][peer[c][1]]
+                                 for c in sum(even_labels, []))
         return ans
 
     def KLPProjection(self):
         return python_KLP(self)
 
     def split_link_diagram(self, destroy_original=False):
         """
@@ -1275,39 +1391,34 @@
         True
         """
         if recursively:
             return copy.deepcopy(self)
         else:
             crossings = [Crossing(c.label) for c in self.crossings]
             old_to_new = dict(zip(self.crossings, crossings))
-            loose_strands = set(
-                [(n, i) for n in range(len(crossings)) for i in range(4)])
-            while loose_strands:
-                n, i = loose_strands.pop()
-                adj_c, adj_i = self.crossings[n].adjacent[i]
-                adj_n = self.crossings.index(adj_c)
-                crossings[n][i] = crossings[adj_n][adj_i]
-                loose_strands.remove((adj_n, adj_i))
-
-            # Orient the new crossings.
-            for old, new in old_to_new.items():
-                new.make_tail(0)
-                e = 3 if old.sign == 1 else 1
-                new.make_tail(e)
-                new.orient()
-
-            component_starts = []
-            for component in self.link_components:
-                old_crossing, entry_point = component[0]
-                crossing = old_to_new[old_crossing]
-                component_starts.append(
-                    CrossingEntryPoint(crossing, entry_point))
+
+            for old_cross, new_cross in old_to_new.items():
+                new_cross.sign = old_cross.sign
+                new_cross.directions = old_cross.directions.copy()
+                new_cross.strand_components = old_cross.strand_components.copy()
+                new_cross.strand_labels = old_cross.strand_labels.copy()
+                for i in range(4):
+                    adj_cross, adj_index = old_cross.adjacent[i]
+                    new_cross.adjacent[i] = (old_to_new[adj_cross], adj_index)
+
             link = self.__class__(crossings=crossings,
                                   check_planarity=False, build=False)
-            link._build(component_starts=component_starts)
+            link.link_components = []
+            for old_component in self.link_components:
+                new_component = []
+                for old_crossing, entry_point in old_component:
+                    crossing = old_to_new[old_crossing]
+                    new_component.append(CrossingEntryPoint(crossing, entry_point))
+                link.link_components.append(new_component)
+
             link.name = self.name
             return link
 
     def mirror(self):
         """
         Returns the mirror image of the link, preserving link orientations and
         component order.
@@ -1410,15 +1521,15 @@
 
 
 def vertex_to_KLP(c, v):
     i = v if c.sign == 1 else (v - 1) % 4
     return ['Ybackward', 'Xforward', 'Yforward', 'Xbackward'][i]
 
 
-class KLPCrossing(object):
+class KLPCrossing():
     """
     SnapPea uses a convention where the orientation
     of the strands is fixed in the master picture but
     which strand is on top varies.
     """
 
     def __init__(self, c):
```

### Comparing `spherogram-2.1/spherogram_src/links/morse.py` & `spherogram-2.2/spherogram_src/links/morse.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 To each corner of a face of D is classified into "large", "flat", or
 "small" (which is the default) as per Figure 3 of [DP], which
 correspond to integers 2, 1, and 0 respectively.  The geometric
 conditions are
 
 * Every vertex has either a single "large" angle or two "flat" ones which
-are opposite.
+  are opposite.
 
 * The sum of the corner types around every face is degree - 2, with the
-exception of the exterior face (which is degree + 2).
+  exception of the exterior face (which is degree + 2).
 
 This code written by Nathan Dunfield who claims (not very plausibly) that
 he will write a paper about this algorithm at some point.  The bit that
 annoys him is that [DP] is polynomial time, but the algorithm here is not
 known to be.  The issue is that [DP] creates a very special kind of ILP
 (a network flow) which can be solved in polynomial time, but below we're
 reduced to using a generic ILP solver.
@@ -43,20 +43,22 @@
 
 
 def morse_via_LP(link, solver='GLPK'):
     """
     An integer linear program which computes the Morse number of the given
     link diagram.
 
-    sage: K = RationalTangle(23, 43).denominator_closure()
-    sage: morse, details = morse_via_LP(K)
-    sage: morse
-    2
-    sage: morse_via_LP(Link('8_20'))[0]
-    3
+    EXAMPLES::
+
+        sage: K = RationalTangle(23, 43).denominator_closure()
+        sage: morse, details = morse_via_LP(K)
+        sage: morse
+        2
+        sage: morse_via_LP(Link('8_20'))[0]
+        3
     """
     LP = MixedIntegerLinearProgram(maximization=False, solver=solver)
 
     # Near a crossing, the level sets of the height function are either
     # horizontal or vertical, and so there are two flat corners which
     # must be opposite.
     hor_cross = LP.new_variable(binary=True)
@@ -92,15 +94,17 @@
     LP.set_objective(sum(large_edge.values()))
     morse = int(LP.solve())
     assert morse % 2 == 0
     return morse // 2, LP.get_values([hor_cross, vert_cross, flat_edge, large_edge, exterior])
 
 
 def have_positive_value(D):
-    return [k for k, v in D.items() if v > 0]
+    for k, v in D.items():
+        if v > 0:
+            yield k
 
 
 class ImmutableValueDict(dict):
     def __setitem__(self, index, value):
         if index in self:
             if self[index] != value:
                 raise ValueError("Can't change an assigned value")
@@ -143,27 +147,27 @@
 
         heights = [link.heights[cs.crossing] for cs in ans]
         assert heights == sorted(heights)
         ans.heights = heights
         return ans
 
 
-class MorseLinkDiagram(object):
+class MorseLinkDiagram():
     """
     A planar link diagram with a height function on R^2 which
     is Morse on the link.
     """
 
     def __init__(self, link, solver='GLPK'):
         self.link = link = link.copy()
         morse, values = morse_via_LP(link, solver)
         self.morse_number = morse
         self.bends = set(have_positive_value(values[3]))
         self.faces = link.faces()
-        self.exterior = self.faces[have_positive_value(values[4])[0]]
+        self.exterior = self.faces[next(iter(have_positive_value(values[4])))]
         for c in have_positive_value(values[0]):
             c.kind = 'horizontal'
         for c in have_positive_value(values[1]):
             c.kind = 'vertical'
         self.orient_edges()
         self.set_heights()
         self.upward_snakes()
@@ -221,18 +225,21 @@
         """
         The two upward strands below the crossing.
         """
         kinds = self.orientations
         a = CrossingStrand(crossing, 0)
         b = a.rotate()
         upmin = set(['up', 'min'])
+        test_a = kinds[a] in upmin
         while True:
-            if set([kinds[a], kinds[b]]).issubset(upmin):
+            test_b = kinds[b] in upmin
+            if test_a and test_b:
                 return a, b
             a, b = b, b.rotate()
+            test_a = test_b
 
     def adjacent_upwards(self, crossing_strand):
         a, b = crossing_strand.rotate(), crossing_strand.rotate(-1)
         if self.orientations[a] in ['up', 'min']:
             return a
         else:
             assert self.orientations[b] in ['up', 'min']
@@ -286,15 +293,15 @@
         kinds = self.orientations
         self.snakes = snakes = []
         for cs in self.bends:
             if kinds[cs] == 'min':
                 snakes += [UpwardSnake(cs, self),
                            UpwardSnake(cs.opposite(), self)]
 
-        self.strand_to_snake = dict()
+        self.strand_to_snake = {}
         for snake in snakes:
             for s in snake:
                 self.strand_to_snake[s] = snake
             self.strand_to_snake[snake.final] = snake
 
         self.pack_snakes()
 
@@ -312,15 +319,15 @@
             a = b.opposite()
             S.add_edge(to_snake[a], to_snake[b])
 
         snake_pos = basic_topological_numbering(S)
         self.S, self.snake_pos = S, snake_pos
         heights = self.heights
         max_height = max(heights.values())
-        snakes_at_height = dict()
+        snakes_at_height = {}
         for h in range(max_height + 1):
             at_this_height = []
             for snake in snakes:
                 if heights[snake[0].crossing] <= h <= heights[snake[-1].crossing]:
                     at_this_height.append(snake)
 
             at_this_height.sort(key=lambda s: snake_pos[s])
@@ -330,15 +337,16 @@
         self.snakes_at_height = snakes_at_height
 
     def is_bridge(self):
         """
         Returns whether the link is in bridge position with respect to this
         height function.
         """
-        return sorted(self.snake_pos.values()) == list(range(len(self.snakes)))
+        return all(i == j
+                   for i, j in enumerate(sorted(self.snake_pos.values())))
 
     def bridge(self):
         if not self.is_bridge():
             raise ValueError("Morse function doesn't give a bridge diagram")
 
         def to_index(cs):
             return self.snake_pos[self.strand_to_snake[cs]]
@@ -364,15 +372,15 @@
             return tuple(sorted([to_index(cs), to_index(cn)]))
 
         top = set(top_pairing(snake) for snake in self.snakes)
 
         return BridgeDiagram(bottom, [cd[1] for cd in cross_data], top)
 
 
-class BridgeDiagram(object):
+class BridgeDiagram():
     """
     A proper bridge diagram of a link, that is, a height function
     where all the mins are below all the maxes.
     """
 
     def __init__(self, bottom, crossings, top):
         self.bottom, self.crossings, self.top = bottom, crossings, top
```

### Comparing `spherogram-2.1/spherogram_src/links/ordered_set.py` & `spherogram-2.2/spherogram_src/links/ordered_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class OrderedSet():
     def __init__(self, iterable=None):
         if iterable is not None:
-            self.elts = {e:None for e in iterable}
+            self.elts = {e: None for e in iterable}
         else:
             self.elts = dict()
 
     def __len__(self):
         return len(self.elts)
 
     def __contains__(self, key):
@@ -15,15 +15,15 @@
         self.elts[key] = None
 
     def discard(self, key):
         if key in self.elts:
             self.elts.pop(key)
 
     def __iter__(self):
-        return iter(self.elts.keys())
+        return iter(self.elts)
 
     def pop(self):
         return self.elts.popitem()[0]
 
     def update(self, sequence):
         for s in sequence:
             self.elts[s] = None
@@ -41,15 +41,16 @@
     def __repr__(self):
         if not self:
             return '%s()' % (self.__class__.__name__,)
         return '%s(%r)' % (self.__class__.__name__, list(self))
 
     def __eq__(self, other):
         if isinstance(other, OrderedSet):
-            return len(self) == len(other) and list(self) == list(other)
+            return len(self) == len(other) and all(x == y
+                                                   for x, y in zip(self, other))
         return set(self) == set(other)
 
 
 if __name__ == '__main__':
     s = OrderedSet('abracadaba')
     t = OrderedSet('simsalabim')
     print(s == t, t == t)
```

### Comparing `spherogram-2.1/spherogram_src/links/orthogonal.py` & `spherogram-2.2/spherogram_src/links/orthogonal.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,15 +659,15 @@
 
     def random_link():
         return link_from_manifold(HTLinkExteriors.random())
 
     def check_faces(link):
         faces = link.faces()
         assert len(link.vertices) - len(link.edges) + len(faces) == 2
-        assert set(Counter(sum(faces, [])).values()) == set([1])
+        assert all(val == 1 for val in Counter(sum(faces, [])).values())
         assert link.is_planar()
 
     def test_face_method(N):
         for i in range(N):
             check_faces(random_link())
 
     def element(S):
```

### Comparing `spherogram-2.1/spherogram_src/links/planar_isotopy.py` & `spherogram-2.2/spherogram_src/links/planar_isotopy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,277 +1,293 @@
 import spherogram
 
 """
-This file contains functions to distinguish tangle diagrams up to planar 
-isotopy. It can allow for roots, as well as distinguishing the shadows or 
+This file contains functions to distinguish tangle diagrams up to planar
+isotopy. It can allow for roots, as well as distinguishing the shadows or
 the tangle diagrams with the information of whether a crossing is over or under.
 """
 
+
 def rotate_list(L, s):
     n = len(L)
-    return [ L[(i + s) % n] for i in range(n) ]
+    return [L[(i + s) % n] for i in range(n)]
+
 
 def flip(L):
-    half = len(L)/2
+    half = len(L) // 2
     for i in range(half):
-        L[i],L[i+half] = L[i+half],L[i]
+        L[i], L[i + half] = L[i + half], L[i]
+
 
 def clear_orientations(crossings):
     for c in crossings:
         c.directions.clear()
         c.sign = 0
 
 
-def isosig(tangle,root = None, over_or_under = False):
+def isosig(tangle, root=None, over_or_under=False):
     strands, loops, orientations, crossing_order, over_or_under_data = all_cross_strands(tangle)
     isosig_strands = []
     isosig_loops = []
-    if root != None:
+    if root is not None:
         want_root = True
         root_position = crossing_order.index(root.crossing)
         root_tuple = tuple(root)
         root_tuple_op = tuple(root.rotate(2))
     else:
         want_root = False
     found_root = False
     root_isosig = None
-    for strand,end in strands:
-        isst = map(lambda cs: crossing_order.index(cs[0]),strand)
+    for strand, end in strands:
+        isst = [crossing_order.index(cs[0]) for cs in strand]
         if (want_root) and (not found_root) and (root_position in isst):
-            root_strand_indices = [i for i in range(len(isst)) if isst[i]==root_position]
+            root_strand_indices = [i for i, isti in enumerate(isst)
+                                   if isti == root_position]
             for root_strand_index in root_strand_indices:
                 if root_tuple == strand[root_strand_index]:
                     found_root = True
-                    root_isosig = (root_position,(strands.index((strand,end)),root_strand_index),-1,'s')
+                    root_isosig = (root_position, (strands.index((strand, end)), root_strand_index), -1, 's')
                 elif root_tuple_op == strand[root_strand_index]:
                     found_root = True
-                    root_isosig = (root_position,(strands.index((strand,end)),root_strand_index),1,'s')
-        isosig_strands.append((tuple(isst),end))
+                    root_isosig = (root_position, (strands.index((strand, end)), root_strand_index), 1, 's')
+        isosig_strands.append((tuple(isst), end))
     for loop in loops:
-        isl = map(lambda cs: crossing_order.index(cs[0]),loop)
+        isl = [crossing_order.index(cs[0]) for cs in loop]
         if (want_root) and (not found_root) and (root_position in isl):
-            root_loop_indices = [i for i in range(len(isl)) if isl[i]==root_position]
+            root_loop_indices = [i for i, isli in enumerate(isl)
+                                 if isli == root_position]
             for root_loop_index in root_loop_indices:
                 if root_tuple == loop[root_loop_index]:
                     found_root = True
-                    root_isosig = (root_position,(loops.index(loop),root_loop_index),-1,'l')
+                    root_isosig = (root_position, (loops.index(loop), root_loop_index), -1, 'l')
                 elif root_tuple_op == loop[root_loop_index]:
                     found_root = True
-                    root_isosig = (root_position,(loops.index(loop),root_loop_index),1,'l')
+                    root_isosig = (root_position, (loops.index(loop), root_loop_index), 1, 'l')
         isosig_loops.append(tuple(isl))
     isosig_over_or_under = []
     if over_or_under:
         isosig_over_or_under = [over_or_under_data[c] for c in crossing_order]
     isosig_orientations = [orientations[c] for c in crossing_order]
-    return (len(tangle.crossings),tangle.n),tuple(isosig_strands),tuple(isosig_loops),tuple(isosig_orientations), tuple(isosig_over_or_under), root_isosig
+    return (len(tangle.crossings), tangle.boundary), tuple(isosig_strands), tuple(isosig_loops), tuple(isosig_orientations), tuple(isosig_over_or_under), root_isosig
 
-def min_isosig(tangle,root=None,over_or_under=False):
-    if root != None:
+
+def min_isosig(tangle, root=None, over_or_under=False):
+    if root is not None:
         cs_name = cslabel(root)
     isosigs = []
-    for i in range(tangle.n*2):
-        rotated_tangle = tangle.circular_rotate(i)
-        if root != None:
-            rotated_root = crossing_strand_from_name(rotated_tangle,cs_name)
+    for i in range(tangle.boundary[0] + tangle.boundary[1]):
+        rotated_tangle = tangle.reshape((tangle.boundary[0] + tangle.boundary[1], 0), i)
+        if root is not None:
+            rotated_root = crossing_strand_from_name(rotated_tangle, cs_name)
         else:
             rotated_root = None
-        isosigs.append(isosig(rotated_tangle, root=rotated_root,over_or_under=over_or_under))
+        isosigs.append(isosig(rotated_tangle, root=rotated_root,
+                              over_or_under=over_or_under))
     return min(isosigs)
 
 
 def isosig_with_gluings(tangle, gluings, root=None):
-    return (isosig(tangle,root = root),tuple(gluings))
+    return (isosig(tangle, root=root), tuple(gluings))
+
 
-def min_isosig_with_gluings(tangle, gluings, root = None):
-    if root != None:
+def min_isosig_with_gluings(tangle, gluings, root=None):
+    if root is not None:
         cs_name = cslabel(root)
     isosigs = []
-    for i in range(tangle.n*2):
-        rotated_tangle = tangle.circular_rotate(i)
-        if root != None:
-            rotated_root = crossing_strand_from_name(rotated_tangle,cs_name)
+    for i in range(tangle.boundary[0] + tangle.boundary[1]):
+        rotated_tangle = tangle.reshape((tangle.boundary[0] + tangle.boundary[1], 0), i)
+        if root is not None:
+            rotated_root = crossing_strand_from_name(rotated_tangle, cs_name)
         else:
             rotated_root = None
-        #permuting the indices in the gluings
-        perm = range(len(tangle.adjacent))
-        perm[len(perm)/2:] = reversed(perm[len(perm)/2:])
-        perm = rotate_list(perm,i)
-        perm[len(perm)/2:] = reversed(perm[len(perm)/2:])
+        # permuting the indices in the gluings
+        perm = range(tangle.boundary[0] + tangle.boundary[1])
+        perm[tangle.boundary[0]:] = reversed(perm[tangle.boundary[0]:])
+        perm = rotate_list(perm, i)
         rotated_gluings = []
         for g in gluings:
-            new_g = [perm[g[0]],perm[g[1]]]
+            new_g = [perm[g[0]], perm[g[1]]]
             new_g.sort()
             rotated_gluings.append(tuple(new_g))
         rotated_gluings.sort()
-        isosigs.append(isosig_with_gluings(rotated_tangle, rotated_gluings,root=rotated_root))        
-
-
+        isosigs.append(isosig_with_gluings(rotated_tangle, rotated_gluings,
+                                           root=rotated_root))
     return min(isosigs)
 
 
 def crossing_orientations(strands):
     """
     Given the strands, compute the orientations (+1 or -1) for each crossing
     in the tangle
     """
     orientations = {}
     over_or_under = {}
     css_seen = []
     for strand in strands:
         for cs in strand:
-            for seen_cs in css_seen: 
+            for seen_cs in css_seen:
                 if cs[0] == seen_cs[0]:
-                    orientation = (cs[1]-seen_cs[1])%4
+                    orientation = (cs[1] - seen_cs[1]) % 4
                     if orientation == 3:
                         orientation = -1
-                    orientations[cs[0]]=orientation
-                    over_or_under[cs[0]] = (cs[1]%2)
+                    orientations[cs[0]] = orientation
+                    over_or_under[cs[0]] = (cs[1] % 2)
                     break
-            css_seen.append(cs) #didn't find cs
+            css_seen.append(cs)  # didn't find cs
     return orientations, over_or_under
 
-"""
-Give a list of the crossing strands encountered starting at 
-a strand on the boundary of a tangle and moving to the other
-end of that strand.
-"""
-def cross_strand(tangle,i):
-    if i >= 2*tangle.n:
-        raise Exception("Not a valid start position for strand")
+
+def cross_strand(tangle, i):
+    """
+    Give a list of the crossing strands encountered starting at
+    a strand on the boundary of a tangle and moving to the other
+    end of that strand.
+    """
+    if i >= tangle.boundary[0] + tangle.boundary[1]:
+        raise ValueError("not a valid start position for strand")
     cs = tangle.adjacent[i]
     strand = [cs]
-    while (cs[0],(cs[1]+2)%4) not in tangle.adjacent:
-        cs = cs[0].adjacent[(cs[1]+2)%4]
+    while (cs[0], (cs[1] + 2) % 4) not in tangle.adjacent:
+        cs = cs[0].adjacent[(cs[1] + 2) % 4]
         strand.append(cs)
     return strand
 
+
 def loop_strand(cs):
     """
     Get the closed loop starting at crossing strand cs
     """
     strand = [cs]
-    cs = cs[0].adjacent[(cs[1]+2)%4]
+    cs = cs[0].adjacent[(cs[1] + 2) % 4]
     while cs not in strand:
         strand.append(cs)
-        cs = cs[0].adjacent[(cs[1]+2)%4]
+        cs = cs[0].adjacent[(cs[1] + 2) % 4]
     return strand
 
+
 def all_cross_strands(tangle):
     """
-    Returns all the strands but without duplicate in the opposite direction,
-    starting at position 0 and going clockwise, and then components that 
+    Return all the strands but without duplicate in the opposite direction,
+    starting at position 0 and going clockwise, and then components that
     don't intersect the boundary.
     """
-    other_ends_seen = [] #use to eliminate duplicate strand in other direction
+    other_ends_seen = []  # use to eliminate duplicate strand in other direction
     strands = []
     strands_with_ends = []
     loops = []
-    clockwise_order = range(tangle.n)
-    clockwise_order.extend(reversed(range(tangle.n,tangle.n*2)))
+    tm, tn = tangle.boundary
+    clockwise_order = list(range(tm))
+    clockwise_order.extend(reversed(range(tm, tm + tn)))
     for i in clockwise_order:
         if i not in other_ends_seen:
-            strand = cross_strand(tangle,i)
+            strand = cross_strand(tangle, i)
             cs = strand[-1]
-            end = tangle.adjacent.index((cs[0],(cs[1]+2)%4))
+            end = tangle.adjacent.index((cs[0], (cs[1] + 2) % 4))
             if end not in other_ends_seen:
                 strands.append(strand)
-                strands_with_ends.append((strand,end))
+                strands_with_ends.append((strand, end))
                 other_ends_seen.append(end)
     orientations, over_or_under = crossing_orientations(strands)
     cs_seen = [cs for strand in strands for cs in strand]
     seen_once = set(cs[0] for cs in cs_seen)
     for crossing in orientations:
         seen_once.remove(crossing)
     for strand in strands:
         for cs in strand:
             if cs[0] in seen_once:
-                loop = loop_strand((cs[0],(cs[1]+1)%4))
+                loop = loop_strand((cs[0], (cs[1] + 1) % 4))
                 loops.append(loop)
                 cs_seen.extend(loop)
                 for loop_cs in loop:
                     if loop_cs[0] in seen_once:
                         for seen_cs in cs_seen:
                             if loop_cs[0] == seen_cs[0]:
-                                orientation = (loop_cs[1]-seen_cs[1])%4
+                                orientation = (loop_cs[1] - seen_cs[1]) % 4
                                 if orientation == 3:
                                     orientation = -1
-                                orientations[loop_cs[0]]=orientation
-                                over_or_under[loop_cs[0]] = loop_cs[1]%2
+                                orientations[loop_cs[0]] = orientation
+                                over_or_under[loop_cs[0]] = loop_cs[1] % 2
                                 seen_once.remove(loop_cs[0])
                                 break
                     else:
                         seen_once.add(loop_cs[0])
-    while len(orientations)<len(tangle.crossings):
+    while len(orientations) < len(tangle.crossings):
         for loop in loops:
             for cs in loop:
                 if cs[0] in seen_once:
-                     loop = loop_strand((cs[0],(cs[1]+1)%4))
-                     loops.append(loop)
-                     cs_seen.extend(loop)
-                     for loop_cs in loop:
-                         if loop_cs[0] in seen_once:
-                             for seen_cs in cs_seen:
-                                 if loop_cs[0] == seen_cs[0]:
-                                     orientation = (loop_cs[1]-seen_cs[1])%4
-                                     if orientation == 3:
-                                         orientation = -1
-                                     orientations[loop_cs[0]]=orientation
-                                     over_or_under[loop_cs[0]]= loop_cs[1]%2
-                                     seen_once.remove(loop_cs[0])
-                                     break
-                         else:
-                             seen_once.add(loop_cs[0])
-    crossings = map(lambda x: x[0], cs_seen)
+                    loop = loop_strand((cs[0], (cs[1] + 1) % 4))
+                    loops.append(loop)
+                    cs_seen.extend(loop)
+                    for loop_cs in loop:
+                        if loop_cs[0] in seen_once:
+                            for seen_cs in cs_seen:
+                                if loop_cs[0] == seen_cs[0]:
+                                    orientation = (loop_cs[1] - seen_cs[1]) % 4
+                                    if orientation == 3:
+                                        orientation = -1
+                                    orientations[loop_cs[0]] = orientation
+                                    over_or_under[loop_cs[0]] = loop_cs[1] % 2
+                                    seen_once.remove(loop_cs[0])
+                                    break
+                        else:
+                            seen_once.add(loop_cs[0])
+    crossings = [x[0] for x in cs_seen]
     crossing_order = []
     for c in crossings:
         if c not in crossing_order:
             crossing_order.append(c)
-    return strands_with_ends,loops,orientations,crossing_order, over_or_under
+    return strands_with_ends, loops, orientations, crossing_order, over_or_under
+
 
 def cslabel(cs):
     """
     Label of crossing strand, without frills
     """
-    return (cs[0].label,cs[1])
+    return (cs[0].label, cs[1])
 
-def crossing_strand_from_name(link,csname):
+
+def crossing_strand_from_name(link, csname):
     """
     Find crossing strand object from it's name in the format of cslabel above
     """
     for c in link.crossings:
         if c.label == csname[0]:
             return c.crossing_strands()[csname[1]]
-    raise Exception("Crossing not found")
+    raise ValueError("crossing not found")
+
 
-def crossing_from_name(link,crossname):
+def crossing_from_name(link, crossname):
     for c in link.crossings:
         if c.label == crossname:
             return c
-    raise Exception("Crossing not found")
+    raise ValueError("crossing not found")
+
 
-def analogous_crossing_strand(link,cs):
+def analogous_crossing_strand(link, cs):
     """
     Get a crossing in link with the same label as cs
     """
-    return crossing_strand_from_name(link,cslabel(cs))
+    return crossing_strand_from_name(link, cslabel(cs))
+
 
 def cut_strand(link, cs):
     """
     Cut a link along a strand to get a tangle with 1 strand
     """
     link_copy = link.copy()
-    cs_copy = crossing_strand_from_name(link_copy,cslabel(cs))
+    cs_copy = crossing_strand_from_name(link_copy, cslabel(cs))
     op = cs_copy.opposite()
     cs_copy.crossing.adjacent[cs_copy.strand_index] = None
     op.crossing.adjacent[op.strand_index] = None
-    T = spherogram.Tangle(1, link_copy.crossings, [(cs_copy.crossing,cs_copy.strand_index),(op.crossing,op.strand_index)])
-    return T
+    return spherogram.Tangle(1, link_copy.crossings,
+                             [(cs_copy.crossing, cs_copy.strand_index),
+                              (op.crossing, op.strand_index)])
 
 
-def link_isosig(link, root = None, over_or_under = False ):
+def link_isosig(link, root=None, over_or_under=False):
     """
     A list of data which encodes a planar isotopy class of links instead of
     tangles.  This is just the minimal isosig gotten by cutting all possible
     strands to get a tangle with 1 strand.
     """
-    isosigs = [cut_strand(link,cs).isosig(root,over_or_under) for cs in link.crossing_strands()]
-    return min(isosigs)
+    return min(cut_strand(link, cs).isosig(root, over_or_under)
+               for cs in link.crossing_strands())
```

### Comparing `spherogram-2.1/spherogram_src/links/random_links.py` & `spherogram-2.2/spherogram_src/links/random_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,106 +4,105 @@
 Code written as part of a 2013 Illinois Geometry Lab project by
 
 Nathan Dunfield, Alexander Ehrenberg, Shiladitya Bhattacharyya, and Dongming Lei
 
 Details to hopefully appear in some paper or other.  I wouldn't hold
 your breath, though.
 """
-
 import random
 from .. import graphs
 from . import links, twist
 from spherogram.planarmap import random_map as raw_random_map
 
 
 class LinkGenerationError(Exception):
     def __init__(self, num_tries):
         message = "Didn't generate requested link after %d tries." % num_tries
         Exception.__init__(self, message)
 
+
 def random_map(num_verts, edge_conn_param=4,
                num_link_comps=0, max_tries=100):
     """
     Returns a dictionary of endpoints of edges in the form:
 
     (signed edge) -> (vertex, position)
     """
     if isinstance(num_verts, list):
         data = num_verts
     else:
         data = raw_random_map(num_verts, edge_conn_param,
                               num_link_comps, max_tries)
         if data is None:
             raise LinkGenerationError(max_tries)
-        
 
     vertex_adjacencies = []
     for vertex, adjacencies in data:
         if random.randrange(2):
             adjacencies = adjacencies[1:] + adjacencies[:1]
         vertex_adjacencies.append(adjacencies)
 
     edge_adjacencies = dict()
     for v, edges in enumerate(vertex_adjacencies):
         for i, edge in enumerate(edges):
             edge_adjacencies[edge] = (v, i)
     return edge_adjacencies
-        
+
+
 def map_to_link(map):
     num_edges = len(map) // 2
-    crossings = [links.Crossing() for i in range(num_edges//2)]
-    for e in range(1, num_edges+1):
-        (a, i), (b,j) = map[e], map[-e]
+    crossings = [links.Crossing() for i in range(num_edges // 2)]
+    for e in range(1, num_edges + 1):
+        (a, i), (b, j) = map[e], map[-e]
         crossings[a][i] = crossings[b][j]
-    ans = links.Link(crossings, check_planarity=False)
-    return ans
+    return links.Link(crossings, check_planarity=False)
+
 
 def num_self_crossings(component):
     comp_set = set(component)
-    return len([ce for ce in component if ce.other() in comp_set])
-    
+    return len([1 for ce in component if ce.other() in comp_set])
+
+
 def longest_components(link, num_components):
     components = link.link_components
     self_crosses = [(num_self_crossings(comp), i)
                     for i, comp in enumerate(components)]
     self_crosses.sort(reverse=True)
     return [components[x[1]] for x in self_crosses[:num_components]]
 
+
 def simplified_prime_pieces(link, simplify_fun):
-    ans = []
     cur = link.deconnect_sum(True)
-    while len(cur):
+    while cur:
         L = cur.pop()
         if simplify_fun(L):
             cur += L.deconnect_sum(True)
         else:
-            ans.append(L)
-    return ans
+            yield L
+
 
 def largest_prime_piece(link, simplify_fun):
     pieces = simplified_prime_pieces(link, simplify_fun)
-    if len(pieces) == 0:
-        return links.Link([])
-    return max(pieces, key=lambda L:len(L.crossings))
+    return max(pieces, key=lambda L: len(L.crossings), default=links.Link([]))
 
 
 def random_link(crossings,
-                num_components = 'any', 
-                initial_map_gives_link = False,
-                alternating = False,
-                consistent_twist_regions = False,
-                simplify = 'basic',
-                prime_decomposition = True,
-                return_all_pieces = False, 
+                num_components='any',
+                initial_map_gives_link=False,
+                alternating=False,
+                consistent_twist_regions=False,
+                simplify='basic',
+                prime_decomposition=True,
+                return_all_pieces=False,
                 max_tries=100):
     """
     Generates a random link from a model that starts with a random
     4-valent planar graph sampled with the uniform distribution by
     Schaeffer's `PlanarMap program.
-    <http://www.lix.polytechnique.fr/~schaeffe/PagesWeb/PlanarMap/index-en.html>`_ 
+    <http://www.lix.polytechnique.fr/~schaeffe/PagesWeb/PlanarMap/index-en.html>`_
 
     The ``crossings`` argument specifies the number of vertices of the
     initial planar graph G; the number of crossing in the returned knot
     will typically be less. The meanings of the optional arguments are as
     follows:
 
     1. ``num_components``: The number of components of the returned link.
@@ -151,49 +150,47 @@
        Warning: If ``prime_decomposition=True`` and
        ``return_all_pieces=False``, then the link returned may have
        fewer components than requested.  This is because a prime piece
        can have fewer components than the link as a whole.
 
 
     Some examples:
-    
+
     >>> K = random_link(25, num_components=1, initial_map_gives_link=True, alternating=True)
     >>> K
     <Link: 1 comp; 25 cross>
 
     >>> L= random_link(30, consistent_twist_regions=True, simplify = 'global')
     >>> isinstance(random_link(30, return_all_pieces=True), list)
     True
     """
-
     # This means no trivial loops.  PlanarMap accepts 6, which means
-    # no bigons, but this is unbearably slow.  
+    # no bigons, but this is unbearably slow.
     edge_conn_param = 4
 
-    # Generate the initial link    
+    # Generate the initial link
     if num_components == 'any':
         plane_map = random_map(crossings, edge_conn_param)
         link = map_to_link(plane_map)
     elif initial_map_gives_link:
         plane_map = random_map(crossings, edge_conn_param,
                                num_components, max_tries)
         link = map_to_link(plane_map)
     else:
         for i in range(max_tries):
             plane_map = random_map(crossings, edge_conn_param)
             link = map_to_link(plane_map)
             if len(link.link_components) >= num_components:
                 break
-        
+
         comps = longest_components(link, num_components)
         link = link.sublink(comps)
         if len(link.link_components) != num_components:
             raise LinkGenerationError(max_tries)
 
-
     # Adjust the currently random crossings to match the request
 
     if alternating:
         link = link.alternating()
         return link
 
     if consistent_twist_regions:
@@ -203,30 +200,29 @@
 
     def simplify_func(link):
         if isinstance(simplify, dict):
             return link.simplify(**simplify)
         elif isinstance(simplify, str):
             return link.simplify(mode=simplify)
         return False
-            
+
     simplify_func(link)
-            
-    # Pull into "prime" pieces, if requested.  
-    
+
+    # Pull into "prime" pieces, if requested.
+
     if prime_decomposition:
         if return_all_pieces:
-            return simplified_prime_pieces(link, simplify_func)
+            return list(simplified_prime_pieces(link, simplify_func))
         else:
             return largest_prime_piece(link, simplify_func)
     else:
-        return link 
+        return link
 
-#def random_knot(crossings, **kwargs):
-#    return random_link(crossings, num_components=1, **kwargs)
-#
-#def new_random_knot(crossings, prime_decomposition=True):
-#    return random_knot(crossings, edge_conn_param=4,
-#                initial_map_gives_knot=True, 
-#                return_all_pieces=False, 
-#                prime_decomposition=prime_decomposition,
-#                consistent_twist_regions=True)
+# def random_knot(crossings, **kwargs):
+#     return random_link(crossings, num_components=1, **kwargs)
 
+# def new_random_knot(crossings, prime_decomposition=True):
+#     return random_knot(crossings, edge_conn_param=4,
+#                 initial_map_gives_knot=True,
+#                 return_all_pieces=False,
+#                 prime_decomposition=prime_decomposition,
+#                 consistent_twist_regions=True)
```

### Comparing `spherogram-2.1/spherogram_src/links/seifert.py` & `spherogram-2.2/spherogram_src/links/seifert.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 
     Uses the algorithm described in:
 
     J. Collins, "An algorithm for computing the Seifert matrix of a link
     from a braid representation." (2007).
     """
     arrows = braid_arrows(link)
-    strands = set([x[1] for x in arrows])
+    strands = set(x[1] for x in arrows)
     grouped_by_strand = [[x for x in arrows if x[1] == strand]
                          for strand in strands]
     hom_gens = [[(group[i][0], group[i + 1][0], group[i][2], group[i + 1][2])
                  for i in range(len(group) - 1)] for group in grouped_by_strand]
     num_gens = sum(map(len, hom_gens))
     matrix = [[0] * num_gens for i in range(num_gens)]
     entries = [(i, j) for i, hgi in enumerate(hom_gens)
```

### Comparing `spherogram-2.1/spherogram_src/links/simplify.py` & `spherogram-2.2/spherogram_src/links/simplify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Simplifying link diagrams.
 
 Important notes:
 
 * The link diagram is modified in place.  All the relevant parts of the
-data structure are updated at each step.
+  data structure are updated at each step.
 
 * Unknot components which are also unlinked may be silently discarded.
 """
 
 from .links import Link, Strand, Crossing, CrossingStrand
 from .ordered_set import OrderedSet
 from .. import graphs
@@ -19,42 +19,43 @@
 
 def remove_crossings(link, eliminate):
     """
     Deletes the given crossings. Assumes that they have already been
     disconnected from the rest of the link, so this just updates
     link.crossings and link.link_components.
     """
+
     if len(eliminate):
         for C in eliminate:
             link.crossings.remove(C)
         new_components = []
         for component in link.link_components:
             for C in eliminate:
                 for cep in C.entry_points():
                     try:
                         component.remove(cep)
                     except ValueError:
                         pass
             if len(component):
                 new_components.append(component)
-        components_removed = len(link.link_components)-len(new_components)
+        components_removed = len(link.link_components) - len(new_components)
         link.unlinked_unknot_components += components_removed
         link.link_components = new_components
 
 
 def reidemeister_I(link, C):
     """
     Does a type-1 simplification on the given crossing C if possible.
 
     Returns the pair: {crossings eliminated}, {crossings changed}
     """
     elim, changed = set(), set()
     for i in range(4):
-        if C.adjacent[i] == (C, (i+1)%4):
-            (A, a), (B, b) = C.adjacent[i+2], C.adjacent[i+3]
+        if C.adjacent[i] == (C, (i + 1) % 4):
+            (A, a), (B, b) = C.adjacent[i + 2], C.adjacent[i + 3]
             elim = set([C])
             if C != A:
                 A[a] = B[b]
                 changed = set([A, B])
 
     remove_crossings(link, elim)
     return elim, changed
@@ -66,63 +67,73 @@
     possible.
 
     Returns the pair: {crossings eliminated}, {crossings changed}
     """
     eliminated, changed = reidemeister_I(link, A)
     if not eliminated:
         for a in range(4):
-            (B, b), (C, c) = A.adjacent[a], A.adjacent[a+1]
-            if B == C and (b-1) % 4 == c and (a+b) % 2 == 0:
+            (B, b), (C, c) = A.adjacent[a], A.adjacent[a + 1]
+            if B == C and (b - 1) % 4 == c and (a + b) % 2 == 0:
                 eliminated, changed = reidemeister_I(link, B)
                 if eliminated:
                     break
                 else:
-                    W, w = A.adjacent[a+2]
-                    X, x = A.adjacent[a+3]
-                    Y, y = B.adjacent[b+1]
-                    Z, z = B.adjacent[b+2]
+                    W, w = A.adjacent[a + 2]
+                    X, x = A.adjacent[a + 3]
+                    Y, y = B.adjacent[b + 1]
+                    Z, z = B.adjacent[b + 2]
                     eliminated = set([A, B])
                     if W != B:
                         W[w] = Z[z]
                         changed.update(set([W, Z]))
                     if X != B:
                         X[x] = Y[y]
                         changed.update(set([X, Y]))
                     remove_crossings(link, eliminated)
                     break
 
     return eliminated, changed
 
-def basic_simplify(link):
+
+def basic_simplify(link, build_components=True, to_visit=None,
+                   force_build_components=False):
     """
     Do Reidemeister I and II moves until none are possible.
     """
-    to_visit, eliminated = set(link.crossings), set()
+    if to_visit is None:
+        to_visit = set(link.crossings)
+    eliminated = set()
     while to_visit:
         crossing = to_visit.pop()
         elim, changed = reidemeister_I_and_II(link, crossing)
         assert not elim.intersection(changed)
         eliminated.update(elim)
         to_visit.difference_update(elim)
         to_visit.update(changed)
 
     success = len(eliminated) > 0
 
     # Redo the strand labels (used for DT codes)
-    if success:
+    if (success and build_components) or force_build_components:
         component_starts = []
         for component in link.link_components:
-            a, b = component[:2]
+            assert len(component) > 0
+            if len(component) > 1:
+                a, b = component[:2]
+            else:
+                a = component[0]
+                b = a.next()
             if a.strand_label() % 2 == 0:
                 component_starts.append(a)
             else:
                 component_starts.append(b)
         link._build_components(component_starts)
     return success
 
+
 def possible_type_III_moves(link):
     """
     Returns all triples of crossings where a type III move is possible.
 
     In this example, one type III move is forbidden since a crossing
     repeats twice.
 
@@ -130,43 +141,47 @@
     >>> len(possible_type_III_moves(L))
     1
     """
     ans = []
     for face in link.faces():
         if len(face) == 3:
             if sum(ce.strand_index % 2 for ce in face) in [1, 2]:
-                while(face[1][1]% 2 != 0 or face[2][1]% 2 != 1):    # renumber face_list
+                while(face[1][1] % 2 != 0 or face[2][1] % 2 != 1):    # renumber face_list
                     face = [face[1], face[2], face[0]]
-                if len(set([e.crossing for e in face])) == 3:  # No repeated crossings
+                if len(set(e.crossing for e in face)) == 3:  # No repeated crossings
                     ans.append(face)
     return ans
 
+
 def insert_strand(X, x):
     Y, y = X.adjacent[x]
     S = Strand()
     S[0], S[1] = X[x], Y[y]
     return S
 
+
 def reidemeister_III(link, triple):
     """
     Performs the given type III move.  Modifies the given link but doesn't
     update its lists of link components.
     """
     A, B, C = [t.crossing for t in triple]
-    a, b, c =  [t.strand_index for t in triple]
+    a, b, c = [t.strand_index for t in triple]
     # We insert Strands around the border of the triple to make the code more
     # transparent and eliminate some special cases.
-    old_border =  [(C, c-1), (C, c-2), (A, a-1), (A, a-2), (B, b-1), (B, b-2)]
+    old_border = [(C, c - 1), (C, c - 2), (A, a - 1),
+                  (A, a - 2), (B, b - 1), (B, b - 2)]
     border_strands = [insert_strand(*P) for P in old_border]
-    new_boarder = [(A,a), (B, b+1), (B, b), (C, c+1), (C, c), (A, a+1)]
-    for i, (X,x) in enumerate(new_boarder):
+    new_boarder = [(A, a), (B, b + 1), (B, b), (C, c + 1), (C, c), (A, a + 1)]
+    for i, (X, x) in enumerate(new_boarder):
         X[x] = border_strands[i][0]
-    A[a-1], B[b-1], C[c-1] = B[b+2], C[c+2], A[a+2]
+    A[a - 1], B[b - 1], C[c - 1] = B[b + 2], C[c + 2], A[a + 2]
     [S.fuse() for S in border_strands]
 
+
 def simplify_via_level_type_III(link, max_consecutive_failures=100):
     """
     Applies a series of type III moves to the link, simplifying it via type
     I and II moves whenever possible.
     """
     failures, success = 0, False
     if basic_simplify(link):
@@ -181,29 +196,32 @@
             success = True
         else:
             failures += 1
 
     link._build_components()
     return success
 
+
 def common_element(X, Y):
-    return list(set(X) & set(Y))[0]
+    return next(iter(set(X) & set(Y)))
+
 
 class Face(tuple):
     """
     A complementary region of the link diagram.
     """
     def __new__(cls, edges, label=None):
         ans = tuple.__new__(cls, edges)
         ans.label = label
         return ans
 
     def __repr__(self):
         return "<F%d>" % self.label
 
+
 class DualGraphOfFaces(graphs.Graph):
     """
     The dual graph to a link diagram D, whose vertices correspond to
     complementary regions (faces) of D and whose edges are dual to the
     edges of D.
     """
     def __init__(self, link):
@@ -215,35 +233,35 @@
                 to_face[edge] = face
 
         for edge, face in to_face.items():
             neighbor = to_face[edge.opposite()]
             if face.label < neighbor.label:
                 dual_edge = self.add_edge(face, neighbor)
                 dual_edge.interface = (edge, edge.opposite())
-                dual_edge.label= len(self.edges) - 1
+                dual_edge.label = len(self.edges) - 1
 
-        #assert self.is_planar()
+        # assert self.is_planar()
 
     def two_cycles(self):
         """
-        Finds all two cycles and returns them as a pair of CrossingStrands which
-        are dual to the edges in the cycle.  The crossing strands are
+        Find all two cycles and yield them as a pair of CrossingStrands which
+        are dual to the edges in the cycle.
+
+        The crossing strands are
         oriented consistently with respect to one of the faces which a
         vertex for the cycle.
         """
-        cycles = []
         for face0 in self.vertices:
             for dual_edge0 in self.incident(face0):
                 face1 = dual_edge0(face0)
                 if face0.label < face1.label:
                     for dual_edge1 in self.incident(face1):
                         if dual_edge0.label < dual_edge1.label and dual_edge1(face1) == face0:
-                            cycles.append( (common_element(face0, dual_edge0.interface),
-                                            common_element(face0, dual_edge1.interface)))
-        return cycles
+                            yield (common_element(face0, dual_edge0.interface),
+                                   common_element(face0, dual_edge1.interface))
 
 
 def dual_graph_as_nx(link):
     corners = OrderedSet([CrossingStrand(c, i)
                           for c in link.crossings for i in range(4)])
     faces = []
     to_face_index = dict()
@@ -259,22 +277,22 @@
                 break
             else:
                 to_face_index[next] = count
                 corners.remove(next)
                 face.append(next)
 
     G = nx.Graph()
-    to_face = {edge:faces[f] for edge, f in to_face_index.items()}
+    to_face = {edge: faces[f] for edge, f in to_face_index.items()}
 
     for edge, face in to_face.items():
         opp_edge = edge.opposite()
         neighbor = to_face[opp_edge]
         if face.label < neighbor.label:
             G.add_edge(face.label, neighbor.label,
-                       interface={face.label:edge, neighbor.label:opp_edge})
+                       interface={face.label: edge, neighbor.label: opp_edge})
 
     G.edge_to_face = to_face_index
     return G
 
 
 def deconnect_sum(link):
     """
@@ -286,14 +304,15 @@
         C, c = cs1.opposite()
         D, d = cs1
         A[a] = D[d]
         B[b] = C[c]
     link._build_components()
     return link.split_link_diagram(destroy_original=True)
 
+
 def dual_edges(overstrand, graph):
     """
     Find the set of crossings and edges of the dual graph encountered
     by moving along the link starting at startcep for length crossings.
     Also returns the next crossing entry point immediately after.
     """
 
@@ -307,59 +326,73 @@
     endpoint = overstrand[-1].next()
     final_f1 = graph.edge_to_face[endpoint]
     final_f2 = graph.edge_to_face[endpoint.opposite()]
     edges_crossed.append((final_f1, final_f2))
 
     return edges_crossed
 
+
 def extend_strand_forward(kind, strand, end_cep):
     """
     Extend the strand by adding on end_cep and what comes after it
     until you hit a crossing which is not of the given kind
     (over/under).
     """
     cep = end_cep.next()
     strand.append(end_cep)
+    start_cep = strand[0].previous()
     while getattr(cep, 'is_' + kind + '_crossing')():
+        if cep.next() == start_cep:  # prevents extending too far
+            break
         strand.append(cep)
         cep = cep.next()
         if cep == strand[0]:
             break
 
+
 def extend_strand_backward(kind, strand, start_cep):
     """
     Extend the strand by adding on end_cep and what comes before it
     until you hit a crossing which is not of the given kind
     (over/under).
     """
-
     cep = start_cep.previous()
     strand.insert(0, start_cep)
+    end_cep = strand[-1].next()
     while getattr(cep, 'is_' + kind + '_crossing')():
-        strand.insert(0,cep)
+        if cep.previous() == end_cep:  # prevents extending too far
+            break
+        strand.insert(0, cep)
         cep = cep.previous()
         if cep == strand[-1]:
             break
 
+
 def pickup_strand(link, dual_graph, kind, strand):
     """
-    Simplify the given (over/under)crossing strand by erasing from the diagram and
-    then finding a path that minimizes the number of edges it has to cross
-    over to connect the same endpoints. Returns number of crossings removed.
+    Simplify the given (over/under)crossing strand by erasing it from
+    the diagram and then finding a path that minimizes the number of
+    edges it has to cross over to connect the same endpoints. Returns
+    number of crossings removed.
     """
+    init_link_cross_count = len(link.crossings)
     G = dual_graph
     startcep = strand[0].previous()
 
     if startcep == strand[-1]:
         # Totally overcrossing loop, must be totally unlinked and
         # unknotted
-        remove_strand(strand)
+        remove_strand(link, strand)
+        return len(strand)
+    if startcep == strand[-1].next() and startcep.other() in strand:
+        # We have a figure-8 curve with a single crossing in front
+        # of the rest of the components.
+        remove_strand(link, [startcep] + strand)
         return len(strand)
-    length = len(strand)
-    crossing_set = set([cep.crossing for cep in strand])
+    crossing_set = set(cep.crossing for cep in strand)
     endpoint = strand[-1].next()
 
     if endpoint.crossing in crossing_set:
         # Strand crosses itself underneath
         extend_strand_forward(kind, strand, endpoint)
         return pickup_strand(link, G, kind, strand)
     if startcep.crossing in crossing_set:
@@ -379,34 +412,46 @@
     new_len = sum(G[f0][f1]['weight'] for f0, f1 in zip(path, path[1:]))
     crossingsremoved = len(crossing_set) - new_len
     if crossingsremoved == 0:
         return 0
 
     # creating a new list of crossings from which to rebuild the link,
     # remove old overcross
-    newcrossings = link.crossings
+    newcrossings = []
 
-    cr = remove_strand(link, strand)
+    removed = remove_strand(link, strand)
     loose_end = startcep.rotate(2)
 
     # find new sequence of overcrossings to create
-    for i in range(len(path)-1):
+    for i in range(len(path) - 1):
         label = 'new%d' % i
-        f1, f2 = path[i:i+2]
+        f1, f2 = path[i:i + 2]
         edge = G[f1][f2]
         if edge['weight'] > 0:
             cep_to_cross = G[f1][f2]['interface'][f1]
             new_crossing, loose_end = cross(link, cep_to_cross, kind, loose_end, label)
             newcrossings.append(new_crossing)
 
     ec, ecep = endpoint.crossing, endpoint.strand_index
     ec[ecep] = loose_end
-    link._rebuild()
 
-    return crossingsremoved
+    link.crossings.extend(newcrossings)
+    active = set()
+    for C in removed:
+        for i in range(4):
+            D = C.adjacent[i][0]
+            if D not in removed:
+                active.add(D)
+
+    active.update(newcrossings)
+    basic_simplify(link, force_build_components=True, to_visit=active)
+
+    final_cross_removed = init_link_cross_count - len(link.crossings)
+    assert final_cross_removed >= crossingsremoved
+    return final_cross_removed
 
 
 def strand_pickup(link, kind):
     """
     Simplifies link by optimizing the path of the longest sequence of overcrossings.
     Returns a new link and the number of crossings removed.
     """
@@ -427,74 +472,84 @@
     """
     Delete an overstrand or understrand from a link.  If the strand is
     a loop, it doesn't leave any loose strands and removes the
     loop. Otherwise, there will be two strands left in the link not
     attached to anything.  This function assumes that the start and
     end of the strand are not places where strands crosses itself.
     """
-    #only add bridge strands for the places where the strand doesn't cross itself
+    # only add bridge strands for the places where the strand doesn't cross itself
     crossings_seen = [s.crossing for s in strand]
     crossing_set = set()
     for c in crossings_seen:
         if c in crossing_set:
             crossing_set.remove(c)
         else:
             crossing_set.add(c)
 
     start_cep = strand[0].previous()
     end_cep = strand[-1].next()
-    bridge_strands = dict([(c, Strand('strand'+str(c.label))) for c in crossing_set])
+    bridge_strands = {c: Strand('strand' + str(c.label)) for c in crossing_set}
     for cep in strand:
         c = cep.crossing
         if c not in crossing_set:
             continue
-        strand_index = cep.strand_index
         right_cs = cep.rotate(1).opposite()
         left_cs = cep.rotate(3).opposite()
         if right_cs.crossing in crossing_set:
             signs_equal = (c.sign == right_cs.crossing.sign)
             bridge_strands[c][0] = bridge_strands[right_cs.crossing][signs_equal]
         else:
             bridge_strands[c][0] = right_cs.crossing[right_cs.strand_index]
         if left_cs.crossing in crossing_set:
             signs_equal = (c.sign == left_cs.crossing.sign)
-            bridge_strands[c][1] = bridge_strands[left_cs.crossing][1-signs_equal]
+            bridge_strands[c][1] = bridge_strands[left_cs.crossing][1 - signs_equal]
         else:
             bridge_strands[c][1] = left_cs.crossing[left_cs.strand_index]
-    remove_crossings(link,set(crossings_seen))
+    remove_crossings(link, set(crossings_seen))
 
     for s in bridge_strands.values():
         s.fuse()
 
-    return len(crossing_set)
+    return set(crossings_seen)
 
 
 def cross(link, cep_to_cross, kind, loose_end, label):
     """
     Create a new (over/under) crossing along the edge defined by
     cep_to_cross and its opposite, and attach one side to a given
     position loose_end.
     """
-    if kind == 'over':
-        a, b, c, d = 0, 1, 2, 3
-    else:
-        assert kind == 'under'
-        a, b, c, d = 3, 0, 1, 2
 
-    new_crossing = Crossing(label)
-    new_crossing[b] = loose_end
     ic = cep_to_cross
     ico = ic.opposite()
     while ic.crossing not in link.crossings:
         ic = ic.next()
     while ico.crossing not in link.crossings:
         ico = ico.next()
+    left_to_right = not ic.crossing.is_incoming(ic.strand_index)
+
+    if kind == 'over':
+        if left_to_right:
+            a, b, c, d = 2, 3, 0, 1
+        else:
+            a, b, c, d = 0, 1, 2, 3
+    else:
+        assert kind == 'under'
+        a, b, c, d = 3, 0, 1, 2
+
+    new_crossing = Crossing(label)
+    new_crossing[b] = loose_end
     new_crossing[c] = ic
     new_crossing[a] = ico
-
+    new_crossing.make_tail(b)
+    if left_to_right:
+        new_crossing.make_tail(c)
+    else:
+        new_crossing.make_tail(a)
+    new_crossing.orient()
     return new_crossing, new_crossing.crossing_strands()[d]
 
 
 def over_or_under_strands(link, kind):
     """
     Returns a list of the sequences of (over/under) crossings (which
     are lists of CrossingEntryPoints), sorted in descending order
@@ -517,22 +572,25 @@
             if forward_cep.crossing == start_crossing:
                 is_loop = True
                 break
             forward_strand.append(forward_cep)
             forward_cep = forward_cep.next()
         backwards_strand = []
         backwards_cep = cep.previous()
-        if not is_loop:
+        if is_loop:
+            strand = forward_strand
+        else:
             while criteria(backwards_cep):
                 backwards_strand.append(backwards_cep)
                 backwards_cep = backwards_cep.previous()
             strand = backwards_strand[::-1]
             strand.extend(forward_strand)
-            strands.append(strand)
-            ceps.difference_update(strand)
+
+        strands.append(strand)
+        ceps.difference_update(strand)
 
     return sorted(strands, key=len, reverse=True)
 
 
 def randomize_within_lengths(items):
     by_lens = collections.defaultdict(list)
     for item in items:
@@ -540,15 +598,15 @@
     ans = []
     for length, some_items in sorted(by_lens.items(), reverse=True):
         random.shuffle(some_items)
         ans += some_items
     return ans
 
 
-def reverse_type_I(link,crossing_strand,label,hand,rebuild=False):
+def reverse_type_I(link, crossing_strand, label, hand, rebuild=False):
     """
     Add a loop on the strand at crossing_strand with a given label and
     'handedness' hand (twisting left or right).
     """
     D = Crossing(label)
     link.crossings.append(D)
     cs1 = crossing_strand
@@ -563,26 +621,24 @@
     else:
         D[2] = D[3]
         cs1ec, cs1cep = cs1.crossing, cs1.strand_index
         D[0] = cs1ec[cs1cep]
         cs2ec, cs2cep = cs2.crossing, cs2.strand_index
         D[1] = cs2ec[cs2cep]
     if rebuild:
-        comp_sts = [comp[0] for comp in link.link_components]
-        link._rebuild(component_starts=comp_sts)
+        link._rebuild(same_components_and_orientations=True)
 
 
-def random_reverse_type_I(link,label,rebuild=False):
+def random_reverse_type_I(link, label, rebuild=False):
     """
     Randomly adds a loop in a strand, adding one crossing with given label
     """
-
     cs = random.choice(link.crossing_strands())
-    lr = random.choice(['left','right'])
-    reverse_type_I(link,cs,label,lr,rebuild=rebuild)
+    lr = random.choice(['left', 'right'])
+    reverse_type_I(link, cs, label, lr, rebuild=rebuild)
 
 
 def reverse_type_II(link, c, d, label1, label2, rebuild=False):
     """
     Cross two strands defined by two crossing strands c and d in the same face.
     """
 
@@ -595,118 +651,118 @@
     new1[0], new1[1] = dop_cross[dop_ep], c_cross[c_ep]
     new2[1], new2[2] = cop_cross[cop_ep], d_cross[d_ep]
 
     link.crossings.append(new1)
     link.crossings.append(new2)
 
     if rebuild:
-        comp_sts = [comp[0] for comp in link.link_components]
-        link._rebuild(component_starts = comp_sts)
+        link._rebuild(same_components_and_orientations=True)
 
 
 def random_reverse_type_II(link, label1, label2, rebuild=False):
     """
     Randomly crosses two strands, adding two crossings, with labels
     label1 and label2
     """
 
     faces = link.faces()
     while True:
         face = random.choice(faces)
-        if len(face)>1:
+        if len(face) > 1:
             break
-    c, d = random.sample(face,2)
-    reverse_type_II(link,c,d,label1,label2,rebuild=rebuild)
+    c, d = random.sample(face, 2)
+    reverse_type_II(link, c, d, label1, label2, rebuild=rebuild)
 
-def random_reverse_move(link,t,n):
+
+def random_reverse_move(link, t, n):
     """
     Performs a crossing increasing move of type t, where t is 1, 2, or 3
     n is for labeling the new crossings
     """
     if t == 1:
-        random_reverse_type_I(link,'new'+str(n))
+        random_reverse_type_I(link, 'new' + str(n))
     elif t == 2:
-        random_reverse_type_II(link,'new'+str(n),'new'+str(n+1))
+        random_reverse_type_II(link, 'new' + str(n), 'new' + str(n + 1))
     else:
         poss_moves = possible_type_III_moves(link)
         if len(poss_moves) != 0:
             reidemeister_III(link, random.choice(poss_moves))
 
 
-def backtrack(link, num_steps = 10, prob_type_1 = .3, prob_type_2 = .3):
+def backtrack(link, num_steps=10, prob_type_1=.3, prob_type_2=.3):
     """
     Randomly perform a series of Reidemeister moves which increase or preserve
     the number of crossings of a link diagram, with the number of such moves
     num_steps.  Can set the probability of type I or type II moves, so the
     remainder is then the probability of type III. Use the method backtrack
     in the Link class.
     """
     if len(link) == 0:
         return
 
     n = 0
     if prob_type_1 + prob_type_2 > 1:
-        raise Exception("Probabilities add to more than 1")
+        raise ValueError("Probabilities add to more than 1")
     p1 = prob_type_1
     p2 = p1 + prob_type_2
     for i in range(num_steps):
-        x = random.uniform(0,1)
+        x = random.uniform(0, 1)
         if x < p1:
             t = 1
         elif p1 < x < p2:
             t = 2
         else:
             t = 3
 
-        n += t%3
+        n += t % 3
 
-        random_reverse_move(link,t,n)
+        random_reverse_move(link, t, n)
 
     link._rebuild(same_components_and_orientations=True)
 
 
 def clear_orientations(link):
     """
     Resets the orientations on the crossings of a link to default values
     """
     link.link_components = None
     for i in link.crossings:
         i.sign = 0
         i.directions.clear()
 
+
 def relabel_crossings(link):
     """
     Relabel the crossings as integers
     """
-    for i,cr in enumerate(link.crossings):
+    for i, cr in enumerate(link.crossings):
         cr.label = str(i)
 
 
 def pickup_simplify(link, type_III=0):
     """
     Optimizes the overcrossings on a diagram, then the undercrossings,
     simplifying in between until the process stabilizes.
     """
-    def intermediate_simplify(a_link):
-        if type_III:
-            simplify_via_level_type_III(a_link, type_III)
-        else:
-            basic_simplify(a_link)
-
     L = link
     init_num_crossings = len(L.crossings)
-    intermediate_simplify(L)
+    if type_III:
+        simplify_via_level_type_III(link, type_III)
+    else:
+        basic_simplify(L, build_components=False)
     stabilized = init_num_crossings == 0
 
     while not stabilized:
         old_cross = len(L.crossings)
         strand_pickup(L, 'over')
-        intermediate_simplify(L)
+        if type_III:
+            simplify_via_level_type_III(link, type_III)
 
         strand_pickup(L, 'under')
-        intermediate_simplify(L)
-
+        if type_III:
+            simplify_via_level_type_III(link, type_III)
 
         new_cross = len(L.crossings)
         stabilized = new_cross == 0 or new_cross == old_cross
 
+    L._rebuild()
     return len(L.crossings) != init_num_crossings
```

### Comparing `spherogram-2.1/spherogram_src/links/test/__init__.py` & `spherogram-2.2/spherogram_src/links/test/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,222 +3,223 @@
 import doctest
 import sys
 from random import randrange
 from . import test_montesinos
 from ...sage_helper import _within_sage
 if _within_sage:
     from sage.rings.polynomial.laurent_polynomial_ring import LaurentPolynomialRing
-    from sage.all import QQ
-    
+    from sage.rings.rational_field import QQ
+
+
 class TestLinkFunctions(unittest.TestCase):
-    
+
     def setUp(self):
         # Trefoil
         a = spherogram.Crossing('a')
         b = spherogram.Crossing('b')
         c = spherogram.Crossing('c')
         a[2] = b[1]
         b[3] = c[0]
         c[2] = a[1]
         a[3] = b[0]
         b[2] = c[1]
         c[3] = a[0]
-        self.Tref = spherogram.Link([a,b,c])
+        self.Tref = spherogram.Link([a, b, c])
 
         self.K3_1 = spherogram.Link('3_1')
         self.K7_2 = spherogram.Link('7_2')
         self.K8_3 = spherogram.Link('8_3')
         self.K8_13 = spherogram.Link('8_13')
 
         # Hopf Link
-        a = spherogram.Crossing('a') 
-        b = spherogram.Crossing('b') 
-        a[0]=b[1] 
-        a[1]=b[0] 
-        a[2]=b[3] 
-        a[3]=b[2] 
-        self.L2a1 = spherogram.Link([a,b])
-
-        #Borromean Link (3) 
-        a = spherogram.Crossing('a') 
-        b = spherogram.Crossing('b') 
-        c = spherogram.Crossing('c') 
-        d = spherogram.Crossing('d') 
-        e = spherogram.Crossing('e') 
-        f = spherogram.Crossing('f') 
+        a = spherogram.Crossing('a')
+        b = spherogram.Crossing('b')
+        a[0] = b[1]
+        a[1] = b[0]
+        a[2] = b[3]
+        a[3] = b[2]
+        self.L2a1 = spherogram.Link([a, b])
+
+        # Borromean Link (3)
+        a = spherogram.Crossing('a')
+        b = spherogram.Crossing('b')
+        c = spherogram.Crossing('c')
+        d = spherogram.Crossing('d')
+        e = spherogram.Crossing('e')
+        f = spherogram.Crossing('f')
         a[2] = f[1]
-        a[3] = e[0] 
-        b[1] = a[0] 
-        b[2] = e[3] 
-        c[0] = a[1] 
-        c[1] = b[0] 
-        d[3] = c[2] 
-        d[0] = b[3] 
-        e[2] = d[1] 
-        e[1] = f[0] 
-        f[2] = c[3] 
-        f[3] = d[2] 
-        self.Borr = spherogram.Link([a,b,c,d,e,f])
-        
+        a[3] = e[0]
+        b[1] = a[0]
+        b[2] = e[3]
+        c[0] = a[1]
+        c[1] = b[0]
+        d[3] = c[2]
+        d[0] = b[3]
+        e[2] = d[1]
+        e[1] = f[0]
+        f[2] = c[3]
+        f[3] = d[2]
+        self.Borr = spherogram.Link([a, b, c, d, e, f])
+
         self.L6a2 = spherogram.Link('L6a2')
         self.L6a4 = spherogram.Link('L6a4')
         self.L7a3 = spherogram.Link('L7a3')
         self.L10n1 = spherogram.Link('L10n1')
 
         self.knots = [self.K3_1, self.K7_2, self.K8_3, self.K8_13]
         self.links = [self.L2a1, self.L6a4, self.L6a2, self.L7a3, self.L10n1]
         self.all_links = self.knots + self.links
-               
+
     def random_knot(self):
-        random_index = randrange(0,len(self.knots))
+        random_index = randrange(0, len(self.knots))
         return self.knots[random_index]
 
     def random_link(self):
-        random_index = randrange(0,len(self.links))
+        random_index = randrange(0, len(self.links))
         return self.links[random_index]
 
     def testWrithe(self):
-        self.assertEqual(abs(self.Tref.writhe()),       3)
-        self.assertEqual(abs(self.K3_1.writhe()),       3)
-        self.assertEqual(abs(self.K7_2.writhe()),       7)
-        self.assertEqual(abs(self.K8_3.writhe()),       0)
-        self.assertEqual(abs(self.K8_13.writhe()),      2)
-        self.assertEqual(abs(self.L2a1.writhe()),       2)
-        self.assertEqual(abs(self.L6a2.writhe()),       6)
-        self.assertEqual(abs(self.Borr.writhe()),       0)
-        self.assertEqual(abs(self.L6a4.writhe()),       0)
-        self.assertEqual(abs(self.L7a3.writhe()),       3)
+        self.assertEqual(abs(self.Tref.writhe()), 3)
+        self.assertEqual(abs(self.K3_1.writhe()), 3)
+        self.assertEqual(abs(self.K7_2.writhe()), 7)
+        self.assertEqual(abs(self.K8_3.writhe()), 0)
+        self.assertEqual(abs(self.K8_13.writhe()), 2)
+        self.assertEqual(abs(self.L2a1.writhe()), 2)
+        self.assertEqual(abs(self.L6a2.writhe()), 6)
+        self.assertEqual(abs(self.Borr.writhe()), 0)
+        self.assertEqual(abs(self.L6a4.writhe()), 0)
+        self.assertEqual(abs(self.L7a3.writhe()), 3)
 
     def testLinkingNumber(self):
         for k in self.knots:
-            self.assertEqual(k.linking_number(),           0)
-        self.assertEqual(abs(self.L2a1.linking_number()),  1)
-        self.assertEqual(abs(self.L6a2.linking_number()),  3)
-        self.assertEqual(abs(self.Borr.linking_number()),  0)
-        self.assertEqual(abs(self.L6a4.linking_number()),  0)
-        self.assertEqual(abs(self.L7a3.linking_number()),  0)
+            self.assertEqual(k.linking_number(), 0)
+        self.assertEqual(abs(self.L2a1.linking_number()), 1)
+        self.assertEqual(abs(self.L6a2.linking_number()), 3)
+        self.assertEqual(abs(self.Borr.linking_number()), 0)
+        self.assertEqual(abs(self.L6a4.linking_number()), 0)
+        self.assertEqual(abs(self.L7a3.linking_number()), 0)
 
     def testLinkingMatrix(self):
         A = [[0]]
         B = [[0, -1], [-1, 0]]
         B2 = [[0, 1], [1, 0]]
         C = [[0, -3], [-3, 0]]
         C2 = [[0, 3], [3, 0]]
-        D = [[0,0,0],[0,0,0],[0,0,0]]
+        D = [[0, 0, 0], [0, 0, 0], [0, 0, 0]]
         E = [[0, 0], [0, 0]]
         for k in self.knots:
-            self.assertEqual(k.linking_matrix(),      A)
-        self.assertTrue(self.L2a1.linking_matrix() == B or self.L2a1.linking_matrix() == B2)
-        self.assertTrue(self.L6a2.linking_matrix() == C or self.L6a2.linking_matrix() == C2)
-        self.assertEqual(self.Borr.linking_matrix(),       D)
-        self.assertEqual(self.L6a4.linking_matrix(),       D)
-        self.assertEqual(self.L7a3.linking_matrix(),       E)
+            self.assertEqual(k.linking_matrix(), A)
+        self.assertIn(self.L2a1.linking_matrix(), [B, B2])
+        self.assertIn(self.L6a2.linking_matrix(), [C, C2])
+        self.assertEqual(self.Borr.linking_matrix(), D)
+        self.assertEqual(self.L6a4.linking_matrix(), D)
+        self.assertEqual(self.L7a3.linking_matrix(), E)
 
     def testKnotGroup(self):
         # Correct number of generators? abelian invariants?
         for k in self.all_links:
-            self.assertEqual(len(k.knot_group().generators()),             len(k.crossings))
-            self.assertEqual(k.knot_group().abelian_invariants()[0],       0)
-            self.assertEqual(len(k.knot_group().abelian_invariants()),     len(k.link_components))
-       
+            self.assertEqual(len(k.knot_group().generators()), len(k.crossings))
+            self.assertEqual(k.knot_group().abelian_invariants()[0], 0)
+            self.assertEqual(len(k.knot_group().abelian_invariants()), len(k.link_components))
+
     def testAlexanderPoly(self):
-        from sage.all import var, sqrt
-        L = LaurentPolynomialRing(QQ,'t')
+        from sage.all import SR
+        L = LaurentPolynomialRing(QQ, 't')
         t = L.gen()
-        a = var('a')
-        L3v = LaurentPolynomialRing(QQ,['t1','t2','t3'])
+        a = SR.var('a')
+        L3v = LaurentPolynomialRing(QQ, ['t1', 't2', 't3'])
         t1, t2, t3 = L3v.gens()
         # method = 'wirt'
-        self.assertEqual(self.Tref.alexander_polynomial(),       1 - t + t**2)
-        self.assertEqual(self.K3_1.alexander_polynomial(),       1 - t + t**2)
-        self.assertEqual(self.K7_2.alexander_polynomial(),       3 - 5*t + 3*t**2)
-        self.assertEqual(self.K8_3.alexander_polynomial(),       4 - 9*t + 4*t**2)
-        self.assertEqual(self.K8_13.alexander_polynomial(),      2 - 7*t + 11*t**2 - 7*t**3 + 2*t**4)
-        self.assertEqual(self.L2a1.alexander_polynomial(),       1)
-        self.assertEqual(self.Borr.alexander_polynomial(),       t1*t2*t3 - t1*t2 - t1*t3 - t2*t3 + t1 + t2 + t3 - 1)
-        self.assertEqual(self.L6a4.alexander_polynomial(),       t1*t2*t3 - t1*t2 - t1*t3 - t2*t3 + t1 + t2 + t3 - 1)
+        self.assertEqual(self.Tref.alexander_polynomial(), 1 - t + t**2)
+        self.assertEqual(self.K3_1.alexander_polynomial(), 1 - t + t**2)
+        self.assertEqual(self.K7_2.alexander_polynomial(), 3 - 5*t + 3*t**2)
+        self.assertEqual(self.K8_3.alexander_polynomial(), 4 - 9*t + 4*t**2)
+        self.assertEqual(self.K8_13.alexander_polynomial(), 2 - 7*t + 11*t**2 - 7*t**3 + 2*t**4)
+        self.assertEqual(self.L2a1.alexander_polynomial(), 1)
+        self.assertEqual(self.Borr.alexander_polynomial(), t1*t2*t3 - t1*t2 - t1*t3 - t2*t3 + t1 + t2 + t3 - 1)
+        self.assertEqual(self.L6a4.alexander_polynomial(), t1*t2*t3 - t1*t2 - t1*t3 - t2*t3 + t1 + t2 + t3 - 1)
 
         # method = 'snappy'
         try:
             import snappy
-            self.assertEqual(self.Tref.alexander_polynomial(method='snappy'),       a**2 - a + 1)
+            self.assertEqual(self.Tref.alexander_polynomial(method='snappy'), a**2 - a + 1)
             self.assertEqual(self.K3_1.alexander_polynomial(method='snappy'), a**2 - a + 1)
-            self.assertEqual(self.K7_2.alexander_polynomial(method='snappy'),       3*a**2 - 5*a + 3)
-            self.assertEqual(self.K8_3.alexander_polynomial(method='snappy'),       4*a**2 - 9*a + 4)
-            self.assertEqual(self.K8_13.alexander_polynomial(method='snappy'),      2*a**4 - 7*a**3 + 11*a**2 - 7*a + 2)
+            self.assertEqual(self.K7_2.alexander_polynomial(method='snappy'), 3*a**2 - 5*a + 3)
+            self.assertEqual(self.K8_3.alexander_polynomial(method='snappy'), 4*a**2 - 9*a + 4)
+            self.assertEqual(self.K8_13.alexander_polynomial(method='snappy'), 2*a**4 - 7*a**3 + 11*a**2 - 7*a + 2)
         except ImportError:
             pass
-        
+
     def testConnectedSum(self):
         repeat = 3
         while repeat > 0:
             k1 = self.random_knot()
             k2 = self.random_knot()
             Sum = k1.connected_sum(k2)
-            self.assertEqual(Sum.alexander_polynomial(), k1.alexander_polynomial()*k2.alexander_polynomial())
-            self.assertEqual(Sum.signature(),      k1.signature()+k2.signature())
-            self.assertEqual(Sum.determinant(),    k1.determinant()*k2.determinant())
-            repeat -=1
+            self.assertEqual(Sum.alexander_polynomial(), k1.alexander_polynomial() * k2.alexander_polynomial())
+            self.assertEqual(Sum.signature(), k1.signature() + k2.signature())
+            self.assertEqual(Sum.determinant(), k1.determinant() * k2.determinant())
+            repeat -= 1
 
     def testSignature(self):
-        self.assertEqual(abs(self.Tref.signature()),       2)
-        self.assertEqual(abs(self.K3_1.signature()),       2)
-        self.assertEqual(abs(self.K7_2.signature()),       2)
-        self.assertEqual(abs(self.K8_3.signature()),       0)
-        self.assertEqual(abs(self.K8_13.signature()),      0)
-        self.assertEqual(abs(self.L2a1.signature()),       1)
-        self.assertEqual(abs(self.L6a2.signature()),       3)
-        self.assertEqual(abs(self.Borr.signature()),       0)
-        self.assertEqual(abs(self.L6a4.signature()),       0)
-        self.assertEqual(abs(self.L7a3.signature()),       3)
+        self.assertEqual(abs(self.Tref.signature()), 2)
+        self.assertEqual(abs(self.K3_1.signature()), 2)
+        self.assertEqual(abs(self.K7_2.signature()), 2)
+        self.assertEqual(abs(self.K8_3.signature()), 0)
+        self.assertEqual(abs(self.K8_13.signature()), 0)
+        self.assertEqual(abs(self.L2a1.signature()), 1)
+        self.assertEqual(abs(self.L6a2.signature()), 3)
+        self.assertEqual(abs(self.Borr.signature()), 0)
+        self.assertEqual(abs(self.L6a4.signature()), 0)
+        self.assertEqual(abs(self.L7a3.signature()), 3)
 
     def testCopy(self):
         repeat = 3
         while repeat > 0:
             k1 = self.random_knot()
             k1_prime = k1.copy()
-            self.assertEqual(k1.determinant(),    k1_prime.determinant())
-            self.assertEqual(k1.writhe(),         k1_prime.writhe())
-            self.assertEqual(k1.signature(),      k1_prime.signature())
+            self.assertEqual(k1.determinant(), k1_prime.determinant())
+            self.assertEqual(k1.writhe(), k1_prime.writhe())
+            self.assertEqual(k1.signature(), k1_prime.signature())
             self.assertEqual(k1.alexander_polynomial(), k1_prime.alexander_polynomial())
-            repeat-=1
+            repeat -= 1
 
         repeat = 3
         while repeat > 0:
             k2 = self.random_link()
             k2_prime = k2.copy()
-            self.assertEqual(k2.determinant(),    k2_prime.determinant())
-            self.assertEqual(k2.writhe(),         k2_prime.writhe())
-            self.assertEqual(k2.signature(),      k2_prime.signature())
+            self.assertEqual(k2.determinant(), k2_prime.determinant())
+            self.assertEqual(k2.writhe(), k2_prime.writhe())
+            self.assertEqual(k2.signature(), k2_prime.signature())
             self.assertEqual(k2.alexander_polynomial(), k2_prime.alexander_polynomial())
-            repeat-=1
+            repeat -= 1
 
     def testMirror(self):
         return
         repeat = 3
         while repeat > 0:
             k1 = self.random_knot()
             k1_prime = k1.mirror()
-            self.assertTrue(k1.signature() == -1*k1_prime.signature(), msg="knot signature failed for "+ repr(k1))
-            self.assertTrue(k1.writhe() == -1*k1_prime.writhe(), msg="knot writhe failed for "+repr(k1))
-            repeat-=1
-            
+            self.assertTrue(k1.signature() == -1*k1_prime.signature(), msg="knot signature failed for " + repr(k1))
+            self.assertTrue(k1.writhe() == -1*k1_prime.writhe(), msg="knot writhe failed for " + repr(k1))
+            repeat -= 1
+
         repeat = 3
         while repeat > 0:
             k2 = self.random_link()
             k2_prime = k2.mirror()
             self.assertTrue(k2.signature() == -1*k2_prime.signature(), msg="link signature failed for " + repr(k2))
             self.assertTrue(k2.writhe() == -1*k2_prime.writhe(), msg="link writhe failed for " + repr(k2))
-            repeat-=1
+            repeat -= 1
 
     def testDet(self):
         self.assertEqual(self.K3_1.determinant(),                 3)
         self.assertEqual(self.K3_1.determinant(method='color'),   3)
         self.assertEqual(self.K3_1.determinant(method='goeritz'), 3)
-        
+
         self.assertEqual(self.Tref.determinant(),                 3)
         self.assertEqual(self.Tref.determinant(method='color'),   3)
         self.assertEqual(self.Tref.determinant(method='goeritz'), 3)
 
         self.assertEqual(self.K7_2.determinant(),                 11)
         self.assertEqual(self.K7_2.determinant(method='color'),   11)
         self.assertEqual(self.K7_2.determinant(method='goeritz'), 11)
@@ -252,38 +253,37 @@
         self.assertEqual(self.L7a3.determinant(method='goeritz'), 16)
 
     def testWhiteGraph(self):
         repeat = 3
         while repeat > 0:
             k1 = self.random_knot()
             self.assertTrue(k1.white_graph().is_planar())
-            repeat-=1
+            repeat -= 1
 
         repeat = 3
         while repeat > 0:
             k2 = self.random_link()
             self.assertTrue(k2.white_graph().is_planar())
-            repeat-=1
+            repeat -= 1
 
     def testJonesPolynomial(self):
-        L = LaurentPolynomialRing(QQ,'q')
+        L = LaurentPolynomialRing(QQ, 'q')
         q = L.gen()
         data = [('K3_1', ('q^3 + q - 1', -4)),
                 ('K7_2', ('q^7 - q^6 + 2*q^5 - 2*q^4 + 2*q^3 - q^2 + q - 1', -8)),
                 ('K8_3', ('q^8 - q^7 + 2*q^6 - 3*q^5 + 3*q^4 - 3*q^3 + 2*q^2 - q + 1', -4)),
                 ('K8_13', ('-q^8 + 2*q^7 - 3*q^6 + 5*q^5 - 5*q^4 + 5*q^3 - 4*q^2 + 3*q - 1', -3)),
                 ('L6a2', ('-q^6 + q^5 - 2*q^4 + 2*q^3 - 2*q^2 + q - 1', 1)),
                 ('L6a4', ('-q^6 + 3*q^5 - 2*q^4 + 4*q^3 - 2*q^2 + 3*q - 1', -3)),
                 ('L7a3', ('-q^7 + q^6 - 3*q^5 + 2*q^4 - 3*q^3 + 3*q^2 - 2*q + 1', -7)),
                 ('L10n1', ('q^8 - 2*q^7 + 2*q^6 - 4*q^5 + 3*q^4 - 3*q^3 + 2*q^2 - 2*q + 1', -2))]
         for link_name, (poly, exp) in data:
             link = getattr(self, link_name)
-            self.assertEqual(link.jones_polynomial(new_convention=False), L(poly)*q**exp)
+            self.assertEqual(link.jones_polynomial(new_convention=False),
+                             L(poly) * q**exp)
+
 
 def run():
     test_montesinos.test(15)
     if _within_sage:
         suite = unittest.TestLoader().loadTestsFromTestCase(TestLinkFunctions)
         unittest.TextTestRunner(verbosity=2, stream=sys.stdout).run(suite)
-
-
-
```

### Comparing `spherogram-2.1/spherogram_src/links/test/old_testing_code.py` & `spherogram-2.2/spherogram_src/links/test/old_testing_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,88 @@
+import sys
 from . import links, tangles
+
 Crossing, Link, RationalTangle, IdentityBraid = links.Crossing, links.Link, tangles.RationalTangle, tangles.IdentityBraid
-import os
-import sys
-import re
 
 # ----- Some basic tests, constructing links by hand -------
 
+
 def figure8():
     a, b, c, d = [Crossing(x) for x in 'abcd']
     a[0] = c[1]
     a[1] = d[0]
     a[2] = b[1]
     a[3] = b[0]
     b[2] = d[3]
     b[3] = c[2]
     c[3] = d[2]
     c[0] = d[1]
-    return Link([a,b,c,d])
+    return Link([a, b, c, d])
+
 
 def punct_torus():
     a = Crossing('a')
     a[0] = a[2]
     a[1] = a[3]
     return Link([a], check_planarity=False)
 
+
 def whitehead():
-    a, b, c, d, e =  crossings = [Crossing(x) for x in 'abcde']
+    a, b, c, d, e = crossings = [Crossing(x) for x in 'abcde']
     a[0] = b[3]
     a[1] = d[0]
     a[2] = d[3]
     a[3] = c[0]
     b[0] = c[3]
     b[1] = e[2]
     b[2] = e[1]
     c[1] = d[2]
     c[2] = e[3]
     d[1] = e[0]
     return Link(crossings)
- 
+
+
 def basic_test():
-    K, W, T = figure8(), whitehead(), punct_torus()
-    print( K.is_planar(), W.is_planar(), punct_torus().is_planar() )
-    print( K.PD_code(True) )
-    print( K.DT_code(True) , K.peer_code())
-    print( W.PD_code(True) )
-    print( W.DT_code(True) , K.peer_code())
+    K, W, _ = figure8(), whitehead(), punct_torus()
+    print(K.is_planar(), W.is_planar(), punct_torus().is_planar())
+    print(K.PD_code(True))
+    print(K.DT_code(True), K.peer_code())
+    print(W.PD_code(True))
+    print(W.DT_code(True), K.peer_code())
 
 
 # ----- checking the SnapPy link exterior code ------------
 
 def knot(fractions):
     if len(fractions) == 1:
         return RationalTangle(*fractions[0]).denominator_closure()
     else:
         A, B, C = [RationalTangle(*f) for f in fractions]
         T = A + B + C
         return T.numerator_closure()
 
+
 def some_knots():
-    from . import hyperbolic_montesinos 
-    return [ (K, knot(fractions)) for K, fractions in hyperbolic_montesinos.knots] 
+    from . import hyperbolic_montesinos
+    return [(K, knot(fractions))
+            for K, fractions in hyperbolic_montesinos.knots]
+
 
 def exterior_test():
     try:
         import snappy
     except ImportError:
         print("SnapPy not installed, skipping link exterior test.")
 
     print(figure8().exterior().volume(), whitehead().exterior().volume())
 
     C, Id = RationalTangle(1), IdentityBraid(1)
     x = C | Id
     y = Id | (-C)
-    print((x*y*x*y).denominator_closure().exterior().volume())
+    print((x * y * x * y).denominator_closure().exterior().volume())
 
     for name, K in some_knots():
         M0, M1 = K.exterior(), snappy.Manifold(K.DT_code(True))
         N0 = snappy.LinkExteriors.identify(M0)
         N1 = snappy.LinkExteriors.identify(M1)
         assert N0.name() == name and N1.name() == name
 
@@ -85,43 +91,43 @@
 
 def alexander_polynomial_test():
     """
     Export a bunch of Montesinos knots as PD diagrams and
     compute the Alexander polynomials via KnotTheory and
     also Sage.  Make sure they match.
     """
-    
     try:
         sys.path.append('/Users/dunfield/work/python')
         import nsagetools
     except ImportError:
         print("Skipping this test as you're not within Sage and/or are not Nathan.")
-        return 
+        return
 
     from sage.all import mathematica, PolynomialRing, ZZ
 
     mathematica.execute('AppendTo[$Path, "/pkgs"]')
     mathematica.execute('<<KnotTheory`')
     mathematica.execute('Off[KnotTheory::loading]')
     mathematica.execute('Off[KnotTheory::credits]')
     mathematica.execute('MyAlex[L_] := CoefficientList[t^100*Alexander[L][t], t]')
 
     def alex_by_KnotTheory(L):
         p = mathematica.MyAlex(L.PD_code(True)).sage()
-        i = min( [i for i,c in enumerate(p) if c != 0])
+        i = next(iter(i for i, c in enumerate(p) if c != 0))
         R = PolynomialRing(ZZ, 'a')
         return R(p[i:])
 
     def alex_match(L):
         p1 = alex_by_KnotTheory(L)
         p2 = nsagetools.alexander_polynomial(L.exterior())
         return 0 in [p1 - p2, p1 + p2]
 
     for name, K in some_knots():
         assert alex_match(K)
 
     print("Checked Alexander polynomials via KnotTheory for these 167 knots.")
 
+
 if __name__ == '__main__':
     basic_test()
     exterior_test()
     alexander_polynomial_test()
```

### Comparing `spherogram-2.1/spherogram_src/links/test/test_montesinos.py` & `spherogram-2.2/spherogram_src/links/test/test_montesinos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-import sys, random
+import random
 try:
     import snappy
     _have_snappy = True
 except ImportError:
     print('Could not import snappy in test_montesinos.py.')
     _have_snappy = False
 from spherogram import RationalTangle
 
 knots = [['4_1', [(2, 5)]], ['5_2', [(3, 7)]], ['6_1', [(4, 9)]], ['6_2', [(4, 11)]], ['6_3', [(5, 13)]], ['7_2', [(5, 11)]], ['7_3', [(4, 13)]], ['7_4', [(4, 15)]], ['7_5', [(7, 17)]], ['7_6', [(7, 19)]], ['7_7', [(8, 21)]], ['8_1', [(6, 13)]], ['8_2', [(6, 17)]], ['8_3', [(4, 17)]], ['8_4', [(5, 19)]], ['8_5', [(1, 3), (1, 3), (1, 2)]], ['8_6', [(10, 23)]], ['8_7', [(9, 23)]], ['8_8', [(9, 25)]], ['8_9', [(7, 25)]], ['8_10', [(1, 3), (2, 3), (1, 2)]], ['8_11', [(10, 27)]], ['8_12', [(12, 29)]], ['8_13', [(11, 29)]], ['8_14', [(12, 31)]], ['8_15', [(2, 3), (2, 3), (1, 2)]], ['8_20', [(1, 3), (2, 3), (-1, 2)]], ['8_21', [(2, 3), (2, 3), (-1, 2)]], ['9_2', [(7, 15)]], ['9_3', [(6, 19)]], ['9_4', [(5, 21)]], ['9_5', [(6, 23)]], ['9_6', [(11, 27)]], ['9_7', [(13, 29)]], ['9_8', [(11, 31)]], ['9_9', [(9, 31)]], ['9_10', [(10, 33)]], ['9_11', [(14, 33)]], ['9_12', [(13, 35)]], ['9_13', [(10, 37)]], ['9_14', [(14, 37)]], ['9_15', [(16, 39)]], ['9_16', [(1, 3), (1, 3), (3, 2)]], ['9_17', [(14, 39)]], ['9_18', [(17, 41)]], ['9_19', [(16, 41)]], ['9_20', [(15, 41)]], ['9_21', [(18, 43)]], ['9_22', [(3, 5), (1, 3), (1, 2)]], ['9_23', [(19, 45)]], ['9_24', [(1, 3), (2, 3), (3, 2)]], ['9_25', [(2, 5), (2, 3), (1, 2)]], ['9_26', [(18, 47)]], ['9_27', [(19, 49)]], ['9_28', [(2, 3), (2, 3), (3, 2)]], ['9_30', [(3, 5), (2, 3), (1, 2)]], ['9_31', [(21, 55)]], ['9_35', [(1, 3), (1, 3), (1, 3)]], ['9_36', [(2, 5), (1, 3), (1, 2)]], ['9_37', [(1, 3), (2, 3), (2, 3)]], ['9_42', [(2, 5), (1, 3), (-1, 2)]], ['9_43', [(3, 5), (1, 3), (-1, 2)]], ['9_44', [(2, 5), (2, 3), (-1, 2)]], ['9_45', [(3, 5), (2, 3), (-1, 2)]], ['9_46', [(1, 3), (1, 3), (-1, 3)]], ['9_48', [(2, 3), (2, 3), (-1, 3)]], ['10_1', [(8, 17)]], ['10_2', [(8, 23)]], ['10_3', [(6, 25)]], ['10_4', [(7, 27)]], ['10_5', [(13, 33)]], ['10_6', [(16, 37)]], ['10_7', [(16, 43)]], ['10_8', [(6, 29)]], ['10_9', [(11, 39)]], ['10_10', [(17, 45)]], ['10_11', [(13, 43)]], ['10_12', [(17, 47)]], ['10_13', [(22, 53)]], ['10_14', [(22, 57)]], ['10_15', [(19, 43)]], ['10_16', [(14, 47)]], ['10_17', [(9, 41)]], ['10_18', [(23, 55)]], ['10_19', [(14, 51)]], ['10_20', [(16, 35)]], ['10_21', [(16, 45)]], ['10_22', [(13, 49)]], ['10_23', [(23, 59)]], ['10_24', [(24, 55)]], ['10_25', [(24, 65)]], ['10_26', [(17, 61)]], ['10_27', [(27, 71)]], ['10_28', [(19, 53)]], ['10_29', [(26, 63)]], ['10_30', [(26, 67)]], ['10_31', [(25, 57)]], ['10_32', [(29, 69)]], ['10_33', [(18, 65)]], ['10_34', [(13, 37)]], ['10_35', [(20, 49)]], ['10_36', [(20, 51)]], ['10_37', [(23, 53)]], ['10_38', [(25, 59)]], ['10_39', [(22, 61)]], ['10_40', [(29, 75)]], ['10_41', [(26, 71)]], ['10_42', [(31, 81)]], ['10_43', [(27, 73)]], ['10_44', [(30, 79)]], ['10_45', [(34, 89)]], ['10_46', [(1, 5), (1, 3), (1, 2)]], ['10_47', [(1, 5), (2, 3), (1, 2)]], ['10_48', [(4, 5), (1, 3), (1, 2)]], ['10_49', [(4, 5), (2, 3), (1, 2)]], ['10_50', [(3, 7), (1, 3), (1, 2)]], ['10_51', [(3, 7), (2, 3), (1, 2)]], ['10_52', [(4, 7), (1, 3), (1, 2)]], ['10_53', [(4, 7), (2, 3), (1, 2)]], ['10_54', [(2, 7), (1, 3), (1, 2)]], ['10_55', [(2, 7), (2, 3), (1, 2)]], ['10_56', [(5, 7), (1, 3), (1, 2)]], ['10_57', [(5, 7), (2, 3), (1, 2)]], ['10_58', [(2, 5), (2, 5), (1, 2)]], ['10_59', [(2, 5), (3, 5), (1, 2)]], ['10_60', [(3, 5), (3, 5), (1, 2)]], ['10_61', [(1, 4), (1, 3), (1, 3)]], ['10_62', [(1, 4), (1, 3), (2, 3)]], ['10_63', [(1, 4), (2, 3), (2, 3)]], ['10_64', [(3, 4), (1, 3), (1, 3)]], ['10_65', [(3, 4), (1, 3), (2, 3)]], ['10_66', [(3, 4), (2, 3), (2, 3)]], ['10_67', [(2, 5), (1, 3), (2, 3)]], ['10_68', [(3, 5), (1, 3), (1, 3)]], ['10_69', [(3, 5), (2, 3), (2, 3)]], ['10_70', [(2, 5), (1, 3), (3, 2)]], ['10_71', [(2, 5), (2, 3), (3, 2)]], ['10_72', [(3, 5), (1, 3), (3, 2)]], ['10_73', [(3, 5), (2, 3), (3, 2)]], ['10_74', [(1, 3), (1, 3), (5, 3)]], ['10_75', [(2, 3), (2, 3), (5, 3)]], ['10_76', [(1, 3), (1, 3), (5, 2)]], ['10_77', [(1, 3), (2, 3), (5, 2)]], ['10_78', [(2, 3), (2, 3), (5, 2)]], ['10_125', [(1, 5), (2, 3), (-1, 2)]], ['10_126', [(4, 5), (1, 3), (-1, 2)]], ['10_127', [(4, 5), (2, 3), (-1, 2)]], ['10_128', [(3, 7), (1, 3), (-1, 2)]], ['10_129', [(3, 7), (2, 3), (-1, 2)]], ['10_130', [(4, 7), (1, 3), (-1, 2)]], ['10_131', [(4, 7), (2, 3), (-1, 2)]], ['10_132', [(2, 7), (1, 3), (-1, 2)]], ['10_133', [(2, 7), (2, 3), (-1, 2)]], ['10_134', [(5, 7), (1, 3), (-1, 2)]], ['10_135', [(5, 7), (2, 3), (-1, 2)]], ['10_136', [(2, 5), (2, 5), (-1, 2)]], ['10_137', [(2, 5), (3, 5), (-1, 2)]], ['10_138', [(3, 5), (3, 5), (-1, 2)]], ['10_139', [(1, 4), (1, 3), (-2, 3)]], ['10_140', [(1, 4), (1, 3), (-1, 3)]], ['10_141', [(1, 4), (2, 3), (-1, 3)]], ['10_142', [(3, 4), (1, 3), (-2, 3)]], ['10_143', [(3, 4), (1, 3), (-1, 3)]], ['10_144', [(3, 4), (2, 3), (-1, 3)]], ['10_145', [(2, 5), (1, 3), (-2, 3)]], ['10_146', [(2, 5), (2, 3), (-1, 3)]], ['10_147', [(3, 5), (1, 3), (-1, 3)]]]
 
+
 def knot(fractions):
     if len(fractions) == 1:
         return RationalTangle(*fractions[0]).denominator_closure()
     else:
         A, B, C = [RationalTangle(*f) for f in fractions]
         T = A + B + C
         return T.numerator_closure()
 
+
 def test(N=len(knots)):
     if not _have_snappy:
         print('Skipping Montesinos tests --- will be run by SnapPy.\n')
         return
     else:
         print('Running Montesinos tests for Spherogram.\n')
     for name, fractions in random.sample(knots, N):
```

### Comparing `spherogram-2.1/spherogram_src/links/twist.py` & `spherogram-2.2/spherogram_src/links/twist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 """
-Switching crossings to make each twist region consistent.  
+Switching crossings to make each twist region consistent.
 """
 
 from .links import CrossingStrand
 from ..graphs import CyclicList
 
-class  TwistRegionCap:
+
+class TwistRegionCap:
     def __init__(self, crossing_strand):
         self.cs = crossing_strand
 
     def sign(self):
         return self.cs.strand_index % 2
 
     def swap_crossing(self):
         self.cs.crossing.rotate_by_90()
-    
+
 
 class TwistRegionCrossing(TwistRegionCap):
     """
     A crossing together with a chosen bigon.  Recorded by the CrossingStrand
     which gives the side of said bigon which is "most clockwise" when viewed from
-    the crossing.  
+    the crossing.
     """
     def __init__(self, crossing):
         if isinstance(crossing, CrossingStrand):
             self.cs = crossing
         else:
             assert is_end_of_twist_region(crossing)
             neighbors = CyclicList(C for (C, i) in crossing.adjacent)
             for i in range(4):
-                if neighbors[i] == neighbors[i+1]:
+                if neighbors[i] == neighbors[i + 1]:
                     self.cs = CrossingStrand(crossing, i)
 
     def next(self):
         # Move along edge to next crossing and rotate to preferred side of bigon.
         cs = self.cs.opposite().rotate(1)
         C, e = cs
-        if C.adjacent[e][0] != C.adjacent[e+1][0]:
+        if C.adjacent[e][0] != C.adjacent[e + 1][0]:
             return TwistRegionCap(cs)
         return TwistRegionCrossing(cs)
 
     def __repr__(self):
         return "<Twist: %s>" % (self.cs, )
 
+
 class TwistRegion:
     def __init__(self, crossing):
         C = TwistRegionCrossing(crossing)
         crossings = [C]
         while isinstance(C, TwistRegionCrossing):
             C = C.next()
             crossings.append(C)
-                        
+
         self.crossings = crossings
 
     def signs(self):
         return [C.sign() for C in self.crossings]
-    
+
     def make_consistent(self):
         sign = self.crossings[0].sign()
         for C in self.crossings:
             if C.sign() != sign:
                 C.swap_crossing()
-        
+
     def __len__(self):
         return len(self.crossings)
-    
-def is_end_of_twist_region(crossing):
-    return len(set([C for (C, i) in crossing.adjacent])) == 3
+
+
+def is_end_of_twist_region(crossing) -> bool:
+    return len(set(C for (C, i) in crossing.adjacent)) == 3
+
 
 def make_twist_regions_consistent(link):
     """
     Changes crossings so that no bigon permits a Type II move cancelling
-    the pair of crossings at the end of the bigon.  The system is that the 
+    the pair of crossings at the end of the bigon.  The system is that the
     end crossing with the lowest label "wins" in determining the type of the twist
     region.  The code assumes that no link component is effectively a meridian
     loop for another component; said differently, no two bigons share a
     common edge.
 
     Note, this implementation fails if given something like a (2, n) torus link.
     """
-    ans = []
     for C in link.crossings:
         if is_end_of_twist_region(C):
             twist = TwistRegion(C)
             twist.make_consistent()
     link._rebuild()
```

### Comparing `spherogram-2.1/spherogram_src/presentations.py` & `spherogram-2.2/spherogram_src/presentations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .graphs import ReducedGraph, Digraph, Poset
 from collections import deque
 import operator
 
 
-class Alphabet(object):
+class Alphabet():
     """
     An Alphabet translates between integers and strings.
     Call as a function to go from string to integer; use getitem
     to go from integer to string.
     """
 
     def __init__(self, identity, pos, neg, separator=''):
@@ -25,17 +25,16 @@
         return n if n < self.size else n - 2 * self.size
 
     def spell(self, int_list):
         """
         Convert a sequence of integers to a string.
         """
         if int_list:
-            return self.separator.join([self[x] for x in int_list])
-        else:
-            return self[0]
+            return self.separator.join(self[x] for x in int_list)
+        return self[0]
 
 
 abc = Alphabet('1',
                'abcdefghijklmnopqrstuvwxyz',
                'ABCDEFGHIJKLMNOPQRSTUVWXYZ')
 
 ABC = Alphabet('1',
@@ -165,15 +164,15 @@
     def shuffle(self, perm_dict={}):
         """
         Permute generators according to the supplied dictionary.
         Keys must be positive integers.  Values may be negative.
         The set of keys must equal the set of values up to sign.
         """
         abs_image = set(map(operator.abs, perm_dict.values()))
-        if set(perm_dict.keys()) != abs_image:
+        if set(perm_dict) != abs_image:
             raise ValueError('Not a permutation!')
         for n in range(len(self)):
             x = self[n]
             self[n] = perm_dict.get(x, x) if x > 0 else -perm_dict.get(-x, -x)
 
     def powers(self, start=0):
         """
@@ -252,15 +251,15 @@
     def __le__(self, other):
         return not self > other
 
     def __ge__(self, other):
         return not self < other
 
 
-class WhiteheadMove(object):
+class WhiteheadMove():
     """
     Holds the data describing a Whitehead move.
     """
 
     def __init__(self, letter, cut_set, generators, alphabet):
         self.letter = letter
         self.cut_set = cut_set
@@ -280,15 +279,15 @@
                 sub += self.alphabet[x]
                 if x not in self.cut_set and x != -self.letter:
                     sub += self.alphabet[-self.letter]
             subs.append(sub)
         return ', '.join(subs)
 
 
-class Presentation(object):
+class Presentation():
     """
     A Presentation contains a list of CyclicWords as relators and a
     list of (integer) letters as generators.  The generators are
     implicitly defined by their appearance in some relator.  Other
     generators can be provided in an optional list.  Instantiate with
     a list of objects that can be used to instantiate a CyclicWord,
     i.e. strings or lists of non-zero integers.
@@ -310,15 +309,15 @@
                 self.generators.update([abs(l) for l in r])
 
     def __repr__(self):
         generators = ', '.join(self.alphabet[x] for x in self.generators)
         return 'generators: [%s]\nrelators: %s' % (generators, self.relators)
 
     def __len__(self):
-        return sum([len(W) for W in self.relators])
+        return sum(len(W) for W in self.relators)
 
     def __eq__(self, other):
         return (self.relators == other.relators and
                 self.generators == other.generators)
 
     def whitehead_graph(self):
         Wh = ReducedGraph()
@@ -483,24 +482,24 @@
                 for child in left.children():
                     queue.append(child)
             else:
                 break
         relators = queue[0].presentation.relators
         ordering = queue[0].ordering
         generators = tuple(range(1, len(self.generators) + 1))
-        return tuple([tuple(R.rewrite(ordering)) for R in relators]), generators
+        return tuple(tuple(R.rewrite(ordering)) for R in relators), generators
 
     def magma_string(self):
-        gens = sorted([self.alphabet[g] for g in self.generators])
+        gens = sorted(self.alphabet[g] for g in self.generators)
         ans = 'Group<' + ', '.join(gens) + ' | '
-        ans += ', '.join([R.verbose_string() for R in self.relators])
+        ans += ', '.join(R.verbose_string() for R in self.relators)
         return ans + '>'
 
 
-class CanonizeNode(object):
+class CanonizeNode():
     def __init__(self, presentation, remaining, ordering=[]):
         self.presentation = presentation
         self.generators = presentation.generators
         self.relators = presentation.relators
         self.remaining = remaining
         self.ordering = ordering
```

### Comparing `spherogram-2.1/spherogram_src/sage_helper.py` & `spherogram-2.2/spherogram_src/sage_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,25 +15,28 @@
     _within_sage = True
 except Exception:
     _within_sage = False
     import decorator
 
 
 import doctest
-import re
-import types
 
 
 class SageNotAvailable(Exception):
     pass
 
 
 if _within_sage:
     def sage_method(function):
         function._sage_method = True
         return function
+    from packaging.version import parse
+    from sage.version import version as _sage_version
+    sage_pd_clockwise = (parse(_sage_version) <= parse('10.1.beta0'))
 else:
     def _sage_method(function, *args, **kw):
         raise SageNotAvailable('Sorry, this feature requires using SnapPy inside Sage.')
-        
+
     def sage_method(function):
         return decorator.decorator(_sage_method, function)
+
+    sage_pd_clockwise = None
```

### Comparing `spherogram-2.1/spherogram_src/test_helper.py` & `spherogram-2.2/spherogram_src/test_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,59 +29,62 @@
 import re
 import types
 
 
 class SageNotAvailable(Exception):
     pass
 
+
 if _within_sage:
     def sage_method(function):
         function._sage_method = True
         return function
 else:
     def _sage_method(function, *args, **kw):
         raise SageNotAvailable('Sorry, this feature requires using SnapPy inside Sage.')
-        
+
     def sage_method(function):
         return decorator.decorator(_sage_method, function)
 
 
 SNAPPY_FLAG = doctest.register_optionflag('SNAPPY')
 
+
 def filter_out_snappy(pieces):
     ans = []
     for piece in pieces:
         if _have_snappy or not isinstance(piece, doctest.Example):
             ans.append(piece)
         elif not piece.options.get(SNAPPY_FLAG, False):
             ans.append(piece)
     return ans
-            
-        
+
+
 if _within_sage:
     class DocTestParser(doctest.DocTestParser):
         def parse(self, string, name='<string>'):
             string = re.subn(r'(\n\s*)sage:|(\A\s*)sage:', r'\g<1>>>>', string)[0]
             pieces = doctest.DocTestParser.parse(self, string, name)
             return filter_out_snappy(pieces)
 
     globs = dict()
 else:
     class DocTestParser(doctest.DocTestParser):
         def parse(self, string, name='<string>'):
             pieces = doctest.DocTestParser.parse(self, string, name)
             return filter_out_snappy(pieces)
 
-        
     globs = dict()
 
+
 def print_results(module, results):
     print(module.__name__ + ':')
-    print('   %s failures out of %s tests.' %  (results.failed, results.attempted))
-    
+    print('   %s failures out of %s tests.' % (results.failed, results.attempted))
+
+
 def doctest_modules(modules, verbose=False, print_info=True, extraglobs=dict()):
     finder = doctest.DocTestFinder(parser=DocTestParser())
 #    full_extraglobals = dict(globs.items() + extraglobs.items())
     full_extraglobals = globs.copy()
     full_extraglobals.update(extraglobs)
     failed, attempted = 0, 0
     for module in modules:
@@ -96,12 +99,7 @@
         attempted += result.attempted
         if print_info:
             print_results(module, result)
 
     if print_info:
         print('\nAll doctests:\n   %s failures out of %s tests.' % (failed, attempted))
     return doctest.TestResults(failed, attempted)
-    
-
-        
-    
-
```

