# Comparing `tmp/types-circuitpython-8.1.0b1.tar.gz` & `tmp/types-circuitpython-8.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-circuitpython-8.1.0b1.tar", last modified: Tue May 16 15:44:15 2023, max compression
+gzip compressed data, was "types-circuitpython-8.1.0b2.tar", last modified: Tue May 16 15:44:48 2023, max compression
```

## Comparing `types-circuitpython-8.1.0b1.tar` & `types-circuitpython-8.1.0b2.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.232574 types-circuitpython-8.1.0b1/
--rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.1.0b1/LICENSE
--rw-r--r--   0 timon      (501) staff       (20)     3630 2023-05-16 15:44:15.232030 types-circuitpython-8.1.0b1/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2573 2023-05-16 15:44:12.000000 types-circuitpython-8.1.0b1/README.md
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.165948 types-circuitpython-8.1.0b1/bindings/
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.168917 types-circuitpython-8.1.0b1/bindings/__future__/
--rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/__future__/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.169405 types-circuitpython-8.1.0b1/bindings/_bleio/
--rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/_bleio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.170044 types-circuitpython-8.1.0b1/bindings/_eve/
--rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/_eve/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.170588 types-circuitpython-8.1.0b1/bindings/_pew/
--rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/_pew/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.171069 types-circuitpython-8.1.0b1/bindings/_pixelmap/
--rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/_pixelmap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.171476 types-circuitpython-8.1.0b1/bindings/_stage/
--rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/_stage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.171882 types-circuitpython-8.1.0b1/bindings/adafruit_bus_device/
--rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.172438 types-circuitpython-8.1.0b1/bindings/adafruit_pixelbuf/
--rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.172927 types-circuitpython-8.1.0b1/bindings/aesio/
--rw-r--r--   0 timon      (501) staff       (20)     2602 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/aesio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.173392 types-circuitpython-8.1.0b1/bindings/alarm/
--rw-r--r--   0 timon      (501) staff       (20)     7021 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/alarm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.173813 types-circuitpython-8.1.0b1/bindings/analogbufio/
--rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/analogbufio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.174237 types-circuitpython-8.1.0b1/bindings/analogio/
--rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/analogio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.174793 types-circuitpython-8.1.0b1/bindings/atexit/
--rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/atexit/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.175451 types-circuitpython-8.1.0b1/bindings/audiobusio/
--rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/audiobusio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.176106 types-circuitpython-8.1.0b1/bindings/audiocore/
--rw-r--r--   0 timon      (501) staff       (20)     4614 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/audiocore/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.176768 types-circuitpython-8.1.0b1/bindings/audioio/
--rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/audioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.177468 types-circuitpython-8.1.0b1/bindings/audiomixer/
--rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/audiomixer/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.183173 types-circuitpython-8.1.0b1/bindings/audiomp3/
--rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/audiomp3/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.183829 types-circuitpython-8.1.0b1/bindings/audiopwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4448 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/audiopwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.184482 types-circuitpython-8.1.0b1/bindings/bitbangio/
--rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/bitbangio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.185135 types-circuitpython-8.1.0b1/bindings/bitmaptools/
--rw-r--r--   0 timon      (501) staff       (20)    12387 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/bitmaptools/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.185870 types-circuitpython-8.1.0b1/bindings/bitops/
--rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/bitops/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.186956 types-circuitpython-8.1.0b1/bindings/board/
--rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-16 15:44:02.000000 types-circuitpython-8.1.0b1/bindings/board/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.193849 types-circuitpython-8.1.0b1/bindings/busio/
--rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/busio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.194763 types-circuitpython-8.1.0b1/bindings/camera/
--rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/camera/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.195320 types-circuitpython-8.1.0b1/bindings/canio/
--rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/canio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.195827 types-circuitpython-8.1.0b1/bindings/countio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/countio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.196264 types-circuitpython-8.1.0b1/bindings/digitalio/
--rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/digitalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.196700 types-circuitpython-8.1.0b1/bindings/displayio/
--rw-r--r--   0 timon      (501) staff       (20)    39536 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/displayio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.197491 types-circuitpython-8.1.0b1/bindings/dualbank/
--rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/dualbank/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.197943 types-circuitpython-8.1.0b1/bindings/floppyio/
--rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/floppyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.198339 types-circuitpython-8.1.0b1/bindings/fontio/
--rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/fontio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.198764 types-circuitpython-8.1.0b1/bindings/framebufferio/
--rw-r--r--   0 timon      (501) staff       (20)     3553 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/framebufferio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.199165 types-circuitpython-8.1.0b1/bindings/frequencyio/
--rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/frequencyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.199615 types-circuitpython-8.1.0b1/bindings/getpass/
--rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/getpass/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.200122 types-circuitpython-8.1.0b1/bindings/gifio/
--rw-r--r--   0 timon      (501) staff       (20)     5582 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/gifio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.200544 types-circuitpython-8.1.0b1/bindings/gnss/
--rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/gnss/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.201016 types-circuitpython-8.1.0b1/bindings/hashlib/
--rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/hashlib/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.201415 types-circuitpython-8.1.0b1/bindings/i2ctarget/
--rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/i2ctarget/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.201861 types-circuitpython-8.1.0b1/bindings/imagecapture/
--rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/imagecapture/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.202273 types-circuitpython-8.1.0b1/bindings/ipaddress/
--rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/ipaddress/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.202680 types-circuitpython-8.1.0b1/bindings/is31fl3741/
--rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/is31fl3741/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.203084 types-circuitpython-8.1.0b1/bindings/keypad/
--rw-r--r--   0 timon      (501) staff       (20)    13080 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/keypad/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.203558 types-circuitpython-8.1.0b1/bindings/math/
--rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/math/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.204000 types-circuitpython-8.1.0b1/bindings/mdns/
--rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/mdns/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.204491 types-circuitpython-8.1.0b1/bindings/memorymap/
--rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/memorymap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.204981 types-circuitpython-8.1.0b1/bindings/memorymonitor/
--rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/memorymonitor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.205516 types-circuitpython-8.1.0b1/bindings/microcontroller/
--rw-r--r--   0 timon      (501) staff       (20)     6071 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/microcontroller/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.205928 types-circuitpython-8.1.0b1/bindings/msgpack/
--rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/msgpack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.206390 types-circuitpython-8.1.0b1/bindings/neopixel_write/
--rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/neopixel_write/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.206845 types-circuitpython-8.1.0b1/bindings/nvm/
--rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/nvm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.207436 types-circuitpython-8.1.0b1/bindings/onewireio/
--rw-r--r--   0 timon      (501) staff       (20)     1646 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/onewireio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.207990 types-circuitpython-8.1.0b1/bindings/os/
--rw-r--r--   0 timon      (501) staff       (20)     3776 2023-05-16 15:44:03.000000 types-circuitpython-8.1.0b1/bindings/os/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.208577 types-circuitpython-8.1.0b1/bindings/paralleldisplay/
--rw-r--r--   0 timon      (501) staff       (20)     2416 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.208991 types-circuitpython-8.1.0b1/bindings/ps2io/
--rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/ps2io/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.209417 types-circuitpython-8.1.0b1/bindings/pulseio/
--rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/pulseio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.209837 types-circuitpython-8.1.0b1/bindings/pwmio/
--rw-r--r--   0 timon      (501) staff       (20)     5906 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/pwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.210237 types-circuitpython-8.1.0b1/bindings/qrio/
--rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/qrio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.210732 types-circuitpython-8.1.0b1/bindings/rainbowio/
--rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/rainbowio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.211264 types-circuitpython-8.1.0b1/bindings/random/
--rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/random/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.211728 types-circuitpython-8.1.0b1/bindings/rgbmatrix/
--rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.212214 types-circuitpython-8.1.0b1/bindings/rotaryio/
--rw-r--r--   0 timon      (501) staff       (20)     2660 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/rotaryio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.212690 types-circuitpython-8.1.0b1/bindings/rtc/
--rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/rtc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.213371 types-circuitpython-8.1.0b1/bindings/sdcardio/
--rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/sdcardio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.213984 types-circuitpython-8.1.0b1/bindings/sdioio/
--rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/sdioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.214614 types-circuitpython-8.1.0b1/bindings/sharpdisplay/
--rw-r--r--   0 timon      (501) staff       (20)     1763 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.215123 types-circuitpython-8.1.0b1/bindings/socketpool/
--rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/socketpool/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.215732 types-circuitpython-8.1.0b1/bindings/ssl/
--rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/ssl/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.216322 types-circuitpython-8.1.0b1/bindings/storage/
--rw-r--r--   0 timon      (501) staff       (20)     5949 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/storage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.216807 types-circuitpython-8.1.0b1/bindings/struct/
--rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/struct/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.217352 types-circuitpython-8.1.0b1/bindings/supervisor/
--rw-r--r--   0 timon      (501) staff       (20)    10816 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/supervisor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.218423 types-circuitpython-8.1.0b1/bindings/synthio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/synthio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.218883 types-circuitpython-8.1.0b1/bindings/terminalio/
--rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/terminalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.219310 types-circuitpython-8.1.0b1/bindings/time/
--rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/time/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.219884 types-circuitpython-8.1.0b1/bindings/touchio/
--rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/touchio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.220554 types-circuitpython-8.1.0b1/bindings/traceback/
--rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/traceback/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.221507 types-circuitpython-8.1.0b1/bindings/uheap/
--rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/uheap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.222175 types-circuitpython-8.1.0b1/bindings/usb/
--rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/usb/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.222641 types-circuitpython-8.1.0b1/bindings/usb_cdc/
--rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/usb_cdc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.223225 types-circuitpython-8.1.0b1/bindings/usb_hid/
--rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/usb_hid/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.223830 types-circuitpython-8.1.0b1/bindings/usb_host/
--rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/usb_host/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.224366 types-circuitpython-8.1.0b1/bindings/usb_midi/
--rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/usb_midi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.225186 types-circuitpython-8.1.0b1/bindings/ustack/
--rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/ustack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.225814 types-circuitpython-8.1.0b1/bindings/vectorio/
--rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/vectorio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.226703 types-circuitpython-8.1.0b1/bindings/watchdog/
--rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:44:04.000000 types-circuitpython-8.1.0b1/bindings/watchdog/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.227302 types-circuitpython-8.1.0b1/bindings/wifi/
--rw-r--r--   0 timon      (501) staff       (20)     9256 2023-05-16 15:44:05.000000 types-circuitpython-8.1.0b1/bindings/wifi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.227937 types-circuitpython-8.1.0b1/bindings/zlib/
--rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:44:05.000000 types-circuitpython-8.1.0b1/bindings/zlib/__init__.pyi
--rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.1.0b1/pyproject.toml
--rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:44:15.232782 types-circuitpython-8.1.0b1/setup.cfg
--rw-r--r--   0 timon      (501) staff       (20)     2181 2023-05-16 15:44:05.000000 types-circuitpython-8.1.0b1/setup.py
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:15.231206 types-circuitpython-8.1.0b1/types_circuitpython.egg-info/
--rw-r--r--   0 timon      (501) staff       (20)     3630 2023-05-16 15:44:15.000000 types-circuitpython-8.1.0b1/types_circuitpython.egg-info/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:44:15.000000 types-circuitpython-8.1.0b1/types_circuitpython.egg-info/SOURCES.txt
--rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:44:15.000000 types-circuitpython-8.1.0b1/types_circuitpython.egg-info/dependency_links.txt
--rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:44:15.000000 types-circuitpython-8.1.0b1/types_circuitpython.egg-info/requires.txt
--rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:44:15.000000 types-circuitpython-8.1.0b1/types_circuitpython.egg-info/top_level.txt
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.163987 types-circuitpython-8.1.0b2/
+-rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.1.0b2/LICENSE
+-rw-r--r--   0 timon      (501) staff       (20)     3630 2023-05-16 15:44:48.163519 types-circuitpython-8.1.0b2/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2573 2023-05-16 15:44:12.000000 types-circuitpython-8.1.0b2/README.md
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.113285 types-circuitpython-8.1.0b2/bindings/
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.115922 types-circuitpython-8.1.0b2/bindings/__future__/
+-rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/__future__/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.116332 types-circuitpython-8.1.0b2/bindings/_bleio/
+-rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_bleio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.116860 types-circuitpython-8.1.0b2/bindings/_eve/
+-rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_eve/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.117389 types-circuitpython-8.1.0b2/bindings/_pew/
+-rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_pew/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.117796 types-circuitpython-8.1.0b2/bindings/_pixelmap/
+-rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_pixelmap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.118175 types-circuitpython-8.1.0b2/bindings/_stage/
+-rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/_stage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.118547 types-circuitpython-8.1.0b2/bindings/adafruit_bus_device/
+-rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.118930 types-circuitpython-8.1.0b2/bindings/adafruit_pixelbuf/
+-rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.119336 types-circuitpython-8.1.0b2/bindings/aesio/
+-rw-r--r--   0 timon      (501) staff       (20)     2602 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/aesio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.119782 types-circuitpython-8.1.0b2/bindings/alarm/
+-rw-r--r--   0 timon      (501) staff       (20)     7021 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/alarm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.120203 types-circuitpython-8.1.0b2/bindings/analogbufio/
+-rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/analogbufio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.120641 types-circuitpython-8.1.0b2/bindings/analogio/
+-rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/analogio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.121065 types-circuitpython-8.1.0b2/bindings/atexit/
+-rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/atexit/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.121479 types-circuitpython-8.1.0b2/bindings/audiobusio/
+-rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiobusio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.121928 types-circuitpython-8.1.0b2/bindings/audiocore/
+-rw-r--r--   0 timon      (501) staff       (20)     4607 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiocore/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.122354 types-circuitpython-8.1.0b2/bindings/audioio/
+-rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.122739 types-circuitpython-8.1.0b2/bindings/audiomixer/
+-rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiomixer/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.123217 types-circuitpython-8.1.0b2/bindings/audiomp3/
+-rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiomp3/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.123701 types-circuitpython-8.1.0b2/bindings/audiopwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4448 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/audiopwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.124131 types-circuitpython-8.1.0b2/bindings/bitbangio/
+-rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/bitbangio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.124604 types-circuitpython-8.1.0b2/bindings/bitmaptools/
+-rw-r--r--   0 timon      (501) staff       (20)    13492 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/bitmaptools/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.125005 types-circuitpython-8.1.0b2/bindings/bitops/
+-rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:44:36.000000 types-circuitpython-8.1.0b2/bindings/bitops/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.125374 types-circuitpython-8.1.0b2/bindings/board/
+-rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/board/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.125766 types-circuitpython-8.1.0b2/bindings/busio/
+-rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/busio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.126205 types-circuitpython-8.1.0b2/bindings/camera/
+-rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/camera/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.126573 types-circuitpython-8.1.0b2/bindings/canio/
+-rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/canio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.127115 types-circuitpython-8.1.0b2/bindings/countio/
+-rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/countio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.127836 types-circuitpython-8.1.0b2/bindings/digitalio/
+-rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/digitalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.128528 types-circuitpython-8.1.0b2/bindings/displayio/
+-rw-r--r--   0 timon      (501) staff       (20)    40033 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/displayio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.129403 types-circuitpython-8.1.0b2/bindings/dualbank/
+-rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/dualbank/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.130238 types-circuitpython-8.1.0b2/bindings/floppyio/
+-rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/floppyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.131021 types-circuitpython-8.1.0b2/bindings/fontio/
+-rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/fontio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.131726 types-circuitpython-8.1.0b2/bindings/framebufferio/
+-rw-r--r--   0 timon      (501) staff       (20)     3743 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/framebufferio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.132550 types-circuitpython-8.1.0b2/bindings/frequencyio/
+-rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/frequencyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.133259 types-circuitpython-8.1.0b2/bindings/getpass/
+-rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/getpass/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.133922 types-circuitpython-8.1.0b2/bindings/gifio/
+-rw-r--r--   0 timon      (501) staff       (20)     5691 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/gifio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.134555 types-circuitpython-8.1.0b2/bindings/gnss/
+-rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/gnss/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.135296 types-circuitpython-8.1.0b2/bindings/hashlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/hashlib/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.135992 types-circuitpython-8.1.0b2/bindings/i2ctarget/
+-rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/i2ctarget/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.136653 types-circuitpython-8.1.0b2/bindings/imagecapture/
+-rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/imagecapture/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.137340 types-circuitpython-8.1.0b2/bindings/ipaddress/
+-rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/ipaddress/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.137967 types-circuitpython-8.1.0b2/bindings/is31fl3741/
+-rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/is31fl3741/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.138567 types-circuitpython-8.1.0b2/bindings/keypad/
+-rw-r--r--   0 timon      (501) staff       (20)    13080 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/keypad/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.139297 types-circuitpython-8.1.0b2/bindings/math/
+-rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/math/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.140100 types-circuitpython-8.1.0b2/bindings/mdns/
+-rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/mdns/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.141073 types-circuitpython-8.1.0b2/bindings/memorymap/
+-rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/memorymap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.142176 types-circuitpython-8.1.0b2/bindings/memorymonitor/
+-rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/memorymonitor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.143280 types-circuitpython-8.1.0b2/bindings/microcontroller/
+-rw-r--r--   0 timon      (501) staff       (20)     6071 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/microcontroller/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.143898 types-circuitpython-8.1.0b2/bindings/msgpack/
+-rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/msgpack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.144820 types-circuitpython-8.1.0b2/bindings/neopixel_write/
+-rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/neopixel_write/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.145835 types-circuitpython-8.1.0b2/bindings/nvm/
+-rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/nvm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.146636 types-circuitpython-8.1.0b2/bindings/onewireio/
+-rw-r--r--   0 timon      (501) staff       (20)     1671 2023-05-16 15:44:37.000000 types-circuitpython-8.1.0b2/bindings/onewireio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.147204 types-circuitpython-8.1.0b2/bindings/os/
+-rw-r--r--   0 timon      (501) staff       (20)     3750 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/os/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.147603 types-circuitpython-8.1.0b2/bindings/paralleldisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     2416 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.147992 types-circuitpython-8.1.0b2/bindings/ps2io/
+-rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/ps2io/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.148356 types-circuitpython-8.1.0b2/bindings/pulseio/
+-rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/pulseio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.148754 types-circuitpython-8.1.0b2/bindings/pwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     5906 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/pwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.149123 types-circuitpython-8.1.0b2/bindings/qrio/
+-rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/qrio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.149490 types-circuitpython-8.1.0b2/bindings/rainbowio/
+-rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rainbowio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.149852 types-circuitpython-8.1.0b2/bindings/random/
+-rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/random/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.150209 types-circuitpython-8.1.0b2/bindings/rgbmatrix/
+-rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.150559 types-circuitpython-8.1.0b2/bindings/rotaryio/
+-rw-r--r--   0 timon      (501) staff       (20)     2660 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rotaryio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.151124 types-circuitpython-8.1.0b2/bindings/rtc/
+-rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/rtc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.151568 types-circuitpython-8.1.0b2/bindings/sdcardio/
+-rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/sdcardio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.152041 types-circuitpython-8.1.0b2/bindings/sdioio/
+-rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/sdioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.152499 types-circuitpython-8.1.0b2/bindings/sharpdisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     1763 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.152919 types-circuitpython-8.1.0b2/bindings/socketpool/
+-rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/socketpool/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.153331 types-circuitpython-8.1.0b2/bindings/ssl/
+-rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/ssl/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.153717 types-circuitpython-8.1.0b2/bindings/storage/
+-rw-r--r--   0 timon      (501) staff       (20)     5949 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/storage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.154123 types-circuitpython-8.1.0b2/bindings/struct/
+-rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/struct/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.154502 types-circuitpython-8.1.0b2/bindings/supervisor/
+-rw-r--r--   0 timon      (501) staff       (20)    10934 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/supervisor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.154887 types-circuitpython-8.1.0b2/bindings/synthio/
+-rw-r--r--   0 timon      (501) staff       (20)     6160 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/synthio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.155270 types-circuitpython-8.1.0b2/bindings/terminalio/
+-rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/terminalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.155657 types-circuitpython-8.1.0b2/bindings/time/
+-rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/time/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.156030 types-circuitpython-8.1.0b2/bindings/touchio/
+-rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/touchio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.156433 types-circuitpython-8.1.0b2/bindings/traceback/
+-rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/traceback/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.156838 types-circuitpython-8.1.0b2/bindings/uheap/
+-rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/uheap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.157234 types-circuitpython-8.1.0b2/bindings/usb/
+-rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.157611 types-circuitpython-8.1.0b2/bindings/usb_cdc/
+-rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_cdc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.158003 types-circuitpython-8.1.0b2/bindings/usb_hid/
+-rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_hid/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.158395 types-circuitpython-8.1.0b2/bindings/usb_host/
+-rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_host/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.158793 types-circuitpython-8.1.0b2/bindings/usb_midi/
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/usb_midi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.159160 types-circuitpython-8.1.0b2/bindings/ustack/
+-rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/ustack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.159539 types-circuitpython-8.1.0b2/bindings/vectorio/
+-rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/vectorio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.159919 types-circuitpython-8.1.0b2/bindings/watchdog/
+-rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/watchdog/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.160303 types-circuitpython-8.1.0b2/bindings/wifi/
+-rw-r--r--   0 timon      (501) staff       (20)     9835 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/wifi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.160684 types-circuitpython-8.1.0b2/bindings/zlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:44:38.000000 types-circuitpython-8.1.0b2/bindings/zlib/__init__.pyi
+-rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.1.0b2/pyproject.toml
+-rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:44:48.164167 types-circuitpython-8.1.0b2/setup.cfg
+-rw-r--r--   0 timon      (501) staff       (20)     2181 2023-05-16 15:44:39.000000 types-circuitpython-8.1.0b2/setup.py
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:44:48.162939 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/
+-rw-r--r--   0 timon      (501) staff       (20)     3630 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/SOURCES.txt
+-rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/dependency_links.txt
+-rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/requires.txt
+-rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:44:48.000000 types-circuitpython-8.1.0b2/types_circuitpython.egg-info/top_level.txt
```

### Comparing `types-circuitpython-8.1.0b1/LICENSE` & `types-circuitpython-8.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/PKG-INFO` & `types-circuitpython-8.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.1.0b1
+Version: 8.1.0b2
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
```

### Comparing `types-circuitpython-8.1.0b1/README.md` & `types-circuitpython-8.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/__future__/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/__future__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/_bleio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/_eve/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/_pew/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/_pixelmap/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/_stage/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/adafruit_pixelbuf/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/aesio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/alarm/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/analogbufio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/analogio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/atexit/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/audiobusio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/audiocore/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/audiocore/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class RawSample:
     """A raw audio sample buffer in memory"""
 
     def __init__(
         self, buffer: ReadableBuffer, *, channel_count: int = 1, sample_rate: int = 8000
     ) -> None:
-        """Create a RawSample based on the given buffer of signed values. If channel_count is more than
+        """Create a RawSample based on the given buffer of values. If channel_count is more than
         1 then each channel's samples should alternate. In other words, for a two channel buffer, the
         first sample will be for channel 1, the second sample will be for channel two, the third for
         channel 1 and so on.
 
         :param ~circuitpython_typing.ReadableBuffer buffer: A buffer with samples
         :param int channel_count: The number of channels in the buffer
         :param int sample_rate: The desired playback sample rate
```

### Comparing `types-circuitpython-8.1.0b1/bindings/audioio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/audiomixer/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/audiomp3/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/audiopwmio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/bitbangio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/bitmaptools/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/bitmaptools/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -269,7 +269,48 @@
 
     :param bitmap dest_bitmap: Destination bitmap.  It must have a value_count of 2 or 65536.  The stored values are 0 and the maximum pixel value.
     :param bitmap source_bitmap: Source bitmap that contains the graphical region to be dithered.  It must have a value_count of 65536.
     :param colorspace: The colorspace of the image.  The supported colorspaces are ``RGB565``, ``BGR565``, ``RGB565_SWAPPED``, and ``BGR565_SWAPPED``
     :param algorithm: The dither algorithm to use, one of the `DitherAlgorithm` values.
     """
     ...
+
+def draw_circle(
+    dest_bitmap: displayio.Bitmap, x: int, y: int, radius: int, value: int
+) -> None:
+    """Draws a circle into a bitmap specified using a center (x0,y0) and radius r.
+
+    :param bitmap dest_bitmap: Destination bitmap that will be written into
+    :param int x: x-pixel position of the circle's center
+    :param int y: y-pixel position of the circle's center
+    :param int radius: circle's radius
+    :param int value: Bitmap palette index that will be written into the
+           circle in the destination bitmap
+
+    .. code-block:: Python
+
+       import board
+       import displayio
+       import bitmaptools
+
+       display = board.DISPLAY
+       main_group = displayio.Group()
+       display.root_group = main_group
+
+       palette = displayio.Palette(2)
+       palette[0] = 0xffffff
+       palette[1] = 0x440044
+
+       bmp = displayio.Bitmap(128,128, 2)
+       bmp.fill(0)
+
+       bitmaptools.circle(64,64, 32, 1)
+
+       tilegrid = displayio.TileGrid(bitmap=bmp, pixel_shader=palette)
+       main_group.append(tilegrid)
+
+       while True:
+           pass
+
+    """
+
+    ...
```

### Comparing `types-circuitpython-8.1.0b1/bindings/bitops/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/board/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/busio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/camera/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/canio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/countio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/digitalio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/displayio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/displayio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 
 import typing
 from typing import Optional, Tuple, Union
 
 import busio
 import circuitpython_typing
 import microcontroller
-import paralleldisplay
 import vectorio
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
 
+CIRCUITPYTHON_TERMINAL: Group
+"""The `displayio.Group` that is the displayed serial terminal (REPL)."""
+
+import paralleldisplay
+
 def release_displays() -> None:
     """Releases any actively used displays so their buses and pins can be used again. This will also
     release the builtin display on boards that have one. You will need to reinitialize it yourself
     afterwards. This may take seconds to complete if an active EPaperDisplay is refreshing.
 
     Use this once in your code.py if you initialize a display. Place it right before the
     initialization so the display is active as long as possible."""
@@ -318,15 +322,16 @@
     """Gets the height of the board"""
     rotation: int
     """The rotation of the display as an int in degrees."""
     bus: _DisplayBus
     """The bus being used by the display"""
     root_group: Group
     """The root group on the display.
