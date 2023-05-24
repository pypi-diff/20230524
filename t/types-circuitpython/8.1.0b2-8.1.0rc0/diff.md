# Comparing `tmp/types-circuitpython-8.1.0b2.tar.gz` & `tmp/types-circuitpython-8.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-circuitpython-8.1.0b2.tar", last modified: Tue May 16 15:44:48 2023, max compression
+gzip compressed data, was "types-circuitpython-8.1.0rc0.tar", last modified: Wed May 24 01:40:16 2023, max compression
```

## Comparing `types-circuitpython-8.1.0b2.tar` & `types-circuitpython-8.1.0rc0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.163987 types-circuitpython-8.1.0b2/
--rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.1.0b2/LICENSE
--rw-r--r--   0 timon      (501) staff       (20)     3630 2023-05-16 15:44:48.163519 types-circuitpython-8.1.0b2/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2573 2023-05-16 15:44:12.000000 types-circuitpython-8.1.0b2/README.md
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.113285 types-circuitpython-8.1.0b2/bindings/
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.115922 types-circuitpython-8.1.0b2/bindings/__future__/
--rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/__future__/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.116332 types-circuitpython-8.1.0b2/bindings/_bleio/
--rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_bleio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.116860 types-circuitpython-8.1.0b2/bindings/_eve/
--rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_eve/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.117389 types-circuitpython-8.1.0b2/bindings/_pew/
--rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_pew/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.117796 types-circuitpython-8.1.0b2/bindings/_pixelmap/
--rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_pixelmap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.118175 types-circuitpython-8.1.0b2/bindings/_stage/
--rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_stage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.118547 types-circuitpython-8.1.0b2/bindings/adafruit_bus_device/
--rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.118930 types-circuitpython-8.1.0b2/bindings/adafruit_pixelbuf/
--rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.119336 types-circuitpython-8.1.0b2/bindings/aesio/
--rw-r--r--   0 timon      (501) staff       (20)     2602 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/aesio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.119782 types-circuitpython-8.1.0b2/bindings/alarm/
--rw-r--r--   0 timon      (501) staff       (20)     7021 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/alarm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.120203 types-circuitpython-8.1.0b2/bindings/analogbufio/
--rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/analogbufio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.120641 types-circuitpython-8.1.0b2/bindings/analogio/
--rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/analogio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.121065 types-circuitpython-8.1.0b2/bindings/atexit/
--rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/atexit/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.121479 types-circuitpython-8.1.0b2/bindings/audiobusio/
--rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiobusio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.121928 types-circuitpython-8.1.0b2/bindings/audiocore/
--rw-r--r--   0 timon      (501) staff       (20)     4607 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiocore/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.122354 types-circuitpython-8.1.0b2/bindings/audioio/
--rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.122739 types-circuitpython-8.1.0b2/bindings/audiomixer/
--rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiomixer/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.123217 types-circuitpython-8.1.0b2/bindings/audiomp3/
--rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiomp3/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.123701 types-circuitpython-8.1.0b2/bindings/audiopwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4448 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiopwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.124131 types-circuitpython-8.1.0b2/bindings/bitbangio/
--rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/bitbangio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.124604 types-circuitpython-8.1.0b2/bindings/bitmaptools/
--rw-r--r--   0 timon      (501) staff       (20)    13492 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/bitmaptools/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.125005 types-circuitpython-8.1.0b2/bindings/bitops/
--rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/bitops/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.125374 types-circuitpython-8.1.0b2/bindings/board/
--rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/board/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.125766 types-circuitpython-8.1.0b2/bindings/busio/
--rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/busio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.126205 types-circuitpython-8.1.0b2/bindings/camera/
--rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/camera/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.126573 types-circuitpython-8.1.0b2/bindings/canio/
--rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/canio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.127115 types-circuitpython-8.1.0b2/bindings/countio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/countio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.127836 types-circuitpython-8.1.0b2/bindings/digitalio/
--rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/digitalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.128528 types-circuitpython-8.1.0b2/bindings/displayio/
--rw-r--r--   0 timon      (501) staff       (20)    40033 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/displayio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.129403 types-circuitpython-8.1.0b2/bindings/dualbank/
--rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/dualbank/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.130238 types-circuitpython-8.1.0b2/bindings/floppyio/
--rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/floppyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.131021 types-circuitpython-8.1.0b2/bindings/fontio/
--rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/fontio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.131726 types-circuitpython-8.1.0b2/bindings/framebufferio/
--rw-r--r--   0 timon      (501) staff       (20)     3743 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/framebufferio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.132550 types-circuitpython-8.1.0b2/bindings/frequencyio/
--rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/frequencyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.133259 types-circuitpython-8.1.0b2/bindings/getpass/
--rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/getpass/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.133922 types-circuitpython-8.1.0b2/bindings/gifio/
--rw-r--r--   0 timon      (501) staff       (20)     5691 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/gifio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.134555 types-circuitpython-8.1.0b2/bindings/gnss/
--rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/gnss/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.135296 types-circuitpython-8.1.0b2/bindings/hashlib/
--rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/hashlib/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.135992 types-circuitpython-8.1.0b2/bindings/i2ctarget/
--rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/i2ctarget/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.136653 types-circuitpython-8.1.0b2/bindings/imagecapture/
--rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/imagecapture/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.137340 types-circuitpython-8.1.0b2/bindings/ipaddress/
--rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/ipaddress/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.137967 types-circuitpython-8.1.0b2/bindings/is31fl3741/
--rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/is31fl3741/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.138567 types-circuitpython-8.1.0b2/bindings/keypad/
--rw-r--r--   0 timon      (501) staff       (20)    13080 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/keypad/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.139297 types-circuitpython-8.1.0b2/bindings/math/
--rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/math/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.140100 types-circuitpython-8.1.0b2/bindings/mdns/
--rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/mdns/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.141073 types-circuitpython-8.1.0b2/bindings/memorymap/
--rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/memorymap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.142176 types-circuitpython-8.1.0b2/bindings/memorymonitor/
--rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/memorymonitor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.143280 types-circuitpython-8.1.0b2/bindings/microcontroller/
--rw-r--r--   0 timon      (501) staff       (20)     6071 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/microcontroller/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.143898 types-circuitpython-8.1.0b2/bindings/msgpack/
--rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/msgpack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.144820 types-circuitpython-8.1.0b2/bindings/neopixel_write/
--rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/neopixel_write/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.145835 types-circuitpython-8.1.0b2/bindings/nvm/
--rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/nvm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.146636 types-circuitpython-8.1.0b2/bindings/onewireio/
--rw-r--r--   0 timon      (501) staff       (20)     1671 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/onewireio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.147204 types-circuitpython-8.1.0b2/bindings/os/
--rw-r--r--   0 timon      (501) staff       (20)     3750 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/os/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.147603 types-circuitpython-8.1.0b2/bindings/paralleldisplay/
--rw-r--r--   0 timon      (501) staff       (20)     2416 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.147992 types-circuitpython-8.1.0b2/bindings/ps2io/
--rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/ps2io/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.148356 types-circuitpython-8.1.0b2/bindings/pulseio/
--rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/pulseio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.148754 types-circuitpython-8.1.0b2/bindings/pwmio/
--rw-r--r--   0 timon      (501) staff       (20)     5906 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/pwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.149123 types-circuitpython-8.1.0b2/bindings/qrio/
--rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/qrio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.149490 types-circuitpython-8.1.0b2/bindings/rainbowio/
--rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rainbowio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.149852 types-circuitpython-8.1.0b2/bindings/random/
--rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/random/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.150209 types-circuitpython-8.1.0b2/bindings/rgbmatrix/
--rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.150559 types-circuitpython-8.1.0b2/bindings/rotaryio/
--rw-r--r--   0 timon      (501) staff       (20)     2660 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rotaryio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.151124 types-circuitpython-8.1.0b2/bindings/rtc/
--rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rtc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.151568 types-circuitpython-8.1.0b2/bindings/sdcardio/
--rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/sdcardio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.152041 types-circuitpython-8.1.0b2/bindings/sdioio/
--rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/sdioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.152499 types-circuitpython-8.1.0b2/bindings/sharpdisplay/
--rw-r--r--   0 timon      (501) staff       (20)     1763 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.152919 types-circuitpython-8.1.0b2/bindings/socketpool/
--rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/socketpool/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.153331 types-circuitpython-8.1.0b2/bindings/ssl/
--rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/ssl/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.153717 types-circuitpython-8.1.0b2/bindings/storage/
--rw-r--r--   0 timon      (501) staff       (20)     5949 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/storage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.154123 types-circuitpython-8.1.0b2/bindings/struct/
--rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/struct/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.154502 types-circuitpython-8.1.0b2/bindings/supervisor/
--rw-r--r--   0 timon      (501) staff       (20)    10934 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/supervisor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.154887 types-circuitpython-8.1.0b2/bindings/synthio/
--rw-r--r--   0 timon      (501) staff       (20)     6160 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/synthio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.155270 types-circuitpython-8.1.0b2/bindings/terminalio/
--rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/terminalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.155657 types-circuitpython-8.1.0b2/bindings/time/
--rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/time/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.156030 types-circuitpython-8.1.0b2/bindings/touchio/
--rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/touchio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.156433 types-circuitpython-8.1.0b2/bindings/traceback/
--rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/traceback/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.156838 types-circuitpython-8.1.0b2/bindings/uheap/
--rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/uheap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.157234 types-circuitpython-8.1.0b2/bindings/usb/
--rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.157611 types-circuitpython-8.1.0b2/bindings/usb_cdc/
--rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_cdc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.158003 types-circuitpython-8.1.0b2/bindings/usb_hid/
--rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_hid/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.158395 types-circuitpython-8.1.0b2/bindings/usb_host/
--rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_host/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.158793 types-circuitpython-8.1.0b2/bindings/usb_midi/
--rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_midi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.159160 types-circuitpython-8.1.0b2/bindings/ustack/
--rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/ustack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.159539 types-circuitpython-8.1.0b2/bindings/vectorio/
--rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/vectorio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.159919 types-circuitpython-8.1.0b2/bindings/watchdog/
--rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/watchdog/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.160303 types-circuitpython-8.1.0b2/bindings/wifi/
--rw-r--r--   0 timon      (501) staff       (20)     9835 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/wifi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.160684 types-circuitpython-8.1.0b2/bindings/zlib/
--rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/zlib/__init__.pyi
--rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.1.0b2/pyproject.toml
--rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:44:48.164167 types-circuitpython-8.1.0b2/setup.cfg
--rw-r--r--   0 timon      (501) staff       (20)     2181 2023-05-16 15:44:39.000000 types-circuitpython-8.1.0b2/setup.py
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.162939 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/
--rw-r--r--   0 timon      (501) staff       (20)     3630 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/SOURCES.txt
--rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/dependency_links.txt
--rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/requires.txt
--rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/top_level.txt
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.192585 types-circuitpython-8.1.0rc0/
+-rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.1.0rc0/LICENSE
+-rw-r--r--   0 timon      (501) staff       (20)     3860 2023-05-24 01:40:16.192232 types-circuitpython-8.1.0rc0/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-23 18:25:46.000000 types-circuitpython-8.1.0rc0/README.md
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.144021 types-circuitpython-8.1.0rc0/bindings/
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.145897 types-circuitpython-8.1.0rc0/bindings/__future__/
+-rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-24 01:40:06.000000 types-circuitpython-8.1.0rc0/bindings/__future__/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.146202 types-circuitpython-8.1.0rc0/bindings/_bleio/
+-rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_bleio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.146573 types-circuitpython-8.1.0rc0/bindings/_eve/
+-rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_eve/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.146931 types-circuitpython-8.1.0rc0/bindings/_pew/
+-rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_pew/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.147247 types-circuitpython-8.1.0rc0/bindings/_pixelmap/
+-rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_pixelmap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.147555 types-circuitpython-8.1.0rc0/bindings/_stage/
+-rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_stage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.147854 types-circuitpython-8.1.0rc0/bindings/adafruit_bus_device/
+-rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.148168 types-circuitpython-8.1.0rc0/bindings/adafruit_pixelbuf/
+-rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.148486 types-circuitpython-8.1.0rc0/bindings/aesio/
+-rw-r--r--   0 timon      (501) staff       (20)     2602 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/aesio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.148788 types-circuitpython-8.1.0rc0/bindings/alarm/
+-rw-r--r--   0 timon      (501) staff       (20)     7021 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/alarm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.149096 types-circuitpython-8.1.0rc0/bindings/analogbufio/
+-rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/analogbufio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.149412 types-circuitpython-8.1.0rc0/bindings/analogio/
+-rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/analogio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.149731 types-circuitpython-8.1.0rc0/bindings/atexit/
+-rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/atexit/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150041 types-circuitpython-8.1.0rc0/bindings/audiobusio/
+-rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiobusio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150352 types-circuitpython-8.1.0rc0/bindings/audiocore/
+-rw-r--r--   0 timon      (501) staff       (20)     4607 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiocore/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150657 types-circuitpython-8.1.0rc0/bindings/audioio/
+-rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150962 types-circuitpython-8.1.0rc0/bindings/audiomixer/
+-rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiomixer/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.151274 types-circuitpython-8.1.0rc0/bindings/audiomp3/
+-rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiomp3/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.151583 types-circuitpython-8.1.0rc0/bindings/audiopwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4448 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiopwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.151885 types-circuitpython-8.1.0rc0/bindings/bitbangio/
+-rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/bitbangio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.152192 types-circuitpython-8.1.0rc0/bindings/bitmaptools/
+-rw-r--r--   0 timon      (501) staff       (20)    13492 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/bitmaptools/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.152503 types-circuitpython-8.1.0rc0/bindings/bitops/
+-rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/bitops/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.152800 types-circuitpython-8.1.0rc0/bindings/board/
+-rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/board/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.153097 types-circuitpython-8.1.0rc0/bindings/busio/
+-rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/busio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.153545 types-circuitpython-8.1.0rc0/bindings/camera/
+-rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/camera/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.153998 types-circuitpython-8.1.0rc0/bindings/canio/
+-rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/canio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.154558 types-circuitpython-8.1.0rc0/bindings/countio/
+-rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/countio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.155128 types-circuitpython-8.1.0rc0/bindings/digitalio/
+-rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/digitalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.155684 types-circuitpython-8.1.0rc0/bindings/displayio/
+-rw-r--r--   0 timon      (501) staff       (20)    40361 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/displayio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.156365 types-circuitpython-8.1.0rc0/bindings/dualbank/
+-rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/dualbank/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.156800 types-circuitpython-8.1.0rc0/bindings/floppyio/
+-rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/floppyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.157205 types-circuitpython-8.1.0rc0/bindings/fontio/
+-rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/fontio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.157808 types-circuitpython-8.1.0rc0/bindings/framebufferio/
+-rw-r--r--   0 timon      (501) staff       (20)     3743 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/framebufferio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.158419 types-circuitpython-8.1.0rc0/bindings/frequencyio/
+-rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/frequencyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.159003 types-circuitpython-8.1.0rc0/bindings/getpass/
+-rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/getpass/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.159346 types-circuitpython-8.1.0rc0/bindings/gifio/
+-rw-r--r--   0 timon      (501) staff       (20)     5691 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/gifio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.159690 types-circuitpython-8.1.0rc0/bindings/gnss/
+-rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/gnss/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.160233 types-circuitpython-8.1.0rc0/bindings/hashlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/hashlib/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.160852 types-circuitpython-8.1.0rc0/bindings/i2ctarget/
+-rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/i2ctarget/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.161607 types-circuitpython-8.1.0rc0/bindings/imagecapture/
+-rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/imagecapture/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.162309 types-circuitpython-8.1.0rc0/bindings/ipaddress/
+-rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/ipaddress/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.163048 types-circuitpython-8.1.0rc0/bindings/is31fl3741/
+-rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/is31fl3741/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.163845 types-circuitpython-8.1.0rc0/bindings/keypad/
+-rw-r--r--   0 timon      (501) staff       (20)    13080 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/keypad/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.164674 types-circuitpython-8.1.0rc0/bindings/math/
+-rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/math/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.165378 types-circuitpython-8.1.0rc0/bindings/mdns/
+-rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/mdns/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.166235 types-circuitpython-8.1.0rc0/bindings/memorymap/
+-rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/memorymap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.166853 types-circuitpython-8.1.0rc0/bindings/memorymonitor/
+-rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/memorymonitor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.167517 types-circuitpython-8.1.0rc0/bindings/microcontroller/
+-rw-r--r--   0 timon      (501) staff       (20)     6388 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/microcontroller/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.168136 types-circuitpython-8.1.0rc0/bindings/msgpack/
+-rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/msgpack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.168713 types-circuitpython-8.1.0rc0/bindings/neopixel_write/
+-rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/neopixel_write/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.169263 types-circuitpython-8.1.0rc0/bindings/nvm/
+-rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/nvm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.169811 types-circuitpython-8.1.0rc0/bindings/onewireio/
+-rw-r--r--   0 timon      (501) staff       (20)     1671 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/onewireio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.170389 types-circuitpython-8.1.0rc0/bindings/os/
+-rw-r--r--   0 timon      (501) staff       (20)     3750 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/os/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.170961 types-circuitpython-8.1.0rc0/bindings/paralleldisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     2416 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.171520 types-circuitpython-8.1.0rc0/bindings/ps2io/
+-rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/ps2io/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.172108 types-circuitpython-8.1.0rc0/bindings/pulseio/
+-rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/pulseio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.172726 types-circuitpython-8.1.0rc0/bindings/pwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     5906 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/pwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.173317 types-circuitpython-8.1.0rc0/bindings/qrio/
+-rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/qrio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.174270 types-circuitpython-8.1.0rc0/bindings/rainbowio/
+-rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rainbowio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.175290 types-circuitpython-8.1.0rc0/bindings/random/
+-rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/random/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.176109 types-circuitpython-8.1.0rc0/bindings/rgbmatrix/
+-rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.176762 types-circuitpython-8.1.0rc0/bindings/rotaryio/
+-rw-r--r--   0 timon      (501) staff       (20)     2660 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rotaryio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.177428 types-circuitpython-8.1.0rc0/bindings/rtc/
+-rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rtc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.178088 types-circuitpython-8.1.0rc0/bindings/sdcardio/
+-rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/sdcardio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.178710 types-circuitpython-8.1.0rc0/bindings/sdioio/
+-rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/sdioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.179349 types-circuitpython-8.1.0rc0/bindings/sharpdisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     1763 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.180000 types-circuitpython-8.1.0rc0/bindings/socketpool/
+-rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/socketpool/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.180572 types-circuitpython-8.1.0rc0/bindings/ssl/
+-rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/ssl/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.181147 types-circuitpython-8.1.0rc0/bindings/storage/
+-rw-r--r--   0 timon      (501) staff       (20)     5949 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/storage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.181657 types-circuitpython-8.1.0rc0/bindings/struct/
+-rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/struct/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.182206 types-circuitpython-8.1.0rc0/bindings/supervisor/
+-rw-r--r--   0 timon      (501) staff       (20)    10934 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/supervisor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.182748 types-circuitpython-8.1.0rc0/bindings/synthio/
+-rw-r--r--   0 timon      (501) staff       (20)    14321 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/synthio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.183292 types-circuitpython-8.1.0rc0/bindings/terminalio/
+-rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/terminalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.183807 types-circuitpython-8.1.0rc0/bindings/time/
+-rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/time/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.184332 types-circuitpython-8.1.0rc0/bindings/touchio/
+-rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/touchio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.184840 types-circuitpython-8.1.0rc0/bindings/traceback/
+-rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/traceback/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.185356 types-circuitpython-8.1.0rc0/bindings/uheap/
+-rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/uheap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.185894 types-circuitpython-8.1.0rc0/bindings/usb/
+-rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.186444 types-circuitpython-8.1.0rc0/bindings/usb_cdc/
+-rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_cdc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.186950 types-circuitpython-8.1.0rc0/bindings/usb_hid/
+-rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_hid/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.187466 types-circuitpython-8.1.0rc0/bindings/usb_host/
+-rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_host/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.188066 types-circuitpython-8.1.0rc0/bindings/usb_midi/
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_midi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.188513 types-circuitpython-8.1.0rc0/bindings/ustack/
+-rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/ustack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.188879 types-circuitpython-8.1.0rc0/bindings/vectorio/
+-rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/vectorio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.189215 types-circuitpython-8.1.0rc0/bindings/watchdog/
+-rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/watchdog/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.189555 types-circuitpython-8.1.0rc0/bindings/wifi/
+-rw-r--r--   0 timon      (501) staff       (20)    10381 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/wifi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.189881 types-circuitpython-8.1.0rc0/bindings/zlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/zlib/__init__.pyi
+-rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.1.0rc0/pyproject.toml
+-rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-24 01:40:16.192689 types-circuitpython-8.1.0rc0/setup.cfg
+-rw-r--r--   0 timon      (501) staff       (20)     2179 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/setup.py
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.191753 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/
+-rw-r--r--   0 timon      (501) staff       (20)     3860 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/SOURCES.txt
+-rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/dependency_links.txt
+-rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/requires.txt
+-rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/top_level.txt
```

### Comparing `types-circuitpython-8.1.0b2/LICENSE` & `types-circuitpython-8.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/PKG-INFO` & `types-circuitpython-8.1.0rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.1.0b2
+Version: 8.1.0rc0
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -34,19 +34,28 @@
 
 ![adafruit-circuitpython-typing](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/adafruit-circuitpython-typing.gif)
 
 Coding with `types-circuitpython`:
 
 ![types-circuitpython](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/types-circuitpython.gif)
 
