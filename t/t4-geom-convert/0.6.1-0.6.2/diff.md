# Comparing `tmp/t4_geom_convert-0.6.1.tar.gz` & `tmp/t4_geom_convert-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4_geom_convert-0.6.1.tar", max compression
+gzip compressed data, was "t4_geom_convert-0.6.2.tar", max compression
```

## Comparing `t4_geom_convert-0.6.1.tar` & `t4_geom_convert-0.6.2.tar`

### file list

```diff
@@ -1,301 +1,96 @@
--rw-r--r--   0        0        0    35141 2020-01-07 12:20:18.320103 t4_geom_convert-0.6.1/MIP/LICENSE
--rw-r--r--   0        0        0        0 2019-07-23 12:07:01.746772 t4_geom_convert-0.6.1/MIP/__init__.py
--rw-r--r--   0        0        0        0 2019-07-23 12:06:54.208901 t4_geom_convert-0.6.1/MIP/geom/__init__.py
--rw-r--r--   0        0        0      162 2019-09-18 15:20:04.653442 t4_geom_convert-0.6.1/MIP/geom/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      170 2020-01-17 14:53:12.301431 t4_geom_convert-0.6.1/MIP/geom/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1701 2020-04-06 15:13:18.677720 t4_geom_convert-0.6.1/MIP/geom/__pycache__/cells.cpython-35.pyc
--rw-r--r--   0        0        0     1561 2020-04-07 13:17:40.839729 t4_geom_convert-0.6.1/MIP/geom/__pycache__/cells.cpython-38.pyc
--rw-r--r--   0        0        0      808 2020-04-06 15:13:19.274703 t4_geom_convert-0.6.1/MIP/geom/__pycache__/composition.cpython-35.pyc
--rw-r--r--   0        0        0      691 2021-07-02 09:46:25.640965 t4_geom_convert-0.6.1/MIP/geom/__pycache__/composition.cpython-38.pyc
--rw-r--r--   0        0        0    15683 2020-04-06 15:13:17.931721 t4_geom_convert-0.6.1/MIP/geom/__pycache__/forcad.cpython-35.pyc
--rw-r--r--   0        0        0    14514 2022-02-25 21:02:40.753159 t4_geom_convert-0.6.1/MIP/geom/__pycache__/forcad.cpython-38.pyc
--rw-r--r--   0        0        0     3811 2019-09-18 15:20:06.953410 t4_geom_convert-0.6.1/MIP/geom/__pycache__/main.cpython-35.pyc
--rw-r--r--   0        0        0     3340 2020-01-17 14:53:12.910419 t4_geom_convert-0.6.1/MIP/geom/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0     2718 2020-04-06 15:13:18.697709 t4_geom_convert-0.6.1/MIP/geom/__pycache__/parsegeom.cpython-35.pyc
--rw-r--r--   0        0        0     2481 2020-04-07 13:17:40.849725 t4_geom_convert-0.6.1/MIP/geom/__pycache__/parsegeom.cpython-38.pyc
--rw-r--r--   0        0        0     2890 2020-04-06 15:13:18.709710 t4_geom_convert-0.6.1/MIP/geom/__pycache__/semantics.cpython-35.pyc
--rw-r--r--   0        0        0     4695 2021-12-08 09:19:44.421195 t4_geom_convert-0.6.1/MIP/geom/__pycache__/semantics.cpython-38.pyc
--rw-r--r--   0        0        0     1116 2019-09-18 15:20:04.678442 t4_geom_convert-0.6.1/MIP/geom/__pycache__/surfaces.cpython-35.pyc
--rw-r--r--   0        0        0     1009 2021-12-08 09:19:44.906188 t4_geom_convert-0.6.1/MIP/geom/__pycache__/surfaces.cpython-38.pyc
--rw-r--r--   0        0        0     2181 2020-04-06 15:13:17.960723 t4_geom_convert-0.6.1/MIP/geom/__pycache__/transforms.cpython-35.pyc
--rw-r--r--   0        0        0     2068 2022-03-03 10:33:34.777669 t4_geom_convert-0.6.1/MIP/geom/__pycache__/transforms.cpython-38.pyc
--rw-r--r--   0        0        0     2427 2021-07-05 09:19:23.710002 t4_geom_convert-0.6.1/MIP/geom/another_parser.py
--rw-r--r--   0        0        0     1393 2020-02-21 09:29:30.758624 t4_geom_convert-0.6.1/MIP/geom/cells.py
--rw-r--r--   0        0        0      551 2021-07-02 09:46:22.102009 t4_geom_convert-0.6.1/MIP/geom/composition.py
--rw-r--r--   0        0        0     2461 2019-07-23 12:06:54.244872 t4_geom_convert-0.6.1/MIP/geom/copt.py
--rw-r--r--   0        0        0    14112 2022-02-25 21:02:37.966808 t4_geom_convert-0.6.1/MIP/geom/forcad.py
--rw-r--r--   0        0        0      364 2019-07-23 12:06:54.262904 t4_geom_convert-0.6.1/MIP/geom/grammars/__init__.py
--rw-r--r--   0        0        0      171 2019-09-18 15:20:06.607414 t4_geom_convert-0.6.1/MIP/geom/grammars/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      179 2020-01-17 14:53:12.707433 t4_geom_convert-0.6.1/MIP/geom/grammars/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      886 2019-09-18 15:20:07.143408 t4_geom_convert-0.6.1/MIP/geom/grammars/__pycache__/composition.cpython-35.pyc
--rw-r--r--   0        0        0      844 2020-01-17 14:53:12.984419 t4_geom_convert-0.6.1/MIP/geom/grammars/__pycache__/composition.cpython-38.pyc
--rw-r--r--   0        0        0      340 2021-07-02 09:46:22.107010 t4_geom_convert-0.6.1/MIP/geom/grammars/geom.ebnf
--rw-r--r--   0        0        0     1699 2020-02-21 09:29:30.776628 t4_geom_convert-0.6.1/MIP/geom/grammars/multioperand.py
--rw-r--r--   0        0        0     3615 2019-07-23 12:07:01.770768 t4_geom_convert-0.6.1/MIP/geom/main.py
--rw-r--r--   0        0        0     2704 2020-02-21 09:29:30.780622 t4_geom_convert-0.6.1/MIP/geom/parsegeom.py
--rw-r--r--   0        0        0     3057 2021-07-05 09:19:23.713988 t4_geom_convert-0.6.1/MIP/geom/semantics.py
--rw-r--r--   0        0        0      859 2021-07-05 09:19:23.716988 t4_geom_convert-0.6.1/MIP/geom/surfaces.py
--rw-r--r--   0        0        0     1394 2019-07-23 12:06:54.360873 t4_geom_convert-0.6.1/MIP/geom/testgrammar.py
--rw-r--r--   0        0        0     1756 2022-03-03 10:29:08.794011 t4_geom_convert-0.6.1/MIP/geom/transforms.py
--rw-r--r--   0        0        0       49 2019-07-23 12:06:54.390871 t4_geom_convert-0.6.1/MIP/mip/__init__.py
--rw-r--r--   0        0        0      197 2019-09-18 15:20:04.243449 t4_geom_convert-0.6.1/MIP/mip/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      201 2020-01-17 14:53:12.053431 t4_geom_convert-0.6.1/MIP/mip/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2332 2020-04-06 15:13:17.507731 t4_geom_convert-0.6.1/MIP/mip/__pycache__/blocks.cpython-35.pyc
--rw-r--r--   0        0        0     2128 2021-12-08 09:19:44.028191 t4_geom_convert-0.6.1/MIP/mip/__pycache__/blocks.cpython-38.pyc
--rw-r--r--   0        0        0     2204 2020-04-06 15:13:17.523728 t4_geom_convert-0.6.1/MIP/mip/__pycache__/cards.cpython-35.pyc
--rw-r--r--   0        0        0     2840 2021-07-02 09:46:24.996975 t4_geom_convert-0.6.1/MIP/mip/__pycache__/cards.cpython-38.pyc
--rw-r--r--   0        0        0     1439 2020-01-07 12:21:08.734432 t4_geom_convert-0.6.1/MIP/mip/__pycache__/cellcard.cpython-35.pyc
--rw-r--r--   0        0        0     1336 2021-12-08 09:19:44.103194 t4_geom_convert-0.6.1/MIP/mip/__pycache__/cellcard.cpython-38.pyc
--rw-r--r--   0        0        0      481 2019-09-18 15:20:04.365447 t4_geom_convert-0.6.1/MIP/mip/__pycache__/datacard.cpython-35.pyc
--rw-r--r--   0        0        0     5261 2021-12-08 09:19:44.162202 t4_geom_convert-0.6.1/MIP/mip/__pycache__/datacard.cpython-38.pyc
--rw-r--r--   0        0        0     5398 2020-04-06 15:13:17.476727 t4_geom_convert-0.6.1/MIP/mip/__pycache__/main.cpython-35.pyc
--rw-r--r--   0        0        0     5098 2021-12-08 09:19:43.993194 t4_geom_convert-0.6.1/MIP/mip/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0      608 2019-09-18 15:20:04.342447 t4_geom_convert-0.6.1/MIP/mip/__pycache__/surfacecard.cpython-35.pyc
--rw-r--r--   0        0        0      598 2020-01-17 14:53:12.086439 t4_geom_convert-0.6.1/MIP/mip/__pycache__/surfacecard.cpython-38.pyc
--rw-r--r--   0        0        0     1088 2019-09-18 15:20:04.296448 t4_geom_convert-0.6.1/MIP/mip/__pycache__/utils.cpython-35.pyc
--rw-r--r--   0        0        0     1042 2020-01-17 14:53:12.069434 t4_geom_convert-0.6.1/MIP/mip/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     3088 2021-07-05 09:19:23.719998 t4_geom_convert-0.6.1/MIP/mip/blocks.py
--rw-r--r--   0        0        0     3697 2021-07-02 09:46:22.156011 t4_geom_convert-0.6.1/MIP/mip/cards.py
--rw-r--r--   0        0        0     3035 2021-07-05 09:19:23.723003 t4_geom_convert-0.6.1/MIP/mip/cellcard.py
--rw-r--r--   0        0        0     5144 2021-07-05 09:19:23.726989 t4_geom_convert-0.6.1/MIP/mip/datacard.py
--rw-r--r--   0        0        0     4830 2021-07-05 09:19:23.729992 t4_geom_convert-0.6.1/MIP/mip/main.py
--rw-r--r--   0        0        0      985 2019-07-23 12:06:54.506881 t4_geom_convert-0.6.1/MIP/mip/readme.rst
--rw-r--r--   0        0        0      386 2019-07-23 12:06:54.509911 t4_geom_convert-0.6.1/MIP/mip/surfacecard.py
--rw-r--r--   0        0        0      763 2019-07-23 12:06:54.516881 t4_geom_convert-0.6.1/MIP/mip/utils.py
--rw-r--r--   0        0        0     1073 2019-07-23 12:06:54.553872 t4_geom_convert-0.6.1/MIP/tests.py
--rw-r--r--   0        0        0    10140 2021-07-02 09:46:22.246004 t4_geom_convert-0.6.1/README.md
--rw-r--r--   0        0        0     4372 2022-10-11 13:22:56.898321 t4_geom_convert-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       96 2020-01-29 08:31:48.555823 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/examples/7d04b6175f19883b/95146c243a684b35
--rw-r--r--   0        0        0       11 2020-01-16 16:20:12.243312 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/examples/b5818b9694c7412d/705ef95420cc18dd
--rw-r--r--   0        0        0       18 2020-01-16 16:20:12.899300 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/examples/c02acd8530982b40/5cfcac0889e0496c
--rw-r--r--   0        0        0       16 2020-01-16 16:20:12.623304 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/examples/c02acd8530982b40/ae40659da1193cde
--rw-r--r--   0        0        0       26 2020-01-16 16:20:17.125248 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/examples/f5595e3a381d5483/185bbfdc75a8800f
--rw-r--r--   0        0        0    20688 2020-01-29 08:31:49.134822 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    19174 2020-01-16 16:20:12.600304 t4_geom_convert-0.6.1/t4_geom_convert/.hypothesis/unicode_data/8.0.0/charmap.json.gz
--rw-r--r--   0        0        0      966 2021-07-02 09:46:22.608020 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py
--rw-r--r--   0        0        0     2192 2021-07-02 09:46:22.611003 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.614004 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__init__.py
--rw-r--r--   0        0        0      685 2020-04-06 15:13:19.477713 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__pycache__/CBoundCond.cpython-35.pyc
--rw-r--r--   0        0        0      574 2021-07-02 09:46:25.719961 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__pycache__/CBoundCond.cpython-38.pyc
--rw-r--r--   0        0        0     1890 2020-04-06 15:13:19.438700 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__pycache__/CConversionBoundaryCondition.cpython-35.pyc
--rw-r--r--   0        0        0     1648 2021-07-02 09:46:25.714967 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__pycache__/CConversionBoundaryCondition.cpython-38.pyc
--rw-r--r--   0        0        0      194 2019-09-18 15:20:07.328406 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      202 2021-07-02 09:46:25.708967 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1698 2022-10-10 08:13:16.765702 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/Abundances.py
--rw-r--r--   0        0        0     1784 2021-07-02 09:46:22.620008 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py
--rw-r--r--   0        0        0     1273 2021-07-02 09:46:22.623004 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CCompositionT4.py
--rw-r--r--   0        0        0     1692 2021-07-02 09:46:22.626003 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py
--rw-r--r--   0        0        0     3224 2022-10-10 08:13:16.985692 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py
--rw-r--r--   0        0        0     4271 2022-10-10 08:13:17.228693 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py
--rw-r--r--   0        0        0     1165 2021-07-02 09:46:22.635003 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/ConvertIsotope.py
--rw-r--r--   0        0        0     1483 2021-07-02 09:46:22.637009 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py
--rw-r--r--   0        0        0     1419 2021-07-02 09:46:22.640000 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.643003 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__init__.py
--rw-r--r--   0        0        0     1220 2020-01-07 12:21:10.295398 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/Abundances.cpython-35.pyc
--rw-r--r--   0        0        0     1185 2022-10-10 08:15:17.237388 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/Abundances.cpython-38.pyc
--rw-r--r--   0        0        0     1226 2020-04-06 15:13:19.285705 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CCompositionMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     1059 2021-07-02 09:46:25.645961 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CCompositionMCNP.cpython-38.pyc
--rw-r--r--   0        0        0      919 2020-04-06 15:13:19.224701 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CCompositionT4.cpython-35.pyc
--rw-r--r--   0        0        0      776 2021-07-02 09:46:25.621964 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CCompositionT4.cpython-38.pyc
--rw-r--r--   0        0        0     1948 2019-09-18 15:20:07.116433 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CDictCompositionMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     1775 2021-07-02 09:46:25.631965 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CDictCompositionMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     1769 2019-09-18 15:20:07.107408 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CDictCompositionT4.cpython-35.pyc
--rw-r--r--   0        0        0     1212 2019-12-19 08:45:08.108466 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CIsotopeConversion.cpython-35.pyc
--rw-r--r--   0        0        0     2420 2020-04-06 15:13:19.235706 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CompositionConversionMCNPToT4.cpython-35.pyc
--rw-r--r--   0        0        0     2213 2022-10-10 08:15:16.528389 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/CompositionConversionMCNPToT4.cpython-38.pyc
--rw-r--r--   0        0        0     2958 2020-04-06 15:13:19.211704 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/ConstructCompositionT4.cpython-35.pyc
--rw-r--r--   0        0        0     2771 2022-10-10 08:15:16.214374 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/ConstructCompositionT4.cpython-38.pyc
--rw-r--r--   0        0        0      720 2020-04-06 15:13:19.295713 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/ConvertIsotope.cpython-35.pyc
--rw-r--r--   0        0        0      597 2021-07-02 09:46:25.650967 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/ConvertIsotope.cpython-38.pyc
--rw-r--r--   0        0        0      769 2019-09-18 15:20:07.200404 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/EIsotopeAtomicNumberMCNP.cpython-35.pyc
--rw-r--r--   0        0        0      652 2021-07-02 09:46:25.655963 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/EIsotopeAtomicNumberMCNP.cpython-38.pyc
--rw-r--r--   0        0        0      723 2019-09-18 15:20:07.218409 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/EIsotopeNameElementT4.cpython-35.pyc
--rw-r--r--   0        0        0      624 2021-07-02 09:46:25.664965 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/EIsotopeNameElementT4.cpython-38.pyc
--rw-r--r--   0        0        0      188 2019-09-18 15:20:07.026413 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      196 2021-07-02 09:46:25.607963 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.646013 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Configuration/__init__.py
--rw-r--r--   0        0        0     2629 2019-05-10 12:43:42.906024 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Configuration/__pycache__/CConfigParameters.cpython-35.pyc
--rw-r--r--   0        0        0      380 2019-05-10 12:43:42.914019 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Configuration/__pycache__/CMessages.cpython-35.pyc
--rw-r--r--   0        0        0      190 2019-12-19 08:45:08.630442 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Configuration/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      198 2021-07-02 09:46:25.866961 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Configuration/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.650007 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Exceptions/__init__.py
--rw-r--r--   0        0        0      187 2019-12-19 08:45:08.743446 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Exceptions/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      195 2021-07-02 09:46:25.875961 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Exceptions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    14323 2022-10-10 08:13:17.509686 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py
--rw-r--r--   0        0        0     1529 2021-07-02 09:46:22.671006 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py
--rw-r--r--   0        0        0     5944 2022-10-10 08:13:17.713686 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.690003 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py
--rw-r--r--   0        0        0     5881 2020-01-07 12:21:09.645401 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/CParseMCNPCell.cpython-35.pyc
--rw-r--r--   0        0        0     5603 2020-01-17 14:59:37.351769 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/CParseMCNPCell.cpython-38.pyc
--rw-r--r--   0        0        0    12349 2020-04-06 15:13:18.631712 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/ParseMCNPCell.cpython-35.pyc
--rw-r--r--   0        0        0    10614 2022-10-10 08:15:13.330383 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/ParseMCNPCell.cpython-38.pyc
--rw-r--r--   0        0        0     1047 2020-04-06 15:13:19.250703 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/ParseMCNPComposition.cpython-35.pyc
--rw-r--r--   0        0        0      927 2021-07-02 09:46:25.636963 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/ParseMCNPComposition.cpython-38.pyc
--rw-r--r--   0        0        0     4508 2020-04-06 16:22:52.843064 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/ParseMCNPSurface.cpython-35.pyc
--rw-r--r--   0        0        0     4269 2022-10-10 08:15:10.979419 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/ParseMCNPSurface.cpython-38.pyc
--rw-r--r--   0        0        0      196 2019-09-18 15:20:04.607456 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      204 2021-07-02 09:46:25.174968 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1434 2021-07-02 09:46:22.693002 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py
--rw-r--r--   0        0        0     2865 2022-10-10 08:13:17.984694 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py
--rw-r--r--   0        0        0     1432 2021-07-02 09:46:22.698001 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py
--rw-r--r--   0        0        0     5847 2022-10-10 08:13:18.290686 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.703007 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py
--rw-r--r--   0        0        0      964 2019-09-18 15:20:07.291405 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4BoundCond.cpython-35.pyc
--rw-r--r--   0        0        0      792 2021-07-02 09:46:25.703964 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4BoundCond.cpython-38.pyc
--rw-r--r--   0        0        0     1983 2020-04-06 15:13:19.193703 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4Composition.cpython-35.pyc
--rw-r--r--   0        0        0     1651 2022-10-10 08:15:15.726396 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4Composition.cpython-38.pyc
--rw-r--r--   0        0        0      904 2019-09-18 15:20:07.229408 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4GeomComp.cpython-35.pyc
--rw-r--r--   0        0        0      764 2021-07-02 09:46:25.678964 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4GeomComp.cpython-38.pyc
--rw-r--r--   0        0        0     2681 2020-04-06 15:13:17.572728 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4Geometry.cpython-35.pyc
--rw-r--r--   0        0        0     3002 2022-10-10 08:14:52.259560 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/WriteT4Geometry.cpython-38.pyc
--rw-r--r--   0        0        0      196 2019-09-18 15:20:04.426444 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      204 2021-07-02 09:46:25.062969 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.706999 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/__init__.py
--rw-r--r--   0        0        0      189 2019-09-18 15:20:04.412447 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      197 2021-07-02 09:46:25.056970 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1493 2021-07-02 09:46:22.710003 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py
--rw-r--r--   0        0        0     1122 2021-07-02 09:46:22.712006 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py
--rw-r--r--   0        0        0     2047 2021-07-02 09:46:22.714010 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.717010 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__init__.py
--rw-r--r--   0        0        0     1718 2019-09-18 15:20:07.277403 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/CDictGeomCompT4.cpython-35.pyc
--rw-r--r--   0        0        0     1559 2021-07-02 09:46:25.694962 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/CDictGeomCompT4.cpython-38.pyc
--rw-r--r--   0        0        0      824 2020-04-06 15:13:19.350718 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/CGeomCompT4.cpython-35.pyc
--rw-r--r--   0        0        0      693 2021-07-02 09:46:25.698967 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/CGeomCompT4.cpython-38.pyc
--rw-r--r--   0        0        0     1451 2020-01-07 12:21:10.364400 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/ConstructGeomCompT4.cpython-35.pyc
--rw-r--r--   0        0        0     1226 2021-07-02 09:46:25.689962 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/ConstructGeomCompT4.cpython-38.pyc
--rw-r--r--   0        0        0      185 2019-09-18 15:20:07.259409 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      193 2021-07-02 09:46:25.684960 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2259 2022-10-10 08:13:18.524687 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Progress.py
--rw-r--r--   0        0        0     1366 2021-07-02 09:46:22.722010 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py
--rw-r--r--   0        0        0     7036 2022-10-10 08:13:18.848685 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/CollectionDict.py
--rw-r--r--   0        0        0     1247 2022-02-23 12:53:03.770956 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py
--rw-r--r--   0        0        0     9136 2022-10-10 08:13:19.083688 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py
--rw-r--r--   0        0        0     2721 2021-07-02 09:46:22.735005 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/DTypeConversion.py
--rw-r--r--   0        0        0     2317 2022-02-23 15:04:09.442326 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/Duplicates.py
--rw-r--r--   0        0        0     1597 2022-10-10 08:13:19.356675 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py
--rw-r--r--   0        0        0     1011 2021-07-02 09:46:22.743001 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py
--rw-r--r--   0        0        0    14833 2022-10-10 08:13:19.683699 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/MacroBodies.py
--rw-r--r--   0        0        0     2344 2022-10-10 08:13:19.918672 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceCollection.py
--rw-r--r--   0        0        0      944 2021-07-02 09:46:22.750006 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py
--rw-r--r--   0        0        0     1881 2022-10-10 08:13:20.152669 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py
--rw-r--r--   0        0        0     3786 2022-10-10 08:13:20.360676 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.758998 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__init__.py
--rw-r--r--   0        0        0     1850 2019-09-18 15:20:04.583444 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CDictSurfaceMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     1811 2020-01-17 14:53:12.260434 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CDictSurfaceMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     1688 2019-09-18 15:20:04.735442 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CDictSurfaceT4.cpython-35.pyc
--rw-r--r--   0        0        0     1657 2020-01-17 14:53:12.579424 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CDictSurfaceT4.cpython-38.pyc
--rw-r--r--   0        0        0      560 2020-01-16 15:13:50.268442 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CSurfaceCollection.cpython-35.pyc
--rw-r--r--   0        0        0     1595 2020-01-07 12:21:09.179419 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CSurfaceMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     1563 2020-01-17 14:53:12.335439 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CSurfaceMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     1206 2020-01-07 12:21:09.542404 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CSurfaceT4.cpython-35.pyc
--rw-r--r--   0        0        0     1184 2020-01-17 14:53:12.590423 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CSurfaceT4.cpython-38.pyc
--rw-r--r--   0        0        0     1089 2019-12-19 08:45:09.087442 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CTransformationMCNP.cpython-35.pyc
--rw-r--r--   0        0        0      942 2021-07-02 09:46:25.953970 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CTransformationMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     7096 2022-10-10 08:15:05.983458 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/CollectionDict.cpython-38.pyc
--rw-r--r--   0        0        0     1835 2020-04-06 15:13:17.737727 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ConstructSurfaceT4.cpython-35.pyc
--rw-r--r--   0        0        0      657 2022-02-23 12:57:07.420004 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ConstructSurfaceT4.cpython-38.pyc
--rw-r--r--   0        0        0     5666 2020-04-06 15:13:17.774725 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ConversionSurfaceMCNPToT4.cpython-35.pyc
--rw-r--r--   0        0        0     6846 2022-10-10 08:14:53.030523 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ConversionSurfaceMCNPToT4.cpython-38.pyc
--rw-r--r--   0        0        0     1118 2019-09-18 15:20:04.760442 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/DTypeConversion.cpython-35.pyc
--rw-r--r--   0        0        0      976 2021-07-02 09:46:25.971973 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/DTypeConversion.cpython-38.pyc
--rw-r--r--   0        0        0     2512 2020-04-06 15:13:18.473718 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/Duplicates.cpython-35.pyc
--rw-r--r--   0        0        0     1727 2022-02-23 15:04:12.486335 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/Duplicates.cpython-38.pyc
--rw-r--r--   0        0        0     1068 2020-04-06 15:13:17.986725 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ESurfaceTypeMCNP.cpython-35.pyc
--rw-r--r--   0        0        0      924 2022-10-10 08:15:05.739442 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ESurfaceTypeMCNP.cpython-38.pyc
--rw-r--r--   0        0        0      462 2019-09-18 15:20:04.767441 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ESurfaceTypeT4.cpython-35.pyc
--rw-r--r--   0        0        0      367 2021-07-02 09:46:25.157975 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/ESurfaceTypeT4.cpython-38.pyc
--rw-r--r--   0        0        0    12066 2020-01-15 15:59:19.921453 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/MacroBodies.cpython-35-pytest-5.3.2.pyc
--rw-r--r--   0        0        0    12644 2020-04-06 15:13:18.423715 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/MacroBodies.cpython-35.pyc
--rw-r--r--   0        0        0    11562 2022-10-10 08:15:12.656400 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/MacroBodies.cpython-38.pyc
--rw-r--r--   0        0        0     2020 2020-04-06 15:13:18.450721 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceCollection.cpython-35.pyc
--rw-r--r--   0        0        0     2587 2022-10-10 08:15:10.250407 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceCollection.cpython-38.pyc
--rw-r--r--   0        0        0      502 2021-07-02 09:46:25.169974 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceConversionError.cpython-38.pyc
--rw-r--r--   0        0        0     1490 2020-04-06 16:22:52.875070 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     1333 2022-10-10 08:15:11.629399 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     1878 2020-04-06 16:22:53.055062 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceT4.cpython-35.pyc
--rw-r--r--   0        0        0     3084 2022-10-10 08:15:10.012436 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/SurfaceT4.cpython-38.pyc
--rw-r--r--   0        0        0      184 2019-09-18 15:20:04.528444 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      192 2021-07-02 09:46:25.079972 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    16384 2022-10-10 08:23:04.576666 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/.Transformation.py.swp
--rw-r--r--   0        0        0    16355 2022-10-10 08:13:20.626679 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/Transformation.py
--rw-r--r--   0        0        0      988 2021-07-02 09:46:22.781001 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/TransformationError.py
--rw-r--r--   0        0        0     2931 2022-10-10 08:13:20.825327 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/TransformationQuad.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.786998 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__init__.py
--rw-r--r--   0        0        0     1140 2019-09-18 15:20:05.045436 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/CSurfaceTransformed.cpython-35.pyc
--rw-r--r--   0        0        0     2237 2019-09-18 15:20:05.068435 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/CTransformationQuad.cpython-35.pyc
--rw-r--r--   0        0        0     2533 2019-09-18 15:38:13.845507 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/ConversionSurfaceTransformed.cpython-35.pyc
--rw-r--r--   0        0        0     1207 2019-09-18 15:20:04.882439 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/SurfaceTransformed.cpython-35.pyc
--rw-r--r--   0        0        0     2290 2020-04-06 16:22:52.890068 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/Transformation.cpython-35.pyc
--rw-r--r--   0        0        0    15278 2022-08-05 14:13:18.940129 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/Transformation.cpython-38-pytest-6.2.2.pyc
--rw-r--r--   0        0        0    15165 2022-10-10 08:15:12.001414 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/Transformation.cpython-38.pyc
--rw-r--r--   0        0        0      552 2020-04-06 15:13:18.304721 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/TransformationError.cpython-35.pyc
--rw-r--r--   0        0        0      550 2021-07-02 09:46:25.375971 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/TransformationError.cpython-38.pyc
--rw-r--r--   0        0        0     1886 2020-04-06 15:13:18.038726 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/TransformationQuad.cpython-35.pyc
--rw-r--r--   0        0        0     1621 2022-10-10 08:15:12.289409 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/TransformationQuad.cpython-38.pyc
--rw-r--r--   0        0        0      191 2019-09-18 15:20:04.826441 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      199 2021-07-02 09:46:25.206978 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2263 2021-07-05 09:19:23.949984 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Utils.py
--rw-r--r--   0        0        0    10819 2022-10-10 08:13:21.083311 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/VectUtils.py
--rw-r--r--   0        0        0     1204 2021-07-02 09:46:22.795998 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/ByUniverse.py
--rw-r--r--   0        0        0    21087 2022-10-11 13:22:21.150480 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellConversion.py
--rw-r--r--   0        0        0      983 2021-07-02 09:46:22.801001 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellConversionError.py
--rw-r--r--   0        0        0     4651 2021-07-02 09:46:22.803998 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellInlining.py
--rw-r--r--   0        0        0     3129 2022-10-11 13:22:21.171477 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellMCNP.py
--rw-r--r--   0        0        0     7680 2022-10-10 08:13:21.840663 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py
--rw-r--r--   0        0        0     1628 2021-07-02 09:46:22.823001 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/DictVolumeT4.py
--rw-r--r--   0        0        0    22672 2022-10-10 08:13:22.211665 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/Lattice.py
--rw-r--r--   0        0        0     3379 2021-07-02 09:46:22.828006 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/TreeFunctions.py
--rw-r--r--   0        0        0     2745 2022-10-10 08:13:22.410655 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/VolumeT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.834004 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__init__.py
--rw-r--r--   0        0        0      773 2020-01-07 12:21:10.049402 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/ByUniverse.cpython-35.pyc
--rw-r--r--   0        0        0      644 2021-07-02 09:46:25.591962 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/ByUniverse.cpython-38.pyc
--rw-r--r--   0        0        0    13312 2020-01-16 16:03:51.980108 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CCellConversion.cpython-35.pyc
--rw-r--r--   0        0        0    11611 2020-02-03 22:51:10.134239 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CCellConversion.cpython-38.pyc
--rw-r--r--   0        0        0     2669 2020-01-07 12:21:09.899402 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CCellMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     2553 2020-01-17 14:53:12.883424 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CCellMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     1897 2020-01-07 12:21:09.624402 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CDictCellMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     1802 2020-02-03 16:33:12.460702 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CDictCellMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     1799 2019-09-18 15:20:06.492417 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CDictVolumeT4.cpython-35.pyc
--rw-r--r--   0        0        0     1770 2020-01-17 14:53:12.634430 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CDictVolumeT4.cpython-38.pyc
--rw-r--r--   0        0        0     1151 2019-09-18 15:20:06.976420 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CUniverseDict.cpython-35.pyc
--rw-r--r--   0        0        0     2424 2020-01-07 12:21:10.031407 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CVolumeT4.cpython-35.pyc
--rw-r--r--   0        0        0     2301 2020-01-17 14:53:12.919423 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CVolumeT4.cpython-38.pyc
--rw-r--r--   0        0        0    13081 2020-04-06 16:24:51.202372 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellConversion.cpython-35.pyc
--rw-r--r--   0        0        0    14187 2022-10-11 13:13:07.200337 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellConversion.cpython-38.pyc
--rw-r--r--   0        0        0      537 2021-07-02 09:46:25.587964 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellConversionError.cpython-38.pyc
--rw-r--r--   0        0        0     3873 2021-03-05 16:48:03.159386 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellInlining.cpython-38-pytest-5.3.5.pyc
--rw-r--r--   0        0        0     3780 2021-07-02 09:46:25.596966 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellInlining.cpython-38.pyc
--rw-r--r--   0        0        0     2660 2020-04-06 15:13:19.061709 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellMCNP.cpython-35.pyc
--rw-r--r--   0        0        0     2831 2022-10-10 08:15:14.061382 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/CellMCNP.cpython-38.pyc
--rw-r--r--   0        0        0     6536 2020-04-06 16:25:49.852533 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/ConstructVolumeT4.cpython-35.pyc
--rw-r--r--   0        0        0     6533 2022-10-10 08:15:13.114418 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/ConstructVolumeT4.cpython-38.pyc
--rw-r--r--   0        0        0     2265 2020-04-06 15:13:19.132704 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/DictVolumeT4.cpython-35.pyc
--rw-r--r--   0        0        0     1748 2021-07-02 09:46:25.565962 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/DictVolumeT4.cpython-38.pyc
--rw-r--r--   0        0        0    11730 2019-11-20 18:37:32.851969 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/Lattice.cpython-35-pytest-5.3.0.pyc
--rw-r--r--   0        0        0    22948 2020-04-06 15:13:19.088730 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/Lattice.cpython-35.pyc
--rw-r--r--   0        0        0    22058 2022-10-10 08:15:14.311398 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/Lattice.cpython-38.pyc
--rw-r--r--   0        0        0     2591 2020-04-06 15:13:19.166710 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/TreeFunctions.cpython-35.pyc
--rw-r--r--   0        0        0     3235 2021-03-01 13:35:43.486749 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/TreeFunctions.cpython-38-pytest-5.3.5.pyc
--rw-r--r--   0        0        0     2892 2021-07-02 09:46:25.578967 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/TreeFunctions.cpython-38.pyc
--rw-r--r--   0        0        0     2402 2020-04-06 15:13:19.178705 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/VolumeT4.cpython-35.pyc
--rw-r--r--   0        0        0     2379 2022-10-10 08:15:15.145384 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/VolumeT4.cpython-38.pyc
--rw-r--r--   0        0        0      183 2019-09-18 15:20:06.461418 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      191 2021-07-02 09:46:25.396969 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.837000 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__init__.py
--rw-r--r--   0        0        0     5553 2020-04-06 15:13:19.120703 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/MCNPDataCards.cpython-35.pyc
--rw-r--r--   0        0        0     5193 2020-04-08 10:37:30.472967 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/MCNPDataCards.cpython-38.pyc
--rw-r--r--   0        0        0     1662 2022-10-10 08:14:52.531535 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/Progress.cpython-38.pyc
--rw-r--r--   0        0        0     1760 2021-07-02 15:46:22.966327 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/Utils.cpython-38-pytest-6.2.2.pyc
--rw-r--r--   0        0        0     1644 2021-12-08 09:19:46.862178 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/Utils.cpython-38.pyc
--rw-r--r--   0        0        0     8419 2020-04-06 15:13:18.369717 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/VectUtils.cpython-35.pyc
--rw-r--r--   0        0        0     4852 2020-01-17 16:57:29.047603 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/VectUtils.cpython-38-pytest-5.3.3.pyc
--rw-r--r--   0        0        0    10210 2022-10-10 08:15:10.576431 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/VectUtils.cpython-38.pyc
--rw-r--r--   0        0        0      176 2019-09-18 15:20:04.387445 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0        0        0      184 2021-07-02 09:46:25.050981 t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      960 2021-07-02 09:46:22.856998 t4_geom_convert-0.6.1/t4_geom_convert/__init__.py
--rw-r--r--   0        0        0     8289 2022-10-10 08:13:23.503675 t4_geom_convert-0.6.1/t4_geom_convert/conftest.py
--rw-r--r--   0        0        0     9457 2022-10-10 08:13:23.759324 t4_geom_convert-0.6.1/t4_geom_convert/main.py
--rw-r--r--   0        0        0      354 2020-02-20 16:30:10.454898 t4_geom_convert-0.6.1/t4_geom_convert/tmp_GEOMCOMP_Iphi.imcnp.t4
--rw-r--r--   0        0        0       42 2020-02-20 12:26:48.014349 t4_geom_convert-0.6.1/t4_geom_convert/tmp_GEOMCOMP_chars.imcnp.t4
--rw-r--r--   0        0        0    12264 2022-10-11 13:25:10.958101 t4_geom_convert-0.6.1/setup.py
--rw-r--r--   0        0        0    11373 2022-10-11 13:25:10.961438 t4_geom_convert-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2020-01-07 12:20:18.320103 t4_geom_convert-0.6.2/MIP/LICENSE
+-rw-r--r--   0        0        0        0 2019-07-23 12:07:01.746772 t4_geom_convert-0.6.2/MIP/__init__.py
+-rw-r--r--   0        0        0        0 2019-07-23 12:06:54.208901 t4_geom_convert-0.6.2/MIP/geom/__init__.py
+-rw-r--r--   0        0        0     2427 2021-07-05 09:19:23.710002 t4_geom_convert-0.6.2/MIP/geom/another_parser.py
+-rw-r--r--   0        0        0     1393 2020-02-21 09:29:30.758624 t4_geom_convert-0.6.2/MIP/geom/cells.py
+-rw-r--r--   0        0        0      551 2021-07-02 09:46:22.102009 t4_geom_convert-0.6.2/MIP/geom/composition.py
+-rw-r--r--   0        0        0     2461 2019-07-23 12:06:54.244872 t4_geom_convert-0.6.2/MIP/geom/copt.py
+-rw-r--r--   0        0        0    14112 2022-02-25 21:02:37.966808 t4_geom_convert-0.6.2/MIP/geom/forcad.py
+-rw-r--r--   0        0        0      364 2019-07-23 12:06:54.262904 t4_geom_convert-0.6.2/MIP/geom/grammars/__init__.py
+-rw-r--r--   0        0        0      340 2021-07-02 09:46:22.107010 t4_geom_convert-0.6.2/MIP/geom/grammars/geom.ebnf
+-rw-r--r--   0        0        0     1699 2020-02-21 09:29:30.776628 t4_geom_convert-0.6.2/MIP/geom/grammars/multioperand.py
+-rw-r--r--   0        0        0     3615 2019-07-23 12:07:01.770768 t4_geom_convert-0.6.2/MIP/geom/main.py
+-rw-r--r--   0        0        0     2704 2020-02-21 09:29:30.780622 t4_geom_convert-0.6.2/MIP/geom/parsegeom.py
+-rw-r--r--   0        0        0     3057 2021-07-05 09:19:23.713988 t4_geom_convert-0.6.2/MIP/geom/semantics.py
+-rw-r--r--   0        0        0      859 2021-07-05 09:19:23.716988 t4_geom_convert-0.6.2/MIP/geom/surfaces.py
+-rw-r--r--   0        0        0     1394 2019-07-23 12:06:54.360873 t4_geom_convert-0.6.2/MIP/geom/testgrammar.py
+-rw-r--r--   0        0        0     1756 2022-03-03 10:29:08.794011 t4_geom_convert-0.6.2/MIP/geom/transforms.py
+-rw-r--r--   0        0        0       49 2019-07-23 12:06:54.390871 t4_geom_convert-0.6.2/MIP/mip/__init__.py
+-rw-r--r--   0        0        0     3088 2021-07-05 09:19:23.719998 t4_geom_convert-0.6.2/MIP/mip/blocks.py
+-rw-r--r--   0        0        0     3697 2021-07-02 09:46:22.156011 t4_geom_convert-0.6.2/MIP/mip/cards.py
+-rw-r--r--   0        0        0     3035 2021-07-05 09:19:23.723003 t4_geom_convert-0.6.2/MIP/mip/cellcard.py
+-rw-r--r--   0        0        0     5144 2021-07-05 09:19:23.726989 t4_geom_convert-0.6.2/MIP/mip/datacard.py
+-rw-r--r--   0        0        0     4830 2021-07-05 09:19:23.729992 t4_geom_convert-0.6.2/MIP/mip/main.py
+-rw-r--r--   0        0        0      985 2019-07-23 12:06:54.506881 t4_geom_convert-0.6.2/MIP/mip/readme.rst
+-rw-r--r--   0        0        0      386 2019-07-23 12:06:54.509911 t4_geom_convert-0.6.2/MIP/mip/surfacecard.py
+-rw-r--r--   0        0        0      763 2019-07-23 12:06:54.516881 t4_geom_convert-0.6.2/MIP/mip/utils.py
+-rw-r--r--   0        0        0     1073 2019-07-23 12:06:54.553872 t4_geom_convert-0.6.2/MIP/tests.py
+-rw-r--r--   0        0        0    10140 2021-07-02 09:46:22.246004 t4_geom_convert-0.6.2/README.md
+-rw-r--r--   0        0        0     4372 2023-03-29 15:20:02.237350 t4_geom_convert-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      966 2021-07-02 09:46:22.608020 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py
+-rw-r--r--   0        0        0     2192 2021-07-02 09:46:22.611003 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.614004 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/BoundaryCondition/__init__.py
+-rw-r--r--   0        0        0     1698 2022-10-10 08:13:16.765702 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/Abundances.py
+-rw-r--r--   0        0        0     1784 2021-07-02 09:46:22.620008 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py
+-rw-r--r--   0        0        0     1273 2021-07-02 09:46:22.623004 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CCompositionT4.py
+-rw-r--r--   0        0        0     1692 2021-07-02 09:46:22.626003 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py
+-rw-r--r--   0        0        0     3224 2022-10-10 08:13:16.985692 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py
+-rw-r--r--   0        0        0     4271 2022-10-10 08:13:17.228693 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py
+-rw-r--r--   0        0        0     1165 2021-07-02 09:46:22.635003 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/ConvertIsotope.py
+-rw-r--r--   0        0        0     1483 2021-07-02 09:46:22.637009 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py
+-rw-r--r--   0        0        0     1419 2021-07-02 09:46:22.640000 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.643003 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/__init__.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.646013 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Configuration/__init__.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.650007 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Exceptions/__init__.py
+-rw-r--r--   0        0        0    14497 2023-03-29 15:17:12.426391 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py
+-rw-r--r--   0        0        0     1529 2021-07-02 09:46:22.671006 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py
+-rw-r--r--   0        0        0     5944 2022-10-10 08:13:17.713686 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.690003 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py
+-rw-r--r--   0        0        0     1434 2021-07-02 09:46:22.693002 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py
+-rw-r--r--   0        0        0     2865 2022-10-10 08:13:17.984694 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py
+-rw-r--r--   0        0        0     1432 2021-07-02 09:46:22.698001 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py
+-rw-r--r--   0        0        0     5847 2022-10-10 08:13:18.290686 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.703007 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.706999 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/__init__.py
+-rw-r--r--   0        0        0     1493 2021-07-02 09:46:22.710003 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py
+-rw-r--r--   0        0        0     1122 2021-07-02 09:46:22.712006 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py
+-rw-r--r--   0        0        0     2047 2021-07-02 09:46:22.714010 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.717010 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/__init__.py
+-rw-r--r--   0        0        0     2259 2022-10-10 08:13:18.524687 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Progress.py
+-rw-r--r--   0        0        0     1366 2021-07-02 09:46:22.722010 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py
+-rw-r--r--   0        0        0     7036 2022-10-10 08:13:18.848685 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/CollectionDict.py
+-rw-r--r--   0        0        0     1247 2022-02-23 12:53:03.770956 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py
+-rw-r--r--   0        0        0     9136 2022-10-10 08:13:19.083688 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py
+-rw-r--r--   0        0        0     2721 2021-07-02 09:46:22.735005 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/DTypeConversion.py
+-rw-r--r--   0        0        0     2317 2022-02-23 15:04:09.442326 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/Duplicates.py
+-rw-r--r--   0        0        0     1597 2022-10-10 08:13:19.356675 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py
+-rw-r--r--   0        0        0     1011 2021-07-02 09:46:22.743001 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py
+-rw-r--r--   0        0        0    14833 2022-10-10 08:13:19.683699 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/MacroBodies.py
+-rw-r--r--   0        0        0     2344 2022-10-10 08:13:19.918672 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceCollection.py
+-rw-r--r--   0        0        0      944 2021-07-02 09:46:22.750006 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py
+-rw-r--r--   0        0        0     1881 2022-10-10 08:13:20.152669 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py
+-rw-r--r--   0        0        0     3786 2022-10-10 08:13:20.360676 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceT4.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.758998 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/__init__.py
+-rw-r--r--   0        0        0    16355 2022-10-10 08:13:20.626679 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/Transformation.py
+-rw-r--r--   0        0        0      988 2021-07-02 09:46:22.781001 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/TransformationError.py
+-rw-r--r--   0        0        0     2931 2022-10-10 08:13:20.825327 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/TransformationQuad.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.786998 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/__init__.py
+-rw-r--r--   0        0        0     2263 2021-07-05 09:19:23.949984 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Utils.py
+-rw-r--r--   0        0        0    10819 2022-10-10 08:13:21.083311 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/VectUtils.py
+-rw-r--r--   0        0        0     1204 2021-07-02 09:46:22.795998 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/ByUniverse.py
+-rw-r--r--   0        0        0    21087 2023-03-23 14:23:26.078094 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellConversion.py
+-rw-r--r--   0        0        0      983 2021-07-02 09:46:22.801001 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellConversionError.py
+-rw-r--r--   0        0        0     4651 2021-07-02 09:46:22.803998 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellInlining.py
+-rw-r--r--   0        0        0     3129 2023-03-23 14:23:25.791091 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellMCNP.py
+-rw-r--r--   0        0        0     7680 2022-10-10 08:13:21.840663 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py
+-rw-r--r--   0        0        0     1628 2021-07-02 09:46:22.823001 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/DictVolumeT4.py
+-rw-r--r--   0        0        0    22672 2023-03-28 11:54:19.358217 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/Lattice.py
+-rw-r--r--   0        0        0     3379 2021-07-02 09:46:22.828006 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/TreeFunctions.py
+-rw-r--r--   0        0        0     2745 2022-10-10 08:13:22.410655 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/VolumeT4.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.834004 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/__init__.py
+-rw-r--r--   0        0        0      792 2021-07-02 09:46:22.837000 t4_geom_convert-0.6.2/t4_geom_convert/Kernel/__init__.py
+-rw-r--r--   0        0        0      960 2021-07-02 09:46:22.856998 t4_geom_convert-0.6.2/t4_geom_convert/__init__.py
+-rw-r--r--   0        0        0     8289 2022-10-10 08:13:23.503675 t4_geom_convert-0.6.2/t4_geom_convert/conftest.py
+-rw-r--r--   0        0        0     9457 2022-10-10 08:13:23.759324 t4_geom_convert-0.6.2/t4_geom_convert/main.py
+-rw-r--r--   0        0        0    11892 1970-01-01 00:00:00.000000 t4_geom_convert-0.6.2/setup.py
+-rw-r--r--   0        0        0    11472 1970-01-01 00:00:00.000000 t4_geom_convert-0.6.2/PKG-INFO
```

### Comparing `t4_geom_convert-0.6.1/MIP/LICENSE` & `t4_geom_convert-0.6.2/MIP/LICENSE`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/another_parser.py` & `t4_geom_convert-0.6.2/MIP/geom/another_parser.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/cells.py` & `t4_geom_convert-0.6.2/MIP/geom/cells.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/composition.py` & `t4_geom_convert-0.6.2/MIP/geom/composition.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/copt.py` & `t4_geom_convert-0.6.2/MIP/geom/copt.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/forcad.py` & `t4_geom_convert-0.6.2/MIP/geom/forcad.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/grammars/multioperand.py` & `t4_geom_convert-0.6.2/MIP/geom/grammars/multioperand.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/main.py` & `t4_geom_convert-0.6.2/MIP/geom/main.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/parsegeom.py` & `t4_geom_convert-0.6.2/MIP/geom/parsegeom.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/semantics.py` & `t4_geom_convert-0.6.2/MIP/geom/semantics.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/surfaces.py` & `t4_geom_convert-0.6.2/MIP/geom/surfaces.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/testgrammar.py` & `t4_geom_convert-0.6.2/MIP/geom/testgrammar.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/geom/transforms.py` & `t4_geom_convert-0.6.2/MIP/geom/transforms.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/mip/__pycache__/cards.cpython-38.pyc` & `t4_geom_convert-0.6.2/MIP/mip/cards.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,232 @@
-00000000: 550d 0d0a 0000 0000 6ee0 de60 710e 0000  U.......n..`q...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
-00000030: 6401 6c00 5a00 6500 a001 6402 a101 5a02  d.l.Z.e...d...Z.
-00000040: 6500 a001 6403 a101 5a03 6500 a001 6404  e...d...Z.e...d.
-00000050: a101 5a04 6405 6406 8400 5a05 640e 6408  ..Z.d.d...Z.d.d.
-00000060: 6409 8401 5a06 640a 640b 8400 5a07 640f  d...Z.d.d...Z.d.
-00000070: 640c 640d 8401 5a08 6401 5300 2910 e900  d.d...Z.d.S.)...
-00000080: 0000 004e 7a12 5e5c 737b 302c 347d 5b63  ...Nz.^\s{0,4}[c
-00000090: 435d 285c 737c 2429 7a07 5e5c 737b 352c  C](\s|$)z.^\s{5,
-000000a0: 7d7a 125b 5e24 5d2a 265c 732a 2824 7c5c  }z.[^$]*&\s*($|\
-000000b0: 242e 2a24 2963 0500 0000 0000 0000 0000  $.*$)c..........
-000000c0: 0000 0500 0000 0300 0000 6300 0000 7328  ..........c...s(
-000000d0: 0000 007c 0072 107c 007c 0164 0166 0356  ...|.r.|.|.d.f.V
-000000e0: 0001 007c 0273 247c 0372 247c 037c 0464  ...|.s$|.r$|.|.d
-000000f0: 0266 0356 0001 0064 0053 0029 034e da04  .f.V...d.S.).N..
-00000100: 6361 7264 da04 636d 6e74 a900 2905 5a02  card..cmnt..).Z.
-00000110: 6331 5a02 6e31 da01 665a 0263 325a 026e  c1Z.n1..fZ.c2Z.n
-00000120: 3272 0400 0000 7204 0000 00fa 4b2f 6461  2r....r.....K/da
-00000130: 7461 2f74 6d70 646d 3273 2f64 6d32 3332  ta/tmpdm2s/dm232
-00000140: 3130 372f 7372 632f 7434 5f67 656f 6d5f  107/src/t4_geom_
-00000150: 636f 6e76 6572 742f 7434 5f67 656f 6d5f  convert/t4_geom_
-00000160: 636f 6e76 6572 742f 4d49 502f 6d69 702f  convert/MIP/mip/
-00000170: 6361 7264 732e 7079 da06 5f79 6965 6c64  cards.py.._yield
-00000180: 0f00 0000 7308 0000 0000 0104 010c 0108  ....s...........
-00000190: 0172 0700 0000 4663 0200 0000 0000 0000  .r....Fc........
-000001a0: 0000 0000 0a00 0000 0700 0000 6300 0000  ............c...
-000001b0: 73ca 0000 0067 007d 0267 007d 0364 017d  s....g.}.g.}.d.}
-000001c0: 0464 017d 0564 027d 0674 007c 00a0 01a1  .d.}.d.}.t.|....
-000001d0: 0083 0144 005d 885c 027d 077d 0874 02a0  ...D.].\.}.}.t..
-000001e0: 037c 08a1 0172 3e7c 02a0 047c 08a1 0101  .|...r>|...|....
-000001f0: 0071 2074 057c 087c 0683 0272 727c 0173  .q t.|.|...rr|.s
-00000200: 567c 03a0 067c 02a1 0101 0067 007d 027c  V|...|.....g.}.|
-00000210: 0764 0317 007d 057c 03a0 047c 08a1 0101  .d...}.|...|....
-00000220: 007c 087d 0671 2074 077c 037c 047c 017c  .|.}.q t.|.|.|.|
-00000230: 027c 0583 0544 005d 0a7d 097c 0956 0001  .|...D.].}.|.V..
-00000240: 0071 8267 007d 027c 0764 0317 007d 057c  .q.g.}.|.d...}.|
-00000250: 0867 017d 037c 077d 047c 087d 0671 2074  .g.}.|.}.|.}.q t
-00000260: 077c 037c 047c 017c 027c 0583 0544 005d  .|.|.|.|.|...D.]
-00000270: 0a7d 097c 0956 0001 0071 ba64 0253 0029  .}.|.V...q.d.S.)
-00000280: 0461 4003 0000 0a20 2020 2053 706c 6974  .a@....    Split
-00000290: 2074 6578 7420 696e 2060 626c 6f63 6b60   text in `block`
-000002a0: 2069 6e74 6f20 6361 7264 732e 2052 6574   into cards. Ret
-000002b0: 7572 6e20 6361 7264 2074 6578 742c 206c  urn card text, l
-000002c0: 696e 6520 6e75 6d62 6572 2069 6e20 7468  ine number in th
-000002d0: 6520 626c 6f63 6b0a 2020 2020 616e 6420  e block.    and 
-000002e0: 7479 7065 2028 2763 6172 6427 206f 7220  type ('card' or 
-000002f0: 2763 6d6e 7427 292e 0a0a 2020 2020 5468  'cmnt')...    Th
-00000300: 6520 6062 6c6f 636b 6020 7265 7072 6573  e `block` repres
-00000310: 656e 7473 206f 6e65 2062 6c6f 636b 206f  ents one block o
-00000320: 6620 4d43 4e50 2069 6e70 7574 2066 696c  f MCNP input fil
-00000330: 652c 2077 6869 6368 2069 6e20 6765 6e65  e, which in gene
-00000340: 7261 6c0a 2020 2020 636f 6e73 6973 7473  ral.    consists
-00000350: 206f 6620 6f6e 6520 6f72 206d 6f72 6520   of one or more 
-00000360: 6361 7264 7320 616e 6420 7a65 726f 206f  cards and zero o
-00000370: 7220 6d6f 7265 2063 6f6d 6d65 6e74 206c  r more comment l
-00000380: 696e 6573 2e0a 0a20 2020 2044 6566 696e  ines...    Defin
-00000390: 6974 696f 6e3a 2043 2d63 6f6d 6d65 6e74  ition: C-comment
-000003a0: 2069 7320 6120 636f 6d6d 656e 7420 6c69   is a comment li
-000003b0: 6e65 2069 6e73 6964 6520 6120 6361 7264  ne inside a card
-000003c0: 2e20 422d 636f 6d6d 656e 7420 6973 2061  . B-comment is a
-000003d0: 0a20 2020 2063 6f6d 6d65 6e74 206c 696e  .    comment lin
-000003e0: 6520 6265 7477 6565 6e20 6361 7264 732c  e between cards,
-000003f0: 2069 2e65 2e20 6162 6f76 6520 7468 6520   i.e. above the 
-00000400: 6c69 6e65 2077 6865 7265 2074 6865 206e  line where the n
-00000410: 6578 7420 6361 7264 2062 6567 696e 732e  ext card begins.
-00000420: 0a20 2020 2053 6576 6572 616c 206c 696e  .    Several lin
-00000430: 6573 2077 6974 6820 422d 636f 6d6d 656e  es with B-commen
-00000440: 7473 2063 6f6d 706f 7365 2061 206d 756c  ts compose a mul
-00000450: 7469 2d6c 696e 6520 422d 636f 6d6d 656e  ti-line B-commen
-00000460: 742e 0a0a 2020 2020 5468 6520 432d 636f  t...    The C-co
-00000470: 6d6d 656e 7473 2061 7265 2072 6574 7572  mments are retur
-00000480: 6e65 6420 7769 7468 696e 2063 6172 6473  ned within cards
-00000490: 2e20 5468 6520 422d 636f 6d6d 656e 7473  . The B-comments
-000004a0: 2061 7265 2072 6574 7572 6e65 640a 2020   are returned.  
-000004b0: 2020 7365 7061 7261 7465 6c79 2c20 7768    separately, wh
-000004c0: 656e 2074 6865 2060 736b 6970 636f 6d6d  en the `skipcomm
-000004d0: 656e 7473 6020 666c 6167 2069 7320 4661  ents` flag is Fa
-000004e0: 6c73 652e 2054 6875 732c 2054 776f 2074  lse. Thus, Two t
-000004f0: 7970 6573 206f 660a 2020 2020 656c 656d  ypes of.    elem
-00000500: 656e 7473 2061 7265 2072 6574 7572 6e65  ents are returne
-00000510: 643a 2063 6172 6473 2061 6e64 2042 2d63  d: cards and B-c
-00000520: 6f6d 6d65 6e74 732e 2042 6f74 6820 6172  omments. Both ar
-00000530: 652c 2067 656e 6572 616c 6c79 2c20 6d75  e, generally, mu
-00000540: 6c74 692d 6c69 6e65 0a20 2020 2073 7472  lti-line.    str
-00000550: 696e 6773 2e0a 0a20 2020 2041 2063 6172  ings...    A car
-00000560: 6420 6973 2061 2070 6172 7420 6f66 2074  d is a part of t
-00000570: 6865 2062 6c6f 636b 2063 6f6e 7461 696e  he block contain
-00000580: 696e 6720 616c 6c20 6c69 6e65 7320 6265  ing all lines be
-00000590: 6c6f 6e67 696e 6720 746f 2061 2063 6172  longing to a car
-000005a0: 642c 0a20 2020 2069 6e63 6c75 6469 6e67  d,.    including
-000005b0: 2074 6865 2043 2d63 6f6d 6d65 6e74 732e   the C-comments.
-000005c0: 0a0a 2020 2020 7201 0000 004e e901 0000  ..    r....N....
-000005d0: 0029 08da 0965 6e75 6d65 7261 7465 da0a  .)...enumerate..
-000005e0: 7370 6c69 746c 696e 6573 da0a 7265 5f63  splitlines..re_c
-000005f0: 6f6d 6d65 6e74 da05 6d61 7463 68da 0661  omment..match..a
-00000600: 7070 656e 64da 0f69 735f 636f 6e74 696e  ppend..is_contin
-00000610: 7561 7469 6f6e da06 6578 7465 6e64 7207  uation..extendr.
-00000620: 0000 0029 0ada 0562 6c6f 636b da0c 736b  ...)...block..sk
-00000630: 6970 636f 6d6d 656e 7473 7203 0000 0072  ipcommentsr....r
-00000640: 0200 0000 5a06 6e5f 6361 7264 5a06 6e5f  ....Z.n_cardZ.n_
-00000650: 636d 6e74 5a05 6c70 7265 76da 016e da01  cmntZ.lprev..n..
-00000660: 6cda 0172 7204 0000 0072 0400 0000 7206  l..rr....r....r.
-00000670: 0000 00da 0967 6574 5f63 6172 6473 1600  .....get_cards..
-00000680: 0000 7330 0000 0000 1704 0204 0204 0104  ..s0............
-00000690: 0204 0114 060a 010c 010a 0104 010a 0104  ................
-000006a0: 0108 010a 0106 0314 0108 0104 0108 0106  ................
-000006b0: 0104 0106 0314 0172 1500 0000 6301 0000  .......r....c...
-000006c0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-000006d0: 0043 0000 0073 5a00 0000 6700 7d01 6401  .C...sZ...g.}.d.
-000006e0: 7d02 7c00 4400 5d42 7d03 7c03 6402 6b03  }.|.D.]B}.|.d.k.
-000006f0: 722c 7c01 a000 7c03 a101 0100 7c02 6403  r,|...|.....|.d.
-00000700: 3700 7d02 710c 6404 7c02 6404 1600 1800  7.}.q.d.|.d.....
-00000710: 7d04 7c01 a000 6405 7c04 1400 a101 0100  }.|...d.|.......
-00000720: 7c02 7c04 3700 7d02 710c 6406 a001 7c01  |.|.7.}.q.d...|.
-00000730: a101 5300 2907 61cd 0100 0045 7870 616e  ..S.).a....Expan
-00000740: 6420 7461 6273 2069 6e20 6120 6c69 6e65  d tabs in a line
-00000750: 2e0a 0a20 2020 2054 6865 204d 434e 5020  ...    The MCNP 
-00000760: 6d61 6e75 616c 2073 6179 7320 7468 6174  manual says that
-00000770: 2022 7461 6273 2061 7265 2072 6570 6c61   "tabs are repla
-00000780: 6365 6420 6279 2062 6c61 6e6b 7320 746f  ced by blanks to
-00000790: 2074 6865 206e 6578 740a 2020 2020 382d   the next.    8-
-000007a0: 6368 6172 6163 7465 7220 7461 6220 7374  character tab st
-000007b0: 6f70 2e0a 0a20 2020 203e 3e3e 2065 7870  op...    >>> exp
-000007c0: 616e 645f 7461 6273 2827 5c74 646f 646f  and_tabs('\tdodo
-000007d0: 2729 0a20 2020 2027 2020 2020 2020 2020  ').    '        
-000007e0: 646f 646f 270a 2020 2020 3e3e 3e20 6578  dodo'.    >>> ex
-000007f0: 7061 6e64 5f74 6162 7328 2720 205c 7464  pand_tabs('  \td
-00000800: 6f64 6f27 290a 2020 2020 2720 2020 2020  odo').    '     
-00000810: 2020 2064 6f64 6f27 0a20 2020 203e 3e3e     dodo'.    >>>
-00000820: 2065 7870 616e 645f 7461 6273 2827 2020   expand_tabs('  
-00000830: 2020 2020 5c74 646f 646f 2729 0a20 2020      \tdodo').   
-00000840: 2027 2020 2020 2020 2020 646f 646f 270a   '        dodo'.
-00000850: 2020 2020 3e3e 3e20 6578 7061 6e64 5f74      >>> expand_t
-00000860: 6162 7328 2720 2020 2020 2020 5c74 646f  abs('       \tdo
-00000870: 646f 2729 0a20 2020 2027 2020 2020 2020  do').    '      
-00000880: 2020 646f 646f 270a 2020 2020 3e3e 3e20    dodo'.    >>> 
-00000890: 6578 7061 6e64 5f74 6162 7328 2720 2020  expand_tabs('   
-000008a0: 2020 2020 205c 7464 6f64 6f27 290a 2020       \tdodo').  
-000008b0: 2020 2720 2020 2020 2020 2020 2020 2020    '             
-000008c0: 2020 2064 6f64 6f27 0a20 2020 203e 3e3e     dodo'.    >>>
-000008d0: 2065 7870 616e 645f 7461 6273 2827 5c74   expand_tabs('\t
-000008e0: 5c74 646f 646f 2729 0a20 2020 2027 2020  \tdodo').    '  
-000008f0: 2020 2020 2020 2020 2020 2020 2020 646f                do
-00000900: 646f 270a 2020 2020 7201 0000 00fa 0109  do'.    r.......
-00000910: 7208 0000 00e9 0800 0000 fa01 20da 0029  r........... ..)
-00000920: 0272 0d00 0000 da04 6a6f 696e 2905 da04  .r......join)...
-00000930: 6c69 6e65 5a08 6578 7061 6e64 6564 da01  lineZ.expanded..
-00000940: 69da 0463 6861 725a 086e 5f73 7061 6365  i..charZ.n_space
-00000950: 7372 0400 0000 7204 0000 0072 0600 0000  sr....r....r....
-00000960: da0b 6578 7061 6e64 5f74 6162 7353 0000  ..expand_tabsS..
-00000970: 0073 1400 0000 0013 0401 0401 0801 0801  .s..............
-00000980: 0a01 0a02 0c01 0e01 0a01 721e 0000 0063  ..........r....c
-00000990: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000009a0: 0300 0000 4300 0000 732c 0000 0074 007c  ....C...s,...t.|
-000009b0: 0083 017d 0074 01a0 027c 00a1 0172 1664  ...}.t...|...r.d
-000009c0: 0153 007c 0172 2874 03a0 027c 01a1 0172  .S.|.r(t...|...r
-000009d0: 2864 0153 0064 0253 0029 037a 570a 2020  (d.S.d.S.).zW.  
-000009e0: 2020 4368 6563 6b20 6966 206c 2069 7320    Check if l is 
-000009f0: 6120 636f 6e74 696e 7561 7469 6f6e 206c  a continuation l
-00000a00: 696e 652e 0a0a 2020 2020 6c20 616e 6420  ine...    l and 
-00000a10: 7072 6576 206d 7573 7420 6e6f 7420 6265  prev must not be
-00000a20: 2063 6f6d 6d65 6e74 206c 696e 6573 2e0a   comment lines..
-00000a30: 2020 2020 5446 2904 721e 0000 00da 1672      TF).r......r
-00000a40: 655f 636f 6e74 696e 7561 7469 6f6e 5f73  e_continuation_s
-00000a50: 7061 6365 7372 0c00 0000 da14 7265 5f63  pacesr......re_c
-00000a60: 6f6e 7469 6e75 6174 696f 6e5f 7072 6576  ontinuation_prev
-00000a70: 2902 7213 0000 00da 0470 7265 7672 0400  ).r......prevr..
-00000a80: 0000 7204 0000 0072 0600 0000 720e 0000  ..r....r....r...
-00000a90: 0072 0000 0073 0c00 0000 0008 0801 0a01  .r...s..........
-00000aa0: 0401 0e01 0401 720e 0000 0029 0146 2901  ......r....).F).
-00000ab0: 4e29 09da 0272 65da 0763 6f6d 7069 6c65  N)...re..compile
-00000ac0: 720b 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00000ad0: 0700 0000 7215 0000 0072 1e00 0000 720e  ....r....r....r.
-00000ae0: 0000 0072 0400 0000 7204 0000 0072 0400  ...r....r....r..
-00000af0: 0000 7206 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000b00: 3e04 0000 0073 0e00 0000 0805 0a01 0a01  >....s..........
-00000b10: 0a04 0807 0a3d 081f                      .....=..
+00000000: 2321 2f75 7372 2f62 696e 2f65 6e76 2070  #!/usr/bin/env p
+00000010: 7974 686f 6e0a 2320 2d2a 2d20 636f 6469  ython.# -*- codi
+00000020: 6e67 3a20 7574 662d 3820 2d2a 2d0a 0a69  ng: utf-8 -*-..i
+00000030: 6d70 6f72 7420 7265 0a0a 2222 220a 2222  mport re..""".""
+00000040: 220a 0a72 655f 636f 6d6d 656e 7420 3d20  "..re_comment = 
+00000050: 7265 2e63 6f6d 7069 6c65 2872 275e 5c73  re.compile(r'^\s
+00000060: 7b30 2c34 7d5b 6343 5d28 5c73 7c24 2927  {0,4}[cC](\s|$)'
+00000070: 290a 7265 5f63 6f6e 7469 6e75 6174 696f  ).re_continuatio
+00000080: 6e5f 7370 6163 6573 203d 2072 652e 636f  n_spaces = re.co
+00000090: 6d70 696c 6528 7227 5e5c 737b 352c 7d27  mpile(r'^\s{5,}'
+000000a0: 290a 7265 5f63 6f6e 7469 6e75 6174 696f  ).re_continuatio
+000000b0: 6e5f 7072 6576 203d 2072 652e 636f 6d70  n_prev = re.comp
+000000c0: 696c 6528 7227 5b5e 245d 2a26 5c73 2a28  ile(r'[^$]*&\s*(
+000000d0: 247c 5c24 2e2a 2429 2729 0a0a 0a23 2046  $|\$.*$)')...# F
+000000e0: 756e 6374 696f 6e20 7573 6564 2061 7420  unction used at 
+000000f0: 7477 6f20 706c 6163 6573 2062 656c 6f77  two places below
+00000100: 0a64 6566 205f 7969 656c 6428 6331 2c20  .def _yield(c1, 
+00000110: 6e31 2c20 662c 2063 322c 206e 3229 3a0a  n1, f, c2, n2):.
+00000120: 2020 2020 6966 2063 313a 0a20 2020 2020      if c1:.     
+00000130: 2020 2079 6965 6c64 2063 312c 206e 312c     yield c1, n1,
+00000140: 2027 6361 7264 270a 2020 2020 6966 206e   'card'.    if n
+00000150: 6f74 2066 2061 6e64 2063 323a 0a20 2020  ot f and c2:.   
+00000160: 2020 2020 2079 6965 6c64 2063 322c 206e       yield c2, n
+00000170: 322c 2027 636d 6e74 270a 0a0a 6465 6620  2, 'cmnt'...def 
+00000180: 6765 745f 6361 7264 7328 626c 6f63 6b2c  get_cards(block,
+00000190: 2073 6b69 7063 6f6d 6d65 6e74 733d 4661   skipcomments=Fa
+000001a0: 6c73 6529 3a0a 2020 2020 2222 220a 2020  lse):.    """.  
+000001b0: 2020 5370 6c69 7420 7465 7874 2069 6e20    Split text in 
+000001c0: 6062 6c6f 636b 6020 696e 746f 2063 6172  `block` into car
+000001d0: 6473 2e20 5265 7475 726e 2063 6172 6420  ds. Return card 
+000001e0: 7465 7874 2c20 6c69 6e65 206e 756d 6265  text, line numbe
+000001f0: 7220 696e 2074 6865 2062 6c6f 636b 0a20  r in the block. 
+00000200: 2020 2061 6e64 2074 7970 6520 2827 6361     and type ('ca
+00000210: 7264 2720 6f72 2027 636d 6e74 2729 2e0a  rd' or 'cmnt')..
+00000220: 0a20 2020 2054 6865 2060 626c 6f63 6b60  .    The `block`
+00000230: 2072 6570 7265 7365 6e74 7320 6f6e 6520   represents one 
+00000240: 626c 6f63 6b20 6f66 204d 434e 5020 696e  block of MCNP in
+00000250: 7075 7420 6669 6c65 2c20 7768 6963 6820  put file, which 
+00000260: 696e 2067 656e 6572 616c 0a20 2020 2063  in general.    c
+00000270: 6f6e 7369 7374 7320 6f66 206f 6e65 206f  onsists of one o
+00000280: 7220 6d6f 7265 2063 6172 6473 2061 6e64  r more cards and
+00000290: 207a 6572 6f20 6f72 206d 6f72 6520 636f   zero or more co
+000002a0: 6d6d 656e 7420 6c69 6e65 732e 0a0a 2020  mment lines...  
+000002b0: 2020 4465 6669 6e69 7469 6f6e 3a20 432d    Definition: C-
+000002c0: 636f 6d6d 656e 7420 6973 2061 2063 6f6d  comment is a com
+000002d0: 6d65 6e74 206c 696e 6520 696e 7369 6465  ment line inside
+000002e0: 2061 2063 6172 642e 2042 2d63 6f6d 6d65   a card. B-comme
+000002f0: 6e74 2069 7320 610a 2020 2020 636f 6d6d  nt is a.    comm
+00000300: 656e 7420 6c69 6e65 2062 6574 7765 656e  ent line between
+00000310: 2063 6172 6473 2c20 692e 652e 2061 626f   cards, i.e. abo
+00000320: 7665 2074 6865 206c 696e 6520 7768 6572  ve the line wher
+00000330: 6520 7468 6520 6e65 7874 2063 6172 6420  e the next card 
+00000340: 6265 6769 6e73 2e0a 2020 2020 5365 7665  begins..    Seve
+00000350: 7261 6c20 6c69 6e65 7320 7769 7468 2042  ral lines with B
+00000360: 2d63 6f6d 6d65 6e74 7320 636f 6d70 6f73  -comments compos
+00000370: 6520 6120 6d75 6c74 692d 6c69 6e65 2042  e a multi-line B
+00000380: 2d63 6f6d 6d65 6e74 2e0a 0a20 2020 2054  -comment...    T
+00000390: 6865 2043 2d63 6f6d 6d65 6e74 7320 6172  he C-comments ar
+000003a0: 6520 7265 7475 726e 6564 2077 6974 6869  e returned withi
+000003b0: 6e20 6361 7264 732e 2054 6865 2042 2d63  n cards. The B-c
+000003c0: 6f6d 6d65 6e74 7320 6172 6520 7265 7475  omments are retu
+000003d0: 726e 6564 0a20 2020 2073 6570 6172 6174  rned.    separat
+000003e0: 656c 792c 2077 6865 6e20 7468 6520 6073  ely, when the `s
+000003f0: 6b69 7063 6f6d 6d65 6e74 7360 2066 6c61  kipcomments` fla
+00000400: 6720 6973 2046 616c 7365 2e20 5468 7573  g is False. Thus
+00000410: 2c20 5477 6f20 7479 7065 7320 6f66 0a20  , Two types of. 
+00000420: 2020 2065 6c65 6d65 6e74 7320 6172 6520     elements are 
+00000430: 7265 7475 726e 6564 3a20 6361 7264 7320  returned: cards 
+00000440: 616e 6420 422d 636f 6d6d 656e 7473 2e20  and B-comments. 
+00000450: 426f 7468 2061 7265 2c20 6765 6e65 7261  Both are, genera
+00000460: 6c6c 792c 206d 756c 7469 2d6c 696e 650a  lly, multi-line.
+00000470: 2020 2020 7374 7269 6e67 732e 0a0a 2020      strings...  
+00000480: 2020 4120 6361 7264 2069 7320 6120 7061    A card is a pa
+00000490: 7274 206f 6620 7468 6520 626c 6f63 6b20  rt of the block 
+000004a0: 636f 6e74 6169 6e69 6e67 2061 6c6c 206c  containing all l
+000004b0: 696e 6573 2062 656c 6f6e 6769 6e67 2074  ines belonging t
+000004c0: 6f20 6120 6361 7264 2c0a 2020 2020 696e  o a card,.    in
+000004d0: 636c 7564 696e 6720 7468 6520 432d 636f  cluding the C-co
+000004e0: 6d6d 656e 7473 2e0a 0a20 2020 2022 2222  mments...    """
+000004f0: 0a0a 2020 2020 2320 4c69 7374 206f 6620  ..    # List of 
+00000500: 636f 6d6d 656e 7420 6c69 6e65 730a 2020  comment lines.  
+00000510: 2020 636d 6e74 203d 205b 5d0a 2020 2020    cmnt = [].    
+00000520: 2320 4c69 7374 206f 6620 6c69 6e65 7320  # List of lines 
+00000530: 6465 7363 7269 6269 6e67 2061 2063 6172  describing a car
+00000540: 640a 2020 2020 6361 7264 203d 205b 5d0a  d.    card = [].
+00000550: 2020 2020 2320 4c69 6e65 206e 756d 6265      # Line numbe
+00000560: 7220 7768 6572 6520 6361 7264 206f 7220  r where card or 
+00000570: 626c 6f63 6b20 6f66 2063 6f6d 6d65 6e74  block of comment
+00000580: 7320 7374 6172 7473 3a0a 2020 2020 6e5f  s starts:.    n_
+00000590: 6361 7264 203d 2030 0a20 2020 206e 5f63  card = 0.    n_c
+000005a0: 6d6e 7420 3d20 300a 0a20 2020 206c 7072  mnt = 0..    lpr
+000005b0: 6576 203d 204e 6f6e 6520 2023 2070 7265  ev = None  # pre
+000005c0: 7669 6f75 7320 6361 7264 206c 696e 650a  vious card line.
+000005d0: 2020 2020 666f 7220 6e2c 206c 2069 6e20      for n, l in 
+000005e0: 656e 756d 6572 6174 6528 626c 6f63 6b2e  enumerate(block.
+000005f0: 7370 6c69 746c 696e 6573 2829 293a 0a20  splitlines()):. 
+00000600: 2020 2020 2020 2023 2069 6620 636f 6d6d         # if comm
+00000610: 656e 742c 2074 6865 6e20 2061 6464 2074  ent, then  add t
+00000620: 6f20 626c 6f63 6b20 6f66 2063 6f6d 6d65  o block of comme
+00000630: 6e74 730a 2020 2020 2020 2020 2320 6966  nts.        # if
+00000640: 2063 6f6e 7469 6e75 6174 696f 6e2c 2074   continuation, t
+00000650: 6865 6e20 6170 7065 6e64 2062 6c6f 636b  hen append block
+00000660: 206f 6620 636f 6d6d 656e 7420 7468 6973   of comment this
+00000670: 206c 696e 6520 746f 2063 7572 7265 6e74   line to current
+00000680: 0a20 2020 2020 2020 2023 2063 6172 640a  .        # card.
+00000690: 2020 2020 2020 2020 2320 6966 206e 6577          # if new
+000006a0: 2063 6172 642c 2074 6865 6e20 7969 656c   card, then yiel
+000006b0: 6420 6375 7272 656e 7420 6361 7264 206f  d current card o
+000006c0: 7220 6375 7272 656e 7420 626c 6f63 6b20  r current block 
+000006d0: 6f66 2063 6f6d 6d65 6e74 7320 616e 640a  of comments and.
+000006e0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+000006f0: 2061 206e 6577 2063 7572 7265 6e74 2063   a new current c
+00000700: 6172 640a 2020 2020 2020 2020 6966 2072  ard.        if r
+00000710: 655f 636f 6d6d 656e 742e 6d61 7463 6828  e_comment.match(
+00000720: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
+00000730: 636d 6e74 2e61 7070 656e 6428 6c29 0a20  cmnt.append(l). 
+00000740: 2020 2020 2020 2065 6c69 6620 6973 5f63         elif is_c
+00000750: 6f6e 7469 6e75 6174 696f 6e28 6c2c 206c  ontinuation(l, l
+00000760: 7072 6576 293a 0a20 2020 2020 2020 2020  prev):.         
+00000770: 2020 2069 6620 6e6f 7420 736b 6970 636f     if not skipco
+00000780: 6d6d 656e 7473 3a0a 2020 2020 2020 2020  mments:.        
+00000790: 2020 2020 2020 2020 6361 7264 2e65 7874          card.ext
+000007a0: 656e 6428 636d 6e74 290a 2020 2020 2020  end(cmnt).      
+000007b0: 2020 2020 2020 636d 6e74 203d 205b 5d0a        cmnt = [].
+000007c0: 2020 2020 2020 2020 2020 2020 6e5f 636d              n_cm
+000007d0: 6e74 203d 206e 202b 2031 0a20 2020 2020  nt = n + 1.     
+000007e0: 2020 2020 2020 2063 6172 642e 6170 7065         card.appe
+000007f0: 6e64 286c 290a 2020 2020 2020 2020 2020  nd(l).          
+00000800: 2020 6c70 7265 7620 3d20 6c0a 2020 2020    lprev = l.    
+00000810: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000820: 2020 2020 2020 2320 7468 6973 206d 7573        # this mus
+00000830: 7420 6265 2062 6567 696e 206f 6620 6120  t be begin of a 
+00000840: 6e65 7720 6361 7264 0a20 2020 2020 2020  new card.       
+00000850: 2020 2020 2066 6f72 2072 2069 6e20 5f79       for r in _y
+00000860: 6965 6c64 2863 6172 642c 206e 5f63 6172  ield(card, n_car
+00000870: 642c 2073 6b69 7063 6f6d 6d65 6e74 732c  d, skipcomments,
+00000880: 2063 6d6e 742c 206e 5f63 6d6e 7429 3a0a   cmnt, n_cmnt):.
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 7969 656c 6420 720a 2020 2020 2020 2020  yield r.        
+000008b0: 2020 2020 636d 6e74 203d 205b 5d0a 2020      cmnt = [].  
+000008c0: 2020 2020 2020 2020 2020 6e5f 636d 6e74            n_cmnt
+000008d0: 203d 206e 202b 2031 0a20 2020 2020 2020   = n + 1.       
+000008e0: 2020 2020 2063 6172 6420 3d20 5b6c 5d0a       card = [l].
+000008f0: 2020 2020 2020 2020 2020 2020 6e5f 6361              n_ca
+00000900: 7264 203d 206e 0a20 2020 2020 2020 2020  rd = n.         
+00000910: 2020 206c 7072 6576 203d 206c 0a20 2020     lprev = l.   
+00000920: 2023 2041 7420 7468 6520 656e 6420 6f66   # At the end of
+00000930: 2062 6c6f 636b 2c20 7969 656c 6420 7468   block, yield th
+00000940: 6520 6c61 7374 2063 6172 6420 616e 6420  e last card and 
+00000950: 636f 6d6d 656e 7473 2028 7468 6973 2063  comments (this c
+00000960: 6f64 6520 6d75 7374 2062 650a 2020 2020  ode must be.    
+00000970: 2320 7468 6520 7361 6d65 2061 7320 696e  # the same as in
+00000980: 2060 656c 7365 6020 636c 6175 7365 2061   `else` clause a
+00000990: 626f 7665 290a 2020 2020 666f 7220 7220  bove).    for r 
+000009a0: 696e 205f 7969 656c 6428 6361 7264 2c20  in _yield(card, 
+000009b0: 6e5f 6361 7264 2c20 736b 6970 636f 6d6d  n_card, skipcomm
+000009c0: 656e 7473 2c20 636d 6e74 2c20 6e5f 636d  ents, cmnt, n_cm
+000009d0: 6e74 293a 0a20 2020 2020 2020 2079 6965  nt):.        yie
+000009e0: 6c64 2072 0a0a 0a64 6566 2065 7870 616e  ld r...def expan
+000009f0: 645f 7461 6273 286c 696e 6529 3a0a 2020  d_tabs(line):.  
+00000a00: 2020 7227 2727 4578 7061 6e64 2074 6162    r'''Expand tab
+00000a10: 7320 696e 2061 206c 696e 652e 0a0a 2020  s in a line...  
+00000a20: 2020 5468 6520 4d43 4e50 206d 616e 7561    The MCNP manua
+00000a30: 6c20 7361 7973 2074 6861 7420 2274 6162  l says that "tab
+00000a40: 7320 6172 6520 7265 706c 6163 6564 2062  s are replaced b
+00000a50: 7920 626c 616e 6b73 2074 6f20 7468 6520  y blanks to the 
+00000a60: 6e65 7874 0a20 2020 2038 2d63 6861 7261  next.    8-chara
+00000a70: 6374 6572 2074 6162 2073 746f 702e 0a0a  cter tab stop...
+00000a80: 2020 2020 3e3e 3e20 6578 7061 6e64 5f74      >>> expand_t
+00000a90: 6162 7328 275c 7464 6f64 6f27 290a 2020  abs('\tdodo').  
+00000aa0: 2020 2720 2020 2020 2020 2064 6f64 6f27    '        dodo'
+00000ab0: 0a20 2020 203e 3e3e 2065 7870 616e 645f  .    >>> expand_
+00000ac0: 7461 6273 2827 2020 5c74 646f 646f 2729  tabs('  \tdodo')
+00000ad0: 0a20 2020 2027 2020 2020 2020 2020 646f  .    '        do
+00000ae0: 646f 270a 2020 2020 3e3e 3e20 6578 7061  do'.    >>> expa
+00000af0: 6e64 5f74 6162 7328 2720 2020 2020 205c  nd_tabs('      \
+00000b00: 7464 6f64 6f27 290a 2020 2020 2720 2020  tdodo').    '   
+00000b10: 2020 2020 2064 6f64 6f27 0a20 2020 203e       dodo'.    >
+00000b20: 3e3e 2065 7870 616e 645f 7461 6273 2827  >> expand_tabs('
+00000b30: 2020 2020 2020 205c 7464 6f64 6f27 290a         \tdodo').
+00000b40: 2020 2020 2720 2020 2020 2020 2064 6f64      '        dod
+00000b50: 6f27 0a20 2020 203e 3e3e 2065 7870 616e  o'.    >>> expan
+00000b60: 645f 7461 6273 2827 2020 2020 2020 2020  d_tabs('        
+00000b70: 5c74 646f 646f 2729 0a20 2020 2027 2020  \tdodo').    '  
+00000b80: 2020 2020 2020 2020 2020 2020 2020 646f                do
+00000b90: 646f 270a 2020 2020 3e3e 3e20 6578 7061  do'.    >>> expa
+00000ba0: 6e64 5f74 6162 7328 275c 745c 7464 6f64  nd_tabs('\t\tdod
+00000bb0: 6f27 290a 2020 2020 2720 2020 2020 2020  o').    '       
+00000bc0: 2020 2020 2020 2020 2064 6f64 6f27 0a20           dodo'. 
+00000bd0: 2020 2027 2727 0a20 2020 2065 7870 616e     '''.    expan
+00000be0: 6465 6420 3d20 5b5d 0a20 2020 2069 203d  ded = [].    i =
+00000bf0: 2030 0a20 2020 2066 6f72 2063 6861 7220   0.    for char 
+00000c00: 696e 206c 696e 653a 0a20 2020 2020 2020  in line:.       
+00000c10: 2069 6620 6368 6172 2021 3d20 275c 7427   if char != '\t'
+00000c20: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
+00000c30: 7061 6e64 6564 2e61 7070 656e 6428 6368  panded.append(ch
+00000c40: 6172 290a 2020 2020 2020 2020 2020 2020  ar).            
+00000c50: 6920 2b3d 2031 0a20 2020 2020 2020 2065  i += 1.        e
+00000c60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00000c70: 206e 5f73 7061 6365 7320 3d20 382d 2869   n_spaces = 8-(i
+00000c80: 2538 290a 2020 2020 2020 2020 2020 2020  %8).            
+00000c90: 6578 7061 6e64 6564 2e61 7070 656e 6428  expanded.append(
+00000ca0: 2720 272a 6e5f 7370 6163 6573 290a 2020  ' '*n_spaces).  
+00000cb0: 2020 2020 2020 2020 2020 6920 2b3d 206e            i += n
+00000cc0: 5f73 7061 6365 730a 2020 2020 7265 7475  _spaces.    retu
+00000cd0: 726e 2027 272e 6a6f 696e 2865 7870 616e  rn ''.join(expan
+00000ce0: 6465 6429 0a0a 6465 6620 6973 5f63 6f6e  ded)..def is_con
+00000cf0: 7469 6e75 6174 696f 6e28 6c2c 2070 7265  tinuation(l, pre
+00000d00: 763d 4e6f 6e65 293a 0a20 2020 2022 2222  v=None):.    """
+00000d10: 0a20 2020 2043 6865 636b 2069 6620 6c20  .    Check if l 
+00000d20: 6973 2061 2063 6f6e 7469 6e75 6174 696f  is a continuatio
+00000d30: 6e20 6c69 6e65 2e0a 0a20 2020 206c 2061  n line...    l a
+00000d40: 6e64 2070 7265 7620 6d75 7374 206e 6f74  nd prev must not
+00000d50: 2062 6520 636f 6d6d 656e 7420 6c69 6e65   be comment line
+00000d60: 732e 0a20 2020 2022 2222 0a20 2020 2023  s..    """.    #
+00000d70: 2049 6620 6c20 6861 7320 3520 6f72 206d   If l has 5 or m
+00000d80: 6f72 6520 6c65 6164 696e 6720 7370 6163  ore leading spac
+00000d90: 6573 2c20 6974 2069 7320 6120 636f 6e74  es, it is a cont
+00000da0: 696e 7561 7469 6f6e 2069 6e64 6570 656e  inuation indepen
+00000db0: 6465 6e74 6c79 0a20 2020 2023 206f 6e20  dently.    # on 
+00000dc0: 7072 6576 0a20 2020 206c 203d 2065 7870  prev.    l = exp
+00000dd0: 616e 645f 7461 6273 286c 290a 2020 2020  and_tabs(l).    
+00000de0: 6966 2072 655f 636f 6e74 696e 7561 7469  if re_continuati
+00000df0: 6f6e 5f73 7061 6365 732e 6d61 7463 6828  on_spaces.match(
+00000e00: 6c29 3a0a 2020 2020 2020 2020 7265 7475  l):.        retu
+00000e10: 726e 2054 7275 650a 2020 2020 656c 6966  rn True.    elif
+00000e20: 2070 7265 7620 616e 6420 7265 5f63 6f6e   prev and re_con
+00000e30: 7469 6e75 6174 696f 6e5f 7072 6576 2e6d  tinuation_prev.m
+00000e40: 6174 6368 2870 7265 7629 3a0a 2020 2020  atch(prev):.    
+00000e50: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00000e60: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00000e70: 0a                                       .
```

### Comparing `t4_geom_convert-0.6.1/MIP/mip/blocks.py` & `t4_geom_convert-0.6.2/MIP/mip/blocks.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/mip/cellcard.py` & `t4_geom_convert-0.6.2/MIP/mip/cellcard.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/mip/datacard.py` & `t4_geom_convert-0.6.2/MIP/mip/datacard.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/mip/main.py` & `t4_geom_convert-0.6.2/MIP/mip/main.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/mip/readme.rst` & `t4_geom_convert-0.6.2/MIP/mip/readme.rst`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/mip/utils.py` & `t4_geom_convert-0.6.2/MIP/mip/utils.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/MIP/tests.py` & `t4_geom_convert-0.6.2/MIP/tests.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/README.md` & `t4_geom_convert-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/pyproject.toml` & `t4_geom_convert-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "t4_geom_convert"
-version = "0.6.1"
+version = "0.6.2"
 description = "A tool to convert MCNP geometries into the TRIPOLI-4 format"
 authors = [
   "Davide Mancusi <davide.mancusi@cea.fr>",
   "François-Xavier Hugot <francois-xavier.hugot@cea.fr>",
   "Martin Maurey",
   "Jonathan Faustin"
 ]
```

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/BoundaryCondition/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/BoundaryCondition/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/Abundances.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/Abundances.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CCompositionT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CCompositionT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/ConvertIsotope.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/ConvertIsotope.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Composition/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Composition/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Configuration/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Exceptions/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,18 @@
         '''Parse one cell, return new :class:`~.CellMCNP` object.'''
         material, geometry, option = parsed_cell
 
         material_id, density = self.parse_material(material)
 
         ast_mcnp = get_ast(geometry)
 
-        kw_list = list(reversed(option.lower().replace('(', ' ')
-                                .replace(')', ' ').replace('=', ' ').split()))
+        option = re.sub(' *: *', ':', option)
+        option = (option.lower().replace('(', ' ').replace(')', ' ')
+                  .replace('=', ' '))
+        kw_list = list(reversed(option.split()))
         kws = self.parse_keywords(kw_list)
 
         # replace some missing values with the defaults
         if kws['importance'] is None:
             try:
                 kws['importance'] = self.importances[rank]
             except IndexError:
@@ -287,14 +289,15 @@
             # no need to apply to_cos, MIP takes care of it
         elif len(fill_params) == 3:
             fill_params = [float(param) for param in fill_params[:12]]
             fill_params += [1., 0., 0.,
                             0., 1., 0.,
                             0., 0., 1.]
         elif '*' in elt:
+            fill_params = [float(x) for x in fill_params]
             fill_params[3:] = list(map(to_cos, fill_params[3:12]))
             fill_params = normalize_transform(fill_params)
         elif fill_params:
             # this is the case where the transform parameters were given inline
             fill_params = normalize_transform(fill_params)
 
 
@@ -329,9 +332,10 @@
             # no need to apply to_cos, MIP takes care of it
         elif len(trcl_params) == 3:
             trcl_params = [float(param) for param in trcl_params[:12]]
             trcl_params += [1., 0., 0.,
                             0., 1., 0.,
                             0., 0., 1.]
         elif '*' in elt:
+            trcl_params = [float(x) for x in trcl_params]
             trcl_params[3:] = list(map(to_cos, trcl_params[3:12]))
         return tuple(trcl_params)
```

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/FileHandlers/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/FileHandlers/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/GeomComp/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/GeomComp/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Progress.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Progress.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/CollectionDict.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/CollectionDict.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/DTypeConversion.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/DTypeConversion.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/Duplicates.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/Duplicates.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/MacroBodies.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/MacroBodies.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceCollection.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceCollection.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/SurfaceT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/SurfaceT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Surface/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Surface/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/Transformation.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/Transformation.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/TransformationError.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/TransformationError.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/TransformationQuad.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/TransformationQuad.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Transformation/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Utils.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Utils.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/VectUtils.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/VectUtils.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/ByUniverse.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/ByUniverse.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellConversion.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellConversion.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellConversionError.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellConversionError.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellInlining.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellInlining.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/CellMCNP.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/CellMCNP.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/DictVolumeT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/DictVolumeT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/Lattice.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/Lattice.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/TreeFunctions.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/TreeFunctions.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/VolumeT4.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/VolumeT4.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/Volume/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/Volume/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/Kernel/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/Kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/__init__.py` & `t4_geom_convert-0.6.2/t4_geom_convert/__init__.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/conftest.py` & `t4_geom_convert-0.6.2/t4_geom_convert/conftest.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/t4_geom_convert/main.py` & `t4_geom_convert-0.6.2/t4_geom_convert/main.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-0.6.1/setup.py` & `t4_geom_convert-0.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,25 @@
  't4_geom_convert.Kernel.FileHandlers.Writer',
  't4_geom_convert.Kernel.GeomComp',
  't4_geom_convert.Kernel.Surface',
  't4_geom_convert.Kernel.Transformation',
  't4_geom_convert.Kernel.Volume']
 
 package_data = \
-{'': ['*'],
- 't4_geom_convert': ['.hypothesis/examples/7d04b6175f19883b/*',
-                     '.hypothesis/examples/b5818b9694c7412d/*',
-                     '.hypothesis/examples/c02acd8530982b40/*',
-                     '.hypothesis/examples/f5595e3a381d5483/*',
-                     '.hypothesis/unicode_data/12.1.0/*',
-                     '.hypothesis/unicode_data/8.0.0/*']}
+{'': ['*']}
 
 install_requires = \
 ['importlib-metadata>=4.4,<5.0', 'numpy>=1.23,<2.0', 'tatsu>=5.6,<6.0']
 
 entry_points = \
 {'console_scripts': ['t4_geom_convert = t4_geom_convert.main:main']}
 
 setup_kwargs = {
     'name': 't4-geom-convert',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'A tool to convert MCNP geometries into the TRIPOLI-4 format',
     'long_description': "t4_geom_convert\n===============\n\n[![PyPI version](https://badge.fury.io/py/t4-geom-convert.svg)](https://badge.fury.io/py/t4-geom-convert)\n\nThis repository contains the development version of `t4_geom_convert`, a Python\ntool to convert [MCNP] geometries into the [TRIPOLI-4®] format.\n\nFeatures\n--------\n\nHere is a list of features of the MCNP modelling engine that are\nat least partially supported and converted by `t4_geom_convert`:\n\n* All surface types\n* Boolean cell operators\n* `LIKE n BUT` syntax\n* Affine transformations on surfaces and on cells (see the [Current\n  limitations](#current-limitations) section though)\n* Boundary conditions (reflection, white surfaces)\n* Isotopic compositions and cell densities\n* Universes and fills, even nested, possibly with affine transformations\n* [Lattices](#lattice-conversion)\n\n\nInstallation\n------------\n\n`t4_geom_convert` is available on [PyPI][pypi]. The suggested way to install it\nis to use [the `pip`/`pip3` package manager][pip] and [the `venv`\nmodule][venv]. If `pip3` and `venv` are not available on your machine, you can\nuse your package manager to install them:\n\n```\n# sudo apt install python3-pip python3-venv  # on Debian/Ubuntu\n# sudo yum install python3-pip python3-libs  # on Fedora/CentOS\n```\n\nYou can then create a virtual Python environment and install the latest stable\nversion of `t4_geom_convert` there with\n\n```\n$ python3 -m venv /path/to/some/folder\n$ source /path/to/some/folder/bin/activate\n$ pip3 install -U pip setuptools\n$ pip3 install t4_geom_convert\n```\n\nThis will install the `t4_geom_convert` executable in\n`/path/to/some/folder/bin/t4_geom_convert`. Sourcing\n`/path/to/some/folder/bin/activate` will put `t4_geom_convert` in your `PATH`.\n\nYou can also install the latest development version with\n\n```\n$ pip3 install git+https://github.com/arekfu/t4_geom_convert.git@next\n```\n\nYou can find more information about [`pip3`][pip] and [`venv`][venv] on the\nweb.\n\n\n### Dependencies\n\nThe MCNP input file is parsed by [MIP]. We use a slightly modified version of\nMIP, which is shipped along with `t4_geom_convert`. MIP depends on [TatSu].\n\n`t4_geom_convert` also depends on [NumPy].\n\n\nUsage\n-----\n\nThe basic usage is simply\n\n```\n$ t4_geom_convert <mcnp_input>\n```\n\nThis will create a TRIPOLI-4 output file called `<mcnp_input>.t4` containing\nthe converted geometry.  You can also choose a different name for the output\nfile using the `-o` option.\n\nUse the `-h` option for a list of all available options.\n\n### Lattice conversion\n\n`t4_geom_convert` is capable of handling the conversion of repeated structures\n(lattices). Hexahedral lattices (`LAT=1`) and hexagonal (`LAT=2`) are\nsupported.\n\nThe cell declared as `LAT=1` or `LAT=2` represents the unit cell of the\nlattice, which is assumed to repeat in all directions up to the boundaries of\nthe enclosing cell. Due to limitations of the TRIPOLI-4 representation of\nlattices, we have chosen to represent lattices using a purely surface-based\napproach.  This means that `t4_geom_convert` will actually emit separate cell\ndefinitions for each cell of the lattice that is visible through the enclosing\ncell. The ranges of cell definitions to be emitted must be specified by the\nuser via the `--lattice` command-line option. For instance, consider the\nfollowing MCNP input:\n\n```\nA lattice example\n1 0  -2 1 -4 3 IMP:N=1 U=2 LAT=1\n10 1 -1. -10 IMP:N=1 FILL=2\n1000 0 10 IMP:N=0\n\n1 PX -1.5\n2 PX 1.5\n3 PY -0.5\n4 PY 0.5\n10 SO 4\n\nm1 13027 1.\n```\n\nHere the unit cell is two-dimensional. The lattice fills a sphere of radius\n4.  Assuming the unit cell is indexed as (0,0), the visible lattice cells are\n* (-1, -4) to (-1, 4)\n* (0, -4) to (0, 4)\n* (1, -4) to (1, 4)\n\nThis can be confirmed by visual inspection of the MCNP geometry or by\ngeometrical considerations. Once the index bounds are determined, the\n`--lattice` option must be specified as\n\n```\n$ t4_geom_convert --lattice 1,-1:1,-4:4 <mcnp_input>\n                            ↑  ↑ ↑  ↑ ↑\n             cell number ───┘  │ │  │ └ j-range upper bound\n        i-range lower bound ───┘ │  └─── j-range lower bound\n          i-range upper bound ───┘\n```\n\nThis results in the following TRIPOLI-4 geometry (X-Y cut), where a few cell\nindices have been annotated:\n![example of converted geometry with lattices][lattice_example]\n\nThe syntax for one-dimensional lattices is\n\n```\n--lattice <cell>,<i-from>:<i-to>\n```\n\nand for three-dimensional lattices it is\n\n```\n--lattice <cell>,<i-from>:<i-to>,<j-from>:<j-to>,<k-from>:<k-to>\n```\n\nNote that the `ijk` axes are not necessarily the same as the coordinate axes.\nThe orientation of the lattice axes is specified by MCNP (see the *Lattice\nindexing* paragraph in the User's Manual) and it is determined by the order in\nwhich the surfaces of the unit cell appear specified. In our example, the first\nsurface appearing in the definition of the unit cell is surface `2`; therefore,\nsurface `2` separates the unit cell (0, 0) from cell (1, 0); the next surface\n(`1`) separates the unit cell from cell (-1, 0); the following surfaces, `4`\nand `3`, separate the unit cell from cells (0, 1) and (0, -1), respectively.\n\nFor hexagonal lattices, `t4_geom_convert` follows the convention described in\nthe MCNP manual. The lattice axes are defined by the first and the third plane\nappearing in the definition of the base cell. The positive direction of the\nthird axis (if present) is defined by the normal to the seventh plane appearing\nin the definition.\n\nA lattice unit cell may appear as a fill pattern in several enclosing cells. It\nis currently not possible to specify different fill ranges for each of them.\n\n\n### Fully-specified lattices\n\nMCNP provides a syntax for the specification of lattice with heterogeneous\ncells. An example is\n\n```\nA lattice example\nc cells\n2 0  -21 u=2 imp:n=1\n21 0  21 u=2 imp:n=1\n3 0  -31 u=3 imp:n=1\n31 0  31 u=3 imp:n=1\n10 0  -2 1 3 -4  lat=1 u=20 IMP:N=1\n        FILL=-1:1 -4:4\nc       i=-1   i=0   i=1\n        2      3     2   $ j=-4\n        2      3     2   $ j=-3\n        2      3     2   $ j=-2\n        2      3     2   $ j=-1\n        2      3     2   $ j=0\n        3      3     2   $ j=1\n        3      3     2   $ j=2\n        3      3     2   $ j=3\n        3      3     2   $ j=4\n100 1 -1. -10 IMP:N=1 FILL=20\n1000 0 10 IMP:N=0\n\n1 PX -1.5\n2 PX 1.5\n3 PY -0.5\n4 PY 0.5\n10 SO 4\n21 SO 0.4\n31 SO 0.1\n\nm1 13027 1.\n```\n\nThe `FILL=-1:1 -4:4` option indicates the range of indices where cells will be\nspecified. The universes filling the cells are detailed in the table below,\nwhich by convention loops over the leftmost (`i`) axis first. This syntax is\nsupported by `t4_geom_convert` and does *not* require a `--lattice` option. One\nrestriction applies: none of the subcells may be filled with the universe of\nthe lattice cell itself. This syntax indicates to MCNP that the cell should be\nfilled with the material of the lattice cell. Using `0` as a universe number\nfor the subcells is supported and results in no subcell being generated.\n\nHere is how the example above is converted and rendered in TRIPOLI-4:\n![example of converted geometry with fully-specified\nlattice][lattice_fully_specified]\n\nCurrent limitations\n-------------------\n\nHere is a list of some things that `t4_geom_convert` cannot currently do, but\nmay be able to do in the future (in roughly decreasing order of likelihood):\n\n- [ ] Import the title of the MCNP input file (tracked in [issue\n  #5](https://github.com/arekfu/t4_geom_convert/issues/5))\n- [ ] Handle affine transformations with `m=-1` (the last parameter of the\n  affine transformation) (tracked in [issue\n  #12](https://github.com/arekfu/t4_geom_convert/issues/12))\n- [ ] Optimize fills with negative universes (do not intersect with the\n  enclosing cell) (tracked in [issue\n  #13](https://github.com/arekfu/t4_geom_convert/issues/13))\n- [ ] Warn about isotopes that are missing from the TRIPOLI-4 dictionary\n  (currently you need to edit the converted file by hand and remove the\n  occurrences of the missing isotopes)\n- [ ] Convert cell temperatures\n- [ ] Import comments describing the MCNP cells/surfaces (tracked in [issue\n  #9](https://github.com/arekfu/t4_geom_convert/issues/9))\n- [ ] Provide a way to specify lattice fill ranges per enclosing cell(s) (this\n  needs to be specified in such a way that it works with nested lattices, too)\n- [ ] Deduplicate repeated cell definitions (this is a bit harder than\n  deduplicating surfaces)\n- [ ] Produce a TRIPOLI-4 connectivity map for as many cells as possible\n  (mostly lattices)\n- [ ] Recognize and automatically suppress empty cells (they may be generated\n  by lattice development or fill development)\n  - Use a linear programming solver for cells bounded by planes?\n  - Use a SAT solver in the general case?\n- [ ] Convert (some) MCNP source definitions\n- [ ] Convert (some) MCNP tally definitions\n\nYour help is welcome! Feel free to open an issue if you would like to implement\na new feature or contribute to the project in any way.\n\nThe full changelog is [here](changelog.rst).\n\n\nTesting\n-------\n\nThe correctness of `t4_geom_convert` is tested using [a specific test\noracle](Oracle/README.md), which is included in this repository.\n\n\nReporting bugs\n--------------\n\nPlease report any bug/feature request on [the GitHub issues page][bugs].\n\n\nLicence and acknowledgments\n---------------------------\n\nThe development of `t4_geom_convert` was partially financed by the [EUROfusion]\nconsortium. `t4_geom_convert` is released under the terms of the  [GNU General\nPublic Licence, version 3](COPYING).\n\n\n[bugs]: https://github.com/arekfu/t4_geom_convert/issues\n[EUROfusion]: https://www.euro-fusion.org/\n[lattice_example]: pics/lattice_example.png\n[lattice_fully_specified]: pics/lattice_fully_specified.png\n[MCNP]: https://mcnp.lanl.gov/\n[MIP]: https://github.com/travleev/mip\n[NumPy]: https://numpy.org/\n[pip]: https://packaging.python.org/tutorials/installing-packages/\n[pypi]: https://pypi.org/project/t4-geom-convert/\n[TatSu]: https://tatsu.readthedocs.io/en/stable/\n[TRIPOLI-4®]: https://www.cea.fr/nucleaire/tripoli-4\n[venv]: https://docs.python.org/3/tutorial/venv.html\n",
     'author': 'Davide Mancusi',
     'author_email': 'davide.mancusi@cea.fr',
     'maintainer': 'Davide Mancusi',
     'maintainer_email': 'davide.mancusi@cea.fr',
     'url': 'https://www.cea.fr/energies/tripoli-4/tripoli-4/pre_post_tools/t4_geom_convert/',
```

### Comparing `t4_geom_convert-0.6.1/PKG-INFO` & `t4_geom_convert-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: t4-geom-convert
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool to convert MCNP geometries into the TRIPOLI-4 format
 Home-page: https://www.cea.fr/energies/tripoli-4/tripoli-4/pre_post_tools/t4_geom_convert/
 License: GPL-3.0-or-later
 Author: Davide Mancusi
 Author-email: davide.mancusi@cea.fr
 Maintainer: Davide Mancusi
 Maintainer-email: davide.mancusi@cea.fr
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: importlib-metadata (>=4.4,<5.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: tatsu (>=5.6,<6.0)
 Project-URL: Bug tracker, https://github.com/arekfu/t4_geom_convert/issues/
 Project-URL: Documentation, https://t4-geom-convert.readthedocs.io/
 Project-URL: Repository, https://github.com/arekfu/t4_geom_convert/
```