-    If the root group is set to ``None``, the default CircuitPython terminal will be shown.
+    If the root group is set to `displayio.CIRCUITPYTHON_TERMINAL`, the default CircuitPython terminal will be shown.
+    If the root group is set to ``None``, no output will be shown.
     """
     def fill_row(self, y: int, buffer: WriteableBuffer) -> WriteableBuffer:
         """Extract the pixels from a single row
 
         :param int y: The top edge of the area
         :param ~circuitpython_typing.WriteableBuffer buffer: The buffer in which to place the pixel data
         """
@@ -370,14 +375,15 @@
         busy_state: bool = True,
         seconds_per_frame: float = 180,
         always_toggle_chip_select: bool = False,
         grayscale: bool = False,
         advanced_color_epaper: bool = False,
         two_byte_sequence_length: bool = False,
         start_up_time: float = 0,
+        address_little_endian: bool = False,
     ) -> None:
         """Create a EPaperDisplay object on the given display bus (`displayio.FourWire` or `paralleldisplay.ParallelBus`).
 
         The ``start_sequence`` and ``stop_sequence`` are bitpacked to minimize the ram impact. Every
         command begins with a command byte followed by a byte to determine the parameter count and
         delay. When the top bit of the second byte is 1 (0x80), a delay will occur after the command
         parameters are sent. The remaining 7 bits are the parameter count excluding any delay
