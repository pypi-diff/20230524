# Comparing `tmp/sj201_interface-0.0.3a0-py3-none-any.whl.zip` & `tmp/sj201_interface-0.0.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 26837 bytes, number of entries: 17
--rw-r--r--  2.0 unx     1831 b- defN 23-Mar-28 20:00 sj201_interface/__init__.py
--rw-r--r--  2.0 unx     4084 b- defN 23-Mar-28 20:00 sj201_interface/cli.py
--rw-r--r--  2.0 unx     8436 b- defN 23-Mar-28 20:00 sj201_interface/fan.py
--rw-r--r--  2.0 unx     2877 b- defN 23-Mar-28 20:00 sj201_interface/revisions.py
--rw-r--r--  2.0 unx     7345 b- defN 23-Mar-28 20:00 sj201_interface/switches.py
--rw-r--r--  2.0 unx     1856 b- defN 23-Mar-28 20:00 sj201_interface/version.py
--rw-r--r--  2.0 unx    13263 b- defN 23-Mar-28 20:00 sj201_interface/led/__init__.py
--rw-r--r--  2.0 unx     5129 b- defN 23-Mar-28 20:00 sj201_interface/led/animations.py
--rw-r--r--  2.0 unx     1831 b- defN 23-Mar-28 20:00 sj201_interface/util/__init__.py
--rw-r--r--  2.0 unx     2770 b- defN 23-Mar-28 20:00 sj201_interface/util/patches.py
--rw-r--r--  2.0 unx     7038 b- defN 23-Mar-28 20:00 sj201_interface/util/tas5806.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Mar-28 20:00 sj201_interface-0.0.3a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1912 b- defN 23-Mar-28 20:00 sj201_interface-0.0.3a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 20:00 sj201_interface-0.0.3a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 23-Mar-28 20:00 sj201_interface-0.0.3a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-28 20:00 sj201_interface-0.0.3a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1482 b- defN 23-Mar-28 20:00 sj201_interface-0.0.3a0.dist-info/RECORD
-17 files, 61653 bytes uncompressed, 24379 bytes compressed:  60.5%
+Zip file size: 29175 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-24 02:29 sj201_interface/__init__.py
+-rw-r--r--  2.0 unx     4084 b- defN 23-May-24 02:29 sj201_interface/cli.py
+-rw-r--r--  2.0 unx     8436 b- defN 23-May-24 02:29 sj201_interface/fan.py
+-rw-r--r--  2.0 unx     2732 b- defN 23-May-24 02:29 sj201_interface/revisions.py
+-rw-r--r--  2.0 unx     7345 b- defN 23-May-24 02:29 sj201_interface/switches.py
+-rw-r--r--  2.0 unx     1856 b- defN 23-May-24 02:29 sj201_interface/version.py
+-rw-r--r--  2.0 unx    15223 b- defN 23-May-24 02:29 sj201_interface/led/__init__.py
+-rw-r--r--  2.0 unx     5129 b- defN 23-May-24 02:29 sj201_interface/led/animations.py
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-24 02:29 sj201_interface/util/__init__.py
+-rw-r--r--  2.0 unx     2770 b- defN 23-May-24 02:29 sj201_interface/util/patches.py
+-rw-r--r--  2.0 unx     4996 b- defN 23-May-24 02:29 sj201_interface/util/pwmcontroller.py
+-rw-r--r--  2.0 unx     7038 b- defN 23-May-24 02:29 sj201_interface/util/tas5806.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-24 02:29 sj201_interface-0.0.3a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1912 b- defN 23-May-24 02:29 sj201_interface-0.0.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 02:29 sj201_interface-0.0.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-May-24 02:29 sj201_interface-0.0.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-24 02:29 sj201_interface-0.0.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1576 b- defN 23-May-24 02:29 sj201_interface-0.0.3a1.dist-info/RECORD
+18 files, 68558 bytes uncompressed, 26567 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -24,29 +24,32 @@
 
 Filename: sj201_interface/util/__init__.py
 Comment: 
 
 Filename: sj201_interface/util/patches.py
 Comment: 
 
+Filename: sj201_interface/util/pwmcontroller.py
+Comment: 
+
 Filename: sj201_interface/util/tas5806.py
 Comment: 
 
-Filename: sj201_interface-0.0.3a0.dist-info/LICENSE.md
+Filename: sj201_interface-0.0.3a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: sj201_interface-0.0.3a0.dist-info/METADATA
+Filename: sj201_interface-0.0.3a1.dist-info/METADATA
 Comment: 
 
-Filename: sj201_interface-0.0.3a0.dist-info/WHEEL
+Filename: sj201_interface-0.0.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: sj201_interface-0.0.3a0.dist-info/entry_points.txt
+Filename: sj201_interface-0.0.3a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sj201_interface-0.0.3a0.dist-info/top_level.txt
+Filename: sj201_interface-0.0.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sj201_interface-0.0.3a0.dist-info/RECORD
+Filename: sj201_interface-0.0.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj201_interface/revisions.py