+## Usage
+
+```bash
+# installing the last release
+$ pip install types-circuitpython
+# or installing a specific version
+$ pip install types-circuitpython==8.1.0b2
+```
+
 ## Long term support versions
 
-Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
+Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases), or [CircuitPython tags](https://github.com/adafruit/circuitpython/tags)
 
-[Pypi versions](https://pypi.org/project/types-circuitpython/#history)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-circuitpython?style=flat-square) [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.1.x
     - 8.1.0b2 (Corresponds 8.1.0-beta.2 of CircuitPython's version)
     - 8.1.0b1 (Corresponds 8.1.0-beta.1 of CircuitPython's version)
     - 8.1.0b0 (Corresponds 8.1.0-beta.0 of CircuitPython's version)
     - 8.1.0a2 (Corresponds 8.1.0-alpha.2 of CircuitPython's version)
@@ -71,22 +80,14 @@
 - 7.x
   - 7.3.x
     - 7.3.3
     - 7.3.2
     - 7.3.1
     - 7.3.0
 
-## Usage
-
-```bash
-$ pip install types-circuitpython==7.3.3
-# or
-$ pip install types-circuitpython==8.0.0b0
-```
-
 ## Development
 
 ## Initialization
 
 ```bash
 $ virtualenv .venv
 $ . ./.venv/bin/activate
```

### Comparing `types-circuitpython-8.1.0b2/README.md` & `types-circuitpython-8.1.0rc0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 
 ![adafruit-circuitpython-typing](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/adafruit-circuitpython-typing.gif)
 
 Coding with `types-circuitpython`:
 
 ![types-circuitpython](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/types-circuitpython.gif)
 
+## Usage
+
+```bash
+# installing the last release
+$ pip install types-circuitpython
+# or installing a specific version
+$ pip install types-circuitpython==8.1.0b2
+```
+
 ## Long term support versions
 
-Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
+Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases), or [CircuitPython tags](https://github.com/adafruit/circuitpython/tags)
 
-[Pypi versions](https://pypi.org/project/types-circuitpython/#history)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-circuitpython?style=flat-square) [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.1.x
     - 8.1.0b2 (Corresponds 8.1.0-beta.2 of CircuitPython's version)
     - 8.1.0b1 (Corresponds 8.1.0-beta.1 of CircuitPython's version)
     - 8.1.0b0 (Corresponds 8.1.0-beta.0 of CircuitPython's version)
     - 8.1.0a2 (Corresponds 8.1.0-alpha.2 of CircuitPython's version)
@@ -46,22 +55,14 @@
 - 7.x
   - 7.3.x
     - 7.3.3
     - 7.3.2
     - 7.3.1
     - 7.3.0
 
-## Usage
-
-```bash
-$ pip install types-circuitpython==7.3.3
-# or
-$ pip install types-circuitpython==8.0.0b0
-```
-
 ## Development
 
 ## Initialization
 
 ```bash
 $ virtualenv .venv
 $ . ./.venv/bin/activate
```

### Comparing `types-circuitpython-8.1.0b2/bindings/__future__/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/__future__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/_bleio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/_eve/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/_pew/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/_pixelmap/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/_stage/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/adafruit_pixelbuf/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/aesio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/alarm/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/analogbufio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/analogio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/atexit/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/audiobusio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/audiocore/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/audioio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/audiomixer/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/audiomp3/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/audiopwmio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/bitbangio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/bitmaptools/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/bitops/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/board/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/busio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/camera/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/canio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/countio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/digitalio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/displayio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/displayio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 refer to `this Learn guide
 <https://learn.adafruit.com/circuitpython-display-support-using-displayio>`_.
 """
 
 from __future__ import annotations
 
 import typing
-from typing import Optional, Tuple, Union
+from typing import Iterator, Optional, Tuple, Union
 
 import busio
 import circuitpython_typing
 import microcontroller
 import vectorio
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
 
@@ -566,14 +566,25 @@
         layer: Union[
             vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid
         ],
     ) -> None:
         """Remove the first copy of layer. Raises ValueError if it is not present."""
         ...
     def __bool__(self) -> bool: ...
+    def __contains__(
+        self,
+        item: Union[
+            vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid
+        ],
+    ) -> bool: ...
+    def __iter__(
+        self,
+    ) -> Iterator[
+        Union[vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid]
+    ]: ...
     def __len__(self) -> int:
         """Returns the number of layers in a Group"""
         ...
     def __getitem__(
         self, index: int
     ) -> Union[vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid]:
         """Returns the value at the given index.
```

### Comparing `types-circuitpython-8.1.0b2/bindings/dualbank/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/floppyio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/fontio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/framebufferio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/frequencyio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/getpass/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/gifio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/gnss/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/hashlib/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/i2ctarget/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/imagecapture/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/ipaddress/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/is31fl3741/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/keypad/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/math/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/mdns/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/memorymap/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/memorymonitor/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/microcontroller/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/microcontroller/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -95,16 +95,23 @@
     def __init__(self) -> None:
         """You cannot create an instance of `microcontroller.Processor`.
         Use `microcontroller.cpu` to access the sole instance available."""
         ...
     frequency: int
     """The CPU operating frequency in Hertz.
 
-    **Limitations:** Setting the ``frequency`` is possible only on some i.MX boards.
-    On most boards, ``frequency`` is read-only.
+    **Limitations:** On most boards, ``frequency`` is read-only. Setting
+    the ``frequency`` is possible on RP2040 boards and some i.MX boards.
+
+    .. warning:: Overclocking likely voids your warranties and may reduce
+      the lifetime of the chip.
+
+    .. warning:: Changing the frequency may cause issues with other
+      subsystems, such as USB, PWM, and PIO. To minimize issues, set the CPU
+      frequency before initializing other systems.
     """
     reset_reason: microcontroller.ResetReason
     """The reason the microcontroller started up from reset state."""
     temperature: Optional[float]
     """The on-chip temperature, in Celsius, as a float. (read-only)
 
     Is `None` if the temperature is not available.
```

### Comparing `types-circuitpython-8.1.0b2/bindings/msgpack/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/neopixel_write/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/nvm/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/onewireio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/os/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/paralleldisplay/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/ps2io/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/pulseio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/pwmio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/qrio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/random/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/rgbmatrix/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/rotaryio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/rtc/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/sdcardio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/sdioio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/sharpdisplay/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/socketpool/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/ssl/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/storage/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/struct/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/supervisor/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/terminalio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/time/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/touchio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/traceback/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/usb_cdc/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/usb_hid/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/usb_host/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/usb_midi/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/vectorio/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/watchdog/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/bindings/wifi/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/wifi/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -224,27 +224,42 @@
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
         ipv4_dns: Optional[ipaddress.IPv4Address],
     ) -> None:
         """Sets the IP v4 address of the station. Must include the netmask and gateway. DNS address is optional.
         Setting the address manually will stop the DHCP client."""
         ...
+    def set_ipv4_address_ap(
+        self,
+        *,
+        ipv4: ipaddress.IPv4Address,
+        netmask: ipaddress.IPv4Address,
+        gateway: ipaddress.IPv4Address,
+    ) -> None:
+        """Sets the IP v4 address of the access point. Must include the netmask and gateway."""
+        ...
     ipv4_address: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the station when connected to an access point. None otherwise. (read-only)"""
     ipv4_address_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point, when enabled. None otherwise."""
     ipv4_dns: ipaddress.IPv4Address
     """IP v4 Address of the DNS server to be used."""
     ap_info: Optional[Network]
     """Network object containing BSSID, SSID, authmode, channel, country and RSSI when connected to an access point. None otherwise."""
     def start_dhcp(self) -> None:
-        """Starts the DHCP client."""
+        """Starts the station DHCP client."""
         ...
     def stop_dhcp(self) -> None:
-        """Stops the DHCP client. Needed to assign a static IP address."""
+        """Stops the station DHCP client. Needed to assign a static IP address."""
+        ...
+    def start_dhcp_ap(self) -> None:
+        """Starts the access point DHCP server."""
+        ...
+    def stop_dhcp_ap(self) -> None:
+        """Stops the access point DHCP server. Needed to assign a static IP address."""
         ...
     def ping(
         self, ip: ipaddress.IPv4Address, *, timeout: Optional[float] = 0.5
     ) -> Optional[float]:
         """Ping an IP to test connectivity. Returns echo time in seconds.
         Returns None when it times out."""
         ...
```

### Comparing `types-circuitpython-8.1.0b2/bindings/zlib/__init__.pyi` & `types-circuitpython-8.1.0rc0/bindings/zlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/setup.py` & `types-circuitpython-8.1.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir, path
 
 from setuptools import setup
 
 __name__ = "types-circuitpython"
-__version__ = "8.1.0-beta.2"
+__version__ = "8.1.0-rc.0"
 __repo__ = "https://github.com/hardfury-labs/types-circuitpython"
 __author__ = "HardFury"
 
 
 HERE = path.abspath(path.dirname(__file__))
 BINDINGS_DIR = path.join(HERE, "bindings")
```

### Comparing `types-circuitpython-8.1.0b2/types_circuitpython.egg-info/PKG-INFO` & `types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.1.0b2
+Version: 8.1.0rc0
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -34,19 +34,28 @@
 
 ![adafruit-circuitpython-typing](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/adafruit-circuitpython-typing.gif)
 
 Coding with `types-circuitpython`:
 
 ![types-circuitpython](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/types-circuitpython.gif)
 
+## Usage
+
+```bash
+# installing the last release
+$ pip install types-circuitpython
+# or installing a specific version
+$ pip install types-circuitpython==8.1.0b2
+```
+
 ## Long term support versions
 
-Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
+Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases), or [CircuitPython tags](https://github.com/adafruit/circuitpython/tags)
 
-[Pypi versions](https://pypi.org/project/types-circuitpython/#history)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-circuitpython?style=flat-square) [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.1.x
     - 8.1.0b2 (Corresponds 8.1.0-beta.2 of CircuitPython's version)
     - 8.1.0b1 (Corresponds 8.1.0-beta.1 of CircuitPython's version)
     - 8.1.0b0 (Corresponds 8.1.0-beta.0 of CircuitPython's version)
     - 8.1.0a2 (Corresponds 8.1.0-alpha.2 of CircuitPython's version)
@@ -71,22 +80,14 @@
 - 7.x
   - 7.3.x
     - 7.3.3
     - 7.3.2
     - 7.3.1
     - 7.3.0
 
-## Usage
-
-```bash
-$ pip install types-circuitpython==7.3.3
-# or
-$ pip install types-circuitpython==8.0.0b0
-```
-
 ## Development
 
 ## Initialization
 
 ```bash
 $ virtualenv .venv
 $ . ./.venv/bin/activate
```

### Comparing `types-circuitpython-8.1.0b2/types_circuitpython.egg-info/SOURCES.txt` & `types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b2/types_circuitpython.egg-info/top_level.txt` & `types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/top_level.txt`

 * *Files identical despite different names*

