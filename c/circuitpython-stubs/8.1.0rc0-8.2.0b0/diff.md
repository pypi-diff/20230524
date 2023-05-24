# Comparing `tmp/circuitpython-stubs-8.1.0rc0.tar.gz` & `tmp/circuitpython-stubs-8.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.1.0rc0.tar", last modified: Tue May 16 23:35:58 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.2.0b0.tar", last modified: Wed May 24 15:46:21 2023, max compression
```

## Comparing `circuitpython-stubs-8.1.0rc0.tar` & `circuitpython-stubs-8.2.0b0.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-16 23:35:58.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.626046 circuitpython-stubs-8.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 15:46:21.626046 circuitpython-stubs-8.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-24 15:46:21.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:46:21.626046 circuitpython-stubs-8.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.1.0rc0/README.rst` & `circuitpython-stubs-8.2.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/_bleio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/_eve/__init__.pyi` & `circuitpython-stubs-8.2.0b0/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/_pew/__init__.pyi` & `circuitpython-stubs-8.2.0b0/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.2.0b0/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/_stage/__init__.pyi` & `circuitpython-stubs-8.2.0b0/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.2.0b0/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.2.0b0/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.2.0b0/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/aesio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/alarm/__init__.pyi` & `circuitpython-stubs-8.2.0b0/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.2.0b0/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/alarm/time/__init__.pyi` & `circuitpython-stubs-8.2.0b0/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.2.0b0/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/analogbufio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/analogio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/atexit/__init__.pyi` & `circuitpython-stubs-8.2.0b0/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/audiobusio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/audiocore/__init__.pyi` & `circuitpython-stubs-8.2.0b0/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/audioio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/audiomixer/__init__.pyi` & `circuitpython-stubs-8.2.0b0/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/audiomp3/__init__.pyi` & `circuitpython-stubs-8.2.0b0/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/bitbangio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.2.0b0/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/bitops/__init__.pyi` & `circuitpython-stubs-8.2.0b0/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/board/__init__.pyi` & `circuitpython-stubs-8.2.0b0/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/busio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/camera/__init__.pyi` & `circuitpython-stubs-8.2.0b0/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/canio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/countio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/cyw43/__init__.pyi` & `circuitpython-stubs-8.2.0b0/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/digitalio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/displayio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/dualbank/__init__.pyi` & `circuitpython-stubs-8.2.0b0/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/espcamera/__init__.pyi` & `circuitpython-stubs-8.2.0b0/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/espidf/__init__.pyi` & `circuitpython-stubs-8.2.0b0/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/espnow/__init__.pyi` & `circuitpython-stubs-8.2.0b0/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/espulp/__init__.pyi` & `circuitpython-stubs-8.2.0b0/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/floppyio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/fontio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/framebufferio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/frequencyio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/getpass/__init__.pyi` & `circuitpython-stubs-8.2.0b0/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/gifio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/gnss/__init__.pyi` & `circuitpython-stubs-8.2.0b0/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/hashlib/__init__.pyi` & `circuitpython-stubs-8.2.0b0/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.2.0b0/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/imagecapture/__init__.pyi` & `circuitpython-stubs-8.2.0b0/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ipaddress/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.2.0b0/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/keypad/__init__.pyi` & `circuitpython-stubs-8.2.0b0/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/math/__init__.pyi` & `circuitpython-stubs-8.2.0b0/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/mdns/__init__.pyi` & `circuitpython-stubs-8.2.0b0/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/memorymap/__init__.pyi` & `circuitpython-stubs-8.2.0b0/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.2.0b0/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/microcontroller/__init__.pyi` & `circuitpython-stubs-8.2.0b0/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/msgpack/__init__.pyi` & `circuitpython-stubs-8.2.0b0/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.2.0b0/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/nvm/__init__.pyi` & `circuitpython-stubs-8.2.0b0/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/onewireio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/os/__init__.pyi` & `circuitpython-stubs-8.2.0b0/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.2.0b0/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/picodvi/__init__.pyi` & `circuitpython-stubs-8.2.0b0/picodvi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ps2io/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/pulseio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/pwmio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/qrio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/random/__init__.pyi` & `circuitpython-stubs-8.2.0b0/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.2.0b0/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/rotaryio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/rp2pio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/rtc/__init__.pyi` & `circuitpython-stubs-8.2.0b0/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/samd/__init__.pyi` & `circuitpython-stubs-8.2.0b0/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/sdcardio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/sdioio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/setup.py` & `circuitpython-stubs-8.2.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.2.0b0/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/socketpool/__init__.pyi` & `circuitpython-stubs-8.2.0b0/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ssl/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/storage/__init__.pyi` & `circuitpython-stubs-8.2.0b0/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/struct/__init__.pyi` & `circuitpython-stubs-8.2.0b0/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/supervisor/__init__.pyi` & `circuitpython-stubs-8.2.0b0/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/synthio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/synthio/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Support for multi-channel audio synthesis
 
 At least 2 simultaneous notes are supported.  samd5x, mimxrt10xx and rp2040 platforms support up to 12 notes.
