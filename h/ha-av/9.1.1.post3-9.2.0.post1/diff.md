# Comparing `tmp/ha-av-9.1.1.post3.tar.gz` & `tmp/ha-av-9.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ha-av-9.1.1.post3.tar", last modified: Wed Apr 13 09:36:24 2022, max compression
+gzip compressed data, was "dist/ha-av-9.2.0.post1.tar", last modified: Tue May  3 13:36:27 2022, max compression
```

## Comparing `ha-av-9.1.1.post3.tar` & `ha-av-9.2.0.post1.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/_core.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/about.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/audio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/fifo.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/fifo.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/format.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/format.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/layout.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/layout.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/resampler.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/resampler.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/audio/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/buffer.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/bytesource.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/bytesource.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/codec/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/codec/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/codec/codec.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/codec/codec.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/codec/context.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    22024 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/codec/context.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/container/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/core.pxd
--rwxr-xr-x   0 runner    (1001) docker     (121)    15157 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/core.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/input.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/input.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/output.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8416 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/output.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/pyio.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5253 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/pyio.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/streams.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/container/streams.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/data/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/data/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/descriptor.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/descriptor.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/dictionary.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/dictionary.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/enum.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10643 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/enum.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/error.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10449 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/error.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/filter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/context.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/context.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/filter.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/filter.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/graph.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/graph.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/link.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/link.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/pad.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/filter/pad.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/format.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7055 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/format.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/logging.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/option.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/option.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/packet.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/packet.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/plane.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/sidedata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/sidedata/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/sidedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/sidedata/motionvectors.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/sidedata/motionvectors.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/sidedata/sidedata.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/sidedata/sidedata.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/stream.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/subtitles/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/subtitle.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/subtitles/subtitle.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/av/video/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/format.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/format.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    14336 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/reformatter.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7053 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/reformatter.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/av/video/stream.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/_globals.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/audio.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/buffer.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/codec.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/container.rst
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/enum.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/error.rst
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/error_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/filter.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/packet.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/plane.rst
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/sidedata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/stream.rst
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/subtitles.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/time.rst
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/api/video.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13563 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/docs/cookbook/
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/cookbook/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/cookbook/numpy.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/docs/development/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/development/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/development/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/development/hacking.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11074 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/development/includes.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/development/includes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/development/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/docs/overview/
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/overview/caveats.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/docs/overview/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/examples/basics/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/basics/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/basics/remux.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/basics/save_keyframes.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/basics/thread_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/examples/numpy/
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/numpy/barcode.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/numpy/generate_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/examples/numpy/generate_video_with_pts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/flags.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/ha_av.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libav.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libavcodec/
--rw-r--r--   0 runner    (1001) docker     (121)    11421 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavcodec/avcodec.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libavdevice/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavdevice/avdevice.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libavfilter/
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavfilter/avfilter.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavfilter/avfiltergraph.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavfilter/buffersink.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavfilter/buffersrc.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libavformat/
--rw-r--r--   0 runner    (1001) docker     (121)     7931 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavformat/avformat.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libavutil/
--rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/avutil.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/channel_layout.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/dict.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/error.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/motion_vector.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libavutil/samplefmt.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libswresample/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libswresample/swresample.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/include/libswscale/
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/include/libswscale/swscale.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/
--rw-r--r--   0 runner    (1001) docker     (121)   168273 2022-04-13 09:36:14.000000 ha-av-9.1.1.post3/src/av/_core.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/audio/
--rw-r--r--   0 runner    (1001) docker     (121)   266731 2022-04-13 09:36:20.000000 ha-av-9.1.1.post3/src/av/audio/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (121)   293461 2022-04-13 09:36:21.000000 ha-av-9.1.1.post3/src/av/audio/fifo.c
--rw-r--r--   0 runner    (1001) docker     (121)   214505 2022-04-13 09:36:20.000000 ha-av-9.1.1.post3/src/av/audio/format.c
--rw-r--r--   0 runner    (1001) docker     (121)   351801 2022-04-13 09:36:19.000000 ha-av-9.1.1.post3/src/av/audio/frame.c
--rw-r--r--   0 runner    (1001) docker     (121)   359762 2022-04-13 09:36:20.000000 ha-av-9.1.1.post3/src/av/audio/layout.c
--rw-r--r--   0 runner    (1001) docker     (121)   193089 2022-04-13 09:36:21.000000 ha-av-9.1.1.post3/src/av/audio/plane.c
--rw-r--r--   0 runner    (1001) docker     (121)   304660 2022-04-13 09:36:20.000000 ha-av-9.1.1.post3/src/av/audio/resampler.c
--rw-r--r--   0 runner    (1001) docker     (121)   189595 2022-04-13 09:36:20.000000 ha-av-9.1.1.post3/src/av/audio/stream.c
--rw-r--r--   0 runner    (1001) docker     (121)   227068 2022-04-13 09:36:14.000000 ha-av-9.1.1.post3/src/av/buffer.c
--rw-r--r--   0 runner    (1001) docker     (121)   169363 2022-04-13 09:36:14.000000 ha-av-9.1.1.post3/src/av/bytesource.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/codec/
--rw-r--r--   0 runner    (1001) docker     (121)   425072 2022-04-13 09:36:17.000000 ha-av-9.1.1.post3/src/av/codec/codec.c
--rw-r--r--   0 runner    (1001) docker     (121)   659914 2022-04-13 09:36:17.000000 ha-av-9.1.1.post3/src/av/codec/context.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/container/
--rw-r--r--   0 runner    (1001) docker     (121)   549873 2022-04-13 09:36:19.000000 ha-av-9.1.1.post3/src/av/container/core.c
--rw-r--r--   0 runner    (1001) docker     (121)   423488 2022-04-13 09:36:19.000000 ha-av-9.1.1.post3/src/av/container/input.c
--rw-r--r--   0 runner    (1001) docker     (121)   369544 2022-04-13 09:36:19.000000 ha-av-9.1.1.post3/src/av/container/output.c
--rw-r--r--   0 runner    (1001) docker     (121)   271676 2022-04-13 09:36:18.000000 ha-av-9.1.1.post3/src/av/container/pyio.c
--rw-r--r--   0 runner    (1001) docker     (121)   334845 2022-04-13 09:36:18.000000 ha-av-9.1.1.post3/src/av/container/streams.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/data/
--rw-r--r--   0 runner    (1001) docker     (121)   207114 2022-04-13 09:36:17.000000 ha-av-9.1.1.post3/src/av/data/stream.c
--rw-r--r--   0 runner    (1001) docker     (121)   196054 2022-04-13 09:36:16.000000 ha-av-9.1.1.post3/src/av/descriptor.c
--rw-r--r--   0 runner    (1001) docker     (121)   264489 2022-04-13 09:36:16.000000 ha-av-9.1.1.post3/src/av/dictionary.c
--rw-r--r--   0 runner    (1001) docker     (121)   628354 2022-04-13 09:36:14.000000 ha-av-9.1.1.post3/src/av/enum.c
--rw-r--r--   0 runner    (1001) docker     (121)   491313 2022-04-13 09:36:16.000000 ha-av-9.1.1.post3/src/av/error.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/filter/
--rw-r--r--   0 runner    (1001) docker     (121)   324670 2022-04-13 09:36:21.000000 ha-av-9.1.1.post3/src/av/filter/context.c
--rw-r--r--   0 runner    (1001) docker     (121)   383993 2022-04-13 09:36:21.000000 ha-av-9.1.1.post3/src/av/filter/filter.c
--rw-r--r--   0 runner    (1001) docker     (121)   404956 2022-04-13 09:36:22.000000 ha-av-9.1.1.post3/src/av/filter/graph.c
--rw-r--r--   0 runner    (1001) docker     (121)   222055 2022-04-13 09:36:21.000000 ha-av-9.1.1.post3/src/av/filter/link.c
--rw-r--r--   0 runner    (1001) docker     (121)   235565 2022-04-13 09:36:21.000000 ha-av-9.1.1.post3/src/av/filter/pad.c
--rw-r--r--   0 runner    (1001) docker     (121)   304795 2022-04-13 09:36:15.000000 ha-av-9.1.1.post3/src/av/format.c
--rw-r--r--   0 runner    (1001) docker     (121)   253474 2022-04-13 09:36:15.000000 ha-av-9.1.1.post3/src/av/frame.c
--rw-r--r--   0 runner    (1001) docker     (121)   379960 2022-04-13 09:36:16.000000 ha-av-9.1.1.post3/src/av/logging.c
--rw-r--r--   0 runner    (1001) docker     (121)   306007 2022-04-13 09:36:15.000000 ha-av-9.1.1.post3/src/av/option.c
--rw-r--r--   0 runner    (1001) docker     (121)   305931 2022-04-13 09:36:14.000000 ha-av-9.1.1.post3/src/av/packet.c
--rw-r--r--   0 runner    (1001) docker     (121)   197953 2022-04-13 09:36:16.000000 ha-av-9.1.1.post3/src/av/plane.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/sidedata/
--rw-r--r--   0 runner    (1001) docker     (121)   328285 2022-04-13 09:36:17.000000 ha-av-9.1.1.post3/src/av/sidedata/motionvectors.c
--rw-r--r--   0 runner    (1001) docker     (121)   349786 2022-04-13 09:36:16.000000 ha-av-9.1.1.post3/src/av/sidedata/sidedata.c
--rw-r--r--   0 runner    (1001) docker     (121)   345167 2022-04-13 09:36:15.000000 ha-av-9.1.1.post3/src/av/stream.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/subtitles/
--rw-r--r--   0 runner    (1001) docker     (121)   195334 2022-04-13 09:36:18.000000 ha-av-9.1.1.post3/src/av/subtitles/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (121)   172202 2022-04-13 09:36:17.000000 ha-av-9.1.1.post3/src/av/subtitles/stream.c
--rw-r--r--   0 runner    (1001) docker     (121)   517915 2022-04-13 09:36:18.000000 ha-av-9.1.1.post3/src/av/subtitles/subtitle.c
--rw-r--r--   0 runner    (1001) docker     (121)   205321 2022-04-13 09:36:15.000000 ha-av-9.1.1.post3/src/av/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/video/
--rw-r--r--   0 runner    (1001) docker     (121)   306990 2022-04-13 09:36:23.000000 ha-av-9.1.1.post3/src/av/video/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (121)   398253 2022-04-13 09:36:23.000000 ha-av-9.1.1.post3/src/av/video/format.c
--rw-r--r--   0 runner    (1001) docker     (121)  1204372 2022-04-13 09:36:23.000000 ha-av-9.1.1.post3/src/av/video/frame.c
--rw-r--r--   0 runner    (1001) docker     (121)   255450 2022-04-13 09:36:23.000000 ha-av-9.1.1.post3/src/av/video/plane.c
--rw-r--r--   0 runner    (1001) docker     (121)   278067 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/src/av/video/reformatter.c
--rw-r--r--   0 runner    (1001) docker     (121)   190560 2022-04-13 09:36:23.000000 ha-av-9.1.1.post3/src/av/video/stream.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:24.000000 ha-av-9.1.1.post3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_audiofifo.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_audioformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_audioframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_audiolayout.py
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_audioresampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (121)    11744 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_codec_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_containerformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    14227 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_file_probing.py
--rw-r--r--   0 runner    (1001) docker     (121)     9047 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     9830 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_python_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_seek.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_videoformat.py
--rw-r--r--   0 runner    (1001) docker     (121)    16390 2022-04-13 09:36:10.000000 ha-av-9.1.1.post3/tests/test_videoframe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/_core.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/about.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/fifo.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/fifo.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/layout.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/layout.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/resampler.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/resampler.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/audio/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/buffer.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/bytesource.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/bytesource.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/codec/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/codec/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/codec/codec.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/codec/codec.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/codec/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    22526 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/codec/context.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/container/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/core.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15157 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/input.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/input.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/output.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     8427 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/output.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/pyio.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5253 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/pyio.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/streams.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/container/streams.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/data/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/data/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/descriptor.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/descriptor.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/dictionary.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/dictionary.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/enum.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10754 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/enum.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/error.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10449 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/error.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/filter.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/filter.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/graph.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/graph.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/link.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/link.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/pad.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/filter/pad.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7055 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/logging.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/option.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/option.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/packet.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/packet.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/plane.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/sidedata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/sidedata/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/sidedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/sidedata/motionvectors.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/sidedata/motionvectors.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/sidedata/sidedata.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/sidedata/sidedata.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/stream.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/subtitle.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/subtitles/subtitle.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/av/video/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    14336 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/reformatter.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7053 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/reformatter.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/av/video/stream.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/_globals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/audio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/buffer.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/codec.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/container.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/enum.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/error.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/error_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/packet.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/plane.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/sidedata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/subtitles.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/time.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/api/video.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13563 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/docs/cookbook/
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/cookbook/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/cookbook/numpy.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/development/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/development/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/development/hacking.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11074 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/development/includes.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/development/includes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/development/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/docs/overview/
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/overview/caveats.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/docs/overview/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/examples/basics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/basics/parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/basics/remux.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/basics/save_keyframes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/basics/thread_type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/examples/numpy/
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/numpy/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/numpy/generate_video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/examples/numpy/generate_video_with_pts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/flags.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/ha_av.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/ha_av.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/ha_av.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/ha_av.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/ha_av.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/ha_av.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/ha_av.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libav.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libavcodec/
+-rw-r--r--   0 runner    (1001) docker     (121)    11766 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavcodec/avcodec.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libavdevice/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavdevice/avdevice.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libavfilter/
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavfilter/avfilter.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavfilter/avfiltergraph.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavfilter/buffersink.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavfilter/buffersrc.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libavformat/
+-rw-r--r--   0 runner    (1001) docker     (121)     7931 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavformat/avformat.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libavutil/
+-rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/avutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/channel_layout.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/dict.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/error.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/motion_vector.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libavutil/samplefmt.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libswresample/
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libswresample/swresample.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/include/libswscale/
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/include/libswscale/swscale.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/
+-rw-r--r--   0 runner    (1001) docker     (121)   168569 2022-05-03 13:36:16.000000 ha-av-9.2.0.post1/src/av/_core.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)   267027 2022-05-03 13:36:25.000000 ha-av-9.2.0.post1/src/av/audio/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (121)   293757 2022-05-03 13:36:24.000000 ha-av-9.2.0.post1/src/av/audio/fifo.c
+-rw-r--r--   0 runner    (1001) docker     (121)   214801 2022-05-03 13:36:25.000000 ha-av-9.2.0.post1/src/av/audio/format.c
+-rw-r--r--   0 runner    (1001) docker     (121)   352097 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/src/av/audio/frame.c
+-rw-r--r--   0 runner    (1001) docker     (121)   360058 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/src/av/audio/layout.c
+-rw-r--r--   0 runner    (1001) docker     (121)   193385 2022-05-03 13:36:25.000000 ha-av-9.2.0.post1/src/av/audio/plane.c
+-rw-r--r--   0 runner    (1001) docker     (121)   304956 2022-05-03 13:36:25.000000 ha-av-9.2.0.post1/src/av/audio/resampler.c
+-rw-r--r--   0 runner    (1001) docker     (121)   189891 2022-05-03 13:36:26.000000 ha-av-9.2.0.post1/src/av/audio/stream.c
+-rw-r--r--   0 runner    (1001) docker     (121)   227068 2022-05-03 13:36:14.000000 ha-av-9.2.0.post1/src/av/buffer.c
+-rw-r--r--   0 runner    (1001) docker     (121)   169363 2022-05-03 13:36:15.000000 ha-av-9.2.0.post1/src/av/bytesource.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/codec/
+-rw-r--r--   0 runner    (1001) docker     (121)   425368 2022-05-03 13:36:17.000000 ha-av-9.2.0.post1/src/av/codec/codec.c
+-rw-r--r--   0 runner    (1001) docker     (121)   672602 2022-05-03 13:36:17.000000 ha-av-9.2.0.post1/src/av/codec/context.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/container/
+-rw-r--r--   0 runner    (1001) docker     (121)   550169 2022-05-03 13:36:21.000000 ha-av-9.2.0.post1/src/av/container/core.c
+-rw-r--r--   0 runner    (1001) docker     (121)   423784 2022-05-03 13:36:21.000000 ha-av-9.2.0.post1/src/av/container/input.c
+-rw-r--r--   0 runner    (1001) docker     (121)   369851 2022-05-03 13:36:20.000000 ha-av-9.2.0.post1/src/av/container/output.c
+-rw-r--r--   0 runner    (1001) docker     (121)   271972 2022-05-03 13:36:20.000000 ha-av-9.2.0.post1/src/av/container/pyio.c
+-rw-r--r--   0 runner    (1001) docker     (121)   335141 2022-05-03 13:36:21.000000 ha-av-9.2.0.post1/src/av/container/streams.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   207410 2022-05-03 13:36:20.000000 ha-av-9.2.0.post1/src/av/data/stream.c
+-rw-r--r--   0 runner    (1001) docker     (121)   196350 2022-05-03 13:36:16.000000 ha-av-9.2.0.post1/src/av/descriptor.c
+-rw-r--r--   0 runner    (1001) docker     (121)   264785 2022-05-03 13:36:14.000000 ha-av-9.2.0.post1/src/av/dictionary.c
+-rw-r--r--   0 runner    (1001) docker     (121)   631630 2022-05-03 13:36:14.000000 ha-av-9.2.0.post1/src/av/enum.c
+-rw-r--r--   0 runner    (1001) docker     (121)   491609 2022-05-03 13:36:15.000000 ha-av-9.2.0.post1/src/av/error.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)   324966 2022-05-03 13:36:22.000000 ha-av-9.2.0.post1/src/av/filter/context.c
+-rw-r--r--   0 runner    (1001) docker     (121)   384289 2022-05-03 13:36:22.000000 ha-av-9.2.0.post1/src/av/filter/filter.c
+-rw-r--r--   0 runner    (1001) docker     (121)   405252 2022-05-03 13:36:22.000000 ha-av-9.2.0.post1/src/av/filter/graph.c
+-rw-r--r--   0 runner    (1001) docker     (121)   222351 2022-05-03 13:36:22.000000 ha-av-9.2.0.post1/src/av/filter/link.c
+-rw-r--r--   0 runner    (1001) docker     (121)   235861 2022-05-03 13:36:23.000000 ha-av-9.2.0.post1/src/av/filter/pad.c
+-rw-r--r--   0 runner    (1001) docker     (121)   305091 2022-05-03 13:36:15.000000 ha-av-9.2.0.post1/src/av/format.c
+-rw-r--r--   0 runner    (1001) docker     (121)   253770 2022-05-03 13:36:17.000000 ha-av-9.2.0.post1/src/av/frame.c
+-rw-r--r--   0 runner    (1001) docker     (121)   380256 2022-05-03 13:36:14.000000 ha-av-9.2.0.post1/src/av/logging.c
+-rw-r--r--   0 runner    (1001) docker     (121)   306303 2022-05-03 13:36:15.000000 ha-av-9.2.0.post1/src/av/option.c
+-rw-r--r--   0 runner    (1001) docker     (121)   306227 2022-05-03 13:36:15.000000 ha-av-9.2.0.post1/src/av/packet.c
+-rw-r--r--   0 runner    (1001) docker     (121)   198249 2022-05-03 13:36:15.000000 ha-av-9.2.0.post1/src/av/plane.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/sidedata/
+-rw-r--r--   0 runner    (1001) docker     (121)   328581 2022-05-03 13:36:24.000000 ha-av-9.2.0.post1/src/av/sidedata/motionvectors.c
+-rw-r--r--   0 runner    (1001) docker     (121)   351899 2022-05-03 13:36:24.000000 ha-av-9.2.0.post1/src/av/sidedata/sidedata.c
+-rw-r--r--   0 runner    (1001) docker     (121)   345463 2022-05-03 13:36:16.000000 ha-av-9.2.0.post1/src/av/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (121)   195630 2022-05-03 13:36:23.000000 ha-av-9.2.0.post1/src/av/subtitles/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (121)   172498 2022-05-03 13:36:24.000000 ha-av-9.2.0.post1/src/av/subtitles/stream.c
+-rw-r--r--   0 runner    (1001) docker     (121)   518211 2022-05-03 13:36:23.000000 ha-av-9.2.0.post1/src/av/subtitles/subtitle.c
+-rw-r--r--   0 runner    (1001) docker     (121)   205617 2022-05-03 13:36:16.000000 ha-av-9.2.0.post1/src/av/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/src/av/video/
+-rw-r--r--   0 runner    (1001) docker     (121)   307286 2022-05-03 13:36:18.000000 ha-av-9.2.0.post1/src/av/video/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (121)   398549 2022-05-03 13:36:18.000000 ha-av-9.2.0.post1/src/av/video/format.c
+-rw-r--r--   0 runner    (1001) docker     (121)  1204668 2022-05-03 13:36:20.000000 ha-av-9.2.0.post1/src/av/video/frame.c
+-rw-r--r--   0 runner    (1001) docker     (121)   255746 2022-05-03 13:36:18.000000 ha-av-9.2.0.post1/src/av/video/plane.c
+-rw-r--r--   0 runner    (1001) docker     (121)   278363 2022-05-03 13:36:18.000000 ha-av-9.2.0.post1/src/av/video/reformatter.c
+-rw-r--r--   0 runner    (1001) docker     (121)   190856 2022-05-03 13:36:18.000000 ha-av-9.2.0.post1/src/av/video/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:27.000000 ha-av-9.2.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_audiofifo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_audioformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_audioframe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_audiolayout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_audioresampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_codec_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_containerformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14227 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_file_probing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9047 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9830 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_python_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_seek.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_videoformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16390 2022-05-03 13:36:03.000000 ha-av-9.2.0.post1/tests/test_videoframe.py
```

### Comparing `ha-av-9.1.1.post3/LICENSE.txt` & `ha-av-9.2.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/__init__.py` & `ha-av-9.2.0.post1/av/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-# Add the native FFMPEG and MinGW libraries to executable path, so that the
-# AV pyd files can find them.
 import os
+import sys
 
-if os.name == "nt":
+# Some Python versions distributed by Conda have a buggy `os.add_dll_directory`
+# which prevents binary wheels from finding the FFmpeg DLLs in the `av.libs`
+# directory. We work around this by adding `av.libs` to the PATH.
+if (
+    os.name == "nt"
+    and sys.version_info[:2] in ((3, 8), (3, 9))
+    and os.path.exists(os.path.join(sys.base_prefix, "conda-meta"))
+):
     os.environ["PATH"] = (
-        os.path.abspath(os.path.dirname(__file__)) + os.pathsep + os.environ["PATH"]
+        os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, "av.libs"))
+        + os.pathsep
+        + os.environ["PATH"]
     )
 
 # MUST import the core before anything else in order to initalize the underlying
 # library that is being wrapped.
 from av._core import time_base, library_versions
 
 # Capture logging (by importing it).
```

### Comparing `ha-av-9.1.1.post3/av/__main__.py` & `ha-av-9.2.0.post1/av/__main__.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/_core.pyx` & `ha-av-9.2.0.post1/av/_core.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/codeccontext.pyx` & `ha-av-9.2.0.post1/av/audio/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/fifo.pyx` & `ha-av-9.2.0.post1/av/audio/fifo.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/format.pyx` & `ha-av-9.2.0.post1/av/audio/format.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/frame.pxd` & `ha-av-9.2.0.post1/av/audio/frame.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/frame.pyx` & `ha-av-9.2.0.post1/av/audio/frame.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/layout.pyx` & `ha-av-9.2.0.post1/av/audio/layout.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/audio/resampler.pyx` & `ha-av-9.2.0.post1/av/audio/resampler.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/buffer.pyx` & `ha-av-9.2.0.post1/av/buffer.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/bytesource.pyx` & `ha-av-9.2.0.post1/av/bytesource.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/codec/codec.pyx` & `ha-av-9.2.0.post1/av/codec/codec.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/codec/context.pxd` & `ha-av-9.2.0.post1/av/codec/context.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/codec/context.pyx` & `ha-av-9.2.0.post1/av/codec/context.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import warnings
+
 from libc.errno cimport EAGAIN
 from libc.stdint cimport int64_t, uint8_t
 from libc.string cimport memcpy
 cimport libav as lib
 
 from av.bytesource cimport ByteSource, bytesource
 from av.codec.codec cimport Codec, wrap_codec
 from av.dictionary cimport _Dictionary
 from av.enum cimport define_enum
 from av.error cimport err_check
 from av.packet cimport Packet
 from av.utils cimport avrational_to_fraction, to_avrational
 
+from av.deprecation import AVDeprecationWarning
 from av.dictionary import Dictionary
 
 
 cdef object _cinit_sentinel = object()
 
 
 cdef CodecContext wrap_codec_context(lib.AVCodecContext *c_ctx, const lib.AVCodec *c_codec, bint allocated):
@@ -278,16 +281,16 @@
         # if self.codec.ptr.capabilities & lib.CODEC_CAP_TRUNCATED:
         #     self.ptr.flags |= lib.CODEC_FLAG_TRUNCATED
 
         # TODO: Do this better.
         cdef _Dictionary options = Dictionary()
         options.update(self.options or {})
 
-        # Assert we have a time_base.
-        if not self.ptr.time_base.num:
+        # Assert we have a time_base for encoders.
+        if not self.ptr.time_base.num and self.is_encoder:
             self._set_default_time_base()
 
         err_check(lib.avcodec_open2(self.ptr, self.codec.ptr, &options.ptr))
 
         self.options = dict(options)
 
     cdef _set_default_time_base(self):
@@ -547,17 +550,27 @@
     property profile:
         def __get__(self):
             if self.ptr.codec and lib.av_get_profile_name(self.ptr.codec, self.ptr.profile):
                 return lib.av_get_profile_name(self.ptr.codec, self.ptr.profile)
 
     property time_base:
         def __get__(self):
+            if self.is_decoder:
+                warnings.warn(
+                    "Using CodecContext.time_base for decoders is deprecated.",
+                    AVDeprecationWarning
+                )
             return avrational_to_fraction(&self.ptr.time_base)
 
         def __set__(self, value):
+            if self.is_decoder:
+                warnings.warn(
+                    "Using CodecContext.time_base for decoders is deprecated.",
+                    AVDeprecationWarning
+                )
             to_avrational(value, &self.ptr.time_base)
 
     property codec_tag:
         def __get__(self):
             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(
                 encoding="ascii")
```

### Comparing `ha-av-9.1.1.post3/av/container/core.pxd` & `ha-av-9.2.0.post1/av/container/core.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/container/core.pyx` & `ha-av-9.2.0.post1/av/container/core.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/container/input.pyx` & `ha-av-9.2.0.post1/av/container/input.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/container/output.pyx` & `ha-av-9.2.0.post1/av/container/output.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,14 @@
         # Assert the packet is in stream time.
         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:
             raise ValueError('Bad Packet stream_index.')
         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
         packet._rebase_time(stream.time_base)
 
         # Make another reference to the packet, as av_interleaved_write_frame
-        # takes ownership of it.
+        # takes ownership of the reference.
         self.err_check(lib.av_packet_ref(self.packet_ptr, packet.ptr))
 
         cdef int ret
         with nogil:
             ret = lib.av_interleaved_write_frame(self.ptr, self.packet_ptr)
         self.err_check(ret)
```

### Comparing `ha-av-9.1.1.post3/av/container/pyio.pxd` & `ha-av-9.2.0.post1/av/container/pyio.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/container/pyio.pyx` & `ha-av-9.2.0.post1/av/container/pyio.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/container/streams.pyx` & `ha-av-9.2.0.post1/av/container/streams.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/data/stream.pyx` & `ha-av-9.2.0.post1/av/data/stream.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/datasets.py` & `ha-av-9.2.0.post1/av/datasets.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/deprecation.py` & `ha-av-9.2.0.post1/av/deprecation.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/descriptor.pxd` & `ha-av-9.2.0.post1/av/descriptor.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/descriptor.pyx` & `ha-av-9.2.0.post1/av/descriptor.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/dictionary.pyx` & `ha-av-9.2.0.post1/av/dictionary.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/enum.pyx` & `ha-av-9.2.0.post1/av/enum.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -380,10 +380,11 @@
 cpdef define_enum(name, module, items, bint is_flags=False):
 
     if is_flags:
         base_cls = EnumFlag
     else:
         base_cls = EnumItem
 
-    cls = EnumType(name, (base_cls, ), {'__module__': module}, items)
+    # Some items may be None if they correspond to an unsupported FFmpeg feature
+    cls = EnumType(name, (base_cls, ), {'__module__': module}, [i for i in items if i is not None])
 
     return cls
```

### Comparing `ha-av-9.1.1.post3/av/error.pyx` & `ha-av-9.2.0.post1/av/error.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/filter/context.pyx` & `ha-av-9.2.0.post1/av/filter/context.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/filter/filter.pyx` & `ha-av-9.2.0.post1/av/filter/filter.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/filter/graph.pyx` & `ha-av-9.2.0.post1/av/filter/graph.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/filter/link.pyx` & `ha-av-9.2.0.post1/av/filter/link.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/filter/pad.pxd` & `ha-av-9.2.0.post1/av/filter/pad.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/filter/pad.pyx` & `ha-av-9.2.0.post1/av/filter/pad.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/format.pyx` & `ha-av-9.2.0.post1/av/format.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/frame.pyx` & `ha-av-9.2.0.post1/av/frame.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/logging.pyx` & `ha-av-9.2.0.post1/av/logging.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/option.pyx` & `ha-av-9.2.0.post1/av/option.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/packet.pyx` & `ha-av-9.2.0.post1/av/packet.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/plane.pyx` & `ha-av-9.2.0.post1/av/plane.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/sidedata/motionvectors.pyx` & `ha-av-9.2.0.post1/av/sidedata/motionvectors.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/sidedata/sidedata.pyx` & `ha-av-9.2.0.post1/av/sidedata/sidedata.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     ('SKIP_SAMPLES', lib.AV_FRAME_DATA_SKIP_SAMPLES),
     ('AUDIO_SERVICE_TYPE', lib.AV_FRAME_DATA_AUDIO_SERVICE_TYPE),
     ('MASTERING_DISPLAY_METADATA', lib.AV_FRAME_DATA_MASTERING_DISPLAY_METADATA),
     ('GOP_TIMECODE', lib.AV_FRAME_DATA_GOP_TIMECODE),
     ('SPHERICAL', lib.AV_FRAME_DATA_SPHERICAL),
     ('CONTENT_LIGHT_LEVEL', lib.AV_FRAME_DATA_CONTENT_LIGHT_LEVEL),
     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),
+    # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    ('SEI_UNREGISTERED', lib.AV_FRAME_DATA_SEI_UNREGISTERED) if lib.AV_FRAME_DATA_SEI_UNREGISTERED != -1 else None,
 
     # These are deprecated. See https://github.com/PyAV-Org/PyAV/issues/607
     # ('QP_TABLE_PROPERTIES', lib.AV_FRAME_DATA_QP_TABLE_PROPERTIES),
     # ('QP_TABLE_DATA', lib.AV_FRAME_DATA_QP_TABLE_DATA),
 
 ))
```

### Comparing `ha-av-9.1.1.post3/av/stream.pxd` & `ha-av-9.2.0.post1/av/stream.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/stream.pyx` & `ha-av-9.2.0.post1/av/stream.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/subtitles/codeccontext.pyx` & `ha-av-9.2.0.post1/av/subtitles/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/subtitles/subtitle.pxd` & `ha-av-9.2.0.post1/av/subtitles/subtitle.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/subtitles/subtitle.pyx` & `ha-av-9.2.0.post1/av/subtitles/subtitle.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/utils.pxd` & `ha-av-9.2.0.post1/av/utils.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/utils.pyx` & `ha-av-9.2.0.post1/av/utils.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/codeccontext.pyx` & `ha-av-9.2.0.post1/av/video/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/format.pxd` & `ha-av-9.2.0.post1/av/video/format.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/format.pyx` & `ha-av-9.2.0.post1/av/video/format.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/frame.pxd` & `ha-av-9.2.0.post1/av/video/frame.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/frame.pyx` & `ha-av-9.2.0.post1/av/video/frame.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/plane.pyx` & `ha-av-9.2.0.post1/av/video/plane.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/av/video/reformatter.pyx` & `ha-av-9.2.0.post1/av/video/reformatter.pyx`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/audio.rst` & `ha-av-9.2.0.post1/docs/api/audio.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/codec.rst` & `ha-av-9.2.0.post1/docs/api/codec.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/container.rst` & `ha-av-9.2.0.post1/docs/api/container.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/error.rst` & `ha-av-9.2.0.post1/docs/api/error.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/error_table.py` & `ha-av-9.2.0.post1/docs/api/error_table.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/stream.rst` & `ha-av-9.2.0.post1/docs/api/stream.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/api/time.rst` & `ha-av-9.2.0.post1/docs/api/time.rst`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 
     >>> fh = av.open(path)
     >>> video = fh.streams.video[0]
 
     >>> video.time_base
     Fraction(1, 25)
 
-    >>> video.codec_context.time_base
-    Fraction(1, 50)
-
 Attributes that represent time on those objects will be in that object's ``time_base``:
 
 .. doctest::
 
     >>> video.duration
     168
     >>> float(video.duration * video.time_base)
```

### Comparing `ha-av-9.1.1.post3/docs/api/video.rst` & `ha-av-9.2.0.post1/docs/api/video.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/conf.py` & `ha-av-9.2.0.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/cookbook/basics.rst` & `ha-av-9.2.0.post1/docs/cookbook/basics.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/cookbook/numpy.rst` & `ha-av-9.2.0.post1/docs/cookbook/numpy.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/development/includes.py` & `ha-av-9.2.0.post1/docs/development/includes.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/index.rst` & `ha-av-9.2.0.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/overview/caveats.rst` & `ha-av-9.2.0.post1/docs/overview/caveats.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/docs/overview/installation.rst` & `ha-av-9.2.0.post1/docs/overview/installation.rst`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/basics/parse.py` & `ha-av-9.2.0.post1/examples/basics/parse.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/basics/remux.py` & `ha-av-9.2.0.post1/examples/basics/remux.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/basics/save_keyframes.py` & `ha-av-9.2.0.post1/examples/basics/save_keyframes.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/basics/thread_type.py` & `ha-av-9.2.0.post1/examples/basics/thread_type.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/numpy/barcode.py` & `ha-av-9.2.0.post1/examples/numpy/barcode.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/numpy/generate_video.py` & `ha-av-9.2.0.post1/examples/numpy/generate_video.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/examples/numpy/generate_video_with_pts.py` & `ha-av-9.2.0.post1/examples/numpy/generate_video_with_pts.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/flags.txt` & `ha-av-9.2.0.post1/flags.txt`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/ha_av.egg-info/SOURCES.txt` & `ha-av-9.2.0.post1/ha_av.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libav.pxd` & `ha-av-9.2.0.post1/include/libav.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavcodec/avcodec.pxd` & `ha-av-9.2.0.post1/include/libavcodec/avcodec.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
     uint16_t, int16_t,
     uint32_t, int32_t,
     uint64_t, int64_t
 )
 
 
 cdef extern from "libavcodec/avcodec.h" nogil:
+    """
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    """
 
     # custom
     cdef set pyav_get_available_codecs()
 
     cdef int   avcodec_version()
     cdef char* avcodec_configuration()
     cdef char* avcodec_license()
@@ -279,14 +287,15 @@
         AV_FRAME_DATA_MASTERING_DISPLAY_METADATA
         AV_FRAME_DATA_GOP_TIMECODE
         AV_FRAME_DATA_SPHERICAL
         AV_FRAME_DATA_CONTENT_LIGHT_LEVEL
         AV_FRAME_DATA_ICC_PROFILE
         AV_FRAME_DATA_QP_TABLE_PROPERTIES
         AV_FRAME_DATA_QP_TABLE_DATA
+        AV_FRAME_DATA_SEI_UNREGISTERED
 
     cdef struct AVFrameSideData:
         AVFrameSideDataType type
         uint8_t *data
         int size
         AVDictionary *metadata