```diff
@@ -25,39 +25,38 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from enum import Enum
 from subprocess import Popen, PIPE
 from typing import Optional
+import os
 
 
 class SJ201(Enum):
     r6 = "6"
     r10 = "10"
 
 
 def detect_sj201_revision() -> Optional[SJ201]:
     """
     Detect which revision of SJ201 (if any) is connected.
     """
     tiny_address = "04"
     xmos_address = "2c"
     ti_address = "2f"
-    cmd = "i2cdetect -a -y 1 | grep %s" % (tiny_address,)
-    process = Popen(cmd, stdout=PIPE, stderr=None, shell=True)
-    tiny_is_present = True if process.communicate()[0] else False
-
-    cmd = "i2cdetect -a -y 1 | grep %s" % (xmos_address,)
-    process = Popen(cmd, stdout=PIPE, stderr=None, shell=True)
-    xmos_is_present = True if process.communicate()[0] else False
-
-    cmd = "i2cdetect -a -y 1 | grep %s" % (ti_address,)
-    process = Popen(cmd, stdout=PIPE, stderr=None, shell=True)
-    ti_is_present = True if process.communicate()[0] else False
+
+    i2c_addresses = Popen("i2cdetect -a -y 1", stdout=PIPE, stderr=None, shell=True).communicate()[0].decode("ascii")
+
+    tiny_is_present = tiny_address in i2c_addresses
+    xmos_is_present = xmos_address in i2c_addresses
+    ti_is_present = ti_address in i2c_addresses
 
     if ti_is_present and xmos_is_present:
         if tiny_is_present:
             return SJ201.r6
         else:
             return SJ201.r10
     return None
+
+def sj201_rev10_pwm_fan_overlay_present() -> bool:
+    return os.path.exists('/sys/firmware/devicetree/base/sj201-rev10-pwm-fan@0')
```

## sj201_interface/version.py

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.3a0"
+__version__ = "0.0.3a1"
```

## sj201_interface/led/__init__.py

```diff
@@ -49,15 +49,16 @@
 from enum import Enum
 from time import sleep
 from threading import Thread, Event
 from queue import Queue
 from ovos_utils.log import LOG
 from smbus2.smbus2 import SMBus, I2C_SMBUS_BLOCK_MAX
 
-from sj201_interface.revisions import SJ201, detect_sj201_revision
+from sj201_interface.revisions import SJ201, detect_sj201_revision, sj201_rev10_pwm_fan_overlay_present
+from sj201_interface.util.pwmcontroller import PWMController
 
 
 class Palette(Enum):
     BLACK = (0, 0, 0)
     WHITE = (255, 255, 255)
     YELLOW = (255, 255, 0)
     RED = (255, 0, 0)
@@ -315,14 +316,66 @@
         self.pixels.show()
 
     def set_leds(self, new_leds):
         """set leds from tuple array"""
         for x in range(0, self.num_leds):
             self.set_led(x, new_leds[x])
 
+class HwPwmAwareLed(MycroftLed):
+    def __init__(self, led: MycroftLed):
+        import atexit
+        self.led = led
+        self.pwm = PWMController()
+        self.original_pwm_clck_div = self.pwm.pwm_clk_div.value >> 12
+        self.original_pwm_control = self.pwm.pwm_control.value
+        self.original_pwm1_range = self.pwm.pwm1_range.value
+        # Set the shared PWM Clock Divisor for both PWM channels to the expected value by `rpi_ws281x`
+        self.pwm.pwm_set_clock(8)
+        atexit.register(self.restore_original_registers)
+
+    @property
+    def num_leds(self):
+        return self.led.num_leds
+    
+    def _prep_pwm_clock(self):
+        """Configures PWM1 channel range to expected value for the `rpi_ws281x` library used by AdaFruit Blinka Neopixel"""
+        self.pwm.configure_pwm1(32)
+    
+    def set_led(self, which_led, color, immediate=True):   
+        self._prep_pwm_clock() 
+        return self.led.set_led(which_led, color, immediate)
+
+    def fill(self, color):
+        self._prep_pwm_clock() 
+        return self.led.fill(color)
+
+    def show(self):
+        self._prep_pwm_clock() 
+        return self.led.show()
+
+    def get_led(self, which_led):
+        self._prep_pwm_clock() 
+        return self.led.get_led(which_led)
+
+    def set_leds(self, leds):
+        self._prep_pwm_clock() 
+        return self.led.set_leds(leds)
+
+    def get_capabilities(self):
+        return self.led.get_capabilities()
+    
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.pwm.close()
+
+    def restore_original_registers(self):        
+        with PWMController() as pwm:
+            pwm.pwm_control.value = self.original_pwm_control
+            pwm.pwm_set_clock(self.original_pwm_clck_div)
+            pwm.configure_pwm1(self.original_pwm1_range)
+    
 
 class LedThread(Thread):
     def __init__(self, led_obj, animations=None):
         self.led_obj = led_obj
         self.exit_flag = Event()
         self.animations = animations or {}
         self.queue = Queue()