-
 """
 
 from __future__ import annotations
 
 import typing
-from typing import Optional, Sequence, Union
+from typing import List, Optional, Sequence, Union
 
 from circuitpython_typing import ReadableBuffer
 
+BlockInput = Union["Math", "LFO", float, None]
+"""Blocks and Notes can take any of these types as inputs on certain attributes
+
+A BlockInput can be any of the following types: `Math`, `LFO`, `builtins.float`, `None` (treated same as 0).
+"""
+
 class Envelope:
     def __init__(
         self,
         *,
         attack_time: Optional[float] = 0.1,
         decay_time: Optional[float] = 0.05,
         release_time: Optional[float] = 0.2,
@@ -81,33 +86,168 @@
             pass
           print("stopped")"""
     ...
 
 def midi_to_hz(midi_note: float) -> float:
     """Converts the given midi note (60 = middle C, 69 = concert A) to Hz"""
 
-def onevo_to_hz(ctrl: float) -> float:
+def voct_to_hz(ctrl: float) -> float:
     """Converts a 1v/octave signal to Hz.
 
-    60/12 (5.0) corresponds to middle C, 69/12 is concert A."""
+    24/12 (2.0) corresponds to middle C, 33/12 (2.75) is concert A."""
+
+class LFO:
+    """A low-frequency oscillator block
+
+    Every `rate` seconds, the output of the LFO cycles through its `waveform`.
+    The output at any particular moment is ``waveform[idx] * scale + offset``.
+
+    If `waveform` is None, a triangle waveform is used.
+
+    `rate`, `phase_offset`, `offset`, `scale`, and `once` can be changed at run-time. `waveform` may be mutated.
+
+    `waveform` must be a ``ReadableBuffer`` with elements of type ``'h'``
+    (16-bit signed integer).  Internally, the elements of `waveform` are scaled
+    so that the input range ``[-32768,32767]`` maps to ``[-1.0, 0.99996]``.
+
+    An LFO only updates if it is actually associated with a playing `Synthesizer`,
+    including indirectly via a `Note` or another intermediate LFO.
+
+    Using the same LFO as an input to multiple other LFOs or Notes is OK, but
+    the result if an LFO is tied to multiple Synthtesizer objects is undefined.
+
+    In the current implementation, LFOs are updated every 256 samples. This
+    should be considered an implementation detail, though it affects how LFOs
+    behave for instance when used to implement an integrator (``l.offset = l``).
+    """
+
+    def __init__(
+        self,
+        waveform: ReadableBuffer = None,
+        *,
+        rate: BlockInput = 1.0,
+        scale: BlockInput = 1.0,
+        offset: BlockInput = 0.0,
+        phase_offset: BlockInput = 0.0,
+        once=False,
+        interpolate=True,
+    ):
+        pass
+    waveform: Optional[ReadableBuffer]
+    """The waveform of this lfo. (read-only, but the values in the buffer may be modified dynamically)"""
+    rate: BlockInput
+    """The rate (in Hz) at which the LFO cycles through its waveform"""
+    offset: BlockInput
+    """An additive value applied to the LFO's output"""
+    phase_offset: BlockInput
+    """An additive value applied to the LFO's phase"""
+    scale: BlockInput
+    """An multiplier value applied to the LFO's output"""
+
+    once: bool
+    """True if the waveform should stop when it reaches its last output value, false if it should re-start at the beginning of its waveform
+
+    This applies to the ``phase`` *before* the addition of any ``phase_offset`` """
+
+    interpolate: bool
+    """True if the waveform should perform linear interpolation between values"""
+
+    phase: float
+    """The phase of the oscillator, in the range 0 to 1 (read-only)"""
+
+    value: float
+    """The value of the oscillator (read-only)"""
+
+    def retrigger(self):
+        """Reset the LFO's internal index to the start of the waveform. Most useful when it its `once` property is `True`."""
+
+class MathOperation:
+    """Operation for a Math block"""
+
+    def __call__(self, a: BlockInput, b: BlockInput = 0.0, c: BlockInput = 1.0) -> Math:
+        """A MathOperation enumeration value can be called to construct a Math block that performs that operation"""
+    SUM: "MathOperation"
+    """Computes ``a+b+c``. For 2-input sum, set one argument to ``0.0``. To hold a control value for multiple subscribers, set two arguments to ``0.0``."""
+
+    ADD_SUB: "MathOperation"
+    """Computes ``a+b-c``. For 2-input subtraction, set ``b`` to ``0.0``."""
+
+    PRODUCT: "MathOperation"
+    """Computes ``a*b*c``. For 2-input product, set one argument to ``1.0``."""
+
+    MUL_DIV: "MathOperation"
+    """Computes ``a*b/c``. If ``c`` is zero, the output is ``1.0``."""
 