```

### Comparing `ha-av-9.1.1.post3/include/libavfilter/avfilter.pxd` & `ha-av-9.2.0.post1/include/libavfilter/avfilter.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavfilter/avfiltergraph.pxd` & `ha-av-9.2.0.post1/include/libavfilter/avfiltergraph.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavformat/avformat.pxd` & `ha-av-9.2.0.post1/include/libavformat/avformat.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavutil/avutil.pxd` & `ha-av-9.2.0.post1/include/libavutil/avutil.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavutil/dict.pxd` & `ha-av-9.2.0.post1/include/libavutil/dict.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavutil/error.pxd` & `ha-av-9.2.0.post1/include/libavutil/error.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavutil/frame.pxd` & `ha-av-9.2.0.post1/include/libavutil/frame.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libavutil/samplefmt.pxd` & `ha-av-9.2.0.post1/include/libavutil/samplefmt.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libswresample/swresample.pxd` & `ha-av-9.2.0.post1/include/libswresample/swresample.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/include/libswscale/swscale.pxd` & `ha-av-9.2.0.post1/include/libswscale/swscale.pxd`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/setup.cfg` & `ha-av-9.2.0.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/setup.py` & `ha-av-9.2.0.post1/setup.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/src/av/_core.c` & `ha-av-9.2.0.post1/src/av/_core.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/codeccontext.c` & `ha-av-9.2.0.post1/src/av/audio/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/fifo.c` & `ha-av-9.2.0.post1/src/av/audio/fifo.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/format.c` & `ha-av-9.2.0.post1/src/av/audio/format.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/frame.c` & `ha-av-9.2.0.post1/src/av/audio/frame.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/layout.c` & `ha-av-9.2.0.post1/src/av/audio/layout.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/plane.c` & `ha-av-9.2.0.post1/src/av/audio/plane.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/resampler.c` & `ha-av-9.2.0.post1/src/av/audio/resampler.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/audio/stream.c` & `ha-av-9.2.0.post1/src/av/audio/stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/buffer.c` & `ha-av-9.2.0.post1/src/av/buffer.c`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/src/av/bytesource.c` & `ha-av-9.2.0.post1/src/av/bytesource.c`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/src/av/codec/codec.c` & `ha-av-9.2.0.post1/src/av/codec/codec.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/codec/context.c` & `ha-av-9.2.0.post1/src/av/codec/context.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1547,15 +1555,15 @@
   PyObject *(*_rebase_time)(struct __pyx_obj_2av_5frame_Frame *, AVRational);
   PyObject *(*_copy_internal_attributes)(struct __pyx_obj_2av_5frame_Frame *, struct __pyx_obj_2av_5frame_Frame *, struct __pyx_opt_args_2av_5frame_5Frame__copy_internal_attributes *__pyx_optional_args);
   PyObject *(*_init_user_attributes)(struct __pyx_obj_2av_5frame_Frame *);
 };
 static struct __pyx_vtabstruct_2av_5frame_Frame *__pyx_vtabptr_2av_5frame_Frame;
 
 
-/* "av/codec/context.pyx":141
+/* "av/codec/context.pyx":144
  * 
  * 
  * cdef class CodecContext(object):             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
 
@@ -2104,14 +2112,15 @@
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_open[] = "open";
 static const char __pyx_k_psnr[] = "psnr";
 static const char __pyx_k_qpel[] = "qpel";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_type[] = "type";
+static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_BIDIR[] = "BIDIR";
 static const char __pyx_k_FRAME[] = "FRAME";
 static const char __pyx_k_Flags[] = "Flags";
 static const char __pyx_k_PASS1[] = "PASS1";
 static const char __pyx_k_PASS2[] = "PASS2";
 static const char __pyx_k_SLICE[] = "SLICE";
 static const char __pyx_k_ascii[] = "ascii";
@@ -2160,14 +2169,15 @@
 static const char __pyx_k_encoding[] = "encoding";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_property[] = "property";
 static const char __pyx_k_sentinel[] = "sentinel";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_show_all[] = "show_all";
 static const char __pyx_k_to_bytes[] = "to_bytes";
+static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_LOW_DELAY[] = "LOW_DELAY";
 static const char __pyx_k_NO_OUTPUT[] = "NO_OUTPUT";
 static const char __pyx_k_TRUNCATED[] = "TRUNCATED";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_UNALIGNED[] = "UNALIGNED";
 static const char __pyx_k_byteorder[] = "byteorder";
 static const char __pyx_k_get_flags[] = "_get_flags";
@@ -2184,14 +2194,15 @@
 static const char __pyx_k_ThreadType[] = "ThreadType";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_closed_gop[] = "closed_gop";
 static const char __pyx_k_export_mvs[] = "export_mvs";
 static const char __pyx_k_from_bytes[] = "from_bytes";
 static const char __pyx_k_get_flags2[] = "_get_flags2";
 static const char __pyx_k_is_decoder[] = "is_decoder";
+static const char __pyx_k_is_encoder[] = "is_encoder";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_set_flags2[] = "_set_flags2";
 static const char __pyx_k_DROPCHANGED[] = "DROPCHANGED";
 static const char __pyx_k_Discard_all[] = "Discard all";
 static const char __pyx_k_IGNORE_CROP[] = "IGNORE_CROP";
 static const char __pyx_k_LOOP_FILTER[] = "LOOP_FILTER";
 static const char __pyx_k_MemoryError[] = "MemoryError";
@@ -2214,14 +2225,15 @@
 static const char __pyx_k_global_header[] = "global_header";
 static const char __pyx_k_interlaced_me[] = "interlaced_me";
 static const char __pyx_k_loop_filter_2[] = "loop_filter";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_ro_flush_noop[] = "ro_flush_noop";
 static const char __pyx_k_INTERLACED_DCT[] = "INTERLACED_DCT";
 static const char __pyx_k_OUTPUT_CORRUPT[] = "OUTPUT_CORRUPT";
+static const char __pyx_k_av_deprecation[] = "av.deprecation";
 static const char __pyx_k_interlaced_dct[] = "interlaced_dct";
 static const char __pyx_k_output_corrupt[] = "output_corrupt";
 static const char __pyx_k_Discard_nothing[] = "Discard nothing";
 static const char __pyx_k_Force_low_delay[] = "Force low delay.";
 static const char __pyx_k_No_parser_for_s[] = "No parser for %s";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_Use_fixed_qscale[] = "Use fixed qscale.";
@@ -2230,14 +2242,15 @@
 static const char __pyx_k_AudioCodecContext[] = "AudioCodecContext";
 static const char __pyx_k_VideoCodecContext[] = "VideoCodecContext";
 static const char __pyx_k_Use_interlaced_DCT[] = "Use interlaced DCT.";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_DROP_FRAME_TIMECODE[] = "DROP_FRAME_TIMECODE";
 static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_drop_frame_timecode[] = "drop_frame_timecode";
+static const char __pyx_k_AVDeprecationWarning[] = "AVDeprecationWarning";
 static const char __pyx_k_SubtitleCodecContext[] = "SubtitleCodecContext";
 static const char __pyx_k_av_codec_context_pyx[] = "av/codec/context.pyx";
 static const char __pyx_k_av_audio_codeccontext[] = "av.audio.codeccontext";
 static const char __pyx_k_av_video_codeccontext[] = "av.video.codeccontext";
 static const char __pyx_k_Skip_bitstream_encoding[] = "Skip bitstream encoding.";
 static const char __pyx_k_Cannot_allocate_extradata[] = "Cannot allocate extradata";
 static const char __pyx_k_Discard_all_non_reference[] = "Discard all non reference";
@@ -2276,24 +2289,26 @@
 static const char __pyx_k_Output_even_those_frames_that_mi[] = "Output even those frames that might be corrupted.";
 static const char __pyx_k_Place_global_headers_at_every_ke[] = "Place global headers at every keyframe instead of in extradata.";
 static const char __pyx_k_Place_global_headers_in_extradat[] = "Place global headers in extradata instead of every keyframe.";
 static const char __pyx_k_Show_all_frames_before_the_first[] = "Show all frames before the first keyframe";
 static const char __pyx_k_Timecode_is_in_drop_frame_format[] = "Timecode is in drop frame format. DEPRECATED!!!!";
 static const char __pyx_k_Use_internal_2pass_ratecontrol_i[] = "Use internal 2pass ratecontrol in first pass mode.";
 static const char __pyx_k_Use_only_bitexact_stuff_except_I[] = "Use only bitexact stuff (except (I)DCT).";
+static const char __pyx_k_Using_CodecContext_time_base_for[] = "Using CodecContext.time_base for decoders is deprecated.";
 static const char __pyx_k_Wrapping_CodecContext_with_misma[] = "Wrapping CodecContext with mismatched codec.";
 static const char __pyx_k_error_variables_will_be_set_duri[] = "error[?] variables will be set during encoding.";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_Input_bitstream_might_be_truncat_2[] = "Input bitstream might be truncated at a packet boundaries\n        instead of only at frame boundaries.";
 static const char __pyx_k_Use_internal_2pass_ratecontrol_i_2[] = "Use internal 2pass ratecontrol in second pass mode.";
 static PyObject *__pyx_kp_s_4MV;
 static PyObject *__pyx_kp_s_4_MV_per_MB_allowed_advanced_pre;
 static PyObject *__pyx_n_s_AC_PRED;
 static PyObject *__pyx_n_s_ALL;
 static PyObject *__pyx_n_s_AUTO;
+static PyObject *__pyx_n_s_AVDeprecationWarning;
 static PyObject *__pyx_kp_s_Allow_decoders_to_produce_frames;
 static PyObject *__pyx_kp_s_Allow_non_spec_compliant_speedup;
 static PyObject *__pyx_n_s_AudioCodecContext;
 static PyObject *__pyx_n_s_BIDIR;
 static PyObject *__pyx_n_s_BITEXACT;
 static PyObject *__pyx_kp_s_Base_CodecContext_cannot_decode;
 static PyObject *__pyx_n_s_CHUNKS;
@@ -2381,22 +2396,24 @@
 static PyObject *__pyx_n_s_UNALIGNED;
 static PyObject *__pyx_kp_s_Use_fixed_qscale;
 static PyObject *__pyx_kp_s_Use_interlaced_DCT;
 static PyObject *__pyx_kp_s_Use_internal_2pass_ratecontrol_i;
 static PyObject *__pyx_kp_s_Use_internal_2pass_ratecontrol_i_2;
 static PyObject *__pyx_kp_s_Use_only_bitexact_stuff_except_I;
 static PyObject *__pyx_kp_s_Use_qpel_MC;
+static PyObject *__pyx_kp_s_Using_CodecContext_time_base_for;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_VideoCodecContext;
 static PyObject *__pyx_kp_s_Wrapping_CodecContext_with_misma;
 static PyObject *__pyx_n_s_ac_pred;
 static PyObject *__pyx_n_s_ascii;
 static PyObject *__pyx_n_s_av_audio_codeccontext;
 static PyObject *__pyx_n_s_av_codec_context;
 static PyObject *__pyx_kp_s_av_codec_context_pyx;
+static PyObject *__pyx_n_s_av_deprecation;
 static PyObject *__pyx_n_s_av_dictionary;
 static PyObject *__pyx_kp_s_av_s_s_s_at_0x_x;
 static PyObject *__pyx_n_s_av_subtitles_codeccontext;
 static PyObject *__pyx_n_s_av_video_codeccontext;
 static PyObject *__pyx_n_s_bitexact;
 static PyObject *__pyx_n_s_byteorder;
 static PyObject *__pyx_n_s_c_ctx;
@@ -2432,14 +2449,15 @@
 static PyObject *__pyx_n_s_gray;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_ignore_crop;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_interlaced_dct;
 static PyObject *__pyx_n_s_interlaced_me;
 static PyObject *__pyx_n_s_is_decoder;
+static PyObject *__pyx_n_s_is_encoder;
 static PyObject *__pyx_n_s_little;
 static PyObject *__pyx_n_s_local_header;
 static PyObject *__pyx_kp_s_loop_filter;
 static PyObject *__pyx_n_s_loop_filter_2;
 static PyObject *__pyx_n_s_low_delay;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_mode;
@@ -2478,14 +2496,16 @@
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_to_bytes;
 static PyObject *__pyx_n_s_truncated;
 static PyObject *__pyx_n_s_type;
 static PyObject *__pyx_n_s_unaligned;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_value;
+static PyObject *__pyx_n_s_warn;
+static PyObject *__pyx_n_s_warnings;
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_create(PyObject *__pyx_v_codec, PyObject *__pyx_v_mode); /* proto */
 static int __pyx_pf_2av_5codec_7context_12CodecContext_2__cinit__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, PyObject *__pyx_v_sentinel, CYTHON_UNUSED PyObject *__pyx_v_args, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_4_get_flags(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_6_set_flags(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_8_get_flags2(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_10_set_flags2(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_9extradata___get__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self); /* proto */
@@ -2547,15 +2567,15 @@
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_codeobj__19;
 /* Late includes */
 
-/* "av/codec/context.pyx":20
+/* "av/codec/context.pyx":23
  * 
  * 
  * cdef CodecContext wrap_codec_context(lib.AVCodecContext *c_ctx, const lib.AVCodec *c_codec, bint allocated):             # <<<<<<<<<<<<<<
  *     """Build an av.CodecContext for an existing AVCodecContext."""
  * 
  */
 
@@ -2570,47 +2590,47 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap_codec_context", 0);
 
-  /* "av/codec/context.pyx":26
+  /* "av/codec/context.pyx":29
  * 
  *     # TODO: This.
  *     if c_ctx.codec_type == lib.AVMEDIA_TYPE_VIDEO:             # <<<<<<<<<<<<<<
  *         from av.video.codeccontext import VideoCodecContext
  *         py_ctx = VideoCodecContext(_cinit_sentinel)
  */
   switch (__pyx_v_c_ctx->codec_type) {
     case AVMEDIA_TYPE_VIDEO:
 
-    /* "av/codec/context.pyx":27
+    /* "av/codec/context.pyx":30
  *     # TODO: This.
  *     if c_ctx.codec_type == lib.AVMEDIA_TYPE_VIDEO:
  *         from av.video.codeccontext import VideoCodecContext             # <<<<<<<<<<<<<<
  *         py_ctx = VideoCodecContext(_cinit_sentinel)
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_AUDIO:
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_VideoCodecContext);
     __Pyx_GIVEREF(__pyx_n_s_VideoCodecContext);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_VideoCodecContext);
-    __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_video_codeccontext, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_video_codeccontext, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_VideoCodecContext); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_VideoCodecContext); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_VideoCodecContext = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "av/codec/context.pyx":28
+    /* "av/codec/context.pyx":31
  *     if c_ctx.codec_type == lib.AVMEDIA_TYPE_VIDEO:
  *         from av.video.codeccontext import VideoCodecContext
  *         py_ctx = VideoCodecContext(_cinit_sentinel)             # <<<<<<<<<<<<<<
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_AUDIO:
  *         from av.audio.codeccontext import AudioCodecContext
  */
     __Pyx_INCREF(__pyx_v_VideoCodecContext);
@@ -2622,54 +2642,54 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_2av_5codec_7context__cinit_sentinel) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_2av_5codec_7context__cinit_sentinel);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5codec_7context_CodecContext))))) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5codec_7context_CodecContext))))) __PYX_ERR(0, 31, __pyx_L1_error)
     __pyx_v_py_ctx = ((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "av/codec/context.pyx":26
+    /* "av/codec/context.pyx":29
  * 
  *     # TODO: This.
  *     if c_ctx.codec_type == lib.AVMEDIA_TYPE_VIDEO:             # <<<<<<<<<<<<<<
  *         from av.video.codeccontext import VideoCodecContext
  *         py_ctx = VideoCodecContext(_cinit_sentinel)
  */
     break;
     case AVMEDIA_TYPE_AUDIO:
 
-    /* "av/codec/context.pyx":30
+    /* "av/codec/context.pyx":33
  *         py_ctx = VideoCodecContext(_cinit_sentinel)
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_AUDIO:
  *         from av.audio.codeccontext import AudioCodecContext             # <<<<<<<<<<<<<<
  *         py_ctx = AudioCodecContext(_cinit_sentinel)
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_SUBTITLE:
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_AudioCodecContext);
     __Pyx_GIVEREF(__pyx_n_s_AudioCodecContext);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_AudioCodecContext);
-    __pyx_t_1 = __Pyx_Import(__pyx_n_s_av_audio_codeccontext, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_Import(__pyx_n_s_av_audio_codeccontext, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_AudioCodecContext); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_AudioCodecContext); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_v_AudioCodecContext = __pyx_t_2;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "av/codec/context.pyx":31
+    /* "av/codec/context.pyx":34
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_AUDIO:
  *         from av.audio.codeccontext import AudioCodecContext
  *         py_ctx = AudioCodecContext(_cinit_sentinel)             # <<<<<<<<<<<<<<
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_SUBTITLE:
  *         from av.subtitles.codeccontext import SubtitleCodecContext
  */
     __Pyx_INCREF(__pyx_v_AudioCodecContext);
@@ -2681,54 +2701,54 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_2av_5codec_7context__cinit_sentinel) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_2av_5codec_7context__cinit_sentinel);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_2av_5codec_7context_CodecContext))))) __PYX_ERR(0, 31, __pyx_L1_error)
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_2av_5codec_7context_CodecContext))))) __PYX_ERR(0, 34, __pyx_L1_error)
     __pyx_v_py_ctx = ((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "av/codec/context.pyx":29
+    /* "av/codec/context.pyx":32
  *         from av.video.codeccontext import VideoCodecContext
  *         py_ctx = VideoCodecContext(_cinit_sentinel)
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_AUDIO:             # <<<<<<<<<<<<<<
  *         from av.audio.codeccontext import AudioCodecContext
  *         py_ctx = AudioCodecContext(_cinit_sentinel)
  */
     break;
     case AVMEDIA_TYPE_SUBTITLE:
 
-    /* "av/codec/context.pyx":33
+    /* "av/codec/context.pyx":36
  *         py_ctx = AudioCodecContext(_cinit_sentinel)
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_SUBTITLE:
  *         from av.subtitles.codeccontext import SubtitleCodecContext             # <<<<<<<<<<<<<<
  *         py_ctx = SubtitleCodecContext(_cinit_sentinel)
  *     else:
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_SubtitleCodecContext);
     __Pyx_GIVEREF(__pyx_n_s_SubtitleCodecContext);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_SubtitleCodecContext);
-    __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_subtitles_codeccontext, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_subtitles_codeccontext, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SubtitleCodecContext); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SubtitleCodecContext); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_SubtitleCodecContext = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "av/codec/context.pyx":34
+    /* "av/codec/context.pyx":37
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_SUBTITLE:
  *         from av.subtitles.codeccontext import SubtitleCodecContext
  *         py_ctx = SubtitleCodecContext(_cinit_sentinel)             # <<<<<<<<<<<<<<
  *     else:
  *         py_ctx = CodecContext(_cinit_sentinel)
  */
     __Pyx_INCREF(__pyx_v_SubtitleCodecContext);
@@ -2740,78 +2760,78 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_2av_5codec_7context__cinit_sentinel) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_2av_5codec_7context__cinit_sentinel);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5codec_7context_CodecContext))))) __PYX_ERR(0, 34, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5codec_7context_CodecContext))))) __PYX_ERR(0, 37, __pyx_L1_error)
     __pyx_v_py_ctx = ((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "av/codec/context.pyx":32
+    /* "av/codec/context.pyx":35
  *         from av.audio.codeccontext import AudioCodecContext
  *         py_ctx = AudioCodecContext(_cinit_sentinel)
  *     elif c_ctx.codec_type == lib.AVMEDIA_TYPE_SUBTITLE:             # <<<<<<<<<<<<<<
  *         from av.subtitles.codeccontext import SubtitleCodecContext
  *         py_ctx = SubtitleCodecContext(_cinit_sentinel)
  */
     break;
     default:
 
-    /* "av/codec/context.pyx":36
+    /* "av/codec/context.pyx":39
  *         py_ctx = SubtitleCodecContext(_cinit_sentinel)
  *     else:
  *         py_ctx = CodecContext(_cinit_sentinel)             # <<<<<<<<<<<<<<
  * 
  *     py_ctx.allocated = allocated
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext), __pyx_v_2av_5codec_7context__cinit_sentinel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext), __pyx_v_2av_5codec_7context__cinit_sentinel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_py_ctx = ((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_t_2);
     __pyx_t_2 = 0;
     break;
   }
 
-  /* "av/codec/context.pyx":38
+  /* "av/codec/context.pyx":41
  *         py_ctx = CodecContext(_cinit_sentinel)
  * 
  *     py_ctx.allocated = allocated             # <<<<<<<<<<<<<<
  *     py_ctx._init(c_ctx, c_codec)
  * 
  */
   __pyx_v_py_ctx->allocated = __pyx_v_allocated;
 
-  /* "av/codec/context.pyx":39
+  /* "av/codec/context.pyx":42
  * 
  *     py_ctx.allocated = allocated
  *     py_ctx._init(c_ctx, c_codec)             # <<<<<<<<<<<<<<
  * 
  *     return py_ctx
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_py_ctx->__pyx_vtab)->_init(__pyx_v_py_ctx, __pyx_v_c_ctx, __pyx_v_c_codec); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_py_ctx->__pyx_vtab)->_init(__pyx_v_py_ctx, __pyx_v_c_ctx, __pyx_v_c_codec); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":41
+  /* "av/codec/context.pyx":44
  *     py_ctx._init(c_ctx, c_codec)
  * 
  *     return py_ctx             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_py_ctx));
   __pyx_r = __pyx_v_py_ctx;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":20
+  /* "av/codec/context.pyx":23
  * 
  * 
  * cdef CodecContext wrap_codec_context(lib.AVCodecContext *c_ctx, const lib.AVCodec *c_codec, bint allocated):             # <<<<<<<<<<<<<<
  *     """Build an av.CodecContext for an existing AVCodecContext."""
  * 
  */
 
@@ -2828,15 +2848,15 @@
   __Pyx_XDECREF(__pyx_v_AudioCodecContext);
   __Pyx_XDECREF(__pyx_v_SubtitleCodecContext);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":144
+/* "av/codec/context.pyx":147
  * 
  *     @staticmethod
  *     def create(codec, mode=None):             # <<<<<<<<<<<<<<
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)
  */
 
@@ -2877,15 +2897,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "create") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "create") < 0)) __PYX_ERR(0, 147, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -2893,15 +2913,15 @@
       }
     }
     __pyx_v_codec = values[0];
     __pyx_v_mode = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("create", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("create", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 147, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.create", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2av_5codec_7context_12CodecContext_create(__pyx_v_codec, __pyx_v_mode);
 
@@ -2920,68 +2940,68 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create", 0);
 
-  /* "av/codec/context.pyx":145
+  /* "av/codec/context.pyx":148
  *     @staticmethod
  *     def create(codec, mode=None):
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)             # <<<<<<<<<<<<<<
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)
  *         return wrap_codec_context(c_ctx, cy_codec.ptr, True)
  */
   __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_codec, __pyx_ptype_2av_5codec_5codec_Codec); 
   if ((__pyx_t_2 != 0)) {
-    if (!(likely(((__pyx_v_codec) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_codec, __pyx_ptype_2av_5codec_5codec_Codec))))) __PYX_ERR(0, 145, __pyx_L1_error)
+    if (!(likely(((__pyx_v_codec) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_codec, __pyx_ptype_2av_5codec_5codec_Codec))))) __PYX_ERR(0, 148, __pyx_L1_error)
     __Pyx_INCREF(__pyx_v_codec);
     __pyx_t_1 = __pyx_v_codec;
   } else {
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_codec);
     __Pyx_GIVEREF(__pyx_v_codec);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_codec);
     __Pyx_INCREF(__pyx_v_mode);
     __Pyx_GIVEREF(__pyx_v_mode);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_mode);
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_5codec_5codec_Codec), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_5codec_5codec_Codec), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_v_cy_codec = ((struct __pyx_obj_2av_5codec_5codec_Codec *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":146
+  /* "av/codec/context.pyx":149
  *     def create(codec, mode=None):
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)             # <<<<<<<<<<<<<<
  *         return wrap_codec_context(c_ctx, cy_codec.ptr, True)
  * 
  */
   __pyx_v_c_ctx = avcodec_alloc_context3(__pyx_v_cy_codec->ptr);
 
-  /* "av/codec/context.pyx":147
+  /* "av/codec/context.pyx":150
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)
  *         return wrap_codec_context(c_ctx, cy_codec.ptr, True)             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, sentinel=None, *args, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_2av_5codec_7context_wrap_codec_context(__pyx_v_c_ctx, __pyx_v_cy_codec->ptr, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_2av_5codec_7context_wrap_codec_context(__pyx_v_c_ctx, __pyx_v_cy_codec->ptr, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":144
+  /* "av/codec/context.pyx":147
  * 
  *     @staticmethod
  *     def create(codec, mode=None):             # <<<<<<<<<<<<<<
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)
  */
 
@@ -2995,15 +3015,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cy_codec);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":149
+/* "av/codec/context.pyx":152
  *         return wrap_codec_context(c_ctx, cy_codec.ptr, True)
  * 
  *     def __cinit__(self, sentinel=None, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         if sentinel is not _cinit_sentinel:
  *             raise RuntimeError('Cannot instantiate CodecContext')
  */
 
@@ -3051,15 +3071,15 @@
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sentinel);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 149, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 152, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         default:
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -3091,72 +3111,72 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "av/codec/context.pyx":150
+  /* "av/codec/context.pyx":153
  * 
  *     def __cinit__(self, sentinel=None, *args, **kwargs):
  *         if sentinel is not _cinit_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('Cannot instantiate CodecContext')
  * 
  */
   __pyx_t_1 = (__pyx_v_sentinel != __pyx_v_2av_5codec_7context__cinit_sentinel);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/codec/context.pyx":151
+    /* "av/codec/context.pyx":154
  *     def __cinit__(self, sentinel=None, *args, **kwargs):
  *         if sentinel is not _cinit_sentinel:
  *             raise RuntimeError('Cannot instantiate CodecContext')             # <<<<<<<<<<<<<<
  * 
  *         self.options = {}
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 151, __pyx_L1_error)
+    __PYX_ERR(0, 154, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":150
+    /* "av/codec/context.pyx":153
  * 
  *     def __cinit__(self, sentinel=None, *args, **kwargs):
  *         if sentinel is not _cinit_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('Cannot instantiate CodecContext')
  * 
  */
   }
 
-  /* "av/codec/context.pyx":153
+  /* "av/codec/context.pyx":156
  *             raise RuntimeError('Cannot instantiate CodecContext')
  * 
  *         self.options = {}             # <<<<<<<<<<<<<<
  *         self.stream_index = -1  # This is set by the container immediately.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->options);
   __Pyx_DECREF(__pyx_v_self->options);
   __pyx_v_self->options = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "av/codec/context.pyx":154
+  /* "av/codec/context.pyx":157
  * 
  *         self.options = {}
  *         self.stream_index = -1  # This is set by the container immediately.             # <<<<<<<<<<<<<<
  * 
  *     cdef _init(self, lib.AVCodecContext *ptr, const lib.AVCodec *codec):
  */
   __pyx_v_self->stream_index = -1;
 
-  /* "av/codec/context.pyx":149
+  /* "av/codec/context.pyx":152
  *         return wrap_codec_context(c_ctx, cy_codec.ptr, True)
  * 
  *     def __cinit__(self, sentinel=None, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         if sentinel is not _cinit_sentinel:
  *             raise RuntimeError('Cannot instantiate CodecContext')
  */
 
@@ -3168,15 +3188,15 @@
   __Pyx_AddTraceback("av.codec.context.CodecContext.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":156
+/* "av/codec/context.pyx":159
  *         self.stream_index = -1  # This is set by the container immediately.
  * 
  *     cdef _init(self, lib.AVCodecContext *ptr, const lib.AVCodec *codec):             # <<<<<<<<<<<<<<
  * 
  *         self.ptr = ptr
  */
 
@@ -3188,24 +3208,24 @@
   PyObject *__pyx_t_3 = NULL;
   struct AVCodec const *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_init", 0);
 
-  /* "av/codec/context.pyx":158
+  /* "av/codec/context.pyx":161
  *     cdef _init(self, lib.AVCodecContext *ptr, const lib.AVCodec *codec):
  * 
  *         self.ptr = ptr             # <<<<<<<<<<<<<<
  *         if self.ptr.codec and codec and self.ptr.codec != codec:
  *             raise RuntimeError('Wrapping CodecContext with mismatched codec.')
  */
   __pyx_v_self->ptr = __pyx_v_ptr;
 
-  /* "av/codec/context.pyx":159
+  /* "av/codec/context.pyx":162
  * 
  *         self.ptr = ptr
  *         if self.ptr.codec and codec and self.ptr.codec != codec:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('Wrapping CodecContext with mismatched codec.')
  *         self.codec = wrap_codec(codec if codec != NULL else self.ptr.codec)
  */
   __pyx_t_2 = (__pyx_v_self->ptr->codec != 0);
@@ -3221,84 +3241,84 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_self->ptr->codec != __pyx_v_codec) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "av/codec/context.pyx":160
+    /* "av/codec/context.pyx":163
  *         self.ptr = ptr
  *         if self.ptr.codec and codec and self.ptr.codec != codec:
  *             raise RuntimeError('Wrapping CodecContext with mismatched codec.')             # <<<<<<<<<<<<<<
  *         self.codec = wrap_codec(codec if codec != NULL else self.ptr.codec)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 160, __pyx_L1_error)
+    __PYX_ERR(0, 163, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":159
+    /* "av/codec/context.pyx":162
  * 
  *         self.ptr = ptr
  *         if self.ptr.codec and codec and self.ptr.codec != codec:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('Wrapping CodecContext with mismatched codec.')
  *         self.codec = wrap_codec(codec if codec != NULL else self.ptr.codec)
  */
   }
 
-  /* "av/codec/context.pyx":161
+  /* "av/codec/context.pyx":164
  *         if self.ptr.codec and codec and self.ptr.codec != codec:
  *             raise RuntimeError('Wrapping CodecContext with mismatched codec.')
  *         self.codec = wrap_codec(codec if codec != NULL else self.ptr.codec)             # <<<<<<<<<<<<<<
  * 
  *         # Set reasonable threading defaults.
  */
   if (((__pyx_v_codec != NULL) != 0)) {
     __pyx_t_4 = __pyx_v_codec;
   } else {
     __pyx_t_4 = __pyx_v_self->ptr->codec;
   }
-  __pyx_t_3 = ((PyObject *)__pyx_f_2av_5codec_5codec_wrap_codec(__pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)__pyx_f_2av_5codec_5codec_wrap_codec(__pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->codec);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->codec));
   __pyx_v_self->codec = ((struct __pyx_obj_2av_5codec_5codec_Codec *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "av/codec/context.pyx":166
+  /* "av/codec/context.pyx":169
  *         # count == 0 -> use as many threads as there are CPUs.
  *         # type == 2 -> thread within a frame. This does not change the API.
  *         self.ptr.thread_count = 0             # <<<<<<<<<<<<<<
  *         self.ptr.thread_type = 2
  * 
  */
   __pyx_v_self->ptr->thread_count = 0;
 
-  /* "av/codec/context.pyx":167
+  /* "av/codec/context.pyx":170
  *         # type == 2 -> thread within a frame. This does not change the API.
  *         self.ptr.thread_count = 0
  *         self.ptr.thread_type = 2             # <<<<<<<<<<<<<<
  * 
  *         # Use "ass" format for subtitles (default as of FFmpeg 5.0), not the
  */
   __pyx_v_self->ptr->thread_type = 2;
 
-  /* "av/codec/context.pyx":171
+  /* "av/codec/context.pyx":174
  *         # Use "ass" format for subtitles (default as of FFmpeg 5.0), not the
  *         #deprecated "ass_with_timings" formats.
  *         self.ptr.sub_text_format = 0             # <<<<<<<<<<<<<<
  * 
  *     def _get_flags(self):
  */
   __pyx_v_self->ptr->sub_text_format = 0;
 
-  /* "av/codec/context.pyx":156
+  /* "av/codec/context.pyx":159
  *         self.stream_index = -1  # This is set by the container immediately.
  * 
  *     cdef _init(self, lib.AVCodecContext *ptr, const lib.AVCodec *codec):             # <<<<<<<<<<<<<<
  * 
  *         self.ptr = ptr
  */
 
@@ -3311,15 +3331,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":173
+/* "av/codec/context.pyx":176
  *         self.ptr.sub_text_format = 0
  * 
  *     def _get_flags(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.flags
  * 
  */
 
@@ -3342,29 +3362,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_flags", 0);
 
-  /* "av/codec/context.pyx":174
+  /* "av/codec/context.pyx":177
  * 
  *     def _get_flags(self):
  *         return self.ptr.flags             # <<<<<<<<<<<<<<
  * 
  *     def _set_flags(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":173
+  /* "av/codec/context.pyx":176
  *         self.ptr.sub_text_format = 0
  * 
  *     def _get_flags(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.flags
  * 
  */
 
@@ -3375,15 +3395,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":176
+/* "av/codec/context.pyx":179
  *         return self.ptr.flags
  * 
  *     def _set_flags(self, value):             # <<<<<<<<<<<<<<
  *         self.ptr.flags = value
  * 
  */
 
@@ -3406,25 +3426,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_flags", 0);
 
-  /* "av/codec/context.pyx":177
+  /* "av/codec/context.pyx":180
  * 
  *     def _set_flags(self, value):
  *         self.ptr.flags = value             # <<<<<<<<<<<<<<
  * 
  *     flags = Flags.property(
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_v_self->ptr->flags = __pyx_t_1;
 
-  /* "av/codec/context.pyx":176
+  /* "av/codec/context.pyx":179
  *         return self.ptr.flags
  * 
  *     def _set_flags(self, value):             # <<<<<<<<<<<<<<
  *         self.ptr.flags = value
  * 
  */
 
@@ -3436,15 +3456,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":205
+/* "av/codec/context.pyx":208
  *     closed_gop = flags.flag_property('CLOSED_GOP')
  * 
  *     def _get_flags2(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.flags2
  * 
  */
 
@@ -3467,29 +3487,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_flags2", 0);
 
-  /* "av/codec/context.pyx":206
+  /* "av/codec/context.pyx":209
  * 
  *     def _get_flags2(self):
  *         return self.ptr.flags2             # <<<<<<<<<<<<<<
  * 
  *     def _set_flags2(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->flags2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->flags2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":205
+  /* "av/codec/context.pyx":208
  *     closed_gop = flags.flag_property('CLOSED_GOP')
  * 
  *     def _get_flags2(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.flags2
  * 
  */
 
@@ -3500,15 +3520,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":208
+/* "av/codec/context.pyx":211
  *         return self.ptr.flags2
  * 
  *     def _set_flags2(self, value):             # <<<<<<<<<<<<<<
  *         self.ptr.flags2 = value
  * 
  */
 
@@ -3531,25 +3551,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_flags2", 0);
 
-  /* "av/codec/context.pyx":209
+  /* "av/codec/context.pyx":212
  * 
  *     def _set_flags2(self, value):
  *         self.ptr.flags2 = value             # <<<<<<<<<<<<<<
  * 
  *     flags2 = Flags2.property(
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
   __pyx_v_self->ptr->flags2 = __pyx_t_1;
 
-  /* "av/codec/context.pyx":208
+  /* "av/codec/context.pyx":211
  *         return self.ptr.flags2
  * 
  *     def _set_flags2(self, value):             # <<<<<<<<<<<<<<
  *         self.ptr.flags2 = value
  * 
  */
 
@@ -3561,15 +3581,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":229
+/* "av/codec/context.pyx":232
  * 
  *     property extradata:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if self.ptr.extradata_size > 0:
  *                 return <bytes>(<uint8_t*>self.ptr.extradata)[:self.ptr.extradata_size]
  */
 
@@ -3592,62 +3612,62 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":230
+  /* "av/codec/context.pyx":233
  *     property extradata:
  *         def __get__(self):
  *             if self.ptr.extradata_size > 0:             # <<<<<<<<<<<<<<
  *                 return <bytes>(<uint8_t*>self.ptr.extradata)[:self.ptr.extradata_size]
  *             else:
  */
   __pyx_t_1 = ((__pyx_v_self->ptr->extradata_size > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":231
+    /* "av/codec/context.pyx":234
  *         def __get__(self):
  *             if self.ptr.extradata_size > 0:
  *                 return <bytes>(<uint8_t*>self.ptr.extradata)[:self.ptr.extradata_size]             # <<<<<<<<<<<<<<
  *             else:
  *                 return None
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((const char*)((uint8_t *)__pyx_v_self->ptr->extradata)) + 0, __pyx_v_self->ptr->extradata_size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((const char*)((uint8_t *)__pyx_v_self->ptr->extradata)) + 0, __pyx_v_self->ptr->extradata_size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject*)__pyx_t_2));
     __pyx_r = __pyx_t_2;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":230
+    /* "av/codec/context.pyx":233
  *     property extradata:
  *         def __get__(self):
  *             if self.ptr.extradata_size > 0:             # <<<<<<<<<<<<<<
  *                 return <bytes>(<uint8_t*>self.ptr.extradata)[:self.ptr.extradata_size]
  *             else:
  */
   }
 
-  /* "av/codec/context.pyx":233
+  /* "av/codec/context.pyx":236
  *                 return <bytes>(<uint8_t*>self.ptr.extradata)[:self.ptr.extradata_size]
  *             else:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, data):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "av/codec/context.pyx":229
+  /* "av/codec/context.pyx":232
  * 
  *     property extradata:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if self.ptr.extradata_size > 0:
  *                 return <bytes>(<uint8_t*>self.ptr.extradata)[:self.ptr.extradata_size]
  */
 
@@ -3658,15 +3678,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":235
+/* "av/codec/context.pyx":238
  *                 return None
  * 
  *         def __set__(self, data):             # <<<<<<<<<<<<<<
  *             if not self.is_decoder:
  *                 raise ValueError("Can only set extradata for decoders.")
  */
 
@@ -3692,174 +3712,174 @@
   int __pyx_t_3;
   size_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":236
+  /* "av/codec/context.pyx":239
  * 
  *         def __set__(self, data):
  *             if not self.is_decoder:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Can only set extradata for decoders.")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_decoder); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_decoder); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "av/codec/context.pyx":237
+    /* "av/codec/context.pyx":240
  *         def __set__(self, data):
  *             if not self.is_decoder:
  *                 raise ValueError("Can only set extradata for decoders.")             # <<<<<<<<<<<<<<
  * 
  *             if data is None:
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 237, __pyx_L1_error)
+    __PYX_ERR(0, 240, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":236
+    /* "av/codec/context.pyx":239
  * 
  *         def __set__(self, data):
  *             if not self.is_decoder:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Can only set extradata for decoders.")
  * 
  */
   }
 
-  /* "av/codec/context.pyx":239
+  /* "av/codec/context.pyx":242
  *                 raise ValueError("Can only set extradata for decoders.")
  * 
  *             if data is None:             # <<<<<<<<<<<<<<
  *                 lib.av_freep(&self.ptr.extradata)
  *                 self.ptr.extradata_size = 0
  */
   __pyx_t_3 = (__pyx_v_data == Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "av/codec/context.pyx":240
+    /* "av/codec/context.pyx":243
  * 
  *             if data is None:
  *                 lib.av_freep(&self.ptr.extradata)             # <<<<<<<<<<<<<<
  *                 self.ptr.extradata_size = 0
  *             else:
  */
     av_freep((&__pyx_v_self->ptr->extradata));
 
-    /* "av/codec/context.pyx":241
+    /* "av/codec/context.pyx":244
  *             if data is None:
  *                 lib.av_freep(&self.ptr.extradata)
  *                 self.ptr.extradata_size = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 source = bytesource(data)
  */
     __pyx_v_self->ptr->extradata_size = 0;
 
-    /* "av/codec/context.pyx":239
+    /* "av/codec/context.pyx":242
  *                 raise ValueError("Can only set extradata for decoders.")
  * 
  *             if data is None:             # <<<<<<<<<<<<<<
  *                 lib.av_freep(&self.ptr.extradata)
  *                 self.ptr.extradata_size = 0
  */
     goto __pyx_L4;
   }
 
-  /* "av/codec/context.pyx":243
+  /* "av/codec/context.pyx":246
  *                 self.ptr.extradata_size = 0
  *             else:
  *                 source = bytesource(data)             # <<<<<<<<<<<<<<
  *                 self.ptr.extradata = <uint8_t*>lib.av_realloc(self.ptr.extradata, source.length + lib.AV_INPUT_BUFFER_PADDING_SIZE)
  *                 if not self.ptr.extradata:
  */
   /*else*/ {
-    __pyx_t_1 = ((PyObject *)__pyx_f_2av_10bytesource_bytesource(__pyx_v_data, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_2av_10bytesource_bytesource(__pyx_v_data, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_source = ((struct __pyx_obj_2av_10bytesource_ByteSource *)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "av/codec/context.pyx":244
+    /* "av/codec/context.pyx":247
  *             else:
  *                 source = bytesource(data)
  *                 self.ptr.extradata = <uint8_t*>lib.av_realloc(self.ptr.extradata, source.length + lib.AV_INPUT_BUFFER_PADDING_SIZE)             # <<<<<<<<<<<<<<
  *                 if not self.ptr.extradata:
  *                     raise MemoryError("Cannot allocate extradata")
  */
     __pyx_v_self->ptr->extradata = ((uint8_t *)av_realloc(__pyx_v_self->ptr->extradata, (__pyx_v_source->length + AV_INPUT_BUFFER_PADDING_SIZE)));
 
-    /* "av/codec/context.pyx":245
+    /* "av/codec/context.pyx":248
  *                 source = bytesource(data)
  *                 self.ptr.extradata = <uint8_t*>lib.av_realloc(self.ptr.extradata, source.length + lib.AV_INPUT_BUFFER_PADDING_SIZE)
  *                 if not self.ptr.extradata:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Cannot allocate extradata")
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)
  */
     __pyx_t_2 = ((!(__pyx_v_self->ptr->extradata != 0)) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "av/codec/context.pyx":246
+      /* "av/codec/context.pyx":249
  *                 self.ptr.extradata = <uint8_t*>lib.av_realloc(self.ptr.extradata, source.length + lib.AV_INPUT_BUFFER_PADDING_SIZE)
  *                 if not self.ptr.extradata:
  *                     raise MemoryError("Cannot allocate extradata")             # <<<<<<<<<<<<<<
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)
  *                 self.ptr.extradata_size = source.length
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 246, __pyx_L1_error)
+      __PYX_ERR(0, 249, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":245
+      /* "av/codec/context.pyx":248
  *                 source = bytesource(data)
  *                 self.ptr.extradata = <uint8_t*>lib.av_realloc(self.ptr.extradata, source.length + lib.AV_INPUT_BUFFER_PADDING_SIZE)
  *                 if not self.ptr.extradata:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Cannot allocate extradata")
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)
  */
     }
 
-    /* "av/codec/context.pyx":247
+    /* "av/codec/context.pyx":250
  *                 if not self.ptr.extradata:
  *                     raise MemoryError("Cannot allocate extradata")
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)             # <<<<<<<<<<<<<<
  *                 self.ptr.extradata_size = source.length
  *             self.extradata_set = True
  */
     (void)(memcpy(__pyx_v_self->ptr->extradata, __pyx_v_source->ptr, __pyx_v_source->length));
 
-    /* "av/codec/context.pyx":248
+    /* "av/codec/context.pyx":251
  *                     raise MemoryError("Cannot allocate extradata")
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)
  *                 self.ptr.extradata_size = source.length             # <<<<<<<<<<<<<<
  *             self.extradata_set = True
  * 
  */
     __pyx_t_4 = __pyx_v_source->length;
     __pyx_v_self->ptr->extradata_size = __pyx_t_4;
   }
   __pyx_L4:;
 
-  /* "av/codec/context.pyx":249
+  /* "av/codec/context.pyx":252
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)
  *                 self.ptr.extradata_size = source.length
  *             self.extradata_set = True             # <<<<<<<<<<<<<<
  * 
  *     property extradata_size:
  */
   __pyx_v_self->extradata_set = 1;
 
-  /* "av/codec/context.pyx":235
+  /* "av/codec/context.pyx":238
  *                 return None
  * 
  *         def __set__(self, data):             # <<<<<<<<<<<<<<
  *             if not self.is_decoder:
  *                 raise ValueError("Can only set extradata for decoders.")
  */
 
@@ -3872,15 +3892,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_source);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":252
+/* "av/codec/context.pyx":255
  * 
  *     property extradata_size:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.extradata_size
  * 
  */
 
@@ -3902,29 +3922,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":253
+  /* "av/codec/context.pyx":256
  *     property extradata_size:
  *         def __get__(self):
  *             return self.ptr.extradata_size             # <<<<<<<<<<<<<<
  * 
  *     property is_open:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->extradata_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->extradata_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":252
+  /* "av/codec/context.pyx":255
  * 
  *     property extradata_size:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.extradata_size
  * 
  */
 
@@ -3935,15 +3955,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":256
+/* "av/codec/context.pyx":259
  * 
  *     property is_open:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return lib.avcodec_is_open(self.ptr)
  * 
  */
 
@@ -3965,29 +3985,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":257
+  /* "av/codec/context.pyx":260
  *     property is_open:
  *         def __get__(self):
  *             return lib.avcodec_is_open(self.ptr)             # <<<<<<<<<<<<<<
  * 
  *     property is_encoder:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(avcodec_is_open(__pyx_v_self->ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(avcodec_is_open(__pyx_v_self->ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":256
+  /* "av/codec/context.pyx":259
  * 
  *     property is_open:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return lib.avcodec_is_open(self.ptr)
  * 
  */
 
@@ -3998,15 +4018,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":260
+/* "av/codec/context.pyx":263
  * 
  *     property is_encoder:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return lib.av_codec_is_encoder(self.ptr.codec)
  * 
  */
 
@@ -4028,29 +4048,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":261
+  /* "av/codec/context.pyx":264
  *     property is_encoder:
  *         def __get__(self):
  *             return lib.av_codec_is_encoder(self.ptr.codec)             # <<<<<<<<<<<<<<
  * 
  *     property is_decoder:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(av_codec_is_encoder(__pyx_v_self->ptr->codec)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(av_codec_is_encoder(__pyx_v_self->ptr->codec)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":260
+  /* "av/codec/context.pyx":263
  * 
  *     property is_encoder:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return lib.av_codec_is_encoder(self.ptr.codec)
  * 
  */
 
@@ -4061,15 +4081,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":264
+/* "av/codec/context.pyx":267
  * 
  *     property is_decoder:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return lib.av_codec_is_decoder(self.ptr.codec)
  * 
  */
 
@@ -4091,29 +4111,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":265
+  /* "av/codec/context.pyx":268
  *     property is_decoder:
  *         def __get__(self):
  *             return lib.av_codec_is_decoder(self.ptr.codec)             # <<<<<<<<<<<<<<
  * 
  *     cpdef open(self, bint strict=True):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(av_codec_is_decoder(__pyx_v_self->ptr->codec)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(av_codec_is_decoder(__pyx_v_self->ptr->codec)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":264
+  /* "av/codec/context.pyx":267
  * 
  *     property is_decoder:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return lib.av_codec_is_decoder(self.ptr.codec)
  * 
  */
 
@@ -4124,15 +4144,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":267
+/* "av/codec/context.pyx":270
  *             return lib.av_codec_is_decoder(self.ptr.codec)
  * 
  *     cpdef open(self, bint strict=True):             # <<<<<<<<<<<<<<
  * 
  *         if lib.avcodec_is_open(self.ptr):
  */
 
@@ -4145,14 +4165,15 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
+  int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_strict = __pyx_optional_args->strict;
@@ -4163,19 +4184,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_open); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_open); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2av_5codec_7context_12CodecContext_13open)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 270, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4183,15 +4204,15 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -4204,121 +4225,121 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "av/codec/context.pyx":269
+  /* "av/codec/context.pyx":272
  *     cpdef open(self, bint strict=True):
  * 
  *         if lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *             if strict:
  *                 raise ValueError('CodecContext is already open.')
  */
   __pyx_t_6 = (avcodec_is_open(__pyx_v_self->ptr) != 0);
   if (__pyx_t_6) {
 
-    /* "av/codec/context.pyx":270
+    /* "av/codec/context.pyx":273
  * 
  *         if lib.avcodec_is_open(self.ptr):
  *             if strict:             # <<<<<<<<<<<<<<
  *                 raise ValueError('CodecContext is already open.')
  *             return
  */
     __pyx_t_6 = (__pyx_v_strict != 0);
     if (unlikely(__pyx_t_6)) {
 
-      /* "av/codec/context.pyx":271
+      /* "av/codec/context.pyx":274
  *         if lib.avcodec_is_open(self.ptr):
  *             if strict:
  *                 raise ValueError('CodecContext is already open.')             # <<<<<<<<<<<<<<
  *             return
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 271, __pyx_L1_error)
+      __PYX_ERR(0, 274, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":270
+      /* "av/codec/context.pyx":273
  * 
  *         if lib.avcodec_is_open(self.ptr):
  *             if strict:             # <<<<<<<<<<<<<<
  *                 raise ValueError('CodecContext is already open.')
  *             return
  */
     }
 
-    /* "av/codec/context.pyx":272
+    /* "av/codec/context.pyx":275
  *             if strict:
  *                 raise ValueError('CodecContext is already open.')
  *             return             # <<<<<<<<<<<<<<
  * 
  *         # We might pass partial frames.
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":269
+    /* "av/codec/context.pyx":272
  *     cpdef open(self, bint strict=True):
  * 
  *         if lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *             if strict:
  *                 raise ValueError('CodecContext is already open.')
  */
   }
 
-  /* "av/codec/context.pyx":282
+  /* "av/codec/context.pyx":285
  * 
  *         # TODO: Do this better.
  *         cdef _Dictionary options = Dictionary()             # <<<<<<<<<<<<<<
  *         options.update(self.options or {})
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_2av_10dictionary__Dictionary))))) __PYX_ERR(0, 282, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_2av_10dictionary__Dictionary))))) __PYX_ERR(0, 285, __pyx_L1_error)
   __pyx_v_options = ((struct __pyx_obj_2av_10dictionary__Dictionary *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":283
+  /* "av/codec/context.pyx":286
  *         # TODO: Do this better.
  *         cdef _Dictionary options = Dictionary()
  *         options.update(self.options or {})             # <<<<<<<<<<<<<<
  * 
- *         # Assert we have a time_base.
+ *         # Assert we have a time_base for encoders.
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_options), __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_options), __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_self->options); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_self->options); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 286, __pyx_L1_error)
   if (!__pyx_t_6) {
   } else {
     __Pyx_INCREF(__pyx_v_self->options);
     __pyx_t_4 = __pyx_v_self->options;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_4 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L5_bool_binop_done:;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
@@ -4329,74 +4350,85 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":286
+  /* "av/codec/context.pyx":289
  * 
- *         # Assert we have a time_base.
- *         if not self.ptr.time_base.num:             # <<<<<<<<<<<<<<
+ *         # Assert we have a time_base for encoders.
+ *         if not self.ptr.time_base.num and self.is_encoder:             # <<<<<<<<<<<<<<
  *             self._set_default_time_base()
  * 
  */
-  __pyx_t_6 = ((!(__pyx_v_self->ptr->time_base.num != 0)) != 0);
+  __pyx_t_7 = ((!(__pyx_v_self->ptr->time_base.num != 0)) != 0);
+  if (__pyx_t_7) {
+  } else {
+    __pyx_t_6 = __pyx_t_7;
+    goto __pyx_L8_bool_binop_done;
+  }
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_encoder); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_t_7;
+  __pyx_L8_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "av/codec/context.pyx":287
- *         # Assert we have a time_base.
- *         if not self.ptr.time_base.num:
+    /* "av/codec/context.pyx":290
+ *         # Assert we have a time_base for encoders.
+ *         if not self.ptr.time_base.num and self.is_encoder:
  *             self._set_default_time_base()             # <<<<<<<<<<<<<<
  * 
  *         err_check(lib.avcodec_open2(self.ptr, self.codec.ptr, &options.ptr))
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_set_default_time_base(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_set_default_time_base(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "av/codec/context.pyx":286
+    /* "av/codec/context.pyx":289
  * 
- *         # Assert we have a time_base.
- *         if not self.ptr.time_base.num:             # <<<<<<<<<<<<<<
+ *         # Assert we have a time_base for encoders.
+ *         if not self.ptr.time_base.num and self.is_encoder:             # <<<<<<<<<<<<<<
  *             self._set_default_time_base()
  * 
  */
   }
 
-  /* "av/codec/context.pyx":289
+  /* "av/codec/context.pyx":292
  *             self._set_default_time_base()
  * 
  *         err_check(lib.avcodec_open2(self.ptr, self.codec.ptr, &options.ptr))             # <<<<<<<<<<<<<<
  * 
  *         self.options = dict(options)
  */
-  __pyx_t_7 = __pyx_f_2av_5error_err_check(avcodec_open2(__pyx_v_self->ptr, __pyx_v_self->codec->ptr, (&__pyx_v_options->ptr)), 0, NULL); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_8 = __pyx_f_2av_5error_err_check(avcodec_open2(__pyx_v_self->ptr, __pyx_v_self->codec->ptr, (&__pyx_v_options->ptr)), 0, NULL); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 292, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":291
+  /* "av/codec/context.pyx":294
  *         err_check(lib.avcodec_open2(self.ptr, self.codec.ptr, &options.ptr))
  * 
  *         self.options = dict(options)             # <<<<<<<<<<<<<<
  * 
  *     cdef _set_default_time_base(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), ((PyObject *)__pyx_v_options)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), ((PyObject *)__pyx_v_options)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->options);
   __Pyx_DECREF(__pyx_v_self->options);
   __pyx_v_self->options = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":267
+  /* "av/codec/context.pyx":270
  *             return lib.av_codec_is_decoder(self.ptr.codec)
  * 
  *     cpdef open(self, bint strict=True):             # <<<<<<<<<<<<<<
  * 
  *         if lib.avcodec_is_open(self.ptr):
  */
 
@@ -4446,33 +4478,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_strict);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 267, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 270, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_strict = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strict == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L3_error)
+      __pyx_v_strict = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strict == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 270, __pyx_L3_error)
     } else {
       __pyx_v_strict = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 267, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 270, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2av_5codec_7context_12CodecContext_12open(((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_v_self), __pyx_v_strict);
 
@@ -4489,15 +4521,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.strict = __pyx_v_strict;
-  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->open(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->open(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4506,61 +4538,61 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":293
+/* "av/codec/context.pyx":296
  *         self.options = dict(options)
  * 
  *     cdef _set_default_time_base(self):             # <<<<<<<<<<<<<<
  *         self.ptr.time_base.num = 1
  *         self.ptr.time_base.den = lib.AV_TIME_BASE
  */
 
 static PyObject *__pyx_f_2av_5codec_7context_12CodecContext__set_default_time_base(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_default_time_base", 0);
 
-  /* "av/codec/context.pyx":294
+  /* "av/codec/context.pyx":297
  * 
  *     cdef _set_default_time_base(self):
  *         self.ptr.time_base.num = 1             # <<<<<<<<<<<<<<
  *         self.ptr.time_base.den = lib.AV_TIME_BASE
  * 
  */
   __pyx_v_self->ptr->time_base.num = 1;
 
-  /* "av/codec/context.pyx":295
+  /* "av/codec/context.pyx":298
  *     cdef _set_default_time_base(self):
  *         self.ptr.time_base.num = 1
  *         self.ptr.time_base.den = lib.AV_TIME_BASE             # <<<<<<<<<<<<<<
  * 
  *     cpdef close(self, bint strict=True):
  */
   __pyx_v_self->ptr->time_base.den = AV_TIME_BASE;
 
-  /* "av/codec/context.pyx":293
+  /* "av/codec/context.pyx":296
  *         self.options = dict(options)
  * 
  *     cdef _set_default_time_base(self):             # <<<<<<<<<<<<<<
  *         self.ptr.time_base.num = 1
  *         self.ptr.time_base.den = lib.AV_TIME_BASE
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":297
+/* "av/codec/context.pyx":300
  *         self.ptr.time_base.den = lib.AV_TIME_BASE
  * 
  *     cpdef close(self, bint strict=True):             # <<<<<<<<<<<<<<
  *         if not lib.avcodec_is_open(self.ptr):
  *             if strict:
  */
 
@@ -4590,19 +4622,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2av_5codec_7context_12CodecContext_15close)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4610,15 +4642,15 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -4631,86 +4663,86 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "av/codec/context.pyx":298
+  /* "av/codec/context.pyx":301
  * 
  *     cpdef close(self, bint strict=True):
  *         if not lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *             if strict:
  *                 raise ValueError('CodecContext is already closed.')
  */
   __pyx_t_6 = ((!(avcodec_is_open(__pyx_v_self->ptr) != 0)) != 0);
   if (__pyx_t_6) {
 
-    /* "av/codec/context.pyx":299
+    /* "av/codec/context.pyx":302
  *     cpdef close(self, bint strict=True):
  *         if not lib.avcodec_is_open(self.ptr):
  *             if strict:             # <<<<<<<<<<<<<<
  *                 raise ValueError('CodecContext is already closed.')
  *             return
  */
     __pyx_t_6 = (__pyx_v_strict != 0);
     if (unlikely(__pyx_t_6)) {
 
-      /* "av/codec/context.pyx":300
+      /* "av/codec/context.pyx":303
  *         if not lib.avcodec_is_open(self.ptr):
  *             if strict:
  *                 raise ValueError('CodecContext is already closed.')             # <<<<<<<<<<<<<<
  *             return
  *         err_check(lib.avcodec_close(self.ptr))
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 300, __pyx_L1_error)
+      __PYX_ERR(0, 303, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":299
+      /* "av/codec/context.pyx":302
  *     cpdef close(self, bint strict=True):
  *         if not lib.avcodec_is_open(self.ptr):
  *             if strict:             # <<<<<<<<<<<<<<
  *                 raise ValueError('CodecContext is already closed.')
  *             return
  */
     }
 
-    /* "av/codec/context.pyx":301
+    /* "av/codec/context.pyx":304
  *             if strict:
  *                 raise ValueError('CodecContext is already closed.')
  *             return             # <<<<<<<<<<<<<<
  *         err_check(lib.avcodec_close(self.ptr))
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":298
+    /* "av/codec/context.pyx":301
  * 
  *     cpdef close(self, bint strict=True):
  *         if not lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *             if strict:
  *                 raise ValueError('CodecContext is already closed.')
  */
   }
 
-  /* "av/codec/context.pyx":302
+  /* "av/codec/context.pyx":305
  *                 raise ValueError('CodecContext is already closed.')
  *             return
  *         err_check(lib.avcodec_close(self.ptr))             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __pyx_t_7 = __pyx_f_2av_5error_err_check(avcodec_close(__pyx_v_self->ptr), 0, NULL); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_2av_5error_err_check(avcodec_close(__pyx_v_self->ptr), 0, NULL); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 305, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":297
+  /* "av/codec/context.pyx":300
  *         self.ptr.time_base.den = lib.AV_TIME_BASE
  * 
  *     cpdef close(self, bint strict=True):             # <<<<<<<<<<<<<<
  *         if not lib.avcodec_is_open(self.ptr):
  *             if strict:
  */
 
@@ -4759,33 +4791,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_strict);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "close") < 0)) __PYX_ERR(0, 297, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "close") < 0)) __PYX_ERR(0, 300, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_strict = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strict == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L3_error)
+      __pyx_v_strict = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strict == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 300, __pyx_L3_error)
     } else {
       __pyx_v_strict = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("close", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 297, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("close", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 300, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2av_5codec_7context_12CodecContext_14close(((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_v_self), __pyx_v_strict);
 
@@ -4802,15 +4834,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.strict = __pyx_v_strict;
-  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->close(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->close(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4819,15 +4851,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":304
+/* "av/codec/context.pyx":307
  *         err_check(lib.avcodec_close(self.ptr))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.ptr and self.extradata_set:
  *             lib.av_freep(&self.ptr.extradata)
  */
 
@@ -4844,15 +4876,15 @@
 
 static void __pyx_pf_2av_5codec_7context_12CodecContext_16__dealloc__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "av/codec/context.pyx":305
+  /* "av/codec/context.pyx":308
  * 
  *     def __dealloc__(self):
  *         if self.ptr and self.extradata_set:             # <<<<<<<<<<<<<<
  *             lib.av_freep(&self.ptr.extradata)
  *         if self.ptr and self.allocated:
  */
   __pyx_t_2 = (__pyx_v_self->ptr != 0);
@@ -4862,33 +4894,33 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->extradata_set != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":306
+    /* "av/codec/context.pyx":309
  *     def __dealloc__(self):
  *         if self.ptr and self.extradata_set:
  *             lib.av_freep(&self.ptr.extradata)             # <<<<<<<<<<<<<<
  *         if self.ptr and self.allocated:
  *             lib.avcodec_close(self.ptr)
  */
     av_freep((&__pyx_v_self->ptr->extradata));
 
-    /* "av/codec/context.pyx":305
+    /* "av/codec/context.pyx":308
  * 
  *     def __dealloc__(self):
  *         if self.ptr and self.extradata_set:             # <<<<<<<<<<<<<<
  *             lib.av_freep(&self.ptr.extradata)
  *         if self.ptr and self.allocated:
  */
   }
 
-  /* "av/codec/context.pyx":307
+  /* "av/codec/context.pyx":310
  *         if self.ptr and self.extradata_set:
  *             lib.av_freep(&self.ptr.extradata)
  *         if self.ptr and self.allocated:             # <<<<<<<<<<<<<<
  *             lib.avcodec_close(self.ptr)
  *             lib.avcodec_free_context(&self.ptr)
  */
   __pyx_t_2 = (__pyx_v_self->ptr != 0);
@@ -4898,82 +4930,82 @@
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->allocated != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":308
+    /* "av/codec/context.pyx":311
  *             lib.av_freep(&self.ptr.extradata)
  *         if self.ptr and self.allocated:
  *             lib.avcodec_close(self.ptr)             # <<<<<<<<<<<<<<
  *             lib.avcodec_free_context(&self.ptr)
  *         if self.parser:
  */
     (void)(avcodec_close(__pyx_v_self->ptr));
 
-    /* "av/codec/context.pyx":309
+    /* "av/codec/context.pyx":312
  *         if self.ptr and self.allocated:
  *             lib.avcodec_close(self.ptr)
  *             lib.avcodec_free_context(&self.ptr)             # <<<<<<<<<<<<<<
  *         if self.parser:
  *             lib.av_parser_close(self.parser)
  */
     avcodec_free_context((&__pyx_v_self->ptr));
 
-    /* "av/codec/context.pyx":307
+    /* "av/codec/context.pyx":310
  *         if self.ptr and self.extradata_set:
  *             lib.av_freep(&self.ptr.extradata)
  *         if self.ptr and self.allocated:             # <<<<<<<<<<<<<<
  *             lib.avcodec_close(self.ptr)
  *             lib.avcodec_free_context(&self.ptr)
  */
   }
 
-  /* "av/codec/context.pyx":310
+  /* "av/codec/context.pyx":313
  *             lib.avcodec_close(self.ptr)
  *             lib.avcodec_free_context(&self.ptr)
  *         if self.parser:             # <<<<<<<<<<<<<<
  *             lib.av_parser_close(self.parser)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->parser != 0);
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":311
+    /* "av/codec/context.pyx":314
  *             lib.avcodec_free_context(&self.ptr)
  *         if self.parser:
  *             lib.av_parser_close(self.parser)             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
     av_parser_close(__pyx_v_self->parser);
 
-    /* "av/codec/context.pyx":310
+    /* "av/codec/context.pyx":313
  *             lib.avcodec_close(self.ptr)
  *             lib.avcodec_free_context(&self.ptr)
  *         if self.parser:             # <<<<<<<<<<<<<<
  *             lib.av_parser_close(self.parser)
  * 
  */
   }
 
-  /* "av/codec/context.pyx":304
+  /* "av/codec/context.pyx":307
  *         err_check(lib.avcodec_close(self.ptr))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.ptr and self.extradata_set:
  *             lib.av_freep(&self.ptr.extradata)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "av/codec/context.pyx":313
+/* "av/codec/context.pyx":316
  *             lib.av_parser_close(self.parser)
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return '<av.%s %s/%s at 0x%x>' % (
  *             self.__class__.__name__,
  */
 
@@ -5000,127 +5032,127 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "av/codec/context.pyx":314
+  /* "av/codec/context.pyx":317
  * 
  *     def __repr__(self):
  *         return '<av.%s %s/%s at 0x%x>' % (             # <<<<<<<<<<<<<<
  *             self.__class__.__name__,
  *             self.type or '<notype>',
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "av/codec/context.pyx":315
+  /* "av/codec/context.pyx":318
  *     def __repr__(self):
  *         return '<av.%s %s/%s at 0x%x>' % (
  *             self.__class__.__name__,             # <<<<<<<<<<<<<<
  *             self.type or '<notype>',
  *             self.name or '<nocodec>',
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":316
+  /* "av/codec/context.pyx":319
  *         return '<av.%s %s/%s at 0x%x>' % (
  *             self.__class__.__name__,
  *             self.type or '<notype>',             # <<<<<<<<<<<<<<
  *             self.name or '<nocodec>',
  *             id(self),
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 319, __pyx_L1_error)
   if (!__pyx_t_4) {
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L3_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_kp_s_notype);
   __pyx_t_1 = __pyx_kp_s_notype;
   __pyx_L3_bool_binop_done:;
 
-  /* "av/codec/context.pyx":317
+  /* "av/codec/context.pyx":320
  *             self.__class__.__name__,
  *             self.type or '<notype>',
  *             self.name or '<nocodec>',             # <<<<<<<<<<<<<<
  *             id(self),
  *         )
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 320, __pyx_L1_error)
   if (!__pyx_t_4) {
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_5);
     __pyx_t_3 = __pyx_t_5;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L5_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_kp_s_nocodec);
   __pyx_t_3 = __pyx_kp_s_nocodec;
   __pyx_L5_bool_binop_done:;
 
-  /* "av/codec/context.pyx":318
+  /* "av/codec/context.pyx":321
  *             self.type or '<notype>',
  *             self.name or '<nocodec>',
  *             id(self),             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "av/codec/context.pyx":315
+  /* "av/codec/context.pyx":318
  *     def __repr__(self):
  *         return '<av.%s %s/%s at 0x%x>' % (
  *             self.__class__.__name__,             # <<<<<<<<<<<<<<
  *             self.type or '<notype>',
  *             self.name or '<nocodec>',
  */
-  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_5);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
 
-  /* "av/codec/context.pyx":314
+  /* "av/codec/context.pyx":317
  * 
  *     def __repr__(self):
  *         return '<av.%s %s/%s at 0x%x>' % (             # <<<<<<<<<<<<<<
  *             self.__class__.__name__,
  *             self.type or '<notype>',
  */
-  __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_av_s_s_s_at_0x_x, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_av_s_s_s_at_0x_x, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":313
+  /* "av/codec/context.pyx":316
  *             lib.av_parser_close(self.parser)
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return '<av.%s %s/%s at 0x%x>' % (
  *             self.__class__.__name__,
  */
 
@@ -5135,15 +5167,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":321
+/* "av/codec/context.pyx":324
  *         )
  * 
  *     def parse(self, raw_input=None):             # <<<<<<<<<<<<<<
  *         """Split up a byte stream into list of :class:`.Packet`.
  * 
  */
 
@@ -5176,29 +5208,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_raw_input);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse") < 0)) __PYX_ERR(0, 321, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse") < 0)) __PYX_ERR(0, 324, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_raw_input = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("parse", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 321, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("parse", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 324, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.parse", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2av_5codec_7context_12CodecContext_20parse(((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_v_self), __pyx_v_raw_input);
 
@@ -5227,181 +5259,181 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 0);
 
-  /* "av/codec/context.pyx":338
+  /* "av/codec/context.pyx":341
  *         """
  * 
  *         if not self.parser:             # <<<<<<<<<<<<<<
  *             self.parser = lib.av_parser_init(self.codec.ptr.id)
  *             if not self.parser:
  */
   __pyx_t_1 = ((!(__pyx_v_self->parser != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":339
+    /* "av/codec/context.pyx":342
  * 
  *         if not self.parser:
  *             self.parser = lib.av_parser_init(self.codec.ptr.id)             # <<<<<<<<<<<<<<
  *             if not self.parser:
  *                 raise ValueError('No parser for %s' % self.codec.name)
  */
     __pyx_v_self->parser = av_parser_init(__pyx_v_self->codec->ptr->id);
 
-    /* "av/codec/context.pyx":340
+    /* "av/codec/context.pyx":343
  *         if not self.parser:
  *             self.parser = lib.av_parser_init(self.codec.ptr.id)
  *             if not self.parser:             # <<<<<<<<<<<<<<
  *                 raise ValueError('No parser for %s' % self.codec.name)
  * 
  */
     __pyx_t_1 = ((!(__pyx_v_self->parser != 0)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "av/codec/context.pyx":341
+      /* "av/codec/context.pyx":344
  *             self.parser = lib.av_parser_init(self.codec.ptr.id)
  *             if not self.parser:
  *                 raise ValueError('No parser for %s' % self.codec.name)             # <<<<<<<<<<<<<<
  * 
  *         cdef ByteSource source = bytesource(raw_input, allow_none=True)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->codec), __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->codec), __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_No_parser_for_s, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_No_parser_for_s, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 344, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 341, __pyx_L1_error)
+      __PYX_ERR(0, 344, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":340
+      /* "av/codec/context.pyx":343
  *         if not self.parser:
  *             self.parser = lib.av_parser_init(self.codec.ptr.id)
  *             if not self.parser:             # <<<<<<<<<<<<<<
  *                 raise ValueError('No parser for %s' % self.codec.name)
  * 
  */
     }
 
-    /* "av/codec/context.pyx":338
+    /* "av/codec/context.pyx":341
  *         """
  * 
  *         if not self.parser:             # <<<<<<<<<<<<<<
  *             self.parser = lib.av_parser_init(self.codec.ptr.id)
  *             if not self.parser:
  */
   }
 
-  /* "av/codec/context.pyx":343
+  /* "av/codec/context.pyx":346
  *                 raise ValueError('No parser for %s' % self.codec.name)
  * 
  *         cdef ByteSource source = bytesource(raw_input, allow_none=True)             # <<<<<<<<<<<<<<
  * 
  *         cdef unsigned char *in_data = source.ptr if source is not None else NULL
  */
   __pyx_t_4.__pyx_n = 1;
   __pyx_t_4.allow_none = 1;
-  __pyx_t_2 = ((PyObject *)__pyx_f_2av_10bytesource_bytesource(__pyx_v_raw_input, &__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_2av_10bytesource_bytesource(__pyx_v_raw_input, &__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_source = ((struct __pyx_obj_2av_10bytesource_ByteSource *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":345
+  /* "av/codec/context.pyx":348
  *         cdef ByteSource source = bytesource(raw_input, allow_none=True)
  * 
  *         cdef unsigned char *in_data = source.ptr if source is not None else NULL             # <<<<<<<<<<<<<<
  *         cdef int in_size = source.length if source is not None else 0
  * 
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_source) != Py_None);
   if ((__pyx_t_1 != 0)) {
     __pyx_t_5 = __pyx_v_source->ptr;
   } else {
     __pyx_t_5 = NULL;
   }
   __pyx_v_in_data = __pyx_t_5;
 
-  /* "av/codec/context.pyx":346
+  /* "av/codec/context.pyx":349
  * 
  *         cdef unsigned char *in_data = source.ptr if source is not None else NULL
  *         cdef int in_size = source.length if source is not None else 0             # <<<<<<<<<<<<<<
  * 
  *         cdef unsigned char *out_data
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_source) != Py_None);
   if ((__pyx_t_1 != 0)) {
     __pyx_t_6 = __pyx_v_source->length;
   } else {
     __pyx_t_6 = 0;
   }
   __pyx_v_in_size = __pyx_t_6;
 
-  /* "av/codec/context.pyx":351
+  /* "av/codec/context.pyx":354
  *         cdef int out_size
  *         cdef int consumed
  *         cdef Packet packet = None             # <<<<<<<<<<<<<<
  * 
  *         packets = []
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_packet = ((struct __pyx_obj_2av_6packet_Packet *)Py_None);
 
-  /* "av/codec/context.pyx":353
+  /* "av/codec/context.pyx":356
  *         cdef Packet packet = None
  * 
  *         packets = []             # <<<<<<<<<<<<<<
  * 
  *         while True:
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_packets = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":355
+  /* "av/codec/context.pyx":358
  *         packets = []
  * 
  *         while True:             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
   while (1) {
 
-    /* "av/codec/context.pyx":357
+    /* "av/codec/context.pyx":360
  *         while True:
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 consumed = lib.av_parser_parse2(
  *                     self.parser,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "av/codec/context.pyx":358
+          /* "av/codec/context.pyx":361
  * 
  *             with nogil:
  *                 consumed = lib.av_parser_parse2(             # <<<<<<<<<<<<<<
  *                     self.parser,
  *                     self.ptr,
  */
           __pyx_v_consumed = av_parser_parse2(__pyx_v_self->parser, __pyx_v_self->ptr, (&__pyx_v_out_data), (&__pyx_v_out_size), __pyx_v_in_data, __pyx_v_in_size, AV_NOPTS_VALUE, AV_NOPTS_VALUE, 0);
         }
 
-        /* "av/codec/context.pyx":357
+        /* "av/codec/context.pyx":360
  *         while True:
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 consumed = lib.av_parser_parse2(
  *                     self.parser,
  */
         /*finally:*/ {
@@ -5412,164 +5444,164 @@
             #endif
             goto __pyx_L11;
           }
           __pyx_L11:;
         }
     }
 
-    /* "av/codec/context.pyx":366
+    /* "av/codec/context.pyx":369
  *                     0
  *                 )
  *             err_check(consumed)             # <<<<<<<<<<<<<<
  * 
  *             if out_size:
  */
-    __pyx_t_7 = __pyx_f_2av_5error_err_check(__pyx_v_consumed, 0, NULL); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 366, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_2av_5error_err_check(__pyx_v_consumed, 0, NULL); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 369, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":368
+    /* "av/codec/context.pyx":371
  *             err_check(consumed)
  * 
  *             if out_size:             # <<<<<<<<<<<<<<
  * 
  *                 # We copy the data immediately, as we have yet to figure out
  */
     __pyx_t_1 = (__pyx_v_out_size != 0);
     if (__pyx_t_1) {
 
-      /* "av/codec/context.pyx":382
+      /* "av/codec/context.pyx":385
  *                 # ... but this results in corruption.
  * 
  *                 packet = Packet(out_size)             # <<<<<<<<<<<<<<
  *                 memcpy(packet.ptr.data, out_data, out_size)
  * 
  */
-      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_out_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_out_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 385, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_6packet_Packet), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_6packet_Packet), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 385, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF_SET(__pyx_v_packet, ((struct __pyx_obj_2av_6packet_Packet *)__pyx_t_3));
       __pyx_t_3 = 0;
 
-      /* "av/codec/context.pyx":383
+      /* "av/codec/context.pyx":386
  * 
  *                 packet = Packet(out_size)
  *                 memcpy(packet.ptr.data, out_data, out_size)             # <<<<<<<<<<<<<<
  * 
  *                 packets.append(packet)
  */
       (void)(memcpy(__pyx_v_packet->ptr->data, __pyx_v_out_data, __pyx_v_out_size));
 
-      /* "av/codec/context.pyx":385
+      /* "av/codec/context.pyx":388
  *                 memcpy(packet.ptr.data, out_data, out_size)
  * 
  *                 packets.append(packet)             # <<<<<<<<<<<<<<
  * 
  *             if not in_size:
  */
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_packets, ((PyObject *)__pyx_v_packet)); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 385, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_packets, ((PyObject *)__pyx_v_packet)); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 388, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":368
+      /* "av/codec/context.pyx":371
  *             err_check(consumed)
  * 
  *             if out_size:             # <<<<<<<<<<<<<<
  * 
  *                 # We copy the data immediately, as we have yet to figure out
  */
     }
 
-    /* "av/codec/context.pyx":387
+    /* "av/codec/context.pyx":390
  *                 packets.append(packet)
  * 
  *             if not in_size:             # <<<<<<<<<<<<<<
  *                 # This was a flush. Only one packet should ever be returned.
  *                 break
  */
     __pyx_t_1 = ((!(__pyx_v_in_size != 0)) != 0);
     if (__pyx_t_1) {
 
-      /* "av/codec/context.pyx":389
+      /* "av/codec/context.pyx":392
  *             if not in_size:
  *                 # This was a flush. Only one packet should ever be returned.
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             in_data += consumed
  */
       goto __pyx_L6_break;
 
-      /* "av/codec/context.pyx":387
+      /* "av/codec/context.pyx":390
  *                 packets.append(packet)
  * 
  *             if not in_size:             # <<<<<<<<<<<<<<
  *                 # This was a flush. Only one packet should ever be returned.
  *                 break
  */
     }
 
-    /* "av/codec/context.pyx":391
+    /* "av/codec/context.pyx":394
  *                 break
  * 
  *             in_data += consumed             # <<<<<<<<<<<<<<
  *             in_size -= consumed
  * 
  */
     __pyx_v_in_data = (__pyx_v_in_data + __pyx_v_consumed);
 
-    /* "av/codec/context.pyx":392
+    /* "av/codec/context.pyx":395
  * 
  *             in_data += consumed
  *             in_size -= consumed             # <<<<<<<<<<<<<<
  * 
  *             if not in_size:
  */
     __pyx_v_in_size = (__pyx_v_in_size - __pyx_v_consumed);
 
-    /* "av/codec/context.pyx":394
+    /* "av/codec/context.pyx":397
  *             in_size -= consumed
  * 
  *             if not in_size:             # <<<<<<<<<<<<<<
  *                 # Aaaand now we're done.
  *                 break
  */
     __pyx_t_1 = ((!(__pyx_v_in_size != 0)) != 0);
     if (__pyx_t_1) {
 
-      /* "av/codec/context.pyx":396
+      /* "av/codec/context.pyx":399
  *             if not in_size:
  *                 # Aaaand now we're done.
  *                 break             # <<<<<<<<<<<<<<
  * 
  *         return packets
  */
       goto __pyx_L6_break;
 
-      /* "av/codec/context.pyx":394
+      /* "av/codec/context.pyx":397
  *             in_size -= consumed
  * 
  *             if not in_size:             # <<<<<<<<<<<<<<
  *                 # Aaaand now we're done.
  *                 break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "av/codec/context.pyx":398
+  /* "av/codec/context.pyx":401
  *                 break
  * 
  *         return packets             # <<<<<<<<<<<<<<
  * 
  *     cdef _send_frame_and_recv(self, Frame frame):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_packets);
   __pyx_r = __pyx_v_packets;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":321
+  /* "av/codec/context.pyx":324
  *         )
  * 
  *     def parse(self, raw_input=None):             # <<<<<<<<<<<<<<
  *         """Split up a byte stream into list of :class:`.Packet`.
  * 
  */
 
@@ -5584,15 +5616,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_packet);
   __Pyx_XDECREF(__pyx_v_packets);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":400
+/* "av/codec/context.pyx":403
  *         return packets
  * 
  *     cdef _send_frame_and_recv(self, Frame frame):             # <<<<<<<<<<<<<<
  * 
  *         cdef Packet packet
  */
 
@@ -5608,30 +5640,30 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_send_frame_and_recv", 0);
 
-  /* "av/codec/context.pyx":405
+  /* "av/codec/context.pyx":408
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_send_frame(self.ptr, frame.ptr if frame is not None else NULL)
  *         err_check(res)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/codec/context.pyx":406
+        /* "av/codec/context.pyx":409
  *         cdef int res
  *         with nogil:
  *             res = lib.avcodec_send_frame(self.ptr, frame.ptr if frame is not None else NULL)             # <<<<<<<<<<<<<<
  *         err_check(res)
  * 
  */
         __pyx_t_2 = (((PyObject *)__pyx_v_frame) != Py_None);
@@ -5639,15 +5671,15 @@
           __pyx_t_1 = __pyx_v_frame->ptr;
         } else {
           __pyx_t_1 = NULL;
         }
         __pyx_v_res = avcodec_send_frame(__pyx_v_self->ptr, __pyx_t_1);
       }
 
-      /* "av/codec/context.pyx":405
+      /* "av/codec/context.pyx":408
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_send_frame(self.ptr, frame.ptr if frame is not None else NULL)
  *         err_check(res)
  */
       /*finally:*/ {
@@ -5658,113 +5690,113 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "av/codec/context.pyx":407
+  /* "av/codec/context.pyx":410
  *         with nogil:
  *             res = lib.avcodec_send_frame(self.ptr, frame.ptr if frame is not None else NULL)
  *         err_check(res)             # <<<<<<<<<<<<<<
  * 
  *         out = []
  */
-  __pyx_t_3 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 410, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":409
+  /* "av/codec/context.pyx":412
  *         err_check(res)
  * 
  *         out = []             # <<<<<<<<<<<<<<
  *         while True:
  *             packet = self._recv_packet()
  */
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_out = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "av/codec/context.pyx":410
+  /* "av/codec/context.pyx":413
  * 
  *         out = []
  *         while True:             # <<<<<<<<<<<<<<
  *             packet = self._recv_packet()
  *             if packet:
  */
   while (1) {
 
-    /* "av/codec/context.pyx":411
+    /* "av/codec/context.pyx":414
  *         out = []
  *         while True:
  *             packet = self._recv_packet()             # <<<<<<<<<<<<<<
  *             if packet:
  *                 out.append(packet)
  */
-    __pyx_t_4 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_recv_packet(__pyx_v_self); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_recv_packet(__pyx_v_self); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_2av_6packet_Packet))))) __PYX_ERR(0, 411, __pyx_L1_error)
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_2av_6packet_Packet))))) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_packet, ((struct __pyx_obj_2av_6packet_Packet *)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "av/codec/context.pyx":412
+    /* "av/codec/context.pyx":415
  *         while True:
  *             packet = self._recv_packet()
  *             if packet:             # <<<<<<<<<<<<<<
  *                 out.append(packet)
  *             else:
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_packet)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_packet)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 415, __pyx_L1_error)
     if (__pyx_t_2) {
 
-      /* "av/codec/context.pyx":413
+      /* "av/codec/context.pyx":416
  *             packet = self._recv_packet()
  *             if packet:
  *                 out.append(packet)             # <<<<<<<<<<<<<<
  *             else:
  *                 break
  */
-      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_out, ((PyObject *)__pyx_v_packet)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_out, ((PyObject *)__pyx_v_packet)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 416, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":412
+      /* "av/codec/context.pyx":415
  *         while True:
  *             packet = self._recv_packet()
  *             if packet:             # <<<<<<<<<<<<<<
  *                 out.append(packet)
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "av/codec/context.pyx":415
+    /* "av/codec/context.pyx":418
  *                 out.append(packet)
  *             else:
  *                 break             # <<<<<<<<<<<<<<
  *         return out
  * 
  */
     /*else*/ {
       goto __pyx_L7_break;
     }
     __pyx_L8:;
   }
   __pyx_L7_break:;
 
-  /* "av/codec/context.pyx":416
+  /* "av/codec/context.pyx":419
  *             else:
  *                 break
  *         return out             # <<<<<<<<<<<<<<
  * 
  *     cdef _send_packet_and_recv(self, Packet packet):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_out);
   __pyx_r = __pyx_v_out;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":400
+  /* "av/codec/context.pyx":403
  *         return packets
  * 
  *     cdef _send_frame_and_recv(self, Frame frame):             # <<<<<<<<<<<<<<
  * 
  *         cdef Packet packet
  */
 
@@ -5777,15 +5809,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_packet);
   __Pyx_XDECREF(__pyx_v_out);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":418
+/* "av/codec/context.pyx":421
  *         return out
  * 
  *     cdef _send_packet_and_recv(self, Packet packet):             # <<<<<<<<<<<<<<
  * 
  *         cdef Frame frame
  */
 
@@ -5801,30 +5833,30 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_send_packet_and_recv", 0);
 
-  /* "av/codec/context.pyx":423
+  /* "av/codec/context.pyx":426
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_send_packet(self.ptr, packet.ptr if packet is not None else NULL)
  *         err_check(res)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/codec/context.pyx":424
+        /* "av/codec/context.pyx":427
  *         cdef int res
  *         with nogil:
  *             res = lib.avcodec_send_packet(self.ptr, packet.ptr if packet is not None else NULL)             # <<<<<<<<<<<<<<
  *         err_check(res)
  * 
  */
         __pyx_t_2 = (((PyObject *)__pyx_v_packet) != Py_None);
@@ -5832,15 +5864,15 @@
           __pyx_t_1 = __pyx_v_packet->ptr;
         } else {
           __pyx_t_1 = NULL;
         }
         __pyx_v_res = avcodec_send_packet(__pyx_v_self->ptr, __pyx_t_1);
       }
 
-      /* "av/codec/context.pyx":423
+      /* "av/codec/context.pyx":426
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_send_packet(self.ptr, packet.ptr if packet is not None else NULL)
  *         err_check(res)
  */
       /*finally:*/ {
@@ -5851,113 +5883,113 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "av/codec/context.pyx":425
+  /* "av/codec/context.pyx":428
  *         with nogil:
  *             res = lib.avcodec_send_packet(self.ptr, packet.ptr if packet is not None else NULL)
  *         err_check(res)             # <<<<<<<<<<<<<<
  * 
  *         out = []
  */
-  __pyx_t_3 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":427
+  /* "av/codec/context.pyx":430
  *         err_check(res)
  * 
  *         out = []             # <<<<<<<<<<<<<<
  *         while True:
  *             frame = self._recv_frame()
  */
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_out = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "av/codec/context.pyx":428
+  /* "av/codec/context.pyx":431
  * 
  *         out = []
  *         while True:             # <<<<<<<<<<<<<<
  *             frame = self._recv_frame()
  *             if frame:
  */
   while (1) {
 
-    /* "av/codec/context.pyx":429
+    /* "av/codec/context.pyx":432
  *         out = []
  *         while True:
  *             frame = self._recv_frame()             # <<<<<<<<<<<<<<
  *             if frame:
  *                 out.append(frame)
  */
-    __pyx_t_4 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_recv_frame(__pyx_v_self); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_recv_frame(__pyx_v_self); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 429, __pyx_L1_error)
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_frame, ((struct __pyx_obj_2av_5frame_Frame *)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "av/codec/context.pyx":430
+    /* "av/codec/context.pyx":433
  *         while True:
  *             frame = self._recv_frame()
  *             if frame:             # <<<<<<<<<<<<<<
  *                 out.append(frame)
  *             else:
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_frame)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 430, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_frame)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 433, __pyx_L1_error)
     if (__pyx_t_2) {
 
-      /* "av/codec/context.pyx":431
+      /* "av/codec/context.pyx":434
  *             frame = self._recv_frame()
  *             if frame:
  *                 out.append(frame)             # <<<<<<<<<<<<<<
  *             else:
  *                 break
  */
-      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_out, ((PyObject *)__pyx_v_frame)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_out, ((PyObject *)__pyx_v_frame)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 434, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":430
+      /* "av/codec/context.pyx":433
  *         while True:
  *             frame = self._recv_frame()
  *             if frame:             # <<<<<<<<<<<<<<
  *                 out.append(frame)
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "av/codec/context.pyx":433
+    /* "av/codec/context.pyx":436
  *                 out.append(frame)
  *             else:
  *                 break             # <<<<<<<<<<<<<<
  *         return out
  * 
  */
     /*else*/ {
       goto __pyx_L7_break;
     }
     __pyx_L8:;
   }
   __pyx_L7_break:;
 
-  /* "av/codec/context.pyx":434
+  /* "av/codec/context.pyx":437
  *             else:
  *                 break
  *         return out             # <<<<<<<<<<<<<<
  * 
  *     cdef _prepare_frames_for_encode(self, Frame frame):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_out);
   __pyx_r = __pyx_v_out;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":418
+  /* "av/codec/context.pyx":421
  *         return out
  * 
  *     cdef _send_packet_and_recv(self, Packet packet):             # <<<<<<<<<<<<<<
  * 
  *         cdef Frame frame
  */
 
@@ -5970,15 +6002,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_frame);
   __Pyx_XDECREF(__pyx_v_out);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":436
+/* "av/codec/context.pyx":439
  *         return out
  * 
  *     cdef _prepare_frames_for_encode(self, Frame frame):             # <<<<<<<<<<<<<<
  *         return [frame]
  * 
  */
 
@@ -5987,32 +6019,32 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_prepare_frames_for_encode", 0);
 
-  /* "av/codec/context.pyx":437
+  /* "av/codec/context.pyx":440
  * 
  *     cdef _prepare_frames_for_encode(self, Frame frame):
  *         return [frame]             # <<<<<<<<<<<<<<
  * 
  *     cdef Frame _alloc_next_frame(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_v_frame));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
   PyList_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_frame));
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":436
+  /* "av/codec/context.pyx":439
  *         return out
  * 
  *     cdef _prepare_frames_for_encode(self, Frame frame):             # <<<<<<<<<<<<<<
  *         return [frame]
  * 
  */
 
@@ -6023,15 +6055,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":439
+/* "av/codec/context.pyx":442
  *         return [frame]
  * 
  *     cdef Frame _alloc_next_frame(self):             # <<<<<<<<<<<<<<
  *         raise NotImplementedError('Base CodecContext cannot decode.')
  * 
  */
 
@@ -6040,28 +6072,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_alloc_next_frame", 0);
 
-  /* "av/codec/context.pyx":440
+  /* "av/codec/context.pyx":443
  * 
  *     cdef Frame _alloc_next_frame(self):
  *         raise NotImplementedError('Base CodecContext cannot decode.')             # <<<<<<<<<<<<<<
  * 
  *     cdef _recv_frame(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 440, __pyx_L1_error)
+  __PYX_ERR(0, 443, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":439
+  /* "av/codec/context.pyx":442
  *         return [frame]
  * 
  *     cdef Frame _alloc_next_frame(self):             # <<<<<<<<<<<<<<
  *         raise NotImplementedError('Base CodecContext cannot decode.')
  * 
  */
 
@@ -6071,15 +6103,15 @@
   __Pyx_AddTraceback("av.codec.context.CodecContext._alloc_next_frame", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":442
+/* "av/codec/context.pyx":445
  *         raise NotImplementedError('Base CodecContext cannot decode.')
  * 
  *     cdef _recv_frame(self):             # <<<<<<<<<<<<<<
  * 
  *         if not self._next_frame:
  */
 
@@ -6093,87 +6125,87 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_recv_frame", 0);
 
-  /* "av/codec/context.pyx":444
+  /* "av/codec/context.pyx":447
  *     cdef _recv_frame(self):
  * 
  *         if not self._next_frame:             # <<<<<<<<<<<<<<
  *             self._next_frame = self._alloc_next_frame()
  *         cdef Frame frame = self._next_frame
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->_next_frame)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->_next_frame)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 447, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "av/codec/context.pyx":445
+    /* "av/codec/context.pyx":448
  * 
  *         if not self._next_frame:
  *             self._next_frame = self._alloc_next_frame()             # <<<<<<<<<<<<<<
  *         cdef Frame frame = self._next_frame
  * 
  */
-    __pyx_t_3 = ((PyObject *)((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_alloc_next_frame(__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_alloc_next_frame(__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->_next_frame);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->_next_frame));
     __pyx_v_self->_next_frame = ((struct __pyx_obj_2av_5frame_Frame *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "av/codec/context.pyx":444
+    /* "av/codec/context.pyx":447
  *     cdef _recv_frame(self):
  * 
  *         if not self._next_frame:             # <<<<<<<<<<<<<<
  *             self._next_frame = self._alloc_next_frame()
  *         cdef Frame frame = self._next_frame
  */
   }
 
-  /* "av/codec/context.pyx":446
+  /* "av/codec/context.pyx":449
  *         if not self._next_frame:
  *             self._next_frame = self._alloc_next_frame()
  *         cdef Frame frame = self._next_frame             # <<<<<<<<<<<<<<
  * 
  *         cdef int res
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_self->_next_frame);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_frame = ((struct __pyx_obj_2av_5frame_Frame *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "av/codec/context.pyx":449
+  /* "av/codec/context.pyx":452
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_receive_frame(self.ptr, frame.ptr)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/codec/context.pyx":450
+        /* "av/codec/context.pyx":453
  *         cdef int res
  *         with nogil:
  *             res = lib.avcodec_receive_frame(self.ptr, frame.ptr)             # <<<<<<<<<<<<<<
  * 
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  */
         __pyx_v_res = avcodec_receive_frame(__pyx_v_self->ptr, __pyx_v_frame->ptr);
       }
 
-      /* "av/codec/context.pyx":449
+      /* "av/codec/context.pyx":452
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_receive_frame(self.ptr, frame.ptr)
  * 
  */
       /*finally:*/ {
@@ -6184,15 +6216,15 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "av/codec/context.pyx":452
+  /* "av/codec/context.pyx":455
  *             res = lib.avcodec_receive_frame(self.ptr, frame.ptr)
  * 
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:             # <<<<<<<<<<<<<<
  *             return
  *         err_check(res)
  */
   __pyx_t_1 = ((__pyx_v_res == (-EAGAIN)) != 0);
@@ -6202,88 +6234,88 @@
     goto __pyx_L8_bool_binop_done;
   }
   __pyx_t_1 = ((__pyx_v_res == AVERROR_EOF) != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L8_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "av/codec/context.pyx":453
+    /* "av/codec/context.pyx":456
  * 
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  *             return             # <<<<<<<<<<<<<<
  *         err_check(res)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":452
+    /* "av/codec/context.pyx":455
  *             res = lib.avcodec_receive_frame(self.ptr, frame.ptr)
  * 
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:             # <<<<<<<<<<<<<<
  *             return
  *         err_check(res)
  */
   }
 
-  /* "av/codec/context.pyx":454
+  /* "av/codec/context.pyx":457
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  *             return
  *         err_check(res)             # <<<<<<<<<<<<<<
  * 
  *         if not res:
  */
-  __pyx_t_4 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 457, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":456
+  /* "av/codec/context.pyx":459
  *         err_check(res)
  * 
  *         if not res:             # <<<<<<<<<<<<<<
  *             self._next_frame = None
  *             return frame
  */
   __pyx_t_2 = ((!(__pyx_v_res != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "av/codec/context.pyx":457
+    /* "av/codec/context.pyx":460
  * 
  *         if not res:
  *             self._next_frame = None             # <<<<<<<<<<<<<<
  *             return frame
  * 
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_next_frame);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->_next_frame));
     __pyx_v_self->_next_frame = ((struct __pyx_obj_2av_5frame_Frame *)Py_None);
 
-    /* "av/codec/context.pyx":458
+    /* "av/codec/context.pyx":461
  *         if not res:
  *             self._next_frame = None
  *             return frame             # <<<<<<<<<<<<<<
  * 
  *     cdef _recv_packet(self):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_frame));
     __pyx_r = ((PyObject *)__pyx_v_frame);
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":456
+    /* "av/codec/context.pyx":459
  *         err_check(res)
  * 
  *         if not res:             # <<<<<<<<<<<<<<
  *             self._next_frame = None
  *             return frame
  */
   }
 
-  /* "av/codec/context.pyx":442
+  /* "av/codec/context.pyx":445
  *         raise NotImplementedError('Base CodecContext cannot decode.')
  * 
  *     cdef _recv_frame(self):             # <<<<<<<<<<<<<<
  * 
  *         if not self._next_frame:
  */
 
@@ -6297,15 +6329,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_frame);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":460
+/* "av/codec/context.pyx":463
  *             return frame
  * 
  *     cdef _recv_packet(self):             # <<<<<<<<<<<<<<
  * 
  *         cdef Packet packet = Packet()
  */
 
@@ -6319,52 +6351,52 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_recv_packet", 0);
 
-  /* "av/codec/context.pyx":462
+  /* "av/codec/context.pyx":465
  *     cdef _recv_packet(self):
  * 
  *         cdef Packet packet = Packet()             # <<<<<<<<<<<<<<
  * 
  *         cdef int res
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2av_6packet_Packet)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2av_6packet_Packet)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_packet = ((struct __pyx_obj_2av_6packet_Packet *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":465
+  /* "av/codec/context.pyx":468
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_receive_packet(self.ptr, packet.ptr)
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/codec/context.pyx":466
+        /* "av/codec/context.pyx":469
  *         cdef int res
  *         with nogil:
  *             res = lib.avcodec_receive_packet(self.ptr, packet.ptr)             # <<<<<<<<<<<<<<
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  *             return
  */
         __pyx_v_res = avcodec_receive_packet(__pyx_v_self->ptr, __pyx_v_packet->ptr);
       }
 
-      /* "av/codec/context.pyx":465
+      /* "av/codec/context.pyx":468
  * 
  *         cdef int res
  *         with nogil:             # <<<<<<<<<<<<<<
  *             res = lib.avcodec_receive_packet(self.ptr, packet.ptr)
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  */
       /*finally:*/ {
@@ -6375,15 +6407,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "av/codec/context.pyx":467
+  /* "av/codec/context.pyx":470
  *         with nogil:
  *             res = lib.avcodec_receive_packet(self.ptr, packet.ptr)
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:             # <<<<<<<<<<<<<<
  *             return
  *         err_check(res)
  */
   __pyx_t_3 = ((__pyx_v_res == (-EAGAIN)) != 0);
@@ -6393,75 +6425,75 @@
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_3 = ((__pyx_v_res == AVERROR_EOF) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "av/codec/context.pyx":468
+    /* "av/codec/context.pyx":471
  *             res = lib.avcodec_receive_packet(self.ptr, packet.ptr)
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  *             return             # <<<<<<<<<<<<<<
  *         err_check(res)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":467
+    /* "av/codec/context.pyx":470
  *         with nogil:
  *             res = lib.avcodec_receive_packet(self.ptr, packet.ptr)
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:             # <<<<<<<<<<<<<<
  *             return
  *         err_check(res)
  */
   }
 
-  /* "av/codec/context.pyx":469
+  /* "av/codec/context.pyx":472
  *         if res == -EAGAIN or res == lib.AVERROR_EOF:
  *             return
  *         err_check(res)             # <<<<<<<<<<<<<<
  * 
  *         if not res:
  */
-  __pyx_t_4 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_2av_5error_err_check(__pyx_v_res, 0, NULL); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 472, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":471
+  /* "av/codec/context.pyx":474
  *         err_check(res)
  * 
  *         if not res:             # <<<<<<<<<<<<<<
  *             return packet
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_res != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "av/codec/context.pyx":472
+    /* "av/codec/context.pyx":475
  * 
  *         if not res:
  *             return packet             # <<<<<<<<<<<<<<
  * 
  *     cpdef encode(self, Frame frame=None):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_packet));
     __pyx_r = ((PyObject *)__pyx_v_packet);
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":471
+    /* "av/codec/context.pyx":474
  *         err_check(res)
  * 
  *         if not res:             # <<<<<<<<<<<<<<
  *             return packet
  * 
  */
   }
 
-  /* "av/codec/context.pyx":460
+  /* "av/codec/context.pyx":463
  *             return frame
  * 
  *     cdef _recv_packet(self):             # <<<<<<<<<<<<<<
  * 
  *         cdef Packet packet = Packet()
  */
 
@@ -6475,15 +6507,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_packet);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":474
+/* "av/codec/context.pyx":477
  *             return packet
  * 
  *     cpdef encode(self, Frame frame=None):             # <<<<<<<<<<<<<<
  *         """Encode a list of :class:`.Packet` from the given :class:`.Frame`."""
  * 
  */
 
@@ -6522,15 +6554,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2av_5codec_7context_12CodecContext_23encode)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6539,15 +6571,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_frame)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_frame));
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 474, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6560,15 +6592,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "av/codec/context.pyx":477
+  /* "av/codec/context.pyx":480
  *         """Encode a list of :class:`.Packet` from the given :class:`.Frame`."""
  * 
  *         if self.ptr.codec_type not in [lib.AVMEDIA_TYPE_VIDEO, lib.AVMEDIA_TYPE_AUDIO]:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError('Encoding is only supported for audio and video.')
  * 
  */
   switch (__pyx_v_self->ptr->codec_type) {
@@ -6579,320 +6611,320 @@
     default:
     __pyx_t_5 = 1;
     break;
   }
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "av/codec/context.pyx":478
+    /* "av/codec/context.pyx":481
  * 
  *         if self.ptr.codec_type not in [lib.AVMEDIA_TYPE_VIDEO, lib.AVMEDIA_TYPE_AUDIO]:
  *             raise NotImplementedError('Encoding is only supported for audio and video.')             # <<<<<<<<<<<<<<
  * 
  *         self.open(strict=False)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 481, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 478, __pyx_L1_error)
+    __PYX_ERR(0, 481, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":477
+    /* "av/codec/context.pyx":480
  *         """Encode a list of :class:`.Packet` from the given :class:`.Frame`."""
  * 
  *         if self.ptr.codec_type not in [lib.AVMEDIA_TYPE_VIDEO, lib.AVMEDIA_TYPE_AUDIO]:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError('Encoding is only supported for audio and video.')
  * 
  */
   }
 
-  /* "av/codec/context.pyx":480
+  /* "av/codec/context.pyx":483
  *             raise NotImplementedError('Encoding is only supported for audio and video.')
  * 
  *         self.open(strict=False)             # <<<<<<<<<<<<<<
  * 
  *         frames = self._prepare_frames_for_encode(frame)
  */
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.strict = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->open(__pyx_v_self, 0, &__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->open(__pyx_v_self, 0, &__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":482
+  /* "av/codec/context.pyx":485
  *         self.open(strict=False)
  * 
  *         frames = self._prepare_frames_for_encode(frame)             # <<<<<<<<<<<<<<
  * 
  *         # Assert the frames are in our time base.
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_prepare_frames_for_encode(__pyx_v_self, __pyx_v_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_prepare_frames_for_encode(__pyx_v_self, __pyx_v_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_frames = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":486
+  /* "av/codec/context.pyx":489
  *         # Assert the frames are in our time base.
  *         # TODO: Don't mutate time.
  *         for frame in frames:             # <<<<<<<<<<<<<<
  *             if frame is not None:
  *                 frame._rebase_time(self.ptr.time_base)
  */
   if (likely(PyList_CheckExact(__pyx_v_frames)) || PyTuple_CheckExact(__pyx_v_frames)) {
     __pyx_t_1 = __pyx_v_frames; __Pyx_INCREF(__pyx_t_1); __pyx_t_8 = 0;
     __pyx_t_9 = NULL;
   } else {
-    __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_frames); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
+    __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_frames); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 486, __pyx_L1_error)
+    __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 489, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_9)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 486, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 486, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_9(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 486, __pyx_L1_error)
+          else __PYX_ERR(0, 489, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 486, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_frame, ((struct __pyx_obj_2av_5frame_Frame *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "av/codec/context.pyx":487
+    /* "av/codec/context.pyx":490
  *         # TODO: Don't mutate time.
  *         for frame in frames:
  *             if frame is not None:             # <<<<<<<<<<<<<<
  *                 frame._rebase_time(self.ptr.time_base)
  * 
  */
     __pyx_t_6 = (((PyObject *)__pyx_v_frame) != Py_None);
     __pyx_t_5 = (__pyx_t_6 != 0);
     if (__pyx_t_5) {
 
-      /* "av/codec/context.pyx":488
+      /* "av/codec/context.pyx":491
  *         for frame in frames:
  *             if frame is not None:
  *                 frame._rebase_time(self.ptr.time_base)             # <<<<<<<<<<<<<<
  * 
  *         res = []
  */
-      __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5frame_Frame *)__pyx_v_frame->__pyx_vtab)->_rebase_time(__pyx_v_frame, __pyx_v_self->ptr->time_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 488, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5frame_Frame *)__pyx_v_frame->__pyx_vtab)->_rebase_time(__pyx_v_frame, __pyx_v_self->ptr->time_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "av/codec/context.pyx":487
+      /* "av/codec/context.pyx":490
  *         # TODO: Don't mutate time.
  *         for frame in frames:
  *             if frame is not None:             # <<<<<<<<<<<<<<
  *                 frame._rebase_time(self.ptr.time_base)
  * 
  */
     }
 
-    /* "av/codec/context.pyx":486
+    /* "av/codec/context.pyx":489
  *         # Assert the frames are in our time base.
  *         # TODO: Don't mutate time.
  *         for frame in frames:             # <<<<<<<<<<<<<<
  *             if frame is not None:
  *                 frame._rebase_time(self.ptr.time_base)
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":490
+  /* "av/codec/context.pyx":493
  *                 frame._rebase_time(self.ptr.time_base)
  * 
  *         res = []             # <<<<<<<<<<<<<<
  *         for frame in frames:
  *             for packet in self._send_frame_and_recv(frame):
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_res = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":491
+  /* "av/codec/context.pyx":494
  * 
  *         res = []
  *         for frame in frames:             # <<<<<<<<<<<<<<
  *             for packet in self._send_frame_and_recv(frame):
  *                 self._setup_encoded_packet(packet)
  */
   if (likely(PyList_CheckExact(__pyx_v_frames)) || PyTuple_CheckExact(__pyx_v_frames)) {
     __pyx_t_1 = __pyx_v_frames; __Pyx_INCREF(__pyx_t_1); __pyx_t_8 = 0;
     __pyx_t_9 = NULL;
   } else {
-    __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_frames); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_frames); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 494, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_9)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 491, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 494, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 491, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 494, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_9(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 491, __pyx_L1_error)
+          else __PYX_ERR(0, 494, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 491, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_frame, ((struct __pyx_obj_2av_5frame_Frame *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "av/codec/context.pyx":492
+    /* "av/codec/context.pyx":495
  *         res = []
  *         for frame in frames:
  *             for packet in self._send_frame_and_recv(frame):             # <<<<<<<<<<<<<<
  *                 self._setup_encoded_packet(packet)
  *                 res.append(packet)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_send_frame_and_recv(__pyx_v_self, __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_send_frame_and_recv(__pyx_v_self, __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_10 = 0;
       __pyx_t_11 = NULL;
     } else {
-      __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+      __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 492, __pyx_L1_error)
+      __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 495, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_11)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_2); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 492, __pyx_L1_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_2); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 495, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_2); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 492, __pyx_L1_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_2); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 495, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_11(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 492, __pyx_L1_error)
+            else __PYX_ERR(0, 495, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_v_packet, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "av/codec/context.pyx":493
+      /* "av/codec/context.pyx":496
  *         for frame in frames:
  *             for packet in self._send_frame_and_recv(frame):
  *                 self._setup_encoded_packet(packet)             # <<<<<<<<<<<<<<
  *                 res.append(packet)
  *         return res
  */
-      if (!(likely(((__pyx_v_packet) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_packet, __pyx_ptype_2av_6packet_Packet))))) __PYX_ERR(0, 493, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_setup_encoded_packet(__pyx_v_self, ((struct __pyx_obj_2av_6packet_Packet *)__pyx_v_packet)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+      if (!(likely(((__pyx_v_packet) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_packet, __pyx_ptype_2av_6packet_Packet))))) __PYX_ERR(0, 496, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_setup_encoded_packet(__pyx_v_self, ((struct __pyx_obj_2av_6packet_Packet *)__pyx_v_packet)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 496, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "av/codec/context.pyx":494
+      /* "av/codec/context.pyx":497
  *             for packet in self._send_frame_and_recv(frame):
  *                 self._setup_encoded_packet(packet)
  *                 res.append(packet)             # <<<<<<<<<<<<<<
  *         return res
  * 
  */
-      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, __pyx_v_packet); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 494, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, __pyx_v_packet); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 497, __pyx_L1_error)
 
-      /* "av/codec/context.pyx":492
+      /* "av/codec/context.pyx":495
  *         res = []
  *         for frame in frames:
  *             for packet in self._send_frame_and_recv(frame):             # <<<<<<<<<<<<<<
  *                 self._setup_encoded_packet(packet)
  *                 res.append(packet)
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "av/codec/context.pyx":491
+    /* "av/codec/context.pyx":494
  * 
  *         res = []
  *         for frame in frames:             # <<<<<<<<<<<<<<
  *             for packet in self._send_frame_and_recv(frame):
  *                 self._setup_encoded_packet(packet)
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":495
+  /* "av/codec/context.pyx":498
  *                 self._setup_encoded_packet(packet)
  *                 res.append(packet)
  *         return res             # <<<<<<<<<<<<<<
  * 
  *     cdef _setup_encoded_packet(self, Packet packet):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res);
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":474
+  /* "av/codec/context.pyx":477
  *             return packet
  * 
  *     cpdef encode(self, Frame frame=None):             # <<<<<<<<<<<<<<
  *         """Encode a list of :class:`.Packet` from the given :class:`.Frame`."""
  * 
  */
 
@@ -6943,35 +6975,35 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode") < 0)) __PYX_ERR(0, 474, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode") < 0)) __PYX_ERR(0, 477, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_frame = ((struct __pyx_obj_2av_5frame_Frame *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 474, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 477, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 474, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 477, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_5codec_7context_12CodecContext_22encode(((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_v_self), __pyx_v_frame);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6987,15 +7019,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.frame = __pyx_v_frame;
-  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->encode(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->encode(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7004,54 +7036,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":497
+/* "av/codec/context.pyx":500
  *         return res
  * 
  *     cdef _setup_encoded_packet(self, Packet packet):             # <<<<<<<<<<<<<<
  *         # We coerced the frame's time_base into the CodecContext's during encoding,
  *         # and FFmpeg copied the frame's pts/dts to the packet, so keep track of
  */
 
 static PyObject *__pyx_f_2av_5codec_7context_12CodecContext__setup_encoded_packet(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, struct __pyx_obj_2av_6packet_Packet *__pyx_v_packet) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   AVRational __pyx_t_1;
   __Pyx_RefNannySetupContext("_setup_encoded_packet", 0);
 
-  /* "av/codec/context.pyx":505
+  /* "av/codec/context.pyx":508
  *         # NOTE: if the CodecContext's time_base is altered during encoding, all bets
  *         # are off!
  *         packet._time_base = self.ptr.time_base             # <<<<<<<<<<<<<<
  * 
  *     cpdef decode(self, Packet packet=None):
  */
   __pyx_t_1 = __pyx_v_self->ptr->time_base;
   __pyx_v_packet->_time_base = __pyx_t_1;
 
-  /* "av/codec/context.pyx":497
+  /* "av/codec/context.pyx":500
  *         return res
  * 
  *     cdef _setup_encoded_packet(self, Packet packet):             # <<<<<<<<<<<<<<
  *         # We coerced the frame's time_base into the CodecContext's during encoding,
  *         # and FFmpeg copied the frame's pts/dts to the packet, so keep track of
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":507
+/* "av/codec/context.pyx":510
  *         packet._time_base = self.ptr.time_base
  * 
  *     cpdef decode(self, Packet packet=None):             # <<<<<<<<<<<<<<
  *         """Decode a list of :class:`.Frame` from the given :class:`.Packet`.
  * 
  */
 
@@ -7086,15 +7118,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2av_5codec_7context_12CodecContext_25decode)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -7103,15 +7135,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_packet)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_packet));
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 507, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -7124,187 +7156,187 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "av/codec/context.pyx":516
+  /* "av/codec/context.pyx":519
  *         """
  * 
  *         if not self.codec.ptr:             # <<<<<<<<<<<<<<
  *             raise ValueError('cannot decode unknown codec')
  * 
  */
   __pyx_t_5 = ((!(__pyx_v_self->codec->ptr != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "av/codec/context.pyx":517
+    /* "av/codec/context.pyx":520
  * 
  *         if not self.codec.ptr:
  *             raise ValueError('cannot decode unknown codec')             # <<<<<<<<<<<<<<
  * 
  *         self.open(strict=False)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 517, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 517, __pyx_L1_error)
+    __PYX_ERR(0, 520, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":516
+    /* "av/codec/context.pyx":519
  *         """
  * 
  *         if not self.codec.ptr:             # <<<<<<<<<<<<<<
  *             raise ValueError('cannot decode unknown codec')
  * 
  */
   }
 
-  /* "av/codec/context.pyx":519
+  /* "av/codec/context.pyx":522
  *             raise ValueError('cannot decode unknown codec')
  * 
  *         self.open(strict=False)             # <<<<<<<<<<<<<<
  * 
  *         res = []
  */
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.strict = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->open(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->open(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":521
+  /* "av/codec/context.pyx":524
  *         self.open(strict=False)
  * 
  *         res = []             # <<<<<<<<<<<<<<
  *         for frame in self._send_packet_and_recv(packet):
  *             if isinstance(frame, Frame):
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_res = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":522
+  /* "av/codec/context.pyx":525
  * 
  *         res = []
  *         for frame in self._send_packet_and_recv(packet):             # <<<<<<<<<<<<<<
  *             if isinstance(frame, Frame):
  *                 self._setup_decoded_frame(frame, packet)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_send_packet_and_recv(__pyx_v_self, __pyx_v_packet); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_send_packet_and_recv(__pyx_v_self, __pyx_v_packet); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 522, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 525, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_8(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 522, __pyx_L1_error)
+          else __PYX_ERR(0, 525, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_frame, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "av/codec/context.pyx":523
+    /* "av/codec/context.pyx":526
  *         res = []
  *         for frame in self._send_packet_and_recv(packet):
  *             if isinstance(frame, Frame):             # <<<<<<<<<<<<<<
  *                 self._setup_decoded_frame(frame, packet)
  *             res.append(frame)
  */
     __pyx_t_5 = __Pyx_TypeCheck(__pyx_v_frame, __pyx_ptype_2av_5frame_Frame); 
     __pyx_t_9 = (__pyx_t_5 != 0);
     if (__pyx_t_9) {
 
-      /* "av/codec/context.pyx":524
+      /* "av/codec/context.pyx":527
  *         for frame in self._send_packet_and_recv(packet):
  *             if isinstance(frame, Frame):
  *                 self._setup_decoded_frame(frame, packet)             # <<<<<<<<<<<<<<
  *             res.append(frame)
  *         return res
  */
-      if (!(likely(((__pyx_v_frame) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_frame, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 524, __pyx_L1_error)
-      __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_setup_decoded_frame(__pyx_v_self, ((struct __pyx_obj_2av_5frame_Frame *)__pyx_v_frame), __pyx_v_packet); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
+      if (!(likely(((__pyx_v_frame) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_frame, __pyx_ptype_2av_5frame_Frame))))) __PYX_ERR(0, 527, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_self->__pyx_vtab)->_setup_decoded_frame(__pyx_v_self, ((struct __pyx_obj_2av_5frame_Frame *)__pyx_v_frame), __pyx_v_packet); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 527, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "av/codec/context.pyx":523
+      /* "av/codec/context.pyx":526
  *         res = []
  *         for frame in self._send_packet_and_recv(packet):
  *             if isinstance(frame, Frame):             # <<<<<<<<<<<<<<
  *                 self._setup_decoded_frame(frame, packet)
  *             res.append(frame)
  */
     }
 
-    /* "av/codec/context.pyx":525
+    /* "av/codec/context.pyx":528
  *             if isinstance(frame, Frame):
  *                 self._setup_decoded_frame(frame, packet)
  *             res.append(frame)             # <<<<<<<<<<<<<<
  *         return res
  * 
  */
-    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_res, __pyx_v_frame); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 525, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_res, __pyx_v_frame); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 528, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":522
+    /* "av/codec/context.pyx":525
  * 
  *         res = []
  *         for frame in self._send_packet_and_recv(packet):             # <<<<<<<<<<<<<<
  *             if isinstance(frame, Frame):
  *                 self._setup_decoded_frame(frame, packet)
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":526
+  /* "av/codec/context.pyx":529
  *                 self._setup_decoded_frame(frame, packet)
  *             res.append(frame)
  *         return res             # <<<<<<<<<<<<<<
  * 
  *     cdef _setup_decoded_frame(self, Frame frame, Packet packet):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res);
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":507
+  /* "av/codec/context.pyx":510
  *         packet._time_base = self.ptr.time_base
  * 
  *     cpdef decode(self, Packet packet=None):             # <<<<<<<<<<<<<<
  *         """Decode a list of :class:`.Frame` from the given :class:`.Packet`.
  * 
  */
 
@@ -7353,35 +7385,35 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_packet);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "decode") < 0)) __PYX_ERR(0, 507, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "decode") < 0)) __PYX_ERR(0, 510, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_packet = ((struct __pyx_obj_2av_6packet_Packet *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 507, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("decode", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 510, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_packet), __pyx_ptype_2av_6packet_Packet, 1, "packet", 0))) __PYX_ERR(0, 507, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_packet), __pyx_ptype_2av_6packet_Packet, 1, "packet", 0))) __PYX_ERR(0, 510, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_5codec_7context_12CodecContext_24decode(((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_v_self), __pyx_v_packet);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7397,15 +7429,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.packet = __pyx_v_packet;
-  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->decode(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_2av_5codec_7context_CodecContext->decode(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7414,63 +7446,63 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":528
+/* "av/codec/context.pyx":531
  *         return res
  * 
  *     cdef _setup_decoded_frame(self, Frame frame, Packet packet):             # <<<<<<<<<<<<<<
  * 
  *         # Propagate our manual times.
  */
 
 static PyObject *__pyx_f_2av_5codec_7context_12CodecContext__setup_decoded_frame(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, struct __pyx_obj_2av_5frame_Frame *__pyx_v_frame, struct __pyx_obj_2av_6packet_Packet *__pyx_v_packet) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   AVRational __pyx_t_1;
   __Pyx_RefNannySetupContext("_setup_decoded_frame", 0);
 
-  /* "av/codec/context.pyx":535
+  /* "av/codec/context.pyx":538
  *         # TODO: Somehow get this from the stream so we can not pass the
  *         # packet here (because flushing packets are bogus).
  *         frame._time_base = packet._time_base             # <<<<<<<<<<<<<<
  * 
  *         frame.index = self.ptr.frame_number - 1
  */
   __pyx_t_1 = __pyx_v_packet->_time_base;
   __pyx_v_frame->_time_base = __pyx_t_1;
 
-  /* "av/codec/context.pyx":537
+  /* "av/codec/context.pyx":540
  *         frame._time_base = packet._time_base
  * 
  *         frame.index = self.ptr.frame_number - 1             # <<<<<<<<<<<<<<
  * 
  *     property name:
  */
   __pyx_v_frame->index = (__pyx_v_self->ptr->frame_number - 1);
 
-  /* "av/codec/context.pyx":528
+  /* "av/codec/context.pyx":531
  *         return res
  * 
  *     cdef _setup_decoded_frame(self, Frame frame, Packet packet):             # <<<<<<<<<<<<<<
  * 
  *         # Propagate our manual times.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":540
+/* "av/codec/context.pyx":543
  * 
  *     property name:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.codec.name
  * 
  */
 
@@ -7492,29 +7524,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":541
+  /* "av/codec/context.pyx":544
  *     property name:
  *         def __get__(self):
  *             return self.codec.name             # <<<<<<<<<<<<<<
  * 
  *     property type:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->codec), __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->codec), __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":540
+  /* "av/codec/context.pyx":543
  * 
  *     property name:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.codec.name
  * 
  */
 
@@ -7525,15 +7557,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":544
+/* "av/codec/context.pyx":547
  * 
  *     property type:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.codec.type
  * 
  */
 
@@ -7555,29 +7587,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":545
+  /* "av/codec/context.pyx":548
  *     property type:
  *         def __get__(self):
  *             return self.codec.type             # <<<<<<<<<<<<<<
  * 
  *     property profile:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->codec), __pyx_n_s_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->codec), __pyx_n_s_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":544
+  /* "av/codec/context.pyx":547
  * 
  *     property type:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.codec.type
  * 
  */
 
@@ -7588,15 +7620,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":548
+/* "av/codec/context.pyx":551
  * 
  *     property profile:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if self.ptr.codec and lib.av_get_profile_name(self.ptr.codec, self.ptr.profile):
  *                 return lib.av_get_profile_name(self.ptr.codec, self.ptr.profile)
  */
 
@@ -7620,15 +7652,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":549
+  /* "av/codec/context.pyx":552
  *     property profile:
  *         def __get__(self):
  *             if self.ptr.codec and lib.av_get_profile_name(self.ptr.codec, self.ptr.profile):             # <<<<<<<<<<<<<<
  *                 return lib.av_get_profile_name(self.ptr.codec, self.ptr.profile)
  * 
  */
   __pyx_t_2 = (__pyx_v_self->ptr->codec != 0);
@@ -7638,38 +7670,38 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (av_get_profile_name(__pyx_v_self->ptr->codec, __pyx_v_self->ptr->profile) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":550
+    /* "av/codec/context.pyx":553
  *         def __get__(self):
  *             if self.ptr.codec and lib.av_get_profile_name(self.ptr.codec, self.ptr.profile):
  *                 return lib.av_get_profile_name(self.ptr.codec, self.ptr.profile)             # <<<<<<<<<<<<<<
  * 
  *     property time_base:
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyStr_FromString(av_get_profile_name(__pyx_v_self->ptr->codec, __pyx_v_self->ptr->profile)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyStr_FromString(av_get_profile_name(__pyx_v_self->ptr->codec, __pyx_v_self->ptr->profile)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 553, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":549
+    /* "av/codec/context.pyx":552
  *     property profile:
  *         def __get__(self):
  *             if self.ptr.codec and lib.av_get_profile_name(self.ptr.codec, self.ptr.profile):             # <<<<<<<<<<<<<<
  *                 return lib.av_get_profile_name(self.ptr.codec, self.ptr.profile)
  * 
  */
   }
 
-  /* "av/codec/context.pyx":548
+  /* "av/codec/context.pyx":551
  * 
  *     property profile:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if self.ptr.codec and lib.av_get_profile_name(self.ptr.codec, self.ptr.profile):
  *                 return lib.av_get_profile_name(self.ptr.codec, self.ptr.profile)
  */
 
@@ -7682,20 +7714,20 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":553
+/* "av/codec/context.pyx":556
  * 
  *     property time_base:
  *         def __get__(self):             # <<<<<<<<<<<<<<
- *             return avrational_to_fraction(&self.ptr.time_base)
- * 
+ *             if self.is_decoder:
+ *                 warnings.warn(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_5codec_7context_12CodecContext_9time_base_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_2av_5codec_7context_12CodecContext_9time_base_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7707,58 +7739,161 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_9time_base___get__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":554
+  /* "av/codec/context.pyx":557
  *     property time_base:
  *         def __get__(self):
+ *             if self.is_decoder:             # <<<<<<<<<<<<<<
+ *                 warnings.warn(
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_decoder); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_2) {
+
+    /* "av/codec/context.pyx":558
+ *         def __get__(self):
+ *             if self.is_decoder:
+ *                 warnings.warn(             # <<<<<<<<<<<<<<
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ *                     AVDeprecationWarning
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_warnings); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 558, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_warn); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 558, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "av/codec/context.pyx":560
+ *                 warnings.warn(
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ *                     AVDeprecationWarning             # <<<<<<<<<<<<<<
+ *                 )
+ *             return avrational_to_fraction(&self.ptr.time_base)
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AVDeprecationWarning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = NULL;
+    __pyx_t_6 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_6 = 1;
+      }
+    }
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_4)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_s_Using_CodecContext_time_base_for, __pyx_t_3};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_s_Using_CodecContext_time_base_for, __pyx_t_3};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 558, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      if (__pyx_t_5) {
+        __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
+      }
+      __Pyx_INCREF(__pyx_kp_s_Using_CodecContext_time_base_for);
+      __Pyx_GIVEREF(__pyx_kp_s_Using_CodecContext_time_base_for);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_s_Using_CodecContext_time_base_for);
+      __Pyx_GIVEREF(__pyx_t_3);
+      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_3);
+      __pyx_t_3 = 0;
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "av/codec/context.pyx":557
+ *     property time_base:
+ *         def __get__(self):
+ *             if self.is_decoder:             # <<<<<<<<<<<<<<
+ *                 warnings.warn(
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ */
+  }
+
+  /* "av/codec/context.pyx":562
+ *                     AVDeprecationWarning
+ *                 )
  *             return avrational_to_fraction(&self.ptr.time_base)             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_2av_5utils_avrational_to_fraction((&__pyx_v_self->ptr->time_base)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 554, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2av_5utils_avrational_to_fraction((&__pyx_v_self->ptr->time_base)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":553
+  /* "av/codec/context.pyx":556
  * 
  *     property time_base:
  *         def __get__(self):             # <<<<<<<<<<<<<<
- *             return avrational_to_fraction(&self.ptr.time_base)
- * 
+ *             if self.is_decoder:
+ *                 warnings.warn(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("av.codec.context.CodecContext.time_base.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":556
+/* "av/codec/context.pyx":564
  *             return avrational_to_fraction(&self.ptr.time_base)
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
- *             to_avrational(value, &self.ptr.time_base)
- * 
+ *             if self.is_decoder:
+ *                 warnings.warn(
  */
 
 /* Python wrapper */
 static int __pyx_pw_2av_5codec_7context_12CodecContext_9time_base_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
 static int __pyx_pw_2av_5codec_7context_12CodecContext_9time_base_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -7770,51 +7905,154 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_2av_5codec_7context_12CodecContext_9time_base_2__set__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":557
+  /* "av/codec/context.pyx":565
  * 
  *         def __set__(self, value):
+ *             if self.is_decoder:             # <<<<<<<<<<<<<<
+ *                 warnings.warn(
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_decoder); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_2) {
+
+    /* "av/codec/context.pyx":566
+ *         def __set__(self, value):
+ *             if self.is_decoder:
+ *                 warnings.warn(             # <<<<<<<<<<<<<<
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ *                     AVDeprecationWarning
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_warnings); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_warn); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "av/codec/context.pyx":568
+ *                 warnings.warn(
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ *                     AVDeprecationWarning             # <<<<<<<<<<<<<<
+ *                 )
+ *             to_avrational(value, &self.ptr.time_base)
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AVDeprecationWarning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 568, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = NULL;
+    __pyx_t_6 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_6 = 1;
+      }
+    }
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_4)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_s_Using_CodecContext_time_base_for, __pyx_t_3};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_kp_s_Using_CodecContext_time_base_for, __pyx_t_3};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      if (__pyx_t_5) {
+        __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
+      }
+      __Pyx_INCREF(__pyx_kp_s_Using_CodecContext_time_base_for);
+      __Pyx_GIVEREF(__pyx_kp_s_Using_CodecContext_time_base_for);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_kp_s_Using_CodecContext_time_base_for);
+      __Pyx_GIVEREF(__pyx_t_3);
+      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_3);
+      __pyx_t_3 = 0;
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "av/codec/context.pyx":565
+ * 
+ *         def __set__(self, value):
+ *             if self.is_decoder:             # <<<<<<<<<<<<<<
+ *                 warnings.warn(
+ *                     "Using CodecContext.time_base for decoders is deprecated.",
+ */
+  }
+
+  /* "av/codec/context.pyx":570
+ *                     AVDeprecationWarning
+ *                 )
  *             to_avrational(value, &self.ptr.time_base)             # <<<<<<<<<<<<<<
  * 
  *     property codec_tag:
  */
-  __pyx_t_1 = __pyx_f_2av_5utils_to_avrational(__pyx_v_value, (&__pyx_v_self->ptr->time_base)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2av_5utils_to_avrational(__pyx_v_value, (&__pyx_v_self->ptr->time_base)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":556
+  /* "av/codec/context.pyx":564
  *             return avrational_to_fraction(&self.ptr.time_base)
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
- *             to_avrational(value, &self.ptr.time_base)
- * 
+ *             if self.is_decoder:
+ *                 warnings.warn(
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("av.codec.context.CodecContext.time_base.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":560
+/* "av/codec/context.pyx":573
  * 
  *     property codec_tag:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(
  *                 encoding="ascii")
  */
 
@@ -7838,66 +8076,66 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":561
+  /* "av/codec/context.pyx":574
  *     property codec_tag:
  *         def __get__(self):
  *             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(             # <<<<<<<<<<<<<<
  *                 encoding="ascii")
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_self->ptr->codec_tag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_self->ptr->codec_tag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 561, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 561, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__10, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 561, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 574, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__10, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "av/codec/context.pyx":562
+  /* "av/codec/context.pyx":575
  *         def __get__(self):
  *             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(
  *                 encoding="ascii")             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value):
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_encoding, __pyx_n_s_ascii) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_encoding, __pyx_n_s_ascii) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
 
-  /* "av/codec/context.pyx":561
+  /* "av/codec/context.pyx":574
  *     property codec_tag:
  *         def __get__(self):
  *             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(             # <<<<<<<<<<<<<<
  *                 encoding="ascii")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":560
+  /* "av/codec/context.pyx":573
  * 
  *     property codec_tag:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(
  *                 encoding="ascii")
  */
 
@@ -7910,15 +8148,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":564
+/* "av/codec/context.pyx":577
  *                 encoding="ascii")
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
  *             if isinstance(value, str) and len(value) == 4:
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),
  */
 
@@ -7948,113 +8186,113 @@
   PyObject *__pyx_t_8 = NULL;
   unsigned int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":565
+  /* "av/codec/context.pyx":578
  * 
  *         def __set__(self, value):
  *             if isinstance(value, str) and len(value) == 4:             # <<<<<<<<<<<<<<
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),
  *                                                     byteorder="little", signed=False)
  */
   __pyx_t_2 = PyString_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 578, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_4 == 4) != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (likely(__pyx_t_1)) {
 
-    /* "av/codec/context.pyx":566
+    /* "av/codec/context.pyx":579
  *         def __set__(self, value):
  *             if isinstance(value, str) and len(value) == 4:
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),             # <<<<<<<<<<<<<<
  *                                                     byteorder="little", signed=False)
  *             else:
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_n_s_ascii) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 566, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_n_s_ascii) < 0) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
     __pyx_t_8 = 0;
 
-    /* "av/codec/context.pyx":567
+    /* "av/codec/context.pyx":580
  *             if isinstance(value, str) and len(value) == 4:
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),
  *                                                     byteorder="little", signed=False)             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError("Codec tag should be a 4 character string.")
  */
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 580, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 580, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":566
+    /* "av/codec/context.pyx":579
  *         def __set__(self, value):
  *             if isinstance(value, str) and len(value) == 4:
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),             # <<<<<<<<<<<<<<
  *                                                     byteorder="little", signed=False)
  *             else:
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_6); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_6); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_self->ptr->codec_tag = __pyx_t_9;
 
-    /* "av/codec/context.pyx":565
+    /* "av/codec/context.pyx":578
  * 
  *         def __set__(self, value):
  *             if isinstance(value, str) and len(value) == 4:             # <<<<<<<<<<<<<<
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),
  *                                                     byteorder="little", signed=False)
  */
     goto __pyx_L3;
   }
 
-  /* "av/codec/context.pyx":569
+  /* "av/codec/context.pyx":582
  *                                                     byteorder="little", signed=False)
  *             else:
  *                 raise ValueError("Codec tag should be a 4 character string.")             # <<<<<<<<<<<<<<
  * 
  *     property ticks_per_frame:
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 582, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 569, __pyx_L1_error)
+    __PYX_ERR(0, 582, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "av/codec/context.pyx":564
+  /* "av/codec/context.pyx":577
  *                 encoding="ascii")
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
  *             if isinstance(value, str) and len(value) == 4:
  *                 self.ptr.codec_tag = int.from_bytes(value.encode(encoding="ascii"),
  */
 
@@ -8069,15 +8307,15 @@
   __Pyx_AddTraceback("av.codec.context.CodecContext.codec_tag.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":572
+/* "av/codec/context.pyx":585
  * 
  *     property ticks_per_frame:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.ticks_per_frame
  * 
  */
 
@@ -8099,29 +8337,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":573
+  /* "av/codec/context.pyx":586
  *     property ticks_per_frame:
  *         def __get__(self):
  *             return self.ptr.ticks_per_frame             # <<<<<<<<<<<<<<
  * 
  *     property bit_rate:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->ticks_per_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 573, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->ticks_per_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":572
+  /* "av/codec/context.pyx":585
  * 
  *     property ticks_per_frame:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.ticks_per_frame
  * 
  */
 
@@ -8132,15 +8370,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":576
+/* "av/codec/context.pyx":589
  * 
  *     property bit_rate:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.bit_rate if self.ptr.bit_rate > 0 else None
  * 
  */
 
@@ -8163,36 +8401,36 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":577
+  /* "av/codec/context.pyx":590
  *     property bit_rate:
  *         def __get__(self):
  *             return self.ptr.bit_rate if self.ptr.bit_rate > 0 else None             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int value):
  */
   __Pyx_XDECREF(__pyx_r);
   if (((__pyx_v_self->ptr->bit_rate > 0) != 0)) {
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->bit_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->bit_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(Py_None);
     __pyx_t_1 = Py_None;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":576
+  /* "av/codec/context.pyx":589
  * 
  *     property bit_rate:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.bit_rate if self.ptr.bit_rate > 0 else None
  * 
  */
 
@@ -8204,15 +8442,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":579
+/* "av/codec/context.pyx":592
  *             return self.ptr.bit_rate if self.ptr.bit_rate > 0 else None
  * 
  *         def __set__(self, int value):             # <<<<<<<<<<<<<<
  *             self.ptr.bit_rate = value
  * 
  */
 
@@ -8223,15 +8461,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyInt_As_int(__pyx_arg_value); if (unlikely((__pyx_v_value == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 579, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyInt_As_int(__pyx_arg_value); if (unlikely((__pyx_v_value == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 592, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.bit_rate.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -8243,38 +8481,38 @@
 }
 
 static int __pyx_pf_2av_5codec_7context_12CodecContext_8bit_rate_2__set__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, int __pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":580
+  /* "av/codec/context.pyx":593
  * 
  *         def __set__(self, int value):
  *             self.ptr.bit_rate = value             # <<<<<<<<<<<<<<
  * 
  *     property max_bit_rate:
  */
   __pyx_v_self->ptr->bit_rate = __pyx_v_value;
 
-  /* "av/codec/context.pyx":579
+  /* "av/codec/context.pyx":592
  *             return self.ptr.bit_rate if self.ptr.bit_rate > 0 else None
  * 
  *         def __set__(self, int value):             # <<<<<<<<<<<<<<
  *             self.ptr.bit_rate = value
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":583
+/* "av/codec/context.pyx":596
  * 
  *     property max_bit_rate:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if self.ptr.rc_max_rate > 0:
  *                 return self.ptr.rc_max_rate
  */
 
@@ -8297,61 +8535,61 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":584
+  /* "av/codec/context.pyx":597
  *     property max_bit_rate:
  *         def __get__(self):
  *             if self.ptr.rc_max_rate > 0:             # <<<<<<<<<<<<<<
  *                 return self.ptr.rc_max_rate
  *             else:
  */
   __pyx_t_1 = ((__pyx_v_self->ptr->rc_max_rate > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "av/codec/context.pyx":585
+    /* "av/codec/context.pyx":598
  *         def __get__(self):
  *             if self.ptr.rc_max_rate > 0:
  *                 return self.ptr.rc_max_rate             # <<<<<<<<<<<<<<
  *             else:
  *                 return None
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->rc_max_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->rc_max_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "av/codec/context.pyx":584
+    /* "av/codec/context.pyx":597
  *     property max_bit_rate:
  *         def __get__(self):
  *             if self.ptr.rc_max_rate > 0:             # <<<<<<<<<<<<<<
  *                 return self.ptr.rc_max_rate
  *             else:
  */
   }
 
-  /* "av/codec/context.pyx":587
+  /* "av/codec/context.pyx":600
  *                 return self.ptr.rc_max_rate
  *             else:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *     property bit_rate_tolerance:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "av/codec/context.pyx":583
+  /* "av/codec/context.pyx":596
  * 
  *     property max_bit_rate:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if self.ptr.rc_max_rate > 0:
  *                 return self.ptr.rc_max_rate
  */
 
@@ -8362,15 +8600,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":590
+/* "av/codec/context.pyx":603
  * 
  *     property bit_rate_tolerance:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             self.ptr.bit_rate_tolerance
  * 
  */
 
@@ -8388,39 +8626,39 @@
 }
 
 static PyObject *__pyx_pf_2av_5codec_7context_12CodecContext_18bit_rate_tolerance___get__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":591
+  /* "av/codec/context.pyx":604
  *     property bit_rate_tolerance:
  *         def __get__(self):
  *             self.ptr.bit_rate_tolerance             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int value):
  */
   (void)(__pyx_v_self->ptr->bit_rate_tolerance);
 
-  /* "av/codec/context.pyx":590
+  /* "av/codec/context.pyx":603
  * 
  *     property bit_rate_tolerance:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             self.ptr.bit_rate_tolerance
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":593
+/* "av/codec/context.pyx":606
  *             self.ptr.bit_rate_tolerance
  * 
  *         def __set__(self, int value):             # <<<<<<<<<<<<<<
  *             self.ptr.bit_rate_tolerance = value
  * 
  */
 
@@ -8431,15 +8669,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyInt_As_int(__pyx_arg_value); if (unlikely((__pyx_v_value == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 593, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyInt_As_int(__pyx_arg_value); if (unlikely((__pyx_v_value == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.bit_rate_tolerance.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -8451,38 +8689,38 @@
 }
 
 static int __pyx_pf_2av_5codec_7context_12CodecContext_18bit_rate_tolerance_2__set__(struct __pyx_obj_2av_5codec_7context_CodecContext *__pyx_v_self, int __pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":594
+  /* "av/codec/context.pyx":607
  * 
  *         def __set__(self, int value):
  *             self.ptr.bit_rate_tolerance = value             # <<<<<<<<<<<<<<
  * 
  *     property thread_count:
  */
   __pyx_v_self->ptr->bit_rate_tolerance = __pyx_v_value;
 
-  /* "av/codec/context.pyx":593
+  /* "av/codec/context.pyx":606
  *             self.ptr.bit_rate_tolerance
  * 
  *         def __set__(self, int value):             # <<<<<<<<<<<<<<
  *             self.ptr.bit_rate_tolerance = value
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":603
+/* "av/codec/context.pyx":616
  *         """
  * 
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.thread_count
  * 
  */
 
@@ -8504,29 +8742,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":604
+  /* "av/codec/context.pyx":617
  * 
  *         def __get__(self):
  *             return self.ptr.thread_count             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->thread_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->thread_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":603
+  /* "av/codec/context.pyx":616
  *         """
  * 
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.ptr.thread_count
  * 
  */
 
@@ -8537,15 +8775,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":606
+/* "av/codec/context.pyx":619
  *             return self.ptr.thread_count
  * 
  *         def __set__(self, int value):             # <<<<<<<<<<<<<<
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")
  */
 
@@ -8556,15 +8794,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyInt_As_int(__pyx_arg_value); if (unlikely((__pyx_v_value == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyInt_As_int(__pyx_arg_value); if (unlikely((__pyx_v_value == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 619, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.codec.context.CodecContext.thread_count.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -8581,56 +8819,56 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":607
+  /* "av/codec/context.pyx":620
  * 
  *         def __set__(self, int value):
  *             if lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")
  *             self.ptr.thread_count = value
  */
   __pyx_t_1 = (avcodec_is_open(__pyx_v_self->ptr) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "av/codec/context.pyx":608
+    /* "av/codec/context.pyx":621
  *         def __set__(self, int value):
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")             # <<<<<<<<<<<<<<
  *             self.ptr.thread_count = value
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 608, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 608, __pyx_L1_error)
+    __PYX_ERR(0, 621, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":607
+    /* "av/codec/context.pyx":620
  * 
  *         def __set__(self, int value):
  *             if lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")
  *             self.ptr.thread_count = value
  */
   }
 
-  /* "av/codec/context.pyx":609
+  /* "av/codec/context.pyx":622
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")
  *             self.ptr.thread_count = value             # <<<<<<<<<<<<<<
  * 
  *     property thread_type:
  */
   __pyx_v_self->ptr->thread_count = __pyx_v_value;
 
-  /* "av/codec/context.pyx":606
+  /* "av/codec/context.pyx":619
  *             return self.ptr.thread_count
  * 
  *         def __set__(self, int value):             # <<<<<<<<<<<<<<
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")
  */
 
@@ -8642,15 +8880,15 @@
   __Pyx_AddTraceback("av.codec.context.CodecContext.thread_count.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":618
+/* "av/codec/context.pyx":631
  *         """
  * 
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return ThreadType.get(self.ptr.thread_type, create=True)
  * 
  */
 
@@ -8675,47 +8913,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":619
+  /* "av/codec/context.pyx":632
  * 
  *         def __get__(self):
  *             return ThreadType.get(self.ptr.thread_type, create=True)             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ThreadType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ThreadType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->thread_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->thread_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_create, Py_True) < 0) __PYX_ERR(0, 619, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 619, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_create, Py_True) < 0) __PYX_ERR(0, 632, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":618
+  /* "av/codec/context.pyx":631
  *         """
  * 
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return ThreadType.get(self.ptr.thread_type, create=True)
  * 
  */
 
@@ -8729,15 +8967,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":621
+/* "av/codec/context.pyx":634
  *             return ThreadType.get(self.ptr.thread_type, create=True)
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")
  */
 
@@ -8762,66 +9000,66 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":622
+  /* "av/codec/context.pyx":635
  * 
  *         def __set__(self, value):
  *             if lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")
  *             self.ptr.thread_type = ThreadType[value].value
  */
   __pyx_t_1 = (avcodec_is_open(__pyx_v_self->ptr) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "av/codec/context.pyx":623
+    /* "av/codec/context.pyx":636
  *         def __set__(self, value):
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")             # <<<<<<<<<<<<<<
  *             self.ptr.thread_type = ThreadType[value].value
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 623, __pyx_L1_error)
+    __PYX_ERR(0, 636, __pyx_L1_error)
 
-    /* "av/codec/context.pyx":622
+    /* "av/codec/context.pyx":635
  * 
  *         def __set__(self, value):
  *             if lib.avcodec_is_open(self.ptr):             # <<<<<<<<<<<<<<
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")
  *             self.ptr.thread_type = ThreadType[value].value
  */
   }
 
-  /* "av/codec/context.pyx":624
+  /* "av/codec/context.pyx":637
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")
  *             self.ptr.thread_type = ThreadType[value].value             # <<<<<<<<<<<<<<
  * 
  *     property skip_frame:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ThreadType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 624, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ThreadType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 624, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 624, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 624, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->ptr->thread_type = __pyx_t_4;
 
-  /* "av/codec/context.pyx":621
+  /* "av/codec/context.pyx":634
  *             return ThreadType.get(self.ptr.thread_type, create=True)
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")
  */
 
@@ -8834,15 +9072,15 @@
   __Pyx_AddTraceback("av.codec.context.CodecContext.thread_type.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":633
+/* "av/codec/context.pyx":646
  *         """
  * 
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return SkipType._get(self.ptr.skip_frame, create=True)
  * 
  */
 
@@ -8867,47 +9105,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/codec/context.pyx":634
+  /* "av/codec/context.pyx":647
  * 
  *         def __get__(self):
  *             return SkipType._get(self.ptr.skip_frame, create=True)             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SkipType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SkipType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(__pyx_v_self->ptr->skip_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(__pyx_v_self->ptr->skip_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_create, Py_True) < 0) __PYX_ERR(0, 634, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 634, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_create, Py_True) < 0) __PYX_ERR(0, 647, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "av/codec/context.pyx":633
+  /* "av/codec/context.pyx":646
  *         """
  * 
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return SkipType._get(self.ptr.skip_frame, create=True)
  * 
  */
 
@@ -8921,15 +9159,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/codec/context.pyx":636
+/* "av/codec/context.pyx":649
  *             return SkipType._get(self.ptr.skip_frame, create=True)
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
  *             self.ptr.skip_frame = SkipType[value].value
  */
 
 /* Python wrapper */
@@ -8952,32 +9190,32 @@
   PyObject *__pyx_t_2 = NULL;
   enum AVDiscard __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "av/codec/context.pyx":637
+  /* "av/codec/context.pyx":650
  * 
  *         def __set__(self, value):
  *             self.ptr.skip_frame = SkipType[value].value             # <<<<<<<<<<<<<<
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SkipType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SkipType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = ((enum AVDiscard)__Pyx_PyInt_As_enum__AVDiscard(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_3 = ((enum AVDiscard)__Pyx_PyInt_As_enum__AVDiscard(__pyx_t_1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->ptr->skip_frame = __pyx_t_3;
 
-  /* "av/codec/context.pyx":636
+  /* "av/codec/context.pyx":649
  *             return SkipType._get(self.ptr.skip_frame, create=True)
  * 
  *         def __set__(self, value):             # <<<<<<<<<<<<<<
  *             self.ptr.skip_frame = SkipType[value].value
  */
 
   /* function exit code */
@@ -9650,14 +9888,15 @@
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_s_4MV, __pyx_k_4MV, sizeof(__pyx_k_4MV), 0, 0, 1, 0},
   {&__pyx_kp_s_4_MV_per_MB_allowed_advanced_pre, __pyx_k_4_MV_per_MB_allowed_advanced_pre, sizeof(__pyx_k_4_MV_per_MB_allowed_advanced_pre), 0, 0, 1, 0},
   {&__pyx_n_s_AC_PRED, __pyx_k_AC_PRED, sizeof(__pyx_k_AC_PRED), 0, 0, 1, 1},
   {&__pyx_n_s_ALL, __pyx_k_ALL, sizeof(__pyx_k_ALL), 0, 0, 1, 1},
   {&__pyx_n_s_AUTO, __pyx_k_AUTO, sizeof(__pyx_k_AUTO), 0, 0, 1, 1},
+  {&__pyx_n_s_AVDeprecationWarning, __pyx_k_AVDeprecationWarning, sizeof(__pyx_k_AVDeprecationWarning), 0, 0, 1, 1},
   {&__pyx_kp_s_Allow_decoders_to_produce_frames, __pyx_k_Allow_decoders_to_produce_frames, sizeof(__pyx_k_Allow_decoders_to_produce_frames), 0, 0, 1, 0},
   {&__pyx_kp_s_Allow_non_spec_compliant_speedup, __pyx_k_Allow_non_spec_compliant_speedup, sizeof(__pyx_k_Allow_non_spec_compliant_speedup), 0, 0, 1, 0},
   {&__pyx_n_s_AudioCodecContext, __pyx_k_AudioCodecContext, sizeof(__pyx_k_AudioCodecContext), 0, 0, 1, 1},
   {&__pyx_n_s_BIDIR, __pyx_k_BIDIR, sizeof(__pyx_k_BIDIR), 0, 0, 1, 1},
   {&__pyx_n_s_BITEXACT, __pyx_k_BITEXACT, sizeof(__pyx_k_BITEXACT), 0, 0, 1, 1},
   {&__pyx_kp_s_Base_CodecContext_cannot_decode, __pyx_k_Base_CodecContext_cannot_decode, sizeof(__pyx_k_Base_CodecContext_cannot_decode), 0, 0, 1, 0},
   {&__pyx_n_s_CHUNKS, __pyx_k_CHUNKS, sizeof(__pyx_k_CHUNKS), 0, 0, 1, 1},
@@ -9745,22 +9984,24 @@
   {&__pyx_n_s_UNALIGNED, __pyx_k_UNALIGNED, sizeof(__pyx_k_UNALIGNED), 0, 0, 1, 1},
   {&__pyx_kp_s_Use_fixed_qscale, __pyx_k_Use_fixed_qscale, sizeof(__pyx_k_Use_fixed_qscale), 0, 0, 1, 0},
   {&__pyx_kp_s_Use_interlaced_DCT, __pyx_k_Use_interlaced_DCT, sizeof(__pyx_k_Use_interlaced_DCT), 0, 0, 1, 0},
   {&__pyx_kp_s_Use_internal_2pass_ratecontrol_i, __pyx_k_Use_internal_2pass_ratecontrol_i, sizeof(__pyx_k_Use_internal_2pass_ratecontrol_i), 0, 0, 1, 0},
   {&__pyx_kp_s_Use_internal_2pass_ratecontrol_i_2, __pyx_k_Use_internal_2pass_ratecontrol_i_2, sizeof(__pyx_k_Use_internal_2pass_ratecontrol_i_2), 0, 0, 1, 0},
   {&__pyx_kp_s_Use_only_bitexact_stuff_except_I, __pyx_k_Use_only_bitexact_stuff_except_I, sizeof(__pyx_k_Use_only_bitexact_stuff_except_I), 0, 0, 1, 0},
   {&__pyx_kp_s_Use_qpel_MC, __pyx_k_Use_qpel_MC, sizeof(__pyx_k_Use_qpel_MC), 0, 0, 1, 0},
+  {&__pyx_kp_s_Using_CodecContext_time_base_for, __pyx_k_Using_CodecContext_time_base_for, sizeof(__pyx_k_Using_CodecContext_time_base_for), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_VideoCodecContext, __pyx_k_VideoCodecContext, sizeof(__pyx_k_VideoCodecContext), 0, 0, 1, 1},
   {&__pyx_kp_s_Wrapping_CodecContext_with_misma, __pyx_k_Wrapping_CodecContext_with_misma, sizeof(__pyx_k_Wrapping_CodecContext_with_misma), 0, 0, 1, 0},
   {&__pyx_n_s_ac_pred, __pyx_k_ac_pred, sizeof(__pyx_k_ac_pred), 0, 0, 1, 1},
   {&__pyx_n_s_ascii, __pyx_k_ascii, sizeof(__pyx_k_ascii), 0, 0, 1, 1},
   {&__pyx_n_s_av_audio_codeccontext, __pyx_k_av_audio_codeccontext, sizeof(__pyx_k_av_audio_codeccontext), 0, 0, 1, 1},
   {&__pyx_n_s_av_codec_context, __pyx_k_av_codec_context, sizeof(__pyx_k_av_codec_context), 0, 0, 1, 1},
   {&__pyx_kp_s_av_codec_context_pyx, __pyx_k_av_codec_context_pyx, sizeof(__pyx_k_av_codec_context_pyx), 0, 0, 1, 0},
+  {&__pyx_n_s_av_deprecation, __pyx_k_av_deprecation, sizeof(__pyx_k_av_deprecation), 0, 0, 1, 1},
   {&__pyx_n_s_av_dictionary, __pyx_k_av_dictionary, sizeof(__pyx_k_av_dictionary), 0, 0, 1, 1},
   {&__pyx_kp_s_av_s_s_s_at_0x_x, __pyx_k_av_s_s_s_at_0x_x, sizeof(__pyx_k_av_s_s_s_at_0x_x), 0, 0, 1, 0},
   {&__pyx_n_s_av_subtitles_codeccontext, __pyx_k_av_subtitles_codeccontext, sizeof(__pyx_k_av_subtitles_codeccontext), 0, 0, 1, 1},
   {&__pyx_n_s_av_video_codeccontext, __pyx_k_av_video_codeccontext, sizeof(__pyx_k_av_video_codeccontext), 0, 0, 1, 1},
   {&__pyx_n_s_bitexact, __pyx_k_bitexact, sizeof(__pyx_k_bitexact), 0, 0, 1, 1},
   {&__pyx_n_s_byteorder, __pyx_k_byteorder, sizeof(__pyx_k_byteorder), 0, 0, 1, 1},
   {&__pyx_n_s_c_ctx, __pyx_k_c_ctx, sizeof(__pyx_k_c_ctx), 0, 0, 1, 1},
@@ -9796,14 +10037,15 @@
   {&__pyx_n_s_gray, __pyx_k_gray, sizeof(__pyx_k_gray), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_ignore_crop, __pyx_k_ignore_crop, sizeof(__pyx_k_ignore_crop), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_interlaced_dct, __pyx_k_interlaced_dct, sizeof(__pyx_k_interlaced_dct), 0, 0, 1, 1},
   {&__pyx_n_s_interlaced_me, __pyx_k_interlaced_me, sizeof(__pyx_k_interlaced_me), 0, 0, 1, 1},
   {&__pyx_n_s_is_decoder, __pyx_k_is_decoder, sizeof(__pyx_k_is_decoder), 0, 0, 1, 1},
+  {&__pyx_n_s_is_encoder, __pyx_k_is_encoder, sizeof(__pyx_k_is_encoder), 0, 0, 1, 1},
   {&__pyx_n_s_little, __pyx_k_little, sizeof(__pyx_k_little), 0, 0, 1, 1},
   {&__pyx_n_s_local_header, __pyx_k_local_header, sizeof(__pyx_k_local_header), 0, 0, 1, 1},
   {&__pyx_kp_s_loop_filter, __pyx_k_loop_filter, sizeof(__pyx_k_loop_filter), 0, 0, 1, 0},
   {&__pyx_n_s_loop_filter_2, __pyx_k_loop_filter_2, sizeof(__pyx_k_loop_filter_2), 0, 0, 1, 1},
   {&__pyx_n_s_low_delay, __pyx_k_low_delay, sizeof(__pyx_k_low_delay), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
@@ -9842,174 +10084,176 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_to_bytes, __pyx_k_to_bytes, sizeof(__pyx_k_to_bytes), 0, 0, 1, 1},
   {&__pyx_n_s_truncated, __pyx_k_truncated, sizeof(__pyx_k_truncated), 0, 0, 1, 1},
   {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
   {&__pyx_n_s_unaligned, __pyx_k_unaligned, sizeof(__pyx_k_unaligned), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+  {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
+  {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 143, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 151, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 237, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 246, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(0, 318, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 440, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(0, 321, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 443, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "av/codec/context.pyx":151
+  /* "av/codec/context.pyx":154
  *     def __cinit__(self, sentinel=None, *args, **kwargs):
  *         if sentinel is not _cinit_sentinel:
  *             raise RuntimeError('Cannot instantiate CodecContext')             # <<<<<<<<<<<<<<
  * 
  *         self.options = {}
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Cannot_instantiate_CodecContext); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Cannot_instantiate_CodecContext); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "av/codec/context.pyx":160
+  /* "av/codec/context.pyx":163
  *         self.ptr = ptr
  *         if self.ptr.codec and codec and self.ptr.codec != codec:
  *             raise RuntimeError('Wrapping CodecContext with mismatched codec.')             # <<<<<<<<<<<<<<
  *         self.codec = wrap_codec(codec if codec != NULL else self.ptr.codec)
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_Wrapping_CodecContext_with_misma); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_Wrapping_CodecContext_with_misma); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "av/codec/context.pyx":237
+  /* "av/codec/context.pyx":240
  *         def __set__(self, data):
  *             if not self.is_decoder:
  *                 raise ValueError("Can only set extradata for decoders.")             # <<<<<<<<<<<<<<
  * 
  *             if data is None:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Can_only_set_extradata_for_decod); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Can_only_set_extradata_for_decod); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "av/codec/context.pyx":246
+  /* "av/codec/context.pyx":249
  *                 self.ptr.extradata = <uint8_t*>lib.av_realloc(self.ptr.extradata, source.length + lib.AV_INPUT_BUFFER_PADDING_SIZE)
  *                 if not self.ptr.extradata:
  *                     raise MemoryError("Cannot allocate extradata")             # <<<<<<<<<<<<<<
  *                 memcpy(self.ptr.extradata, source.ptr, source.length)
  *                 self.ptr.extradata_size = source.length
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Cannot_allocate_extradata); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Cannot_allocate_extradata); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "av/codec/context.pyx":271
+  /* "av/codec/context.pyx":274
  *         if lib.avcodec_is_open(self.ptr):
  *             if strict:
  *                 raise ValueError('CodecContext is already open.')             # <<<<<<<<<<<<<<
  *             return
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_CodecContext_is_already_open); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_CodecContext_is_already_open); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "av/codec/context.pyx":300
+  /* "av/codec/context.pyx":303
  *         if not lib.avcodec_is_open(self.ptr):
  *             if strict:
  *                 raise ValueError('CodecContext is already closed.')             # <<<<<<<<<<<<<<
  *             return
  *         err_check(lib.avcodec_close(self.ptr))
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_CodecContext_is_already_closed); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_CodecContext_is_already_closed); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "av/codec/context.pyx":440
+  /* "av/codec/context.pyx":443
  * 
  *     cdef Frame _alloc_next_frame(self):
  *         raise NotImplementedError('Base CodecContext cannot decode.')             # <<<<<<<<<<<<<<
  * 
  *     cdef _recv_frame(self):
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Base_CodecContext_cannot_decode); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Base_CodecContext_cannot_decode); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "av/codec/context.pyx":478
+  /* "av/codec/context.pyx":481
  * 
  *         if self.ptr.codec_type not in [lib.AVMEDIA_TYPE_VIDEO, lib.AVMEDIA_TYPE_AUDIO]:
  *             raise NotImplementedError('Encoding is only supported for audio and video.')             # <<<<<<<<<<<<<<
  * 
  *         self.open(strict=False)
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Encoding_is_only_supported_for_a); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Encoding_is_only_supported_for_a); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 481, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "av/codec/context.pyx":517
+  /* "av/codec/context.pyx":520
  * 
  *         if not self.codec.ptr:
  *             raise ValueError('cannot decode unknown codec')             # <<<<<<<<<<<<<<
  * 
  *         self.open(strict=False)
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_cannot_decode_unknown_codec); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 517, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_cannot_decode_unknown_codec); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 520, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "av/codec/context.pyx":561
+  /* "av/codec/context.pyx":574
  *     property codec_tag:
  *         def __get__(self):
  *             return self.ptr.codec_tag.to_bytes(4, byteorder="little", signed=False).decode(             # <<<<<<<<<<<<<<
  *                 encoding="ascii")
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_int_4); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_int_4); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "av/codec/context.pyx":569
+  /* "av/codec/context.pyx":582
  *                                                     byteorder="little", signed=False)
  *             else:
  *                 raise ValueError("Codec tag should be a 4 character string.")             # <<<<<<<<<<<<<<
  * 
  *     property ticks_per_frame:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Codec_tag_should_be_a_4_characte); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Codec_tag_should_be_a_4_characte); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 582, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "av/codec/context.pyx":608
+  /* "av/codec/context.pyx":621
  *         def __set__(self, int value):
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_count after codec is open.")             # <<<<<<<<<<<<<<
  *             self.ptr.thread_count = value
  * 
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_change_thread_count_after); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 608, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_change_thread_count_after); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "av/codec/context.pyx":623
+  /* "av/codec/context.pyx":636
  *         def __set__(self, value):
  *             if lib.avcodec_is_open(self.ptr):
  *                 raise RuntimeError("Cannot change thread_type after codec is open.")             # <<<<<<<<<<<<<<
  *             self.ptr.thread_type = ThreadType[value].value
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Cannot_change_thread_type_after); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Cannot_change_thread_type_after); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 636, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -10024,47 +10268,47 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "av/codec/context.pyx":45
+  /* "av/codec/context.pyx":48
  * 
  * ThreadType = define_enum('ThreadType', __name__, (
  *     ('NONE', 0),             # <<<<<<<<<<<<<<
  *     ('FRAME', lib.FF_THREAD_FRAME,
  *         """Decode more than one frame at once"""),
  */
-  __pyx_tuple__16 = PyTuple_Pack(2, __pyx_n_s_NONE, __pyx_int_0); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(2, __pyx_n_s_NONE, __pyx_int_0); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "av/codec/context.pyx":84
+  /* "av/codec/context.pyx":87
  *     ('QPEL', lib.AV_CODEC_FLAG_QPEL,
  *         """Use qpel MC."""),
  *     ('DROPCHANGED', 1 << 5,             # <<<<<<<<<<<<<<
  *         """Don't output frames whose parameters differ from first
  *         decoded frame in stream."""),
  */
-  __pyx_tuple__17 = PyTuple_Pack(3, __pyx_n_s_DROPCHANGED, __pyx_int_32, __pyx_kp_s_Don_t_output_frames_whose_parame); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(3, __pyx_n_s_DROPCHANGED, __pyx_int_32, __pyx_kp_s_Don_t_output_frames_whose_parame); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "av/codec/context.pyx":144
+  /* "av/codec/context.pyx":147
  * 
  *     @staticmethod
  *     def create(codec, mode=None):             # <<<<<<<<<<<<<<
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)
  */
-  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_codec, __pyx_n_s_mode, __pyx_n_s_cy_codec, __pyx_n_s_c_ctx); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_codec, __pyx_n_s_mode, __pyx_n_s_cy_codec, __pyx_n_s_c_ctx); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_av_codec_context_pyx, __pyx_n_s_create, 144, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_av_codec_context_pyx, __pyx_n_s_create, 147, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -10136,24 +10380,24 @@
   __pyx_vtable_2av_5codec_7context_CodecContext._setup_encoded_packet = (PyObject *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *, struct __pyx_obj_2av_6packet_Packet *))__pyx_f_2av_5codec_7context_12CodecContext__setup_encoded_packet;
   __pyx_vtable_2av_5codec_7context_CodecContext._setup_decoded_frame = (PyObject *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *, struct __pyx_obj_2av_5frame_Frame *, struct __pyx_obj_2av_6packet_Packet *))__pyx_f_2av_5codec_7context_12CodecContext__setup_decoded_frame;
   __pyx_vtable_2av_5codec_7context_CodecContext._send_frame_and_recv = (PyObject *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *, struct __pyx_obj_2av_5frame_Frame *))__pyx_f_2av_5codec_7context_12CodecContext__send_frame_and_recv;
   __pyx_vtable_2av_5codec_7context_CodecContext._recv_packet = (PyObject *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *))__pyx_f_2av_5codec_7context_12CodecContext__recv_packet;
   __pyx_vtable_2av_5codec_7context_CodecContext._send_packet_and_recv = (PyObject *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *, struct __pyx_obj_2av_6packet_Packet *))__pyx_f_2av_5codec_7context_12CodecContext__send_packet_and_recv;
   __pyx_vtable_2av_5codec_7context_CodecContext._recv_frame = (PyObject *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *))__pyx_f_2av_5codec_7context_12CodecContext__recv_frame;
   __pyx_vtable_2av_5codec_7context_CodecContext._alloc_next_frame = (struct __pyx_obj_2av_5frame_Frame *(*)(struct __pyx_obj_2av_5codec_7context_CodecContext *))__pyx_f_2av_5codec_7context_12CodecContext__alloc_next_frame;
-  if (PyType_Ready(&__pyx_type_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_5codec_7context_CodecContext.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_5codec_7context_CodecContext.tp_dictoffset && __pyx_type_2av_5codec_7context_CodecContext.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_5codec_7context_CodecContext.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2av_5codec_7context_CodecContext.tp_dict, __pyx_vtabptr_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CodecContext, (PyObject *)&__pyx_type_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2av_5codec_7context_CodecContext.tp_dict, __pyx_vtabptr_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CodecContext, (PyObject *)&__pyx_type_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_5codec_7context_CodecContext) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __pyx_ptype_2av_5codec_7context_CodecContext = &__pyx_type_2av_5codec_7context_CodecContext;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -10511,1172 +10755,1203 @@
   (void)__Pyx_modinit_variable_import_code();
   if (unlikely(__Pyx_modinit_function_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "av/codec/context.pyx":14
- * from av.utils cimport avrational_to_fraction, to_avrational
+  /* "av/codec/context.pyx":1
+ * import warnings             # <<<<<<<<<<<<<<
  * 
- * from av.dictionary import Dictionary             # <<<<<<<<<<<<<<
+ * from libc.errno cimport EAGAIN
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "av/codec/context.pyx":16
+ * from av.utils cimport avrational_to_fraction, to_avrational
  * 
+ * from av.deprecation import AVDeprecationWarning             # <<<<<<<<<<<<<<
+ * from av.dictionary import Dictionary
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_Dictionary);
-  __Pyx_GIVEREF(__pyx_n_s_Dictionary);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Dictionary);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_dictionary, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_AVDeprecationWarning);
+  __Pyx_GIVEREF(__pyx_n_s_AVDeprecationWarning);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_AVDeprecationWarning);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_deprecation, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_AVDeprecationWarning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dictionary, __pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AVDeprecationWarning, __pyx_t_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "av/codec/context.pyx":17
  * 
+ * from av.deprecation import AVDeprecationWarning
+ * from av.dictionary import Dictionary             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_n_s_Dictionary);
+  __Pyx_GIVEREF(__pyx_n_s_Dictionary);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Dictionary);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_av_dictionary, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dictionary, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "av/codec/context.pyx":20
+ * 
  * 
  * cdef object _cinit_sentinel = object()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_builtin_object); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(__pyx_v_2av_5codec_7context__cinit_sentinel);
-  __Pyx_DECREF_SET(__pyx_v_2av_5codec_7context__cinit_sentinel, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(__pyx_v_2av_5codec_7context__cinit_sentinel, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "av/codec/context.pyx":44
+  /* "av/codec/context.pyx":47
  * 
  * 
  * ThreadType = define_enum('ThreadType', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', 0),
  *     ('FRAME', lib.FF_THREAD_FRAME,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "av/codec/context.pyx":46
+  /* "av/codec/context.pyx":49
  * ThreadType = define_enum('ThreadType', __name__, (
  *     ('NONE', 0),
  *     ('FRAME', lib.FF_THREAD_FRAME,             # <<<<<<<<<<<<<<
  *         """Decode more than one frame at once"""),
  *     ('SLICE', lib.FF_THREAD_SLICE,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(FF_THREAD_FRAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(FF_THREAD_FRAME); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_FRAME);
   __Pyx_GIVEREF(__pyx_n_s_FRAME);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_FRAME);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Decode_more_than_one_frame_at_on);
   __Pyx_GIVEREF(__pyx_kp_s_Decode_more_than_one_frame_at_on);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_s_Decode_more_than_one_frame_at_on);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":48
+  /* "av/codec/context.pyx":51
  *     ('FRAME', lib.FF_THREAD_FRAME,
  *         """Decode more than one frame at once"""),
  *     ('SLICE', lib.FF_THREAD_SLICE,             # <<<<<<<<<<<<<<
  *         """Decode more than one part of a single frame at once"""),
  *     ('AUTO', lib.FF_THREAD_SLICE | lib.FF_THREAD_FRAME,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(FF_THREAD_SLICE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(FF_THREAD_SLICE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_SLICE);
   __Pyx_GIVEREF(__pyx_n_s_SLICE);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_SLICE);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Decode_more_than_one_part_of_a_s);
   __Pyx_GIVEREF(__pyx_kp_s_Decode_more_than_one_part_of_a_s);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_s_Decode_more_than_one_part_of_a_s);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":50
+  /* "av/codec/context.pyx":53
  *     ('SLICE', lib.FF_THREAD_SLICE,
  *         """Decode more than one part of a single frame at once"""),
  *     ('AUTO', lib.FF_THREAD_SLICE | lib.FF_THREAD_FRAME,             # <<<<<<<<<<<<<<
  *         """Decode using both FRAME and SLICE methods."""),
  * ), is_flags=True)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int((FF_THREAD_SLICE | FF_THREAD_FRAME)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int((FF_THREAD_SLICE | FF_THREAD_FRAME)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_AUTO);
   __Pyx_GIVEREF(__pyx_n_s_AUTO);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_AUTO);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Decode_using_both_FRAME_and_SLIC);
   __Pyx_GIVEREF(__pyx_kp_s_Decode_using_both_FRAME_and_SLIC);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_s_Decode_using_both_FRAME_and_SLIC);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":45
+  /* "av/codec/context.pyx":48
  * 
  * ThreadType = define_enum('ThreadType', __name__, (
  *     ('NONE', 0),             # <<<<<<<<<<<<<<
  *     ('FRAME', lib.FF_THREAD_FRAME,
  *         """Decode more than one frame at once"""),
  */
-  __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_tuple__16);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_5);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
 
-  /* "av/codec/context.pyx":44
+  /* "av/codec/context.pyx":47
  * 
  * 
  * ThreadType = define_enum('ThreadType', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', 0),
  *     ('FRAME', lib.FF_THREAD_FRAME,
  */
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.is_flags = 1;
-  __pyx_t_5 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_ThreadType, __pyx_t_2, __pyx_t_1, 0, &__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_ThreadType, __pyx_t_1, __pyx_t_2, 0, &__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ThreadType, __pyx_t_5) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ThreadType, __pyx_t_5) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "av/codec/context.pyx":54
+  /* "av/codec/context.pyx":57
  * ), is_flags=True)
  * 
  * SkipType = define_enum('SkipType', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', lib.AVDISCARD_NONE,
  *         """Discard nothing"""),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "av/codec/context.pyx":55
+  /* "av/codec/context.pyx":58
  * 
  * SkipType = define_enum('SkipType', __name__, (
  *     ('NONE', lib.AVDISCARD_NONE,             # <<<<<<<<<<<<<<
  *         """Discard nothing"""),
  *     ('DEFAULT', lib.AVDISCARD_DEFAULT,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_NONE);
   __Pyx_GIVEREF(__pyx_n_s_NONE);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_NONE);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_NONE);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_nothing);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_nothing);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_s_Discard_nothing);
-  __pyx_t_1 = 0;
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_s_Discard_nothing);
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":57
+  /* "av/codec/context.pyx":60
  *     ('NONE', lib.AVDISCARD_NONE,
  *         """Discard nothing"""),
  *     ('DEFAULT', lib.AVDISCARD_DEFAULT,             # <<<<<<<<<<<<<<
  *         """Discard useless packets like 0 size packets in AVI"""),
  *     ('NONREF', lib.AVDISCARD_NONREF,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_DEFAULT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_DEFAULT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_DEFAULT);
   __Pyx_GIVEREF(__pyx_n_s_DEFAULT);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_DEFAULT);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_useless_packets_like_0_s);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_useless_packets_like_0_s);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_s_Discard_useless_packets_like_0_s);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":59
+  /* "av/codec/context.pyx":62
  *     ('DEFAULT', lib.AVDISCARD_DEFAULT,
  *         """Discard useless packets like 0 size packets in AVI"""),
  *     ('NONREF', lib.AVDISCARD_NONREF,             # <<<<<<<<<<<<<<
  *         """Discard all non reference"""),
  *     ('BIDIR', lib.AVDISCARD_BIDIR,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONREF); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONREF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_NONREF);
   __Pyx_GIVEREF(__pyx_n_s_NONREF);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_NONREF);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_all_non_reference);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_all_non_reference);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_s_Discard_all_non_reference);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":61
+  /* "av/codec/context.pyx":64
  *     ('NONREF', lib.AVDISCARD_NONREF,
  *         """Discard all non reference"""),
  *     ('BIDIR', lib.AVDISCARD_BIDIR,             # <<<<<<<<<<<<<<
  *         """Discard all bidirectional frames"""),
  *     ('NONINTRA', lib.AVDISCARD_NONINTRA,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_BIDIR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_BIDIR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_n_s_BIDIR);
   __Pyx_GIVEREF(__pyx_n_s_BIDIR);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_BIDIR);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_all_bidirectional_frames);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_all_bidirectional_frames);
   PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_kp_s_Discard_all_bidirectional_frames);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":63
+  /* "av/codec/context.pyx":66
  *     ('BIDIR', lib.AVDISCARD_BIDIR,
  *         """Discard all bidirectional frames"""),
  *     ('NONINTRA', lib.AVDISCARD_NONINTRA,             # <<<<<<<<<<<<<<
  *         """Discard all non intra frames"""),
  *     ('NONKEY', lib.AVDISCARD_NONKEY,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONINTRA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONINTRA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_n_s_NONINTRA);
   __Pyx_GIVEREF(__pyx_n_s_NONINTRA);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_n_s_NONINTRA);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_all_non_intra_frames);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_all_non_intra_frames);
   PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_s_Discard_all_non_intra_frames);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":65
+  /* "av/codec/context.pyx":68
  *     ('NONINTRA', lib.AVDISCARD_NONINTRA,
  *         """Discard all non intra frames"""),
  *     ('NONKEY', lib.AVDISCARD_NONKEY,             # <<<<<<<<<<<<<<
  *         """Discard all frames except keyframes"""),
  *     ('ALL', lib.AVDISCARD_ALL,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONKEY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_NONKEY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_n_s_NONKEY);
   __Pyx_GIVEREF(__pyx_n_s_NONKEY);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_n_s_NONKEY);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_all_frames_except_keyfra);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_all_frames_except_keyfra);
   PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_kp_s_Discard_all_frames_except_keyfra);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":67
+  /* "av/codec/context.pyx":70
  *     ('NONKEY', lib.AVDISCARD_NONKEY,
  *         """Discard all frames except keyframes"""),
  *     ('ALL', lib.AVDISCARD_ALL,             # <<<<<<<<<<<<<<
  *         """Discard all"""),
  * ))
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_ALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVDiscard(AVDISCARD_ALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_n_s_ALL);
   __Pyx_GIVEREF(__pyx_n_s_ALL);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_n_s_ALL);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_all);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_all);
   PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_kp_s_Discard_all);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":55
+  /* "av/codec/context.pyx":58
  * 
  * SkipType = define_enum('SkipType', __name__, (
  *     ('NONE', lib.AVDISCARD_NONE,             # <<<<<<<<<<<<<<
  *         """Discard nothing"""),
  *     ('DEFAULT', lib.AVDISCARD_DEFAULT,
  */
-  __pyx_t_1 = PyTuple_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
+  __pyx_t_2 = PyTuple_New(7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_t_10);
-  __pyx_t_2 = 0;
+  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_t_10);
+  __pyx_t_1 = 0;
   __pyx_t_4 = 0;
   __pyx_t_3 = 0;
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
 
-  /* "av/codec/context.pyx":54
+  /* "av/codec/context.pyx":57
  * ), is_flags=True)
  * 
  * SkipType = define_enum('SkipType', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', lib.AVDISCARD_NONE,
  *         """Discard nothing"""),
  */
-  __pyx_t_10 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_SkipType, __pyx_t_5, __pyx_t_1, 0, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_10 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_SkipType, __pyx_t_5, __pyx_t_2, 0, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SkipType, __pyx_t_10) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SkipType, __pyx_t_10) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "av/codec/context.pyx":71
+  /* "av/codec/context.pyx":74
  * ))
  * 
  * Flags = define_enum('Flags', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', 0),
  *     ('UNALIGNED', lib.AV_CODEC_FLAG_UNALIGNED,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
 
-  /* "av/codec/context.pyx":73
+  /* "av/codec/context.pyx":76
  * Flags = define_enum('Flags', __name__, (
  *     ('NONE', 0),
  *     ('UNALIGNED', lib.AV_CODEC_FLAG_UNALIGNED,             # <<<<<<<<<<<<<<
  *         """Allow decoders to produce frames with data planes that are not aligned
  *         to CPU requirements (e.g. due to cropping)."""),
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_UNALIGNED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_UNALIGNED); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_UNALIGNED);
   __Pyx_GIVEREF(__pyx_n_s_UNALIGNED);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_UNALIGNED);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Allow_decoders_to_produce_frames);
   __Pyx_GIVEREF(__pyx_kp_s_Allow_decoders_to_produce_frames);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_s_Allow_decoders_to_produce_frames);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":76
+  /* "av/codec/context.pyx":79
  *         """Allow decoders to produce frames with data planes that are not aligned
  *         to CPU requirements (e.g. due to cropping)."""),
  *     ('QSCALE', lib.AV_CODEC_FLAG_QSCALE,             # <<<<<<<<<<<<<<
  *         """Use fixed qscale."""),
  *     ('4MV', lib.AV_CODEC_FLAG_4MV,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_QSCALE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_QSCALE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_n_s_QSCALE);
   __Pyx_GIVEREF(__pyx_n_s_QSCALE);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_n_s_QSCALE);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Use_fixed_qscale);
   __Pyx_GIVEREF(__pyx_kp_s_Use_fixed_qscale);
   PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_kp_s_Use_fixed_qscale);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":78
+  /* "av/codec/context.pyx":81
  *     ('QSCALE', lib.AV_CODEC_FLAG_QSCALE,
  *         """Use fixed qscale."""),
  *     ('4MV', lib.AV_CODEC_FLAG_4MV,             # <<<<<<<<<<<<<<
  *         """4 MV per MB allowed / advanced prediction for H.263."""),
  *     ('OUTPUT_CORRUPT', lib.AV_CODEC_FLAG_OUTPUT_CORRUPT,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_4MV); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_4MV); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_kp_s_4MV);
   __Pyx_GIVEREF(__pyx_kp_s_4MV);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_s_4MV);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_4_MV_per_MB_allowed_advanced_pre);
   __Pyx_GIVEREF(__pyx_kp_s_4_MV_per_MB_allowed_advanced_pre);
   PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_s_4_MV_per_MB_allowed_advanced_pre);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":80
+  /* "av/codec/context.pyx":83
  *     ('4MV', lib.AV_CODEC_FLAG_4MV,
  *         """4 MV per MB allowed / advanced prediction for H.263."""),
  *     ('OUTPUT_CORRUPT', lib.AV_CODEC_FLAG_OUTPUT_CORRUPT,             # <<<<<<<<<<<<<<
  *         """Output even those frames that might be corrupted."""),
  *     ('QPEL', lib.AV_CODEC_FLAG_QPEL,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_OUTPUT_CORRUPT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_OUTPUT_CORRUPT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_n_s_OUTPUT_CORRUPT);
   __Pyx_GIVEREF(__pyx_n_s_OUTPUT_CORRUPT);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_OUTPUT_CORRUPT);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Output_even_those_frames_that_mi);
   __Pyx_GIVEREF(__pyx_kp_s_Output_even_those_frames_that_mi);
   PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_kp_s_Output_even_those_frames_that_mi);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":82
+  /* "av/codec/context.pyx":85
  *     ('OUTPUT_CORRUPT', lib.AV_CODEC_FLAG_OUTPUT_CORRUPT,
  *         """Output even those frames that might be corrupted."""),
  *     ('QPEL', lib.AV_CODEC_FLAG_QPEL,             # <<<<<<<<<<<<<<
  *         """Use qpel MC."""),
  *     ('DROPCHANGED', 1 << 5,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_QPEL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_QPEL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_QPEL);
   __Pyx_GIVEREF(__pyx_n_s_QPEL);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_QPEL);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Use_qpel_MC);
   __Pyx_GIVEREF(__pyx_kp_s_Use_qpel_MC);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_s_Use_qpel_MC);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":87
+  /* "av/codec/context.pyx":90
  *         """Don't output frames whose parameters differ from first
  *         decoded frame in stream."""),
  *     ('PASS1', lib.AV_CODEC_FLAG_PASS1,             # <<<<<<<<<<<<<<
  *         """Use internal 2pass ratecontrol in first pass mode."""),
  *     ('PASS2', lib.AV_CODEC_FLAG_PASS2,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_PASS1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_PASS1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_PASS1);
   __Pyx_GIVEREF(__pyx_n_s_PASS1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_PASS1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Use_internal_2pass_ratecontrol_i);
   __Pyx_GIVEREF(__pyx_kp_s_Use_internal_2pass_ratecontrol_i);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_s_Use_internal_2pass_ratecontrol_i);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":89
+  /* "av/codec/context.pyx":92
  *     ('PASS1', lib.AV_CODEC_FLAG_PASS1,
  *         """Use internal 2pass ratecontrol in first pass mode."""),
  *     ('PASS2', lib.AV_CODEC_FLAG_PASS2,             # <<<<<<<<<<<<<<
  *         """Use internal 2pass ratecontrol in second pass mode."""),
  *     ('LOOP_FILTER', lib.AV_CODEC_FLAG_LOOP_FILTER,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_PASS2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_PASS2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_PASS2);
   __Pyx_GIVEREF(__pyx_n_s_PASS2);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PASS2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PASS2);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Use_internal_2pass_ratecontrol_i_2);
   __Pyx_GIVEREF(__pyx_kp_s_Use_internal_2pass_ratecontrol_i_2);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_s_Use_internal_2pass_ratecontrol_i_2);
-  __pyx_t_1 = 0;
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_s_Use_internal_2pass_ratecontrol_i_2);
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":91
+  /* "av/codec/context.pyx":94
  *     ('PASS2', lib.AV_CODEC_FLAG_PASS2,
  *         """Use internal 2pass ratecontrol in second pass mode."""),
  *     ('LOOP_FILTER', lib.AV_CODEC_FLAG_LOOP_FILTER,             # <<<<<<<<<<<<<<
  *         """loop filter."""),
  *     ('GRAY', lib.AV_CODEC_FLAG_GRAY,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_LOOP_FILTER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_LOOP_FILTER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_INCREF(__pyx_n_s_LOOP_FILTER);
   __Pyx_GIVEREF(__pyx_n_s_LOOP_FILTER);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_n_s_LOOP_FILTER);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_loop_filter);
   __Pyx_GIVEREF(__pyx_kp_s_loop_filter);
   PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_s_loop_filter);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":93
+  /* "av/codec/context.pyx":96
  *     ('LOOP_FILTER', lib.AV_CODEC_FLAG_LOOP_FILTER,
  *         """loop filter."""),
  *     ('GRAY', lib.AV_CODEC_FLAG_GRAY,             # <<<<<<<<<<<<<<
  *         """Only decode/encode grayscale."""),
  *     ('PSNR', lib.AV_CODEC_FLAG_PSNR,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_GRAY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_GRAY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_INCREF(__pyx_n_s_GRAY);
   __Pyx_GIVEREF(__pyx_n_s_GRAY);
   PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_n_s_GRAY);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Only_decode_encode_grayscale);
   __Pyx_GIVEREF(__pyx_kp_s_Only_decode_encode_grayscale);
   PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_s_Only_decode_encode_grayscale);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":95
+  /* "av/codec/context.pyx":98
  *     ('GRAY', lib.AV_CODEC_FLAG_GRAY,
  *         """Only decode/encode grayscale."""),
  *     ('PSNR', lib.AV_CODEC_FLAG_PSNR,             # <<<<<<<<<<<<<<
  *         """error[?] variables will be set during encoding."""),
  *     ('TRUNCATED', lib.AV_CODEC_FLAG_TRUNCATED,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_PSNR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_13 = PyTuple_New(3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_PSNR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_13 = PyTuple_New(3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_n_s_PSNR);
   __Pyx_GIVEREF(__pyx_n_s_PSNR);
   PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_n_s_PSNR);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_error_variables_will_be_set_duri);
   __Pyx_GIVEREF(__pyx_kp_s_error_variables_will_be_set_duri);
   PyTuple_SET_ITEM(__pyx_t_13, 2, __pyx_kp_s_error_variables_will_be_set_duri);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":97
+  /* "av/codec/context.pyx":100
  *     ('PSNR', lib.AV_CODEC_FLAG_PSNR,
  *         """error[?] variables will be set during encoding."""),
  *     ('TRUNCATED', lib.AV_CODEC_FLAG_TRUNCATED,             # <<<<<<<<<<<<<<
  *         """Input bitstream might be truncated at a random location
  *         instead of only at frame boundaries."""),
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_TRUNCATED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_TRUNCATED); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_INCREF(__pyx_n_s_TRUNCATED);
   __Pyx_GIVEREF(__pyx_n_s_TRUNCATED);
   PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_n_s_TRUNCATED);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Input_bitstream_might_be_truncat);
   __Pyx_GIVEREF(__pyx_kp_s_Input_bitstream_might_be_truncat);
   PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_s_Input_bitstream_might_be_truncat);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":100
+  /* "av/codec/context.pyx":103
  *         """Input bitstream might be truncated at a random location
  *         instead of only at frame boundaries."""),
  *     ('INTERLACED_DCT', lib.AV_CODEC_FLAG_INTERLACED_DCT,             # <<<<<<<<<<<<<<
  *         """Use interlaced DCT."""),
  *     ('LOW_DELAY', lib.AV_CODEC_FLAG_LOW_DELAY,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_INTERLACED_DCT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_INTERLACED_DCT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_INCREF(__pyx_n_s_INTERLACED_DCT);
   __Pyx_GIVEREF(__pyx_n_s_INTERLACED_DCT);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_n_s_INTERLACED_DCT);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Use_interlaced_DCT);
   __Pyx_GIVEREF(__pyx_kp_s_Use_interlaced_DCT);
   PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_s_Use_interlaced_DCT);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":102
+  /* "av/codec/context.pyx":105
  *     ('INTERLACED_DCT', lib.AV_CODEC_FLAG_INTERLACED_DCT,
  *         """Use interlaced DCT."""),
  *     ('LOW_DELAY', lib.AV_CODEC_FLAG_LOW_DELAY,             # <<<<<<<<<<<<<<
  *         """Force low delay."""),
  *     ('GLOBAL_HEADER', lib.AV_CODEC_FLAG_GLOBAL_HEADER,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_LOW_DELAY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_LOW_DELAY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_INCREF(__pyx_n_s_LOW_DELAY);
   __Pyx_GIVEREF(__pyx_n_s_LOW_DELAY);
   PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_n_s_LOW_DELAY);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Force_low_delay);
   __Pyx_GIVEREF(__pyx_kp_s_Force_low_delay);
   PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_s_Force_low_delay);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":104
+  /* "av/codec/context.pyx":107
  *     ('LOW_DELAY', lib.AV_CODEC_FLAG_LOW_DELAY,
  *         """Force low delay."""),
  *     ('GLOBAL_HEADER', lib.AV_CODEC_FLAG_GLOBAL_HEADER,             # <<<<<<<<<<<<<<
  *         """Place global headers in extradata instead of every keyframe."""),
  *     ('BITEXACT', lib.AV_CODEC_FLAG_BITEXACT,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_GLOBAL_HEADER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_17 = PyTuple_New(3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_GLOBAL_HEADER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_17 = PyTuple_New(3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_INCREF(__pyx_n_s_GLOBAL_HEADER);
   __Pyx_GIVEREF(__pyx_n_s_GLOBAL_HEADER);
   PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_n_s_GLOBAL_HEADER);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Place_global_headers_in_extradat);
   __Pyx_GIVEREF(__pyx_kp_s_Place_global_headers_in_extradat);
   PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_s_Place_global_headers_in_extradat);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":106
+  /* "av/codec/context.pyx":109
  *     ('GLOBAL_HEADER', lib.AV_CODEC_FLAG_GLOBAL_HEADER,
  *         """Place global headers in extradata instead of every keyframe."""),
  *     ('BITEXACT', lib.AV_CODEC_FLAG_BITEXACT,             # <<<<<<<<<<<<<<
  *         """Use only bitexact stuff (except (I)DCT)."""),
  *     ('AC_PRED', lib.AV_CODEC_FLAG_AC_PRED,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_BITEXACT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_18 = PyTuple_New(3); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_BITEXACT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_18 = PyTuple_New(3); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_n_s_BITEXACT);
   __Pyx_GIVEREF(__pyx_n_s_BITEXACT);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_n_s_BITEXACT);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Use_only_bitexact_stuff_except_I);
   __Pyx_GIVEREF(__pyx_kp_s_Use_only_bitexact_stuff_except_I);
   PyTuple_SET_ITEM(__pyx_t_18, 2, __pyx_kp_s_Use_only_bitexact_stuff_except_I);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":108
+  /* "av/codec/context.pyx":111
  *     ('BITEXACT', lib.AV_CODEC_FLAG_BITEXACT,
  *         """Use only bitexact stuff (except (I)DCT)."""),
  *     ('AC_PRED', lib.AV_CODEC_FLAG_AC_PRED,             # <<<<<<<<<<<<<<
  *         """H.263 advanced intra coding / MPEG-4 AC prediction"""),
  *     ('INTERLACED_ME', lib.AV_CODEC_FLAG_INTERLACED_ME,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_AC_PRED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_AC_PRED); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_19);
   __Pyx_INCREF(__pyx_n_s_AC_PRED);
   __Pyx_GIVEREF(__pyx_n_s_AC_PRED);
   PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_n_s_AC_PRED);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_H_263_advanced_intra_coding_MPEG);
   __Pyx_GIVEREF(__pyx_kp_s_H_263_advanced_intra_coding_MPEG);
   PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_s_H_263_advanced_intra_coding_MPEG);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":110
+  /* "av/codec/context.pyx":113
  *     ('AC_PRED', lib.AV_CODEC_FLAG_AC_PRED,
  *         """H.263 advanced intra coding / MPEG-4 AC prediction"""),
  *     ('INTERLACED_ME', lib.AV_CODEC_FLAG_INTERLACED_ME,             # <<<<<<<<<<<<<<
  *         """Interlaced motion estimation"""),
  *     ('CLOSED_GOP', lib.AV_CODEC_FLAG_CLOSED_GOP),
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_INTERLACED_ME); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_20 = PyTuple_New(3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_INTERLACED_ME); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_20 = PyTuple_New(3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_20);
   __Pyx_INCREF(__pyx_n_s_INTERLACED_ME);
   __Pyx_GIVEREF(__pyx_n_s_INTERLACED_ME);
   PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_n_s_INTERLACED_ME);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Interlaced_motion_estimation);
   __Pyx_GIVEREF(__pyx_kp_s_Interlaced_motion_estimation);
   PyTuple_SET_ITEM(__pyx_t_20, 2, __pyx_kp_s_Interlaced_motion_estimation);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":112
+  /* "av/codec/context.pyx":115
  *     ('INTERLACED_ME', lib.AV_CODEC_FLAG_INTERLACED_ME,
  *         """Interlaced motion estimation"""),
  *     ('CLOSED_GOP', lib.AV_CODEC_FLAG_CLOSED_GOP),             # <<<<<<<<<<<<<<
  * ), is_flags=True)
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_CLOSED_GOP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_21 = PyTuple_New(2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG_CLOSED_GOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_21 = PyTuple_New(2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_INCREF(__pyx_n_s_CLOSED_GOP);
   __Pyx_GIVEREF(__pyx_n_s_CLOSED_GOP);
   PyTuple_SET_ITEM(__pyx_t_21, 0, __pyx_n_s_CLOSED_GOP);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_21, 1, __pyx_t_1);
-  __pyx_t_1 = 0;
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_21, 1, __pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":72
+  /* "av/codec/context.pyx":75
  * 
  * Flags = define_enum('Flags', __name__, (
  *     ('NONE', 0),             # <<<<<<<<<<<<<<
  *     ('UNALIGNED', lib.AV_CODEC_FLAG_UNALIGNED,
  *         """Allow decoders to produce frames with data planes that are not aligned
  */
-  __pyx_t_1 = PyTuple_New(20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_tuple__16);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_3);
   __Pyx_INCREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_tuple__17);
+  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 8, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_1, 9, __pyx_t_11);
+  PyTuple_SET_ITEM(__pyx_t_2, 9, __pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_12);
-  PyTuple_SET_ITEM(__pyx_t_1, 10, __pyx_t_12);
+  PyTuple_SET_ITEM(__pyx_t_2, 10, __pyx_t_12);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_1, 11, __pyx_t_13);
+  PyTuple_SET_ITEM(__pyx_t_2, 11, __pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_14);
-  PyTuple_SET_ITEM(__pyx_t_1, 12, __pyx_t_14);
+  PyTuple_SET_ITEM(__pyx_t_2, 12, __pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_15);
-  PyTuple_SET_ITEM(__pyx_t_1, 13, __pyx_t_15);
+  PyTuple_SET_ITEM(__pyx_t_2, 13, __pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_16);
-  PyTuple_SET_ITEM(__pyx_t_1, 14, __pyx_t_16);
+  PyTuple_SET_ITEM(__pyx_t_2, 14, __pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_17);
-  PyTuple_SET_ITEM(__pyx_t_1, 15, __pyx_t_17);
+  PyTuple_SET_ITEM(__pyx_t_2, 15, __pyx_t_17);
   __Pyx_GIVEREF(__pyx_t_18);
-  PyTuple_SET_ITEM(__pyx_t_1, 16, __pyx_t_18);
+  PyTuple_SET_ITEM(__pyx_t_2, 16, __pyx_t_18);
   __Pyx_GIVEREF(__pyx_t_19);
-  PyTuple_SET_ITEM(__pyx_t_1, 17, __pyx_t_19);
+  PyTuple_SET_ITEM(__pyx_t_2, 17, __pyx_t_19);
   __Pyx_GIVEREF(__pyx_t_20);
-  PyTuple_SET_ITEM(__pyx_t_1, 18, __pyx_t_20);
+  PyTuple_SET_ITEM(__pyx_t_2, 18, __pyx_t_20);
   __Pyx_GIVEREF(__pyx_t_21);
-  PyTuple_SET_ITEM(__pyx_t_1, 19, __pyx_t_21);
+  PyTuple_SET_ITEM(__pyx_t_2, 19, __pyx_t_21);
   __pyx_t_5 = 0;
   __pyx_t_9 = 0;
   __pyx_t_8 = 0;
   __pyx_t_7 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = 0;
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
   __pyx_t_16 = 0;
   __pyx_t_17 = 0;
   __pyx_t_18 = 0;
   __pyx_t_19 = 0;
   __pyx_t_20 = 0;
   __pyx_t_21 = 0;
 
-  /* "av/codec/context.pyx":71
+  /* "av/codec/context.pyx":74
  * ))
  * 
  * Flags = define_enum('Flags', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', 0),
  *     ('UNALIGNED', lib.AV_CODEC_FLAG_UNALIGNED,
  */
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.is_flags = 1;
-  __pyx_t_21 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Flags, __pyx_t_10, __pyx_t_1, 0, &__pyx_t_6); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_21 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Flags, __pyx_t_10, __pyx_t_2, 0, &__pyx_t_6); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Flags, __pyx_t_21) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Flags, __pyx_t_21) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
 
-  /* "av/codec/context.pyx":115
+  /* "av/codec/context.pyx":118
  * ), is_flags=True)
  * 
  * Flags2 = define_enum('Flags2', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', 0),
  *     ('FAST', lib.AV_CODEC_FLAG2_FAST,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_21, __pyx_n_s_name); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_21, __pyx_n_s_name); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
 
-  /* "av/codec/context.pyx":117
+  /* "av/codec/context.pyx":120
  * Flags2 = define_enum('Flags2', __name__, (
  *     ('NONE', 0),
  *     ('FAST', lib.AV_CODEC_FLAG2_FAST,             # <<<<<<<<<<<<<<
  *         """Allow non spec compliant speedup tricks."""),
  *     ('NO_OUTPUT', lib.AV_CODEC_FLAG2_NO_OUTPUT,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_FAST); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_FAST); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_n_s_FAST);
   __Pyx_GIVEREF(__pyx_n_s_FAST);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_n_s_FAST);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Allow_non_spec_compliant_speedup);
   __Pyx_GIVEREF(__pyx_kp_s_Allow_non_spec_compliant_speedup);
   PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_kp_s_Allow_non_spec_compliant_speedup);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":119
+  /* "av/codec/context.pyx":122
  *     ('FAST', lib.AV_CODEC_FLAG2_FAST,
  *         """Allow non spec compliant speedup tricks."""),
  *     ('NO_OUTPUT', lib.AV_CODEC_FLAG2_NO_OUTPUT,             # <<<<<<<<<<<<<<
  *         """Skip bitstream encoding."""),
  *     ('LOCAL_HEADER', lib.AV_CODEC_FLAG2_LOCAL_HEADER,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_NO_OUTPUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_20 = PyTuple_New(3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_NO_OUTPUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_20 = PyTuple_New(3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_20);
   __Pyx_INCREF(__pyx_n_s_NO_OUTPUT);
   __Pyx_GIVEREF(__pyx_n_s_NO_OUTPUT);
   PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_n_s_NO_OUTPUT);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Skip_bitstream_encoding);
   __Pyx_GIVEREF(__pyx_kp_s_Skip_bitstream_encoding);
   PyTuple_SET_ITEM(__pyx_t_20, 2, __pyx_kp_s_Skip_bitstream_encoding);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":121
+  /* "av/codec/context.pyx":124
  *     ('NO_OUTPUT', lib.AV_CODEC_FLAG2_NO_OUTPUT,
  *         """Skip bitstream encoding."""),
  *     ('LOCAL_HEADER', lib.AV_CODEC_FLAG2_LOCAL_HEADER,             # <<<<<<<<<<<<<<
  *         """Place global headers at every keyframe instead of in extradata."""),
  *     ('DROP_FRAME_TIMECODE', lib.AV_CODEC_FLAG2_DROP_FRAME_TIMECODE,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_LOCAL_HEADER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_LOCAL_HEADER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_19);
   __Pyx_INCREF(__pyx_n_s_LOCAL_HEADER);
   __Pyx_GIVEREF(__pyx_n_s_LOCAL_HEADER);
   PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_n_s_LOCAL_HEADER);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Place_global_headers_at_every_ke);
   __Pyx_GIVEREF(__pyx_kp_s_Place_global_headers_at_every_ke);
   PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_kp_s_Place_global_headers_at_every_ke);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":123
+  /* "av/codec/context.pyx":126
  *     ('LOCAL_HEADER', lib.AV_CODEC_FLAG2_LOCAL_HEADER,
  *         """Place global headers at every keyframe instead of in extradata."""),
  *     ('DROP_FRAME_TIMECODE', lib.AV_CODEC_FLAG2_DROP_FRAME_TIMECODE,             # <<<<<<<<<<<<<<
  *         """Timecode is in drop frame format. DEPRECATED!!!!"""),
  *     ('CHUNKS', lib.AV_CODEC_FLAG2_CHUNKS,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_DROP_FRAME_TIMECODE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_18 = PyTuple_New(3); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_DROP_FRAME_TIMECODE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_18 = PyTuple_New(3); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_n_s_DROP_FRAME_TIMECODE);
   __Pyx_GIVEREF(__pyx_n_s_DROP_FRAME_TIMECODE);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_n_s_DROP_FRAME_TIMECODE);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Timecode_is_in_drop_frame_format);
   __Pyx_GIVEREF(__pyx_kp_s_Timecode_is_in_drop_frame_format);
   PyTuple_SET_ITEM(__pyx_t_18, 2, __pyx_kp_s_Timecode_is_in_drop_frame_format);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":125
+  /* "av/codec/context.pyx":128
  *     ('DROP_FRAME_TIMECODE', lib.AV_CODEC_FLAG2_DROP_FRAME_TIMECODE,
  *         """Timecode is in drop frame format. DEPRECATED!!!!"""),
  *     ('CHUNKS', lib.AV_CODEC_FLAG2_CHUNKS,             # <<<<<<<<<<<<<<
  *         """Input bitstream might be truncated at a packet boundaries
  *         instead of only at frame boundaries."""),
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_CHUNKS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_17 = PyTuple_New(3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_CHUNKS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_17 = PyTuple_New(3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_INCREF(__pyx_n_s_CHUNKS);
   __Pyx_GIVEREF(__pyx_n_s_CHUNKS);
   PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_n_s_CHUNKS);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Input_bitstream_might_be_truncat_2);
   __Pyx_GIVEREF(__pyx_kp_s_Input_bitstream_might_be_truncat_2);
   PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_s_Input_bitstream_might_be_truncat_2);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":128
+  /* "av/codec/context.pyx":131
  *         """Input bitstream might be truncated at a packet boundaries
  *         instead of only at frame boundaries."""),
  *     ('IGNORE_CROP', lib.AV_CODEC_FLAG2_IGNORE_CROP,             # <<<<<<<<<<<<<<
  *         """Discard cropping information from SPS."""),
  *     ('SHOW_ALL', lib.AV_CODEC_FLAG2_SHOW_ALL,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_IGNORE_CROP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_IGNORE_CROP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_INCREF(__pyx_n_s_IGNORE_CROP);
   __Pyx_GIVEREF(__pyx_n_s_IGNORE_CROP);
   PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_n_s_IGNORE_CROP);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Discard_cropping_information_fro);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_cropping_information_fro);
   PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_s_Discard_cropping_information_fro);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":130
+  /* "av/codec/context.pyx":133
  *     ('IGNORE_CROP', lib.AV_CODEC_FLAG2_IGNORE_CROP,
  *         """Discard cropping information from SPS."""),
  *     ('SHOW_ALL', lib.AV_CODEC_FLAG2_SHOW_ALL,             # <<<<<<<<<<<<<<
  *         """Show all frames before the first keyframe"""),
  *     ('EXPORT_MVS', lib.AV_CODEC_FLAG2_EXPORT_MVS,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_SHOW_ALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_SHOW_ALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_INCREF(__pyx_n_s_SHOW_ALL);
   __Pyx_GIVEREF(__pyx_n_s_SHOW_ALL);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_n_s_SHOW_ALL);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Show_all_frames_before_the_first);
   __Pyx_GIVEREF(__pyx_kp_s_Show_all_frames_before_the_first);
   PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_s_Show_all_frames_before_the_first);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":132
+  /* "av/codec/context.pyx":135
  *     ('SHOW_ALL', lib.AV_CODEC_FLAG2_SHOW_ALL,
  *         """Show all frames before the first keyframe"""),
  *     ('EXPORT_MVS', lib.AV_CODEC_FLAG2_EXPORT_MVS,             # <<<<<<<<<<<<<<
  *         """Export motion vectors through frame side data"""),
  *     ('SKIP_MANUAL', lib.AV_CODEC_FLAG2_SKIP_MANUAL,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_EXPORT_MVS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_EXPORT_MVS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_INCREF(__pyx_n_s_EXPORT_MVS);
   __Pyx_GIVEREF(__pyx_n_s_EXPORT_MVS);
   PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_n_s_EXPORT_MVS);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Export_motion_vectors_through_fr);
   __Pyx_GIVEREF(__pyx_kp_s_Export_motion_vectors_through_fr);
   PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_s_Export_motion_vectors_through_fr);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":134
+  /* "av/codec/context.pyx":137
  *     ('EXPORT_MVS', lib.AV_CODEC_FLAG2_EXPORT_MVS,
  *         """Export motion vectors through frame side data"""),
  *     ('SKIP_MANUAL', lib.AV_CODEC_FLAG2_SKIP_MANUAL,             # <<<<<<<<<<<<<<
  *         """Do not skip samples and export skip information as frame side data"""),
  *     ('RO_FLUSH_NOOP', lib.AV_CODEC_FLAG2_RO_FLUSH_NOOP,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_SKIP_MANUAL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_13 = PyTuple_New(3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_SKIP_MANUAL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_13 = PyTuple_New(3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_n_s_SKIP_MANUAL);
   __Pyx_GIVEREF(__pyx_n_s_SKIP_MANUAL);
   PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_n_s_SKIP_MANUAL);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Do_not_skip_samples_and_export_s);
   __Pyx_GIVEREF(__pyx_kp_s_Do_not_skip_samples_and_export_s);
   PyTuple_SET_ITEM(__pyx_t_13, 2, __pyx_kp_s_Do_not_skip_samples_and_export_s);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":136
+  /* "av/codec/context.pyx":139
  *     ('SKIP_MANUAL', lib.AV_CODEC_FLAG2_SKIP_MANUAL,
  *         """Do not skip samples and export skip information as frame side data"""),
  *     ('RO_FLUSH_NOOP', lib.AV_CODEC_FLAG2_RO_FLUSH_NOOP,             # <<<<<<<<<<<<<<
  *         """Do not reset ASS ReadOrder field on flush (subtitles decoding)"""),
  * ), is_flags=True)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_RO_FLUSH_NOOP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(AV_CODEC_FLAG2_RO_FLUSH_NOOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_INCREF(__pyx_n_s_RO_FLUSH_NOOP);
   __Pyx_GIVEREF(__pyx_n_s_RO_FLUSH_NOOP);
   PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_n_s_RO_FLUSH_NOOP);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Do_not_reset_ASS_ReadOrder_field);
   __Pyx_GIVEREF(__pyx_kp_s_Do_not_reset_ASS_ReadOrder_field);
   PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_s_Do_not_reset_ASS_ReadOrder_field);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
 
-  /* "av/codec/context.pyx":116
+  /* "av/codec/context.pyx":119
  * 
  * Flags2 = define_enum('Flags2', __name__, (
  *     ('NONE', 0),             # <<<<<<<<<<<<<<
  *     ('FAST', lib.AV_CODEC_FLAG2_FAST,
  *         """Allow non spec compliant speedup tricks."""),
  */
-  __pyx_t_1 = PyTuple_New(11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_tuple__16);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_10);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_20);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_20);
+  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_20);
   __Pyx_GIVEREF(__pyx_t_19);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_19);
+  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_19);
   __Pyx_GIVEREF(__pyx_t_18);
-  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_18);
+  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_t_18);
   __Pyx_GIVEREF(__pyx_t_17);
-  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_17);
+  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_17);
   __Pyx_GIVEREF(__pyx_t_16);
-  PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_t_16);
+  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_15);
-  PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_t_15);
+  PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_14);
-  PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_t_14);
+  PyTuple_SET_ITEM(__pyx_t_2, 8, __pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_1, 9, __pyx_t_13);
+  PyTuple_SET_ITEM(__pyx_t_2, 9, __pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_12);
-  PyTuple_SET_ITEM(__pyx_t_1, 10, __pyx_t_12);
+  PyTuple_SET_ITEM(__pyx_t_2, 10, __pyx_t_12);
   __pyx_t_10 = 0;
   __pyx_t_20 = 0;
   __pyx_t_19 = 0;
   __pyx_t_18 = 0;
   __pyx_t_17 = 0;
   __pyx_t_16 = 0;
   __pyx_t_15 = 0;
   __pyx_t_14 = 0;
   __pyx_t_13 = 0;
   __pyx_t_12 = 0;
 
-  /* "av/codec/context.pyx":115
+  /* "av/codec/context.pyx":118
  * ), is_flags=True)
  * 
  * Flags2 = define_enum('Flags2', __name__, (             # <<<<<<<<<<<<<<
  *     ('NONE', 0),
  *     ('FAST', lib.AV_CODEC_FLAG2_FAST,
  */
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.is_flags = 1;
-  __pyx_t_12 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Flags2, __pyx_t_21, __pyx_t_1, 0, &__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_12 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Flags2, __pyx_t_21, __pyx_t_2, 0, &__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Flags2, __pyx_t_12) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Flags2, __pyx_t_12) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-  /* "av/codec/context.pyx":144
+  /* "av/codec/context.pyx":147
  * 
  *     @staticmethod
  *     def create(codec, mode=None):             # <<<<<<<<<<<<<<
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  *         cdef lib.AVCodecContext *c_ctx = lib.avcodec_alloc_context3(cy_codec.ptr)
  */
-  __pyx_t_12 = PyCFunction_NewEx(&__pyx_mdef_2av_5codec_7context_12CodecContext_1create, NULL, __pyx_n_s_av_codec_context); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_12 = PyCFunction_NewEx(&__pyx_mdef_2av_5codec_7context_12CodecContext_1create, NULL, __pyx_n_s_av_codec_context); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_create, __pyx_t_12) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_create, __pyx_t_12) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":143
+  /* "av/codec/context.pyx":146
  * cdef class CodecContext(object):
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create(codec, mode=None):
  *         cdef Codec cy_codec = codec if isinstance(codec, Codec) else Codec(codec, mode)
  */
-  __Pyx_GetNameInClass(__pyx_t_12, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_create); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_12, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_create); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_create, __pyx_t_1) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_create, __pyx_t_2) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":179
+  /* "av/codec/context.pyx":182
  *         self.ptr.flags = value
  * 
  *     flags = Flags.property(             # <<<<<<<<<<<<<<
  *         _get_flags,
  *         _set_flags,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_Flags); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_Flags); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-  /* "av/codec/context.pyx":180
+  /* "av/codec/context.pyx":183
  * 
  *     flags = Flags.property(
  *         _get_flags,             # <<<<<<<<<<<<<<
  *         _set_flags,
  *         """Flag property of :class:`.Flags`."""
  */
-  __Pyx_GetNameInClass(__pyx_t_12, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_get_flags); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_12, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_get_flags); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
 
-  /* "av/codec/context.pyx":181
+  /* "av/codec/context.pyx":184
  *     flags = Flags.property(
  *         _get_flags,
  *         _set_flags,             # <<<<<<<<<<<<<<
  *         """Flag property of :class:`.Flags`."""
  *     )
  */
-  __Pyx_GetNameInClass(__pyx_t_13, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_set_flags); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_13, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_set_flags); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_14 = NULL;
   __pyx_t_22 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
@@ -11685,675 +11960,675 @@
       __Pyx_DECREF_SET(__pyx_t_21, function);
       __pyx_t_22 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_21)) {
     PyObject *__pyx_temp[4] = {__pyx_t_14, __pyx_t_12, __pyx_t_13, __pyx_kp_s_Flag_property_of_class_Flags};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_21)) {
     PyObject *__pyx_temp[4] = {__pyx_t_14, __pyx_t_12, __pyx_t_13, __pyx_kp_s_Flag_property_of_class_Flags};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   } else
   #endif
   {
-    __pyx_t_15 = PyTuple_New(3+__pyx_t_22); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_15 = PyTuple_New(3+__pyx_t_22); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     if (__pyx_t_14) {
       __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_14); __pyx_t_14 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_12);
     PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_22, __pyx_t_12);
     __Pyx_GIVEREF(__pyx_t_13);
     PyTuple_SET_ITEM(__pyx_t_15, 1+__pyx_t_22, __pyx_t_13);
     __Pyx_INCREF(__pyx_kp_s_Flag_property_of_class_Flags);
     __Pyx_GIVEREF(__pyx_kp_s_Flag_property_of_class_Flags);
     PyTuple_SET_ITEM(__pyx_t_15, 2+__pyx_t_22, __pyx_kp_s_Flag_property_of_class_Flags);
     __pyx_t_12 = 0;
     __pyx_t_13 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_t_15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_t_15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   }
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_flags, __pyx_t_1) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_flags, __pyx_t_2) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":185
+  /* "av/codec/context.pyx":188
  *     )
  * 
  *     unaligned = flags.flag_property('UNALIGNED')             # <<<<<<<<<<<<<<
  *     qscale = flags.flag_property('QSCALE')
  *     four_mv = flags.flag_property('4MV')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_UNALIGNED) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_UNALIGNED);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_UNALIGNED) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_UNALIGNED);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_unaligned, __pyx_t_1) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_unaligned, __pyx_t_2) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":186
+  /* "av/codec/context.pyx":189
  * 
  *     unaligned = flags.flag_property('UNALIGNED')
  *     qscale = flags.flag_property('QSCALE')             # <<<<<<<<<<<<<<
  *     four_mv = flags.flag_property('4MV')
  *     output_corrupt = flags.flag_property('OUTPUT_CORRUPT')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_QSCALE) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_QSCALE);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_QSCALE) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_QSCALE);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_qscale, __pyx_t_1) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_qscale, __pyx_t_2) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":187
+  /* "av/codec/context.pyx":190
  *     unaligned = flags.flag_property('UNALIGNED')
  *     qscale = flags.flag_property('QSCALE')
  *     four_mv = flags.flag_property('4MV')             # <<<<<<<<<<<<<<
  *     output_corrupt = flags.flag_property('OUTPUT_CORRUPT')
  *     qpel = flags.flag_property('QPEL')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_kp_s_4MV) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_kp_s_4MV);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_kp_s_4MV) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_kp_s_4MV);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_four_mv, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_four_mv, __pyx_t_2) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":188
+  /* "av/codec/context.pyx":191
  *     qscale = flags.flag_property('QSCALE')
  *     four_mv = flags.flag_property('4MV')
  *     output_corrupt = flags.flag_property('OUTPUT_CORRUPT')             # <<<<<<<<<<<<<<
  *     qpel = flags.flag_property('QPEL')
  *     drop_changed = flags.flag_property('DROPCHANGED')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_OUTPUT_CORRUPT) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_OUTPUT_CORRUPT);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_OUTPUT_CORRUPT) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_OUTPUT_CORRUPT);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_output_corrupt, __pyx_t_1) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_output_corrupt, __pyx_t_2) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":189
+  /* "av/codec/context.pyx":192
  *     four_mv = flags.flag_property('4MV')
  *     output_corrupt = flags.flag_property('OUTPUT_CORRUPT')
  *     qpel = flags.flag_property('QPEL')             # <<<<<<<<<<<<<<
  *     drop_changed = flags.flag_property('DROPCHANGED')
  *     pass1 = flags.flag_property('PASS1')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_QPEL) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_QPEL);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_QPEL) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_QPEL);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_qpel, __pyx_t_1) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_qpel, __pyx_t_2) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":190
+  /* "av/codec/context.pyx":193
  *     output_corrupt = flags.flag_property('OUTPUT_CORRUPT')
  *     qpel = flags.flag_property('QPEL')
  *     drop_changed = flags.flag_property('DROPCHANGED')             # <<<<<<<<<<<<<<
  *     pass1 = flags.flag_property('PASS1')
  *     pass2 = flags.flag_property('PASS2')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_DROPCHANGED) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_DROPCHANGED);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_DROPCHANGED) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_DROPCHANGED);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_drop_changed, __pyx_t_1) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_drop_changed, __pyx_t_2) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":191
+  /* "av/codec/context.pyx":194
  *     qpel = flags.flag_property('QPEL')
  *     drop_changed = flags.flag_property('DROPCHANGED')
  *     pass1 = flags.flag_property('PASS1')             # <<<<<<<<<<<<<<
  *     pass2 = flags.flag_property('PASS2')
  *     loop_filter = flags.flag_property('LOOP_FILTER')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_PASS1) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_PASS1);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_PASS1) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_PASS1);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_pass1, __pyx_t_1) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_pass1, __pyx_t_2) < 0) __PYX_ERR(0, 194, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":192
+  /* "av/codec/context.pyx":195
  *     drop_changed = flags.flag_property('DROPCHANGED')
  *     pass1 = flags.flag_property('PASS1')
  *     pass2 = flags.flag_property('PASS2')             # <<<<<<<<<<<<<<
  *     loop_filter = flags.flag_property('LOOP_FILTER')
  *     gray = flags.flag_property('GRAY')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_PASS2) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_PASS2);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_PASS2) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_PASS2);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_pass2, __pyx_t_1) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_pass2, __pyx_t_2) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":193
+  /* "av/codec/context.pyx":196
  *     pass1 = flags.flag_property('PASS1')
  *     pass2 = flags.flag_property('PASS2')
  *     loop_filter = flags.flag_property('LOOP_FILTER')             # <<<<<<<<<<<<<<
  *     gray = flags.flag_property('GRAY')
  *     psnr = flags.flag_property('PSNR')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_LOOP_FILTER) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_LOOP_FILTER);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_LOOP_FILTER) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_LOOP_FILTER);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_loop_filter_2, __pyx_t_1) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_loop_filter_2, __pyx_t_2) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":194
+  /* "av/codec/context.pyx":197
  *     pass2 = flags.flag_property('PASS2')
  *     loop_filter = flags.flag_property('LOOP_FILTER')
  *     gray = flags.flag_property('GRAY')             # <<<<<<<<<<<<<<
  *     psnr = flags.flag_property('PSNR')
  *     truncated = flags.flag_property('TRUNCATED')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_GRAY) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_GRAY);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_GRAY) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_GRAY);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_gray, __pyx_t_1) < 0) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_gray, __pyx_t_2) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":195
+  /* "av/codec/context.pyx":198
  *     loop_filter = flags.flag_property('LOOP_FILTER')
  *     gray = flags.flag_property('GRAY')
  *     psnr = flags.flag_property('PSNR')             # <<<<<<<<<<<<<<
  *     truncated = flags.flag_property('TRUNCATED')
  *     interlaced_dct = flags.flag_property('INTERLACED_DCT')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_PSNR) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_PSNR);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_PSNR) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_PSNR);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_psnr, __pyx_t_1) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_psnr, __pyx_t_2) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":196
+  /* "av/codec/context.pyx":199
  *     gray = flags.flag_property('GRAY')
  *     psnr = flags.flag_property('PSNR')
  *     truncated = flags.flag_property('TRUNCATED')             # <<<<<<<<<<<<<<
  *     interlaced_dct = flags.flag_property('INTERLACED_DCT')
  *     low_delay = flags.flag_property('LOW_DELAY')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_TRUNCATED) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_TRUNCATED);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_TRUNCATED) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_TRUNCATED);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_truncated, __pyx_t_1) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_truncated, __pyx_t_2) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":197
+  /* "av/codec/context.pyx":200
  *     psnr = flags.flag_property('PSNR')
  *     truncated = flags.flag_property('TRUNCATED')
  *     interlaced_dct = flags.flag_property('INTERLACED_DCT')             # <<<<<<<<<<<<<<
  *     low_delay = flags.flag_property('LOW_DELAY')
  *     global_header = flags.flag_property('GLOBAL_HEADER')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_INTERLACED_DCT) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_INTERLACED_DCT);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_INTERLACED_DCT) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_INTERLACED_DCT);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_interlaced_dct, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_interlaced_dct, __pyx_t_2) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":198
+  /* "av/codec/context.pyx":201
  *     truncated = flags.flag_property('TRUNCATED')
  *     interlaced_dct = flags.flag_property('INTERLACED_DCT')
  *     low_delay = flags.flag_property('LOW_DELAY')             # <<<<<<<<<<<<<<
  *     global_header = flags.flag_property('GLOBAL_HEADER')
  *     bitexact = flags.flag_property('BITEXACT')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_LOW_DELAY) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_LOW_DELAY);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_LOW_DELAY) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_LOW_DELAY);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_low_delay, __pyx_t_1) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_low_delay, __pyx_t_2) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":199
+  /* "av/codec/context.pyx":202
  *     interlaced_dct = flags.flag_property('INTERLACED_DCT')
  *     low_delay = flags.flag_property('LOW_DELAY')
  *     global_header = flags.flag_property('GLOBAL_HEADER')             # <<<<<<<<<<<<<<
  *     bitexact = flags.flag_property('BITEXACT')
  *     ac_pred = flags.flag_property('AC_PRED')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_GLOBAL_HEADER) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_GLOBAL_HEADER);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_GLOBAL_HEADER) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_GLOBAL_HEADER);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_global_header, __pyx_t_1) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_global_header, __pyx_t_2) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":200
+  /* "av/codec/context.pyx":203
  *     low_delay = flags.flag_property('LOW_DELAY')
  *     global_header = flags.flag_property('GLOBAL_HEADER')
  *     bitexact = flags.flag_property('BITEXACT')             # <<<<<<<<<<<<<<
  *     ac_pred = flags.flag_property('AC_PRED')
  *     interlaced_me = flags.flag_property('INTERLACED_ME')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_BITEXACT) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_BITEXACT);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_BITEXACT) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_BITEXACT);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_bitexact, __pyx_t_1) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_bitexact, __pyx_t_2) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":201
+  /* "av/codec/context.pyx":204
  *     global_header = flags.flag_property('GLOBAL_HEADER')
  *     bitexact = flags.flag_property('BITEXACT')
  *     ac_pred = flags.flag_property('AC_PRED')             # <<<<<<<<<<<<<<
  *     interlaced_me = flags.flag_property('INTERLACED_ME')
  *     closed_gop = flags.flag_property('CLOSED_GOP')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_AC_PRED) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_AC_PRED);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_AC_PRED) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_AC_PRED);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_ac_pred, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_ac_pred, __pyx_t_2) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":202
+  /* "av/codec/context.pyx":205
  *     bitexact = flags.flag_property('BITEXACT')
  *     ac_pred = flags.flag_property('AC_PRED')
  *     interlaced_me = flags.flag_property('INTERLACED_ME')             # <<<<<<<<<<<<<<
  *     closed_gop = flags.flag_property('CLOSED_GOP')
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_INTERLACED_ME) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_INTERLACED_ME);
+  __pyx_t_2 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_15, __pyx_n_s_INTERLACED_ME) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_INTERLACED_ME);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_interlaced_me, __pyx_t_1) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_interlaced_me, __pyx_t_2) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":203
+  /* "av/codec/context.pyx":206
  *     ac_pred = flags.flag_property('AC_PRED')
  *     interlaced_me = flags.flag_property('INTERLACED_ME')
  *     closed_gop = flags.flag_property('CLOSED_GOP')             # <<<<<<<<<<<<<<
  * 
  *     def _get_flags2(self):
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_CLOSED_GOP) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_CLOSED_GOP);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_21, __pyx_n_s_CLOSED_GOP) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_CLOSED_GOP);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_closed_gop, __pyx_t_1) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_closed_gop, __pyx_t_2) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":211
+  /* "av/codec/context.pyx":214
  *         self.ptr.flags2 = value
  * 
  *     flags2 = Flags2.property(             # <<<<<<<<<<<<<<
  *         _get_flags2,
  *         _set_flags2,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_Flags2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_Flags2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-  /* "av/codec/context.pyx":212
+  /* "av/codec/context.pyx":215
  * 
  *     flags2 = Flags2.property(
  *         _get_flags2,             # <<<<<<<<<<<<<<
  *         _set_flags2,
  *         """Flag property of :class:`.Flags2`."""
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_get_flags2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_get_flags2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
 
-  /* "av/codec/context.pyx":213
+  /* "av/codec/context.pyx":216
  *     flags2 = Flags2.property(
  *         _get_flags2,
  *         _set_flags2,             # <<<<<<<<<<<<<<
  *         """Flag property of :class:`.Flags2`."""
  *     )
  */
-  __Pyx_GetNameInClass(__pyx_t_13, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_set_flags2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_13, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_set_flags2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_12 = NULL;
   __pyx_t_22 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
@@ -12362,374 +12637,374 @@
       __Pyx_DECREF_SET(__pyx_t_21, function);
       __pyx_t_22 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_21)) {
     PyObject *__pyx_temp[4] = {__pyx_t_12, __pyx_t_15, __pyx_t_13, __pyx_kp_s_Flag_property_of_class_Flags2};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_21)) {
     PyObject *__pyx_temp[4] = {__pyx_t_12, __pyx_t_15, __pyx_t_13, __pyx_kp_s_Flag_property_of_class_Flags2};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_21, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   } else
   #endif
   {
-    __pyx_t_14 = PyTuple_New(3+__pyx_t_22); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_14 = PyTuple_New(3+__pyx_t_22); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     if (__pyx_t_12) {
       __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_12); __pyx_t_12 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_15);
     PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_22, __pyx_t_15);
     __Pyx_GIVEREF(__pyx_t_13);
     PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_22, __pyx_t_13);
     __Pyx_INCREF(__pyx_kp_s_Flag_property_of_class_Flags2);
     __Pyx_GIVEREF(__pyx_kp_s_Flag_property_of_class_Flags2);
     PyTuple_SET_ITEM(__pyx_t_14, 2+__pyx_t_22, __pyx_kp_s_Flag_property_of_class_Flags2);
     __pyx_t_15 = 0;
     __pyx_t_13 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_21, __pyx_t_14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   }
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_flags2, __pyx_t_1) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_flags2, __pyx_t_2) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":217
+  /* "av/codec/context.pyx":220
  *     )
  * 
  *     fast = flags2.flag_property('FAST')             # <<<<<<<<<<<<<<
  *     no_output = flags2.flag_property('NO_OUTPUT')
  *     local_header = flags2.flag_property('LOCAL_HEADER')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_FAST) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_FAST);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_FAST) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_FAST);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_fast, __pyx_t_1) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_fast, __pyx_t_2) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":218
+  /* "av/codec/context.pyx":221
  * 
  *     fast = flags2.flag_property('FAST')
  *     no_output = flags2.flag_property('NO_OUTPUT')             # <<<<<<<<<<<<<<
  *     local_header = flags2.flag_property('LOCAL_HEADER')
  *     drop_frame_timecode = flags2.flag_property('DROP_FRAME_TIMECODE')
  */
-  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_14);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_NO_OUTPUT) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_NO_OUTPUT);
+  __pyx_t_2 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_NO_OUTPUT) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_NO_OUTPUT);
   __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_no_output, __pyx_t_1) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_no_output, __pyx_t_2) < 0) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":219
+  /* "av/codec/context.pyx":222
  *     fast = flags2.flag_property('FAST')
  *     no_output = flags2.flag_property('NO_OUTPUT')
  *     local_header = flags2.flag_property('LOCAL_HEADER')             # <<<<<<<<<<<<<<
  *     drop_frame_timecode = flags2.flag_property('DROP_FRAME_TIMECODE')
  *     chunks = flags2.flag_property('CHUNKS')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_LOCAL_HEADER) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_LOCAL_HEADER);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_LOCAL_HEADER) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_LOCAL_HEADER);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_local_header, __pyx_t_1) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_local_header, __pyx_t_2) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":220
+  /* "av/codec/context.pyx":223
  *     no_output = flags2.flag_property('NO_OUTPUT')
  *     local_header = flags2.flag_property('LOCAL_HEADER')
  *     drop_frame_timecode = flags2.flag_property('DROP_FRAME_TIMECODE')             # <<<<<<<<<<<<<<
  *     chunks = flags2.flag_property('CHUNKS')
  *     ignore_crop = flags2.flag_property('IGNORE_CROP')
  */
-  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_14);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_DROP_FRAME_TIMECODE) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_DROP_FRAME_TIMECODE);
+  __pyx_t_2 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_DROP_FRAME_TIMECODE) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_DROP_FRAME_TIMECODE);
   __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_drop_frame_timecode, __pyx_t_1) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_drop_frame_timecode, __pyx_t_2) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":221
+  /* "av/codec/context.pyx":224
  *     local_header = flags2.flag_property('LOCAL_HEADER')
  *     drop_frame_timecode = flags2.flag_property('DROP_FRAME_TIMECODE')
  *     chunks = flags2.flag_property('CHUNKS')             # <<<<<<<<<<<<<<
  *     ignore_crop = flags2.flag_property('IGNORE_CROP')
  *     show_all = flags2.flag_property('SHOW_ALL')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_CHUNKS) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_CHUNKS);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_CHUNKS) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_CHUNKS);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_chunks, __pyx_t_1) < 0) __PYX_ERR(0, 221, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_chunks, __pyx_t_2) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":222
+  /* "av/codec/context.pyx":225
  *     drop_frame_timecode = flags2.flag_property('DROP_FRAME_TIMECODE')
  *     chunks = flags2.flag_property('CHUNKS')
  *     ignore_crop = flags2.flag_property('IGNORE_CROP')             # <<<<<<<<<<<<<<
  *     show_all = flags2.flag_property('SHOW_ALL')
  *     export_mvs = flags2.flag_property('EXPORT_MVS')
  */
-  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_14);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_IGNORE_CROP) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_IGNORE_CROP);
+  __pyx_t_2 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_IGNORE_CROP) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_IGNORE_CROP);
   __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_ignore_crop, __pyx_t_1) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_ignore_crop, __pyx_t_2) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":223
+  /* "av/codec/context.pyx":226
  *     chunks = flags2.flag_property('CHUNKS')
  *     ignore_crop = flags2.flag_property('IGNORE_CROP')
  *     show_all = flags2.flag_property('SHOW_ALL')             # <<<<<<<<<<<<<<
  *     export_mvs = flags2.flag_property('EXPORT_MVS')
  *     skip_manual = flags2.flag_property('SKIP_MANUAL')
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_SHOW_ALL) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_SHOW_ALL);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_SHOW_ALL) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_SHOW_ALL);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_show_all, __pyx_t_1) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_show_all, __pyx_t_2) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":224
+  /* "av/codec/context.pyx":227
  *     ignore_crop = flags2.flag_property('IGNORE_CROP')
  *     show_all = flags2.flag_property('SHOW_ALL')
  *     export_mvs = flags2.flag_property('EXPORT_MVS')             # <<<<<<<<<<<<<<
  *     skip_manual = flags2.flag_property('SKIP_MANUAL')
  *     ro_flush_noop = flags2.flag_property('RO_FLUSH_NOOP')
  */
-  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_14);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_EXPORT_MVS) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_EXPORT_MVS);
+  __pyx_t_2 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_EXPORT_MVS) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_EXPORT_MVS);
   __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_export_mvs, __pyx_t_1) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_export_mvs, __pyx_t_2) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":225
+  /* "av/codec/context.pyx":228
  *     show_all = flags2.flag_property('SHOW_ALL')
  *     export_mvs = flags2.flag_property('EXPORT_MVS')
  *     skip_manual = flags2.flag_property('SKIP_MANUAL')             # <<<<<<<<<<<<<<
  *     ro_flush_noop = flags2.flag_property('RO_FLUSH_NOOP')
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_21, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
   __pyx_t_21 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_21)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_21);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_SKIP_MANUAL) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_SKIP_MANUAL);
+  __pyx_t_2 = (__pyx_t_21) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_21, __pyx_n_s_SKIP_MANUAL) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_n_s_SKIP_MANUAL);
   __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_skip_manual, __pyx_t_1) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_skip_manual, __pyx_t_2) < 0) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
-  /* "av/codec/context.pyx":226
+  /* "av/codec/context.pyx":229
  *     export_mvs = flags2.flag_property('EXPORT_MVS')
  *     skip_manual = flags2.flag_property('SKIP_MANUAL')
  *     ro_flush_noop = flags2.flag_property('RO_FLUSH_NOOP')             # <<<<<<<<<<<<<<
  * 
  *     property extradata:
  */
-  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_14, (PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext, __pyx_n_s_flags2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_21);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_21))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_21);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
       __Pyx_INCREF(__pyx_t_14);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_21, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_RO_FLUSH_NOOP) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_RO_FLUSH_NOOP);
+  __pyx_t_2 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_21, __pyx_t_14, __pyx_n_s_RO_FLUSH_NOOP) : __Pyx_PyObject_CallOneArg(__pyx_t_21, __pyx_n_s_RO_FLUSH_NOOP);
   __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_ro_flush_noop, __pyx_t_1) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict, __pyx_n_s_ro_flush_noop, __pyx_t_2) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2av_5codec_7context_CodecContext);
 
   /* "av/codec/context.pyx":1
- * from libc.errno cimport EAGAIN             # <<<<<<<<<<<<<<
- * from libc.stdint cimport int64_t, uint8_t
- * from libc.string cimport memcpy
+ * import warnings             # <<<<<<<<<<<<<<
+ * 
+ * from libc.errno cimport EAGAIN
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
```