@@ -411,14 +417,15 @@
         :param bool busy_state: State of the busy pin when the display is busy
         :param float seconds_per_frame: Minimum number of seconds between screen refreshes
         :param bool always_toggle_chip_select: When True, chip select is toggled every byte
         :param bool grayscale: When true, the color ram is the low bit of 2-bit grayscale
         :param bool advanced_color_epaper: When true, the display is a 7-color advanced color epaper (ACeP)
         :param bool two_byte_sequence_length: When true, use two bytes to define sequence length
         :param float start_up_time: Time to wait after reset before sending commands
+        :param bool address_little_endian: Send the least significant byte (not bit) of multi-byte addresses first. Ignored when ram is addressed with one byte
         """
         ...
     def show(self, group: Group) -> None:
         """
         .. note:: `show()` is deprecated and will be removed in CircuitPython 9.0.0.
           Use ``.root_group = group`` instead.
 
@@ -448,15 +455,16 @@
     rotation: int
     """The rotation of the display as an int in degrees."""
     bus: _DisplayBus
     """The bus being used by the display"""
 
     root_group: Group
     """The root group on the epaper display.
-    If the root group is set to ``None``, the default CircuitPython terminal will be shown.
+    If the root group is set to `displayio.CIRCUITPYTHON_TERMINAL`, the default CircuitPython terminal will be shown.
+    If the root group is set to ``None``, no output will be shown.
     """
 
 class FourWire:
     """Manage updating a display over SPI four wire protocol in the background while Python code runs.
     It doesn't handle display initialization."""
 
     def __init__(
```

### Comparing `types-circuitpython-8.1.0b1/bindings/dualbank/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/floppyio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/fontio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/framebufferio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/framebufferio/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -73,8 +73,11 @@
         """Extract the pixels from a single row
 
         :param int y: The top edge of the area
         :param ~circuitpython_typing.WriteableBuffer buffer: The buffer in which to place the pixel data
         """
         ...
     root_group: displayio.Group
-    """The root group on the display."""
+    """The root group on the display.
+    If the root group is set to `displayio.CIRCUITPYTHON_TERMINAL`, the default CircuitPython terminal will be shown.
+    If the root group is set to ``None``, no output will be shown.
+    """
```

### Comparing `types-circuitpython-8.1.0b1/bindings/frequencyio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/getpass/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/gifio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/gifio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Access GIF-format images
 """
 
 from __future__ import annotations
 
 import typing
-from typing import Union
+from typing import Optional, Union
 
 import displayio
 from circuitpython_typing import ReadableBuffer
 
 class GifWriter:
     def __init__(
         self,
@@ -137,14 +137,16 @@
         ...
     width: int
     """Width of the gif. (read only)"""
     height: int
     """Height of the gif. (read only)"""
     bitmap: displayio.Bitmap
     """The bitmap used to hold the current frame."""
+    palette: Optional[displayio.Palette]
+    """The palette for the current frame if it exists."""
     def next_frame(self) -> float:
         """Loads the next frame. Returns expected delay before the next frame in seconds."""
     duration: float
     """Returns the total duration of the GIF in seconds. (read only)"""
     frame_count: int
     """Returns the number of frames in the GIF. (read only)"""
     min_delay: float
```

### Comparing `types-circuitpython-8.1.0b1/bindings/gnss/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/hashlib/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/i2ctarget/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/imagecapture/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/ipaddress/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/is31fl3741/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/keypad/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/math/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/mdns/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/memorymap/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/memorymonitor/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/microcontroller/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/msgpack/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/neopixel_write/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/nvm/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/onewireio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/onewireio/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Low-level bit primitives for Maxim (formerly Dallas Semi) one-wire protocol.
 
-   Protocol definition is here: https://www.maximintegrated.com/en/app-notes/index.mvp/id/126"""
+   Protocol definition is here: https://www.analog.com/en/technical-articles/1wire-communication-through-software.html"""
 
 from __future__ import annotations
 
 import microcontroller
 
 class OneWire:
     def __init__(self, pin: microcontroller.Pin) -> None:
```

### Comparing `types-circuitpython-8.1.0b1/bindings/os/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/os/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """Sync all filesystems."""
     ...
 
 def urandom(size: int) -> str:
     """Returns a string of *size* random bytes based on a hardware True Random
     Number Generator. When not available, it will raise a NotImplementedError.
 
-    **Limitations:** Not yet available on nRF. Not available on SAMD21 due to lack of hardware.
+    **Limitations:** Not available on SAMD21 due to lack of hardware.
     """
     ...
 
 def utime(path: str, times: Tuple[int, int]) -> None:
     """Change the timestamp of a file."""
     ...
```

### Comparing `types-circuitpython-8.1.0b1/bindings/paralleldisplay/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/ps2io/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/pulseio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/pwmio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/qrio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/random/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/rgbmatrix/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/rotaryio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/rtc/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/sdcardio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/sdioio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/sharpdisplay/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/socketpool/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/ssl/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/storage/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/struct/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/supervisor/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/supervisor/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -181,16 +181,18 @@
     """Whether CircuitPython may autoreload based on workflow writes to the filesystem."""
 
     ble_workflow: bool
     """Enable/Disable ble workflow until a reset. This prevents BLE advertising outside of the VM and
     the services used for it."""
 
     next_stack_limit: int
-    """The size of the stack for the next vm run. If its too large, the default will be used."""
+    """The size of the stack for the next vm run. If its too large, the default will be used.
 
+    **Limitations**: Stack size is fixed at startup on the ``espressif`` port; setting this will have no effect.
+    """
     rgb_status_brightness: int
     """Set brightness of status RGB LED from 0-255. This will take effect
     after the current code finishes and the status LED is used to show
     the finish state."""
 
 class SafeModeReason:
     """The reason that CircuitPython went into safe mode.
```

### Comparing `types-circuitpython-8.1.0b1/bindings/terminalio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/time/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/touchio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/traceback/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/usb_cdc/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/usb_hid/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/usb_host/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/usb_midi/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/vectorio/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/watchdog/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/bindings/wifi/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/wifi/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -156,74 +156,84 @@
         ssid: Union[str | ReadableBuffer],
         password: Union[str | ReadableBuffer] = b"",
         *,
         channel: int = 1,
         authmode: Optional[AuthMode] = None,
         max_connections: Optional[int] = 4,
     ) -> None:
-        """Starts an Access Point with the specified ssid and password.
+        """Starts running an access point with the specified ssid and password.
 
         If ``channel`` is given, the access point will use that channel unless
         a station is already operating on a different channel.
 
         If ``authmode`` is not None, the access point will use that Authentication
         mode. If a non-empty password is given, ``authmode`` must not be ``OPEN``.
         If ``authmode`` is not given or is None,
         ``OPEN`` will be used when the password is the empty string,
         otherwise ``authmode`` will be ``WPA_WPA2_PSK``.
 
+        The length of ``password`` must be 8-63 characters if it is ASCII,
+        or exactly 64 hexadecimal characters if it is the hex form of the 256-bit key.
+
         If ``max_connections`` is given, the access point will allow up to
         that number of stations to connect."""
         ...
     def stop_ap(self) -> None:
-        """Stops the Access Point."""
+        """Stops the access point."""
         ...
+    ap_active: bool
+    """True if running as an access point. (read-only)"""
     def connect(
         self,
         ssid: Union[str | ReadableBuffer],
         password: Union[str | ReadableBuffer] = b"",
         *,
         channel: int = 0,
         bssid: Optional[Union[str | ReadableBuffer]] = None,
         timeout: Optional[float] = None,
     ) -> None:
         """Connects to the given ssid and waits for an ip address. Reconnections are handled
         automatically once one connection succeeds.
 
+        The length of ``password`` must be 0 if there is no password, 8-63 characters if it is ASCII,
+        or exactly 64 hexadecimal characters if it is the hex form of the 256-bit key.
+
         By default, this will scan all channels and connect to the access point (AP) with the
         given ``ssid`` and greatest signal strength (rssi).
 
         If ``channel`` is non-zero, the scan will begin with the given channel and connect to
         the first AP with the given ``ssid``. This can speed up the connection time
         significantly because a full scan doesn't occur.
 
         If ``bssid`` is given and not None, the scan will start at the first channel or the one given and
         connect to the AP with the given ``bssid`` and ``ssid``."""
         ...
+    connected: bool
+    """True if connected to an access point (read-only)."""
     ipv4_gateway: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the station gateway when connected to an access point. None otherwise."""
+    """IP v4 Address of the station gateway when connected to an access point. None otherwise. (read-only)"""
     ipv4_gateway_ap: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the access point gateway, when enabled. None otherwise."""
+    """IP v4 Address of the access point gateway, when enabled. None otherwise. (read-only)"""
     ipv4_subnet: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the station subnet when connected to an access point. None otherwise."""
+    """IP v4 Address of the station subnet when connected to an access point. None otherwise. (read-only)"""
     ipv4_subnet_ap: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the access point subnet, when enabled. None otherwise."""
+    """IP v4 Address of the access point subnet, when enabled. None otherwise. (read-only)"""
     def set_ipv4_address(
         self,
         *,
         ipv4: ipaddress.IPv4Address,
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
         ipv4_dns: Optional[ipaddress.IPv4Address],
     ) -> None:
         """Sets the IP v4 address of the station. Must include the netmask and gateway. DNS address is optional.
         Setting the address manually will stop the DHCP client."""
         ...
     ipv4_address: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the station when connected to an access point. None otherwise."""
+    """IP v4 Address of the station when connected to an access point. None otherwise. (read-only)"""
     ipv4_address_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point, when enabled. None otherwise."""
     ipv4_dns: ipaddress.IPv4Address
     """IP v4 Address of the DNS server to be used."""
     ap_info: Optional[Network]
     """Network object containing BSSID, SSID, authmode, channel, country and RSSI when connected to an access point. None otherwise."""
     def start_dhcp(self) -> None:
```

### Comparing `types-circuitpython-8.1.0b1/bindings/zlib/__init__.pyi` & `types-circuitpython-8.1.0b2/bindings/zlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/setup.py` & `types-circuitpython-8.1.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir, path
 
 from setuptools import setup
 
 __name__ = "types-circuitpython"
-__version__ = "8.1.0-beta.1"
+__version__ = "8.1.0-beta.2"
 __repo__ = "https://github.com/hardfury-labs/types-circuitpython"
 __author__ = "HardFury"
 
 
 HERE = path.abspath(path.dirname(__file__))
 BINDINGS_DIR = path.join(HERE, "bindings")
```

### Comparing `types-circuitpython-8.1.0b1/types_circuitpython.egg-info/PKG-INFO` & `types-circuitpython-8.1.0b2/types_circuitpython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.1.0b1
+Version: 8.1.0b2
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
```

### Comparing `types-circuitpython-8.1.0b1/types_circuitpython.egg-info/SOURCES.txt` & `types-circuitpython-8.1.0b2/types_circuitpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0b1/types_circuitpython.egg-info/top_level.txt` & `types-circuitpython-8.1.0b2/types_circuitpython.egg-info/top_level.txt`

 * *Files identical despite different names*