-class BendMode:
-    """Controls the way the ``Note.pitch_bend_depth`` and ``Note.pitch_bend_rate`` properties are interpreted."""
+    SCALE_OFFSET: "MathOperation"
+    """Computes ``(a*b)+c``."""
 
-    STATIC: "BendMode"
-    """The Note's pitch is modified by its ``pitch_bend_depth``. ``pitch_bend_rate`` is ignored."""
+    OFFSET_SCALE: "MathOperation"
+    """Computes ``(a+b)*c``. For 2-input multiplication, set ``b`` to 0."""
 
-    VIBRATO: "BendMode"
-    """The Note's pitch varies by ``±pitch_bend_depth`` at a rate of ``pitch_bend_rate`` Hz."""
+    LERP: "MathOperation"
+    """Computes ``a * (1-c) + b * c``."""
 
-    SWEEP: "BendMode"
-    """The Note's pitch starts at ``Note.frequency`` then sweeps up or down by ``pitch_bend_depth`` over ``1/pitch_bend_rate`` seconds."""
+    CONSTRAINED_LERP: "MathOperation"
+    """Computes ``a * (1-c') + b * c'``, where ``c'`` is constrained to be between ``0.0`` and ``1.0``."""
 
-    SWEEP_IN: "BendMode"
-    """The Note's pitch sweep is the reverse of ``SWEEP`` mode, starting at the bent pitch and arriving at the tuned pitch."""
+    DIV_ADD: "MathOperation"
+    """Computes ``a/b+c``.  If ``b`` is zero, the output is ``c``."""
+
+    ADD_DIV: "MathOperation"
+    """Computes ``(a+b)/c``.  For 2-input product, set ``b`` to ``0.0``."""
+
+    MID: "MathOperation"
+    """Returns the middle of the 3 input values."""
+
+    MAX: "MathOperation"
+    """Returns the biggest of the 3 input values."""
+
+    MIN: "MathOperation"
+    """Returns the smallest of the 3 input values."""
+
+    ABS: "MathOperation"
+    """Returns the absolute value of ``a``."""
+
+class Math:
+    """An arithmetic block
+
+    Performs an arithmetic operation on up to 3 inputs. See the
+    documentation of ``MathOperation`` for the specific functions available.
+
+    The properties can all be changed at run-time.
+
+    An Math only updates if it is actually associated with a playing `Synthesizer`,
+    including indirectly via a `Note` or another intermediate Math.
+
+    Using the same Math as an input to multiple other Maths or Notes is OK, but
+    the result if an Math is tied to multiple Synthtesizer objects is undefined.
+
+    In the current implementation, Maths are updated every 256 samples. This
+    should be considered an implementation detail.
+    """
+
+    def __init__(
+        self,
+        operation: MathOperation,
+        a: BlockInput,
+        b: BlockInput = 0.0,
+        c: BlockInput = 1.0,
+    ):
+        pass
+    a: BlockInput
+    """The first input to the operation"""
+    b: BlockInput
+    """The second input to the operation"""
+    c: BlockInput
+    """The third input to the operation"""
+    operation: MathOperation
+    """The function to compute"""
+
+    value: float
+    """The value of the oscillator (read-only)"""
 
 class MidiTrack:
     """Simple MIDI synth"""
 
     def __init__(
         self,
         buffer: ReadableBuffer,
@@ -160,87 +300,96 @@
     """Offset, in bytes within the midi data, of a decoding error"""
 
 class Note:
     def __init__(
         self,
         *,
         frequency: float,
-        panning: float = 0.0,
+        panning: BlockInput = 0.0,
         waveform: Optional[ReadableBuffer] = None,
         envelope: Optional[Envelope] = None,
-        tremolo_depth: float = 0.0,
-        tremolo_rate: float = 0.0,
-        bend_depth: float = 0.0,
-        bend_rate: float = 0.0,
-        bend_mode: "BendMode" = BendMode.VIBRATO,
+        amplitude: BlockInput = 0.0,
+        bend: BlockInput = 0.0,
+        ring_frequency: float = 0.0,
+        ring_bend: float = 0.0,
+        ring_waveform: Optional[ReadableBuffer] = 0.0,
     ) -> None:
         """Construct a Note object, with a frequency in Hz, and optional panning, waveform, envelope, tremolo (volume change) and bend (frequency change).
 
         If waveform or envelope are `None` the synthesizer object's default waveform or envelope are used.
 
         If the same Note object is played on multiple Synthesizer objects, the result is undefined.
         """
     frequency: float
     """The base frequency of the note, in Hz."""
     filter: bool
     """True if the note should be processed via the synthesizer's FIR filter."""
-    panning: float
+    panning: BlockInput
     """Defines the channel(s) in which the note appears.
 
     -1 is left channel only, 0 is both channels, and 1 is right channel.
     For fractional values, the note plays at full amplitude in one channel
     and partial amplitude in the other channel. For instance -.5 plays at full
     amplitude in the left channel and 1/2 amplitude in the right channel."""
-    tremolo_depth: float
-    """The tremolo depth of the note, from 0 to 1
+    amplitude: BlockInput
+    """The relative amplitude of the note, from 0 to 1
 
-    A depth of 0 disables tremolo. A nonzero value enables tremolo,
-    with the maximum decrease in amplitude being equal to the tremolo
-    depth. A note with a tremolo depth of 1 will fade out to nothing, while
-    a tremolo depth of 0.1 will give a minimum amplitude of 0.9."""
-    tremolo_rate: float
-    """The tremolo rate of the note, in Hz."""
+    An amplitude of 0 makes the note inaudible. It is combined multiplicatively with
+    the value from the note's envelope.
 
-    bend_mode: BendMode
-    """The type of bend operation"""
+    To achieve a tremolo effect, attach an LFO here."""
 
-    bend_depth: float
-    """The bend depth of the note, from -1 to +1
+    bend: BlockInput
+    """The pitch bend depth of the note, from -12 to +12
 
-    A depth of 0 disables bend. A depth of 1 corresponds to a bend of 1
-    octave.  A depth of (1/12) = 0.833 corresponds to a bend of 1 semitone,
+    A depth of 0 plays the programmed frequency. A depth of 1 corresponds to a bend of 1
+    octave.  A depth of (1/12) = 0.0833 corresponds to a bend of 1 semitone,
     and a depth of .00833 corresponds to one musical cent.
+
+    To achieve a vibrato or sweep effect, attach an LFO here.
     """
-    bend_rate: float
-    """The bend rate of the note, in Hz."""
     waveform: Optional[ReadableBuffer]
     """The waveform of this note. Setting the waveform to a buffer of a different size resets the note's phase."""
     envelope: Envelope
     """The envelope of this note"""
 
     ring_frequency: float
     """The ring frequency of the note, in Hz. Zero disables.
 
     For ring to take effect, both ``ring_frequency`` and ``ring_waveform`` must be set."""
+    ring_bend: float
+    """The pitch bend depth of the note's ring waveform, from -12 to +12
+
+    A depth of 0 plays the programmed frequency. A depth of 1 corresponds to a bend of 1
+    octave.  A depth of (1/12) = 0.0833 corresponds to a bend of 1 semitone,
+    and a depth of .00833 corresponds to one musical cent.
+
+    To achieve a vibrato or sweep effect on the ring waveform, attach an LFO here.
+    """
     ring_waveform: Optional[ReadableBuffer]
     """The ring waveform of this note. Setting the ring_waveform to a buffer of a different size resets the note's phase.
 
     For ring to take effect, both ``ring_frequency`` and ``ring_waveform`` must be set."""
 
 NoteSequence = Sequence[Union[int, Note]]
-"""A sequence of notes, which can each be integer MIDI notes or `Note` objects"""
+"""A sequence of notes, which can each be integer MIDI note numbers or `Note` objects"""
+NoteOrNoteSequence = Union[int, Note, NoteSequence]
+"""A note or sequence of notes"""
+LFOOrLFOSequence = Union["LFO", Sequence["LFO"]]
+"""An LFO or a sequence of LFOs"""
 
 class Synthesizer:
     def __init__(
         self,
         *,
         sample_rate: int = 11025,
         channel_count: int = 1,
         waveform: Optional[ReadableBuffer] = None,
         envelope: Optional[Envelope] = None,
+        filter: Optional[ReadableBuffer] = None,
     ) -> None:
         """Create a synthesizer object.
 
         This API is experimental.
 
         Integer notes use MIDI note numbering, with 60 being C4 or Middle C,
         approximately 262Hz. Integer notes use the given waveform & envelope,
@@ -248,47 +397,58 @@
 
         :param int sample_rate: The desired playback sample rate; higher sample rate requires more memory
         :param int channel_count: The number of output channels (1=mono, 2=stereo)
         :param ReadableBuffer waveform: A single-cycle waveform. Default is a 50% duty cycle square wave. If specified, must be a ReadableBuffer of type 'h' (signed 16 bit)
         :param ReadableBuffer filter: Coefficients of an FIR filter to apply to notes with ``filter=True``. If specified, must be a ReadableBuffer of type 'h' (signed 16 bit)
         :param Optional[Envelope] envelope: An object that defines the loudness of a note over time. The default envelope, `None` provides no ramping, voices turn instantly on and off.
         """
-    def press(self, /, press: NoteSequence = ()) -> None:
+    def press(self, /, press: NoteOrNoteSequence = ()) -> None:
         """Turn some notes on.
 
         Pressing a note that was already pressed has no effect.
 
-        :param NoteSequence press: Any sequence of notes."""
-    def release(self, /, release: NoteSequence = ()) -> None:
+        :param NoteOrNoteSequence press: Any sequence of notes."""
+    def release(self, /, release: NoteOrNoteSequence = ()) -> None:
         """Turn some notes off.
 
         Releasing a note that was already released has no effect.
 
-        :param NoteSequence release: Any sequence of notes."""
-    def release_then_press(
-        self, release: NoteSequence = (), press: NoteSequence = ()
+        :param NoteOrNoteSequence release: Any sequence of notes."""
+    def change(
+        self,
+        release: NoteOrNoteSequence = (),
+        press: NoteOrNoteSequence = (),
+        retrigger=LFOOrLFOSequence,
     ) -> None:
-        """Turn some notes on and/or off.
+        """Start notes, stop them, and/or re-trigger some LFOs.
 
-        It is OK to release note that was not actually turned on.
-
-        Pressing a note that was already pressed has no effect.
+        The changes all happen atomically with respect to output generation.
 
-        Releasing and pressing the note again has little effect, but does reset the phase
-        of the note, which may be perceptible as a small glitch.
+        It is OK to release note that was not actually turned on.
 
-        :param NoteSequence release: Any sequence of notes.
-        :param NoteSequence press: Any sequence of notes."""
-    def release_all_then_press(self, /, press: NoteSequence) -> None:
+        Pressing a note that was already pressed returns it to the attack phase
+        but without resetting its amplitude. Releasing a note and immediately
+        pressing it again returns it to the attack phase with an initial
+        amplitude of 0.
+
+        At the same time, the passed LFOs (if any) are retriggered.
+
+        :param NoteOrNoteSequence release: Any sequence of notes.
+        :param NoteOrNoteSequence press: Any sequence of notes.
+        :param LFOOrLFOSequence retrigger: Any sequence of LFOs.
+
+        Note: for compatibility, ``release_then_press`` may be used as an alias
+        for this function. This compatibility name will be removed in 9.0."""
+    def release_all_then_press(self, /, press: NoteOrNoteSequence) -> None:
         """Turn any currently-playing notes off, then turn on the given notes
 
-        Releasing and pressing the note again has little effect, but does reset the phase
-        of the note, which may be perceptible as a small glitch.
+        Releasing a note and immediately pressing it again returns it to the
+        attack phase with an initial amplitude of 0.
 
-        :param NoteSequence press: Any sequence of notes."""
+        :param NoteOrNoteSequence press: Any sequence of notes."""
     def release_all(self) -> None:
         """Turn any currently-playing notes off"""
     def deinit(self) -> None:
         """Deinitialises the object and releases any memory resources for reuse."""
         ...
     def __enter__(self) -> Synthesizer:
         """No-op used by Context Managers."""
@@ -300,9 +460,16 @@
     envelope: Optional[Envelope]
     """The envelope to apply to all notes. `None`, the default envelope, instantly turns notes on and off. The envelope may be changed dynamically, but it affects all notes (even currently playing notes)"""
     sample_rate: int
     """32 bit value that tells how quickly samples are played in Hertz (cycles per second)."""
     pressed: NoteSequence
     """A sequence of the currently pressed notes (read-only property)"""
 
+    blocks: List[BlockInput]
+    """A list of blocks to advance whether or not they are associated with a playing note.
+
+    This can be used to implement 'free-running' LFOs. LFOs associated with playing notes are advanced whether or not they are in this list.
+
+    This property is read-only but its contents may be modified by e.g., calling ``synth.blocks.append()`` or ``synth.blocks.remove()``. It is initially an empty list."""
+
     max_polyphony: int
     """Maximum polyphony of the synthesizer (read-only class property)"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `circuitpython-stubs-8.1.0rc0/terminalio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/time/__init__.pyi` & `circuitpython-stubs-8.2.0b0/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/touchio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/traceback/__init__.pyi` & `circuitpython-stubs-8.2.0b0/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/numpy/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -446,14 +446,18 @@
     """Converts angles from degrees to radians"""
     ...
 
 def sin(a: _ArrayLike) -> ulab.numpy.ndarray:
     """Computes the sine function"""
     ...
 
+def sinc(a: _ArrayLike) -> ulab.numpy.ndarray:
+    """Computes the normalized sinc function"""
+    ...
+
 def sinh(a: _ArrayLike) -> ulab.numpy.ndarray:
     """Computes the hyperbolic sine"""
     ...
 
 def sqrt(a: _ArrayLike) -> ulab.numpy.ndarray:
     """Computes the square root"""
     ...
```

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.2.0b0/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/usb/core/__init__.pyi` & `circuitpython-stubs-8.2.0b0/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.2.0b0/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/usb_hid/__init__.pyi` & `circuitpython-stubs-8.2.0b0/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/usb_host/__init__.pyi` & `circuitpython-stubs-8.2.0b0/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/usb_midi/__init__.pyi` & `circuitpython-stubs-8.2.0b0/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/vectorio/__init__.pyi` & `circuitpython-stubs-8.2.0b0/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/watchdog/__init__.pyi` & `circuitpython-stubs-8.2.0b0/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/wifi/__init__.pyi` & `circuitpython-stubs-8.2.0b0/wifi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0rc0/zlib/__init__.pyi` & `circuitpython-stubs-8.2.0b0/zlib/__init__.pyi`

 * *Files identical despite different names*