### Comparing `ha-av-9.1.1.post3/src/av/container/core.c` & `ha-av-9.2.0.post1/src/av/container/core.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/container/input.c` & `ha-av-9.2.0.post1/src/av/container/input.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/container/output.c` & `ha-av-9.2.0.post1/src/av/container/output.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -5181,15 +5189,15 @@
  */
   __pyx_t_1 = ((struct __pyx_vtabstruct_2av_6packet_Packet *)__pyx_v_packet->__pyx_base.__pyx_vtab)->_rebase_time(__pyx_v_packet, __pyx_v_stream->time_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "av/container/output.pyx":227
  *         # Make another reference to the packet, as av_interleaved_write_frame
- *         # takes ownership of it.
+ *         # takes ownership of the reference.
  *         self.err_check(lib.av_packet_ref(self.packet_ptr, packet.ptr))             # <<<<<<<<<<<<<<
  * 
  *         cdef int ret
  */
   __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), av_packet_ref(__pyx_v_self->packet_ptr, __pyx_v_packet->ptr)); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 227, __pyx_L1_error)
 
   /* "av/container/output.pyx":230
```

### Comparing `ha-av-9.1.1.post3/src/av/container/pyio.c` & `ha-av-9.2.0.post1/src/av/container/pyio.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/container/streams.c` & `ha-av-9.2.0.post1/src/av/container/streams.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/data/stream.c` & `ha-av-9.2.0.post1/src/av/data/stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/descriptor.c` & `ha-av-9.2.0.post1/src/av/descriptor.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/dictionary.c` & `ha-av-9.2.0.post1/src/av/dictionary.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/enum.c` & `ha-av-9.2.0.post1/src/av/enum.c`

 * *Files 1% similar despite different names*

```diff
@@ -1480,14 +1480,31 @@
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* ListCompAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len)) {
+        Py_INCREF(x);
+        PyList_SET_ITEM(list, len, x);
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+#endif
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
@@ -8950,24 +8967,29 @@
  */
 
 static PyObject *__pyx_pw_2av_4enum_3define_enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_2av_4enum_define_enum(PyObject *__pyx_v_name, PyObject *__pyx_v_module, PyObject *__pyx_v_items, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_2av_4enum_define_enum *__pyx_optional_args) {
   int __pyx_v_is_flags = ((int)0);
   PyTypeObject *__pyx_v_base_cls = NULL;
   PyObject *__pyx_v_cls = NULL;
+  PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  Py_ssize_t __pyx_t_8;
+  PyObject *(*__pyx_t_9)(PyObject *);
+  PyObject *__pyx_t_10 = NULL;
+  int __pyx_t_11;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("define_enum", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_is_flags = __pyx_optional_args->is_flags;
@@ -9005,99 +9027,151 @@
   }
 
   /* "av/enum.pyx":385
  *         base_cls = EnumFlag
  *     else:
  *         base_cls = EnumItem             # <<<<<<<<<<<<<<
  * 
- *     cls = EnumType(name, (base_cls, ), {'__module__': module}, items)
+ *     # Some items may be None if they correspond to an unsupported FFmpeg feature
  */
   /*else*/ {
     __Pyx_INCREF(((PyObject *)__pyx_ptype_2av_4enum_EnumItem));
     __pyx_v_base_cls = __pyx_ptype_2av_4enum_EnumItem;
   }
   __pyx_L3:;
 
-  /* "av/enum.pyx":387
- *         base_cls = EnumItem
+  /* "av/enum.pyx":388
  * 
- *     cls = EnumType(name, (base_cls, ), {'__module__': module}, items)             # <<<<<<<<<<<<<<
+ *     # Some items may be None if they correspond to an unsupported FFmpeg feature
+ *     cls = EnumType(name, (base_cls, ), {'__module__': module}, [i for i in items if i is not None])             # <<<<<<<<<<<<<<
  * 
  *     return cls
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_EnumType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_EnumType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject *)__pyx_v_base_cls));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_base_cls));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_base_cls));
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_module, __pyx_v_module) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_6 = NULL;
-  __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_module, __pyx_v_module) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (likely(PyList_CheckExact(__pyx_v_items)) || PyTuple_CheckExact(__pyx_v_items)) {
+    __pyx_t_7 = __pyx_v_items; __Pyx_INCREF(__pyx_t_7); __pyx_t_8 = 0;
+    __pyx_t_9 = NULL;
+  } else {
+    __pyx_t_8 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_items); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_9)) {
+      if (likely(PyList_CheckExact(__pyx_t_7))) {
+        if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_7)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_10 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_10); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 388, __pyx_L1_error)
+        #else
+        __pyx_t_10 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        #endif
+      } else {
+        if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_10); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 388, __pyx_L1_error)
+        #else
+        __pyx_t_10 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        #endif
+      }
+    } else {
+      __pyx_t_10 = __pyx_t_9(__pyx_t_7);
+      if (unlikely(!__pyx_t_10)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 388, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_10);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_10);
+    __pyx_t_10 = 0;
+    __pyx_t_1 = (__pyx_v_i != Py_None);
+    __pyx_t_11 = (__pyx_t_1 != 0);
+    if (__pyx_t_11) {
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_v_i))) __PYX_ERR(0, 388, __pyx_L1_error)
+    }
+  }
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = NULL;
+  __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_6)) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_7 = 1;
+      __pyx_t_12 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_6, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_v_items};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 4+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    PyObject *__pyx_temp[5] = {__pyx_t_7, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_t_6};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 4+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_6, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_v_items};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 4+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    PyObject *__pyx_temp[5] = {__pyx_t_7, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_t_6};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 4+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(4+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    if (__pyx_t_6) {
-      __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+    __pyx_t_10 = PyTuple_New(4+__pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    if (__pyx_t_7) {
+      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_name);
     __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_name);
+    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_12, __pyx_v_name);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_12, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_t_5);
-    __Pyx_INCREF(__pyx_v_items);
-    __Pyx_GIVEREF(__pyx_v_items);
-    PyTuple_SET_ITEM(__pyx_t_8, 3+__pyx_t_7, __pyx_v_items);
+    PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_12, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_10, 3+__pyx_t_12, __pyx_t_6);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = 0;
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cls = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "av/enum.pyx":389
- *     cls = EnumType(name, (base_cls, ), {'__module__': module}, items)
+  /* "av/enum.pyx":390
+ *     cls = EnumType(name, (base_cls, ), {'__module__': module}, [i for i in items if i is not None])
  * 
  *     return cls             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_cls);
   __pyx_r = __pyx_v_cls;
   goto __pyx_L0;
@@ -9113,20 +9187,22 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("av.enum.define_enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_base_cls);
   __Pyx_XDECREF(__pyx_v_cls);
+  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_4enum_3define_enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
```

### Comparing `ha-av-9.1.1.post3/src/av/error.c` & `ha-av-9.2.0.post1/src/av/error.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/filter/context.c` & `ha-av-9.2.0.post1/src/av/filter/context.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/filter/filter.c` & `ha-av-9.2.0.post1/src/av/filter/filter.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/filter/graph.c` & `ha-av-9.2.0.post1/src/av/filter/graph.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/filter/link.c` & `ha-av-9.2.0.post1/src/av/filter/link.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/filter/pad.c` & `ha-av-9.2.0.post1/src/av/filter/pad.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/format.c` & `ha-av-9.2.0.post1/src/av/format.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/frame.c` & `ha-av-9.2.0.post1/src/av/frame.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/logging.c` & `ha-av-9.2.0.post1/src/av/logging.c`

 * *Files 0% similar despite different names*

```diff
@@ -749,14 +749,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/option.c` & `ha-av-9.2.0.post1/src/av/option.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/packet.c` & `ha-av-9.2.0.post1/src/av/packet.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/plane.c` & `ha-av-9.2.0.post1/src/av/plane.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/sidedata/motionvectors.c` & `ha-av-9.2.0.post1/src/av/sidedata/motionvectors.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/sidedata/sidedata.c` & `ha-av-9.2.0.post1/src/av/sidedata/sidedata.c`

 * *Files 2% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1508,15 +1516,15 @@
   PyObject *(*_rebase_time)(struct __pyx_obj_2av_5frame_Frame *, AVRational);
   PyObject *(*_copy_internal_attributes)(struct __pyx_obj_2av_5frame_Frame *, struct __pyx_obj_2av_5frame_Frame *, struct __pyx_opt_args_2av_5frame_5Frame__copy_internal_attributes *__pyx_optional_args);
   PyObject *(*_init_user_attributes)(struct __pyx_obj_2av_5frame_Frame *);
 };
 static struct __pyx_vtabstruct_2av_5frame_Frame *__pyx_vtabptr_2av_5frame_Frame;
 
 
-/* "av/sidedata/sidedata.pyx":45
+/* "av/sidedata/sidedata.pyx":47
  * 
  * 
  * cdef class SideData(Buffer):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, sentinel, Frame frame, int index):
  */
 
@@ -2137,14 +2145,15 @@
 static const char __pyx_k_MotionVectors[] = "MotionVectors";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_MATRIXENCODING[] = "MATRIXENCODING";
 static const char __pyx_k_MOTION_VECTORS[] = "MOTION_VECTORS";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_SEI_UNREGISTERED[] = "SEI_UNREGISTERED";
 static const char __pyx_k_SideDataContainer[] = "_SideDataContainer";
 static const char __pyx_k_AUDIO_SERVICE_TYPE[] = "AUDIO_SERVICE_TYPE";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_CONTENT_LIGHT_LEVEL[] = "CONTENT_LIGHT_LEVEL";
 static const char __pyx_k_SideDataContainer_2[] = "SideDataContainer";
 static const char __pyx_k_av_sidedata_sidedata[] = "av.sidedata.sidedata";
 static const char __pyx_k_av_sidedata_motionvectors[] = "av.sidedata.motionvectors";
@@ -2168,14 +2177,15 @@
 static PyObject *__pyx_n_s_MOTION_VECTORS;
 static PyObject *__pyx_n_s_Mapping;
 static PyObject *__pyx_n_s_MotionVectors;
 static PyObject *__pyx_n_s_PANSCAN;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_REPLAYGAIN;
 static PyObject *__pyx_n_s_RuntimeError;
+static PyObject *__pyx_n_s_SEI_UNREGISTERED;
 static PyObject *__pyx_n_s_SKIP_SAMPLES;
 static PyObject *__pyx_n_s_SPHERICAL;
 static PyObject *__pyx_n_s_STEREO3D;
 static PyObject *__pyx_n_s_SideData;
 static PyObject *__pyx_n_s_SideDataContainer;
 static PyObject *__pyx_n_s_SideDataContainer_2;
 static PyObject *__pyx_n_s_Type;
@@ -2244,15 +2254,15 @@
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_codeobj__7;
 /* Late includes */
 
-/* "av/sidedata/sidedata.pyx":36
+/* "av/sidedata/sidedata.pyx":38
  * 
  * 
  * cdef SideData wrap_side_data(Frame frame, int index):             # <<<<<<<<<<<<<<
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  */
 
@@ -2269,45 +2279,45 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap_side_data", 0);
 
-  /* "av/sidedata/sidedata.pyx":38
+  /* "av/sidedata/sidedata.pyx":40
  * cdef SideData wrap_side_data(Frame frame, int index):
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type             # <<<<<<<<<<<<<<
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  */
   __pyx_t_1 = (__pyx_v_frame->ptr->side_data[__pyx_v_index])->type;
   __pyx_v_type_ = __pyx_t_1;
 
-  /* "av/sidedata/sidedata.pyx":39
+  /* "av/sidedata/sidedata.pyx":41
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:             # <<<<<<<<<<<<<<
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  *     else:
  */
   __pyx_t_2 = ((__pyx_v_type_ == AV_FRAME_DATA_MOTION_VECTORS) != 0);
   if (__pyx_t_2) {
 
-    /* "av/sidedata/sidedata.pyx":40
+    /* "av/sidedata/sidedata.pyx":42
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)             # <<<<<<<<<<<<<<
  *     else:
  *         return SideData(_cinit_bypass_sentinel, frame, index)
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MotionVectors); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MotionVectors); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2316,94 +2326,94 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel, ((PyObject *)__pyx_v_frame), __pyx_t_5};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel, ((PyObject *)__pyx_v_frame), __pyx_t_5};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_6) {
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_INCREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
       __Pyx_GIVEREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
       __Pyx_INCREF(((PyObject *)__pyx_v_frame));
       __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, ((PyObject *)__pyx_v_frame));
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_2av_8sidedata_8sidedata_SideData))))) __PYX_ERR(0, 40, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_2av_8sidedata_8sidedata_SideData))))) __PYX_ERR(0, 42, __pyx_L1_error)
     __pyx_r = ((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "av/sidedata/sidedata.pyx":39
+    /* "av/sidedata/sidedata.pyx":41
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:             # <<<<<<<<<<<<<<
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  *     else:
  */
   }
 
-  /* "av/sidedata/sidedata.pyx":42
+  /* "av/sidedata/sidedata.pyx":44
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  *     else:
  *         return SideData(_cinit_bypass_sentinel, frame, index)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
     __Pyx_GIVEREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
     __Pyx_INCREF(((PyObject *)__pyx_v_frame));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
     PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_frame));
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata_SideData), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata_SideData), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = ((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "av/sidedata/sidedata.pyx":36
+  /* "av/sidedata/sidedata.pyx":38
  * 
  * 
  * cdef SideData wrap_side_data(Frame frame, int index):             # <<<<<<<<<<<<<<
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  */
 
@@ -2418,15 +2428,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":47
+/* "av/sidedata/sidedata.pyx":49
  * cdef class SideData(Buffer):
  * 
  *     def __init__(self, sentinel, Frame frame, int index):             # <<<<<<<<<<<<<<
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')
  */
 
@@ -2463,46 +2473,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sentinel)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 47, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 49, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 47, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 49, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 47, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 49, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_sentinel = values[0];
     __pyx_v_frame = ((struct __pyx_obj_2av_5frame_Frame *)values[1]);