@@ -380,15 +433,15 @@
 def get_led(revision: SJ201) -> MycroftLed:
     """
     Get a MycroftLed object to handle LED controls
     :param revision: SJ201 Board Revision
     :returns: MycroftLed Object
     """
     if revision == SJ201.r10:
-        return R10Led()
+        return HwPwmAwareLed(R10Led()) if sj201_rev10_pwm_fan_overlay_present() else R10Led()
     elif revision == SJ201.r6:
         return R6Led()
     else:
         raise ValueError(f"Unsupported revision: {revision}")
 
 
 def chase(led: MycroftLed = None, color: Palette = Palette.WHITE):
```

## Comparing `sj201_interface-0.0.3a0.dist-info/LICENSE.md` & `sj201_interface-0.0.3a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `sj201_interface-0.0.3a0.dist-info/METADATA` & `sj201_interface-0.0.3a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sj201-interface
-Version: 0.0.3a0
+Version: 0.0.3a1
 Summary: SJ201 Interface
 Home-page: https://github.com/NeonGeckoCom/sj201-interface
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `sj201_interface-0.0.3a0.dist-info/RECORD` & `sj201_interface-0.0.3a1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 sj201_interface/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 sj201_interface/cli.py,sha256=oQDrPvU_bEx30z51qz9ZRms3ED2TCFD1awT1dnE4tAA,4084
 sj201_interface/fan.py,sha256=ClUODlKwf1MpDsS1-AzT6kDmGs4FqLrzl5sXbMzr43g,8436
-sj201_interface/revisions.py,sha256=_iZqplCNCkjqCMfDeSrBm8XETkC1mrGcK5PSOgMivhE,2877
+sj201_interface/revisions.py,sha256=p0_j9bX4Iv_wUrekP56_9YXf90xYqdvnuCBwJ5BHHMU,2732
 sj201_interface/switches.py,sha256=xGphg-YrPd_EyCvQC0Bnk-xQIgMvhykOKxHclOlCQys,7345
-sj201_interface/version.py,sha256=54SN1ajCWotBXuMR-HJRA6siWG7sun_xSmTiu9_hTcI,1856
-sj201_interface/led/__init__.py,sha256=KJtugkCKkDd9UMN7QsboitCwJcXMxG21DSTEnagu4Zk,13263
+sj201_interface/version.py,sha256=xn-MQ8IlYqiu461Y_cya_p21VPQHsy95wyyMpiTOS68,1856
+sj201_interface/led/__init__.py,sha256=O81N8ORtgwwBUIe4Xl-wnKfShAlMnfpwRnKy4smyc3c,15223
 sj201_interface/led/animations.py,sha256=l-Bk5QHZRCfYvUdphFr4gA-94SzIwlcla9OM-4mrJ2A,5129
 sj201_interface/util/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 sj201_interface/util/patches.py,sha256=O3gUv8PholWKj7Zz4hfa164DEBCAmTK1aUJbGGuyvNM,2770
+sj201_interface/util/pwmcontroller.py,sha256=kTuah0nYl0-of-_X2cP1K3IACOvM05kXz1ZX3Qxvvm0,4996
 sj201_interface/util/tas5806.py,sha256=g5ZZhItcShcnwnj6PgeV1srjTX9ubaYQ3KAPvVNNT-c,7038
-sj201_interface-0.0.3a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-sj201_interface-0.0.3a0.dist-info/METADATA,sha256=eNEZKEtgVU34cWJiOBHTUMlmXx65p2twXYnlTWYIgZ8,1912
-sj201_interface-0.0.3a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sj201_interface-0.0.3a0.dist-info/entry_points.txt,sha256=2ws0xV0adHjXLlcrsPe0780ewmDE39F4G1Qa4hshkG8,57
-sj201_interface-0.0.3a0.dist-info/top_level.txt,sha256=fZTrymfpnuk7mKDEja6zHXYD9EVz6qufxcfmKL4TZ6o,16
-sj201_interface-0.0.3a0.dist-info/RECORD,,
+sj201_interface-0.0.3a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+sj201_interface-0.0.3a1.dist-info/METADATA,sha256=b854lxYHaZQqe5nOALLLKQssbSSh072I-yhNC8rVLIY,1912
+sj201_interface-0.0.3a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sj201_interface-0.0.3a1.dist-info/entry_points.txt,sha256=2ws0xV0adHjXLlcrsPe0780ewmDE39F4G1Qa4hshkG8,57
+sj201_interface-0.0.3a1.dist-info/top_level.txt,sha256=fZTrymfpnuk7mKDEja6zHXYD9EVz6qufxcfmKL4TZ6o,16
+sj201_interface-0.0.3a1.dist-info/RECORD,,
```