-    __pyx_v_index = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_index == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
+    __pyx_v_index = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_index == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 47, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 49, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.sidedata.sidedata.SideData.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 49, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_8sidedata_8sidedata_8SideData___init__(((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_v_self), __pyx_v_sentinel, __pyx_v_frame, __pyx_v_index);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -2517,85 +2527,85 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "av/sidedata/sidedata.pyx":48
+  /* "av/sidedata/sidedata.pyx":50
  * 
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame
  */
   __pyx_t_1 = (__pyx_v_sentinel != __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/sidedata/sidedata.pyx":49
+    /* "av/sidedata/sidedata.pyx":51
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')             # <<<<<<<<<<<<<<
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 49, __pyx_L1_error)
+    __PYX_ERR(0, 51, __pyx_L1_error)
 
-    /* "av/sidedata/sidedata.pyx":48
+    /* "av/sidedata/sidedata.pyx":50
  * 
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame
  */
   }
 
-  /* "av/sidedata/sidedata.pyx":50
+  /* "av/sidedata/sidedata.pyx":52
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame             # <<<<<<<<<<<<<<
  *         self.ptr = frame.ptr.side_data[index]
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_frame));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
   __Pyx_GOTREF(__pyx_v_self->frame);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->frame));
   __pyx_v_self->frame = __pyx_v_frame;
 
-  /* "av/sidedata/sidedata.pyx":51
+  /* "av/sidedata/sidedata.pyx":53
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]             # <<<<<<<<<<<<<<
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  * 
  */
   __pyx_v_self->ptr = (__pyx_v_frame->ptr->side_data[__pyx_v_index]);
 
-  /* "av/sidedata/sidedata.pyx":52
+  /* "av/sidedata/sidedata.pyx":54
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]
  *         self.metadata = wrap_dictionary(self.ptr.metadata)             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t _buffer_size(self):
  */
-  __pyx_t_3 = ((PyObject *)__pyx_f_2av_10dictionary_wrap_dictionary(__pyx_v_self->ptr->metadata)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)__pyx_f_2av_10dictionary_wrap_dictionary(__pyx_v_self->ptr->metadata)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->metadata);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->metadata));
   __pyx_v_self->metadata = ((struct __pyx_obj_2av_10dictionary__Dictionary *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "av/sidedata/sidedata.pyx":47
+  /* "av/sidedata/sidedata.pyx":49
  * cdef class SideData(Buffer):
  * 
  *     def __init__(self, sentinel, Frame frame, int index):             # <<<<<<<<<<<<<<
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')
  */
 
@@ -2607,126 +2617,126 @@
   __Pyx_AddTraceback("av.sidedata.sidedata.SideData.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":54
+/* "av/sidedata/sidedata.pyx":56
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  * 
  *     cdef size_t _buffer_size(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.size
  * 
  */
 
 static size_t __pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_size(struct __pyx_obj_2av_8sidedata_8sidedata_SideData *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_buffer_size", 0);
 
-  /* "av/sidedata/sidedata.pyx":55
+  /* "av/sidedata/sidedata.pyx":57
  * 
  *     cdef size_t _buffer_size(self):
  *         return self.ptr.size             # <<<<<<<<<<<<<<
  * 
  *     cdef void* _buffer_ptr(self):
  */
   __pyx_r = __pyx_v_self->ptr->size;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":54
+  /* "av/sidedata/sidedata.pyx":56
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  * 
  *     cdef size_t _buffer_size(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.size
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":57
+/* "av/sidedata/sidedata.pyx":59
  *         return self.ptr.size
  * 
  *     cdef void* _buffer_ptr(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.data
  * 
  */
 
 static void *__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_ptr(struct __pyx_obj_2av_8sidedata_8sidedata_SideData *__pyx_v_self) {
   void *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_buffer_ptr", 0);
 
-  /* "av/sidedata/sidedata.pyx":58
+  /* "av/sidedata/sidedata.pyx":60
  * 
  *     cdef void* _buffer_ptr(self):
  *         return self.ptr.data             # <<<<<<<<<<<<<<
  * 
  *     cdef bint _buffer_writable(self):
  */
   __pyx_r = __pyx_v_self->ptr->data;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":57
+  /* "av/sidedata/sidedata.pyx":59
  *         return self.ptr.size
  * 
  *     cdef void* _buffer_ptr(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.data
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":60
+/* "av/sidedata/sidedata.pyx":62
  *         return self.ptr.data
  * 
  *     cdef bint _buffer_writable(self):             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
 
 static int __pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_writable(CYTHON_UNUSED struct __pyx_obj_2av_8sidedata_8sidedata_SideData *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_buffer_writable", 0);
 
-  /* "av/sidedata/sidedata.pyx":61
+  /* "av/sidedata/sidedata.pyx":63
  * 
  *     cdef bint _buffer_writable(self):
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":60
+  /* "av/sidedata/sidedata.pyx":62
  *         return self.ptr.data
  * 
  *     cdef bint _buffer_writable(self):             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":63
+/* "av/sidedata/sidedata.pyx":65
  *         return False
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<av.sidedata.{self.__class__.__name__} {self.ptr.size} bytes of {self.type} at 0x{<unsigned int>self.ptr.data:0x}>'
  * 
  */
 
@@ -2752,93 +2762,93 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "av/sidedata/sidedata.pyx":64
+  /* "av/sidedata/sidedata.pyx":66
  * 
  *     def __repr__(self):
  *         return f'<av.sidedata.{self.__class__.__name__} {self.ptr.size} bytes of {self.type} at 0x{<unsigned int>self.ptr.data:0x}>'             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_av_sidedata);
   __pyx_t_2 += 13;
   __Pyx_GIVEREF(__pyx_kp_u_av_sidedata);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_av_sidedata);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__2);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__2);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__2);
-  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->ptr->size, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->ptr->size, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u_bytes_of);
   __pyx_t_2 += 10;
   __Pyx_GIVEREF(__pyx_kp_u_bytes_of);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_bytes_of);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_kp_u_at_0x);
   __pyx_t_2 += 6;
   __Pyx_GIVEREF(__pyx_kp_u_at_0x);
   PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_kp_u_at_0x);
-  __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(((unsigned int)__pyx_v_self->ptr->data)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(((unsigned int)__pyx_v_self->ptr->data)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_kp_u_0x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_kp_u_0x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__3);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__3);
   PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_kp_u__3);
-  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":63
+  /* "av/sidedata/sidedata.pyx":65
  *         return False
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<av.sidedata.{self.__class__.__name__} {self.ptr.size} bytes of {self.type} at 0x{<unsigned int>self.ptr.data:0x}>'
  * 
  */
 
@@ -2851,15 +2861,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":67
+/* "av/sidedata/sidedata.pyx":69
  * 
  *     @property
  *     def type(self):             # <<<<<<<<<<<<<<
  *         return Type.get(self.ptr.type) or self.ptr.type
  * 
  */
 
@@ -2886,64 +2896,64 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/sidedata/sidedata.pyx":68
+  /* "av/sidedata/sidedata.pyx":70
  *     @property
  *     def type(self):
  *         return Type.get(self.ptr.type) or self.ptr.type             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
   if (!__pyx_t_6) {
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":67
+  /* "av/sidedata/sidedata.pyx":69
  * 
  *     @property
  *     def type(self):             # <<<<<<<<<<<<<<
  *         return Type.get(self.ptr.type) or self.ptr.type
  * 
  */
 
@@ -3073,15 +3083,15 @@
   __Pyx_AddTraceback("av.sidedata.sidedata.SideData.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":73
+/* "av/sidedata/sidedata.pyx":75
  * cdef class _SideDataContainer(object):
  * 
  *     def __init__(self, Frame frame):             # <<<<<<<<<<<<<<
  * 
  *         self.frame = frame
  */
 
@@ -3110,32 +3120,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_frame = ((struct __pyx_obj_2av_5frame_Frame *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.sidedata.sidedata._SideDataContainer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 75, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_8sidedata_8sidedata_18_SideDataContainer___init__(((struct __pyx_obj_2av_8sidedata_8sidedata__SideDataContainer *)__pyx_v_self), __pyx_v_frame);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -3154,112 +3164,112 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "av/sidedata/sidedata.pyx":75
+  /* "av/sidedata/sidedata.pyx":77
  *     def __init__(self, Frame frame):
  * 
  *         self.frame = frame             # <<<<<<<<<<<<<<
  *         self._by_index = []
  *         self._by_type = {}
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_frame));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
   __Pyx_GOTREF(__pyx_v_self->frame);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->frame));
   __pyx_v_self->frame = __pyx_v_frame;
 
-  /* "av/sidedata/sidedata.pyx":76
+  /* "av/sidedata/sidedata.pyx":78
  * 
  *         self.frame = frame
  *         self._by_index = []             # <<<<<<<<<<<<<<
  *         self._by_type = {}
  * 
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_by_index);
   __Pyx_DECREF(__pyx_v_self->_by_index);
   __pyx_v_self->_by_index = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/sidedata/sidedata.pyx":77
+  /* "av/sidedata/sidedata.pyx":79
  *         self.frame = frame
  *         self._by_index = []
  *         self._by_type = {}             # <<<<<<<<<<<<<<
  * 
  *         cdef int i
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_by_type);
   __Pyx_DECREF(__pyx_v_self->_by_type);
   __pyx_v_self->_by_type = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/sidedata/sidedata.pyx":81
+  /* "av/sidedata/sidedata.pyx":83
  *         cdef int i
  *         cdef SideData data
  *         for i in range(self.frame.ptr.nb_side_data):             # <<<<<<<<<<<<<<
  *             data = wrap_side_data(frame, i)
  *             self._by_index.append(data)
  */
   __pyx_t_2 = __pyx_v_self->frame->ptr->nb_side_data;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "av/sidedata/sidedata.pyx":82
+    /* "av/sidedata/sidedata.pyx":84
  *         cdef SideData data
  *         for i in range(self.frame.ptr.nb_side_data):
  *             data = wrap_side_data(frame, i)             # <<<<<<<<<<<<<<
  *             self._by_index.append(data)
  *             self._by_type[data.type] = data
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_2av_8sidedata_8sidedata_wrap_side_data(__pyx_v_frame, __pyx_v_i)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_2av_8sidedata_8sidedata_wrap_side_data(__pyx_v_frame, __pyx_v_i)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_data, ((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "av/sidedata/sidedata.pyx":83
+    /* "av/sidedata/sidedata.pyx":85
  *         for i in range(self.frame.ptr.nb_side_data):
  *             data = wrap_side_data(frame, i)
  *             self._by_index.append(data)             # <<<<<<<<<<<<<<
  *             self._by_type[data.type] = data
  * 
  */
     if (unlikely(__pyx_v_self->_by_index == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-      __PYX_ERR(0, 83, __pyx_L1_error)
+      __PYX_ERR(0, 85, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_self->_by_index, ((PyObject *)__pyx_v_data)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_self->_by_index, ((PyObject *)__pyx_v_data)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 85, __pyx_L1_error)
 
-    /* "av/sidedata/sidedata.pyx":84
+    /* "av/sidedata/sidedata.pyx":86
  *             data = wrap_side_data(frame, i)
  *             self._by_index.append(data)
  *             self._by_type[data.type] = data             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
     if (unlikely(__pyx_v_self->_by_type == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 84, __pyx_L1_error)
+      __PYX_ERR(0, 86, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_self->_by_type, __pyx_t_1, ((PyObject *)__pyx_v_data)) < 0)) __PYX_ERR(0, 84, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_self->_by_type, __pyx_t_1, ((PyObject *)__pyx_v_data)) < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "av/sidedata/sidedata.pyx":73
+  /* "av/sidedata/sidedata.pyx":75
  * cdef class _SideDataContainer(object):
  * 
  *     def __init__(self, Frame frame):             # <<<<<<<<<<<<<<
  * 
  *         self.frame = frame
  */
 
@@ -3272,15 +3282,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":86
+/* "av/sidedata/sidedata.pyx":88
  *             self._by_type[data.type] = data
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self._by_index)
  * 
  */
 
@@ -3303,33 +3313,33 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "av/sidedata/sidedata.pyx":87
+  /* "av/sidedata/sidedata.pyx":89
  * 
  *     def __len__(self):
  *         return len(self._by_index)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_t_1 = __pyx_v_self->_by_index;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 87, __pyx_L1_error)
+    __PYX_ERR(0, 89, __pyx_L1_error)
   }
-  __pyx_t_2 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_2 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":86
+  /* "av/sidedata/sidedata.pyx":88
  *             self._by_type[data.type] = data
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self._by_index)
  * 
  */
 
@@ -3339,15 +3349,15 @@
   __Pyx_AddTraceback("av.sidedata.sidedata._SideDataContainer.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":89
+/* "av/sidedata/sidedata.pyx":91
  *         return len(self._by_index)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self._by_index)
  * 
  */
 
@@ -3370,32 +3380,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "av/sidedata/sidedata.pyx":90
+  /* "av/sidedata/sidedata.pyx":92
  * 
  *     def __iter__(self):
  *         return iter(self._by_index)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, key):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->_by_index;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":89
+  /* "av/sidedata/sidedata.pyx":91
  *         return len(self._by_index)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self._by_index)
  * 
  */
 
@@ -3407,15 +3417,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":92
+/* "av/sidedata/sidedata.pyx":94
  *         return iter(self._by_index)
  * 
  *     def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(key, int):
  */
 
@@ -3442,101 +3452,101 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "av/sidedata/sidedata.pyx":94
+  /* "av/sidedata/sidedata.pyx":96
  *     def __getitem__(self, key):
  * 
  *         if isinstance(key, int):             # <<<<<<<<<<<<<<
  *             return self._by_index[key]
  * 
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_key); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/sidedata/sidedata.pyx":95
+    /* "av/sidedata/sidedata.pyx":97
  * 
  *         if isinstance(key, int):
  *             return self._by_index[key]             # <<<<<<<<<<<<<<
  * 
  *         type_ = Type.get(key)
  */
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_self->_by_index == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 95, __pyx_L1_error)
+      __PYX_ERR(0, 97, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_by_index, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_by_index, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "av/sidedata/sidedata.pyx":94
+    /* "av/sidedata/sidedata.pyx":96
  *     def __getitem__(self, key):
  * 
  *         if isinstance(key, int):             # <<<<<<<<<<<<<<
  *             return self._by_index[key]
  * 
  */
   }
 
-  /* "av/sidedata/sidedata.pyx":97
+  /* "av/sidedata/sidedata.pyx":99
  *             return self._by_index[key]
  * 
  *         type_ = Type.get(key)             # <<<<<<<<<<<<<<
  *         return self._by_type[type_]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_key);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_type_ = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "av/sidedata/sidedata.pyx":98
+  /* "av/sidedata/sidedata.pyx":100
  * 
  *         type_ = Type.get(key)
  *         return self._by_type[type_]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_self->_by_type == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 98, __pyx_L1_error)
+    __PYX_ERR(0, 100, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->_by_type, __pyx_v_type_); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->_by_type, __pyx_v_type_); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":92
+  /* "av/sidedata/sidedata.pyx":94
  *         return iter(self._by_index)
  * 
  *     def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(key, int):
  */
 
@@ -4663,14 +4673,15 @@
   {&__pyx_n_s_MOTION_VECTORS, __pyx_k_MOTION_VECTORS, sizeof(__pyx_k_MOTION_VECTORS), 0, 0, 1, 1},
   {&__pyx_n_s_Mapping, __pyx_k_Mapping, sizeof(__pyx_k_Mapping), 0, 0, 1, 1},
   {&__pyx_n_s_MotionVectors, __pyx_k_MotionVectors, sizeof(__pyx_k_MotionVectors), 0, 0, 1, 1},
   {&__pyx_n_s_PANSCAN, __pyx_k_PANSCAN, sizeof(__pyx_k_PANSCAN), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_REPLAYGAIN, __pyx_k_REPLAYGAIN, sizeof(__pyx_k_REPLAYGAIN), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
+  {&__pyx_n_s_SEI_UNREGISTERED, __pyx_k_SEI_UNREGISTERED, sizeof(__pyx_k_SEI_UNREGISTERED), 0, 0, 1, 1},
   {&__pyx_n_s_SKIP_SAMPLES, __pyx_k_SKIP_SAMPLES, sizeof(__pyx_k_SKIP_SAMPLES), 0, 0, 1, 1},
   {&__pyx_n_s_SPHERICAL, __pyx_k_SPHERICAL, sizeof(__pyx_k_SPHERICAL), 0, 0, 1, 1},
   {&__pyx_n_s_STEREO3D, __pyx_k_STEREO3D, sizeof(__pyx_k_STEREO3D), 0, 0, 1, 1},
   {&__pyx_n_s_SideData, __pyx_k_SideData, sizeof(__pyx_k_SideData), 0, 0, 1, 1},
   {&__pyx_n_s_SideDataContainer, __pyx_k_SideDataContainer, sizeof(__pyx_k_SideDataContainer), 0, 0, 1, 1},
   {&__pyx_n_s_SideDataContainer_2, __pyx_k_SideDataContainer_2, sizeof(__pyx_k_SideDataContainer_2), 0, 0, 1, 1},
   {&__pyx_n_s_Type, __pyx_k_Type, sizeof(__pyx_k_Type), 0, 0, 1, 1},
@@ -4721,34 +4732,34 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 8, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 51, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 83, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "av/sidedata/sidedata.pyx":49
+  /* "av/sidedata/sidedata.pyx":51
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')             # <<<<<<<<<<<<<<
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_cannot_manually_instatiate_SideD); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_cannot_manually_instatiate_SideD); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.ptr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -4846,34 +4857,34 @@
   __pyx_vtabptr_2av_6buffer_Buffer = (struct __pyx_vtabstruct_2av_6buffer_Buffer*)__Pyx_GetVtable(__pyx_ptype_2av_6buffer_Buffer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_6buffer_Buffer)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_2av_8sidedata_8sidedata_SideData = &__pyx_vtable_2av_8sidedata_8sidedata_SideData;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base = *__pyx_vtabptr_2av_6buffer_Buffer;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base._buffer_size = (size_t (*)(struct __pyx_obj_2av_6buffer_Buffer *))__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_size;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base._buffer_ptr = (void *(*)(struct __pyx_obj_2av_6buffer_Buffer *))__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_ptr;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base._buffer_writable = (int (*)(struct __pyx_obj_2av_6buffer_Buffer *))__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_writable;
   __pyx_type_2av_8sidedata_8sidedata_SideData.tp_base = __pyx_ptype_2av_6buffer_Buffer;
-  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_8sidedata_8sidedata_SideData.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_8sidedata_8sidedata_SideData.tp_dictoffset && __pyx_type_2av_8sidedata_8sidedata_SideData.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_8sidedata_8sidedata_SideData.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2av_8sidedata_8sidedata_SideData.tp_dict, __pyx_vtabptr_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideData, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2av_8sidedata_8sidedata_SideData.tp_dict, __pyx_vtabptr_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideData, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_ptype_2av_8sidedata_8sidedata_SideData = &__pyx_type_2av_8sidedata_8sidedata_SideData;
-  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_dictoffset && __pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideDataContainer, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideDataContainer, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer = &__pyx_type_2av_8sidedata_8sidedata__SideDataContainer;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -5099,14 +5110,16 @@
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -5527,15 +5540,15 @@
   __pyx_t_2 = 0;
 
   /* "av/sidedata/sidedata.pyx":26
  *     ('GOP_TIMECODE', lib.AV_FRAME_DATA_GOP_TIMECODE),
  *     ('SPHERICAL', lib.AV_FRAME_DATA_SPHERICAL),
  *     ('CONTENT_LIGHT_LEVEL', lib.AV_FRAME_DATA_CONTENT_LIGHT_LEVEL),             # <<<<<<<<<<<<<<
  *     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),
- * 
+ *     # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
  */
   __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(AV_FRAME_DATA_CONTENT_LIGHT_LEVEL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_17 = PyTuple_New(2); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_INCREF(__pyx_n_s_CONTENT_LIGHT_LEVEL);
   __Pyx_GIVEREF(__pyx_n_s_CONTENT_LIGHT_LEVEL);
@@ -5544,69 +5557,96 @@
   PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "av/sidedata/sidedata.pyx":27
  *     ('SPHERICAL', lib.AV_FRAME_DATA_SPHERICAL),
  *     ('CONTENT_LIGHT_LEVEL', lib.AV_FRAME_DATA_CONTENT_LIGHT_LEVEL),
  *     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),             # <<<<<<<<<<<<<<
- * 
- *     # These are deprecated. See https://github.com/PyAV-Org/PyAV/issues/607
+ *     # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+ *     ('SEI_UNREGISTERED', lib.AV_FRAME_DATA_SEI_UNREGISTERED) if lib.AV_FRAME_DATA_SEI_UNREGISTERED != -1 else None,
  */
   __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(AV_FRAME_DATA_ICC_PROFILE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_n_s_ICC_PROFILE);
   __Pyx_GIVEREF(__pyx_n_s_ICC_PROFILE);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_n_s_ICC_PROFILE);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_2);
   __pyx_t_2 = 0;
 
+  /* "av/sidedata/sidedata.pyx":29
+ *     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),
+ *     # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+ *     ('SEI_UNREGISTERED', lib.AV_FRAME_DATA_SEI_UNREGISTERED) if lib.AV_FRAME_DATA_SEI_UNREGISTERED != -1 else None,             # <<<<<<<<<<<<<<
+ * 
+ *     # These are deprecated. See https://github.com/PyAV-Org/PyAV/issues/607
+ */
+  if (((AV_FRAME_DATA_SEI_UNREGISTERED != -1L) != 0)) {
+    __pyx_t_19 = __Pyx_PyInt_From_enum__AVFrameSideDataType(AV_FRAME_DATA_SEI_UNREGISTERED); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
+    __pyx_t_20 = PyTuple_New(2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_20);
+    __Pyx_INCREF(__pyx_n_s_SEI_UNREGISTERED);
+    __Pyx_GIVEREF(__pyx_n_s_SEI_UNREGISTERED);
+    PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_n_s_SEI_UNREGISTERED);
+    __Pyx_GIVEREF(__pyx_t_19);
+    PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_19);
+    __pyx_t_19 = 0;
+    __pyx_t_2 = __pyx_t_20;
+    __pyx_t_20 = 0;
+  } else {
+    __Pyx_INCREF(Py_None);
+    __pyx_t_2 = Py_None;
+  }
+
   /* "av/sidedata/sidedata.pyx":12
  * 
  * Type = define_enum('Type', __name__, (
  *     ('PANSCAN', lib.AV_FRAME_DATA_PANSCAN),             # <<<<<<<<<<<<<<
  *     ('A53_CC', lib.AV_FRAME_DATA_A53_CC),
  *     ('STEREO3D', lib.AV_FRAME_DATA_STEREO3D),
  */
-  __pyx_t_2 = PyTuple_New(16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_20 = PyTuple_New(17); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_20, 2, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_20, 3, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_20, 4, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_20, 5, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_20, 6, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_t_10);
+  PyTuple_SET_ITEM(__pyx_t_20, 7, __pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_2, 8, __pyx_t_11);
+  PyTuple_SET_ITEM(__pyx_t_20, 8, __pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_12);
-  PyTuple_SET_ITEM(__pyx_t_2, 9, __pyx_t_12);
+  PyTuple_SET_ITEM(__pyx_t_20, 9, __pyx_t_12);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_2, 10, __pyx_t_13);
+  PyTuple_SET_ITEM(__pyx_t_20, 10, __pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_14);
-  PyTuple_SET_ITEM(__pyx_t_2, 11, __pyx_t_14);
+  PyTuple_SET_ITEM(__pyx_t_20, 11, __pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_15);
-  PyTuple_SET_ITEM(__pyx_t_2, 12, __pyx_t_15);
+  PyTuple_SET_ITEM(__pyx_t_20, 12, __pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_16);
-  PyTuple_SET_ITEM(__pyx_t_2, 13, __pyx_t_16);
+  PyTuple_SET_ITEM(__pyx_t_20, 13, __pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_17);
-  PyTuple_SET_ITEM(__pyx_t_2, 14, __pyx_t_17);
+  PyTuple_SET_ITEM(__pyx_t_20, 14, __pyx_t_17);
   __Pyx_GIVEREF(__pyx_t_18);
-  PyTuple_SET_ITEM(__pyx_t_2, 15, __pyx_t_18);
+  PyTuple_SET_ITEM(__pyx_t_20, 15, __pyx_t_18);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_20, 16, __pyx_t_2);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
@@ -5615,76 +5655,77 @@
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
   __pyx_t_16 = 0;
   __pyx_t_17 = 0;
   __pyx_t_18 = 0;
+  __pyx_t_2 = 0;
 
   /* "av/sidedata/sidedata.pyx":11
  * 
  * 
  * Type = define_enum('Type', __name__, (             # <<<<<<<<<<<<<<
  *     ('PANSCAN', lib.AV_FRAME_DATA_PANSCAN),
  *     ('A53_CC', lib.AV_FRAME_DATA_A53_CC),
  */
-  __pyx_t_18 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Type, __pyx_t_1, __pyx_t_2, 0, NULL); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_18);
+  __pyx_t_2 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Type, __pyx_t_1, __pyx_t_20, 0, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Type, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Type, __pyx_t_18) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
 
-  /* "av/sidedata/sidedata.pyx":101
+  /* "av/sidedata/sidedata.pyx":103
  * 
  * 
  * class SideDataContainer(_SideDataContainer, Mapping):             # <<<<<<<<<<<<<<
  *     pass
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_20 = PyTuple_New(2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
-  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
-  __Pyx_GIVEREF(__pyx_t_18);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_18);
-  __pyx_t_18 = 0;
-  __pyx_t_18 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_18, __pyx_t_2, __pyx_n_s_SideDataContainer_2, __pyx_n_s_SideDataContainer_2, (PyObject *) NULL, __pyx_n_s_av_sidedata_sidedata, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_20, 0, ((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_20, __pyx_n_s_SideDataContainer_2, __pyx_n_s_SideDataContainer_2, (PyObject *) NULL, __pyx_n_s_av_sidedata_sidedata, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_17 = __Pyx_Py3ClassCreate(__pyx_t_18, __pyx_n_s_SideDataContainer_2, __pyx_t_2, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_17);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SideDataContainer_2, __pyx_t_17) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_18 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SideDataContainer_2, __pyx_t_20, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_18);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SideDataContainer_2, __pyx_t_18) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle__SideDataContainer(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2av_8sidedata_8sidedata_1__pyx_unpickle__SideDataContainer, NULL, __pyx_n_s_av_sidedata_sidedata); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle__SideDataContaine, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_20 = PyCFunction_NewEx(&__pyx_mdef_2av_8sidedata_8sidedata_1__pyx_unpickle__SideDataContainer, NULL, __pyx_n_s_av_sidedata_sidedata); if (unlikely(!__pyx_t_20)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle__SideDataContaine, __pyx_t_20) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /* "av/sidedata/sidedata.pyx":1
  * from av.enum cimport define_enum             # <<<<<<<<<<<<<<
  * 
  * from collections.abc import Mapping
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_20 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_20) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -5700,14 +5741,16 @@
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_XDECREF(__pyx_t_18);
+  __Pyx_XDECREF(__pyx_t_19);
+  __Pyx_XDECREF(__pyx_t_20);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init av.sidedata.sidedata", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init av.sidedata.sidedata");
```

### Comparing `ha-av-9.1.1.post3/src/av/stream.c` & `ha-av-9.2.0.post1/src/av/stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/subtitles/codeccontext.c` & `ha-av-9.2.0.post1/src/av/subtitles/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/subtitles/stream.c` & `ha-av-9.2.0.post1/src/av/subtitles/stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/subtitles/subtitle.c` & `ha-av-9.2.0.post1/src/av/subtitles/subtitle.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/utils.c` & `ha-av-9.2.0.post1/src/av/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/video/codeccontext.c` & `ha-av-9.2.0.post1/src/av/video/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/video/format.c` & `ha-av-9.2.0.post1/src/av/video/format.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/video/frame.c` & `ha-av-9.2.0.post1/src/av/video/frame.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/video/plane.c` & `ha-av-9.2.0.post1/src/av/video/plane.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/video/reformatter.c` & `ha-av-9.2.0.post1/src/av/video/reformatter.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/src/av/video/stream.c` & `ha-av-9.2.0.post1/src/av/video/stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `ha-av-9.1.1.post3/tests/common.py` & `ha-av-9.2.0.post1/tests/common.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_audiofifo.py` & `ha-av-9.2.0.post1/tests/test_audiofifo.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_audioformat.py` & `ha-av-9.2.0.post1/tests/test_audioformat.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_audioframe.py` & `ha-av-9.2.0.post1/tests/test_audioframe.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_audiolayout.py` & `ha-av-9.2.0.post1/tests/test_audiolayout.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_audioresampler.py` & `ha-av-9.2.0.post1/tests/test_audioresampler.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_codec.py` & `ha-av-9.2.0.post1/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_codec_context.py` & `ha-av-9.2.0.post1/tests/test_codec_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from fractions import Fraction
 from unittest import SkipTest
 import os
+import warnings
 
 from av import AudioResampler, Codec, Packet
 from av.codec.codec import UnknownCodecError
 from av.video.frame import PictureType
 import av
 
 from .common import TestCase, fate_suite
@@ -75,14 +76,31 @@
         self.assertEqual(ctx.extradata, b"54321")
         self.assertEqual(ctx.extradata_size, 5)
 
         ctx.extradata = None
         self.assertEqual(ctx.extradata, None)
         self.assertEqual(ctx.extradata_size, 0)
 
+    def test_decoder_timebase(self):
+        ctx = av.codec.Codec("h264", "r").create()
+
+        with warnings.catch_warnings(record=True) as captured:
+            self.assertIsNone(ctx.time_base)
+            self.assertEqual(
+                captured[0].message.args[0],
+                "Using CodecContext.time_base for decoders is deprecated.",
+            )
+
+        with warnings.catch_warnings(record=True) as captured:
+            ctx.time_base = Fraction(1, 25)
+            self.assertEqual(
+                captured[0].message.args[0],
+                "Using CodecContext.time_base for decoders is deprecated.",
+            )
+
     def test_encoder_extradata(self):
         ctx = av.codec.Codec("h264", "w").create()
         self.assertEqual(ctx.extradata, None)
         self.assertEqual(ctx.extradata_size, 0)
 
         with self.assertRaises(ValueError) as cm:
             ctx.extradata = b"123"
@@ -353,15 +371,14 @@
                         f.write(packet)
 
             for packet in ctx.encode(None):
                 packet_sizes.append(packet.size)
                 f.write(packet)
 
         ctx = Codec(codec_name, "r").create()
-        ctx.time_base = Fraction(1) / sample_rate
         ctx.sample_rate = sample_rate
         ctx.format = sample_fmt
         ctx.layout = channel_layout
         ctx.channels = channels
         ctx.open()
 
         result_samples = 0
```

### Comparing `ha-av-9.1.1.post3/tests/test_containerformat.py` & `ha-av-9.2.0.post1/tests/test_containerformat.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_decode.py` & `ha-av-9.2.0.post1/tests/test_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from fractions import Fraction
+
 import av
 
 from .common import TestCase, fate_suite
 
 
 class TestDecode(TestCase):
     def test_decoded_video_frame_count(self):
@@ -55,17 +57,16 @@
         ) / audio_stream.time_base.denominator
         self.assertEqual(sample_count, total_samples)
 
     def test_decoded_time_base(self):
 
         container = av.open(fate_suite("h264/interlaced_crop.mp4"))
         stream = container.streams.video[0]
-        codec_context = stream.codec_context
 
-        self.assertNotEqual(stream.time_base, codec_context.time_base)
+        self.assertEqual(stream.time_base, Fraction(1, 25))
 
         for packet in container.demux(stream):
             for frame in packet.decode():
                 self.assertEqual(packet.time_base, frame.time_base)
                 self.assertEqual(stream.time_base, frame.time_base)
                 return
```

### Comparing `ha-av-9.1.1.post3/tests/test_deprecation.py` & `ha-av-9.2.0.post1/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_doctests.py` & `ha-av-9.2.0.post1/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_encode.py` & `ha-av-9.2.0.post1/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_enums.py` & `ha-av-9.2.0.post1/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_errors.py` & `ha-av-9.2.0.post1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_file_probing.py` & `ha-av-9.2.0.post1/tests/test_file_probing.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_filters.py` & `ha-av-9.2.0.post1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_logging.py` & `ha-av-9.2.0.post1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_options.py` & `ha-av-9.2.0.post1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_python_io.py` & `ha-av-9.2.0.post1/tests/test_python_io.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_seek.py` & `ha-av-9.2.0.post1/tests/test_seek.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_streams.py` & `ha-av-9.2.0.post1/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_subtitles.py` & `ha-av-9.2.0.post1/tests/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_timeout.py` & `ha-av-9.2.0.post1/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_videoformat.py` & `ha-av-9.2.0.post1/tests/test_videoformat.py`

 * *Files identical despite different names*

### Comparing `ha-av-9.1.1.post3/tests/test_videoframe.py` & `ha-av-9.2.0.post1/tests/test_videoframe.py`

 * *Files identical despite different names*

