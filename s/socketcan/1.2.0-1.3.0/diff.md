# Comparing `tmp/socketcan-1.2.0.tar.gz` & `tmp/socketcan-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketcan-1.2.0.tar", last modified: Mon Nov 21 19:18:21 2022, max compression
+gzip compressed data, was "socketcan-1.3.0.tar", last modified: Wed May 24 16:44:08 2023, max compression
```

## Comparing `socketcan-1.2.0.tar` & `socketcan-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-21 19:18:21.478238 socketcan-1.2.0/
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    35147 2018-06-01 10:17:25.000000 socketcan-1.2.0/LICENSE
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     7178 2022-11-21 19:18:21.478238 socketcan-1.2.0/PKG-INFO
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     6422 2022-05-16 16:50:02.000000 socketcan-1.2.0/README.md
--rw-rw-r--   0 zeero     (1000) zeero     (1000)      902 2022-11-21 19:17:03.000000 socketcan-1.2.0/pyproject.toml
--rw-rw-r--   0 zeero     (1000) zeero     (1000)       38 2022-11-21 19:18:21.478238 socketcan-1.2.0/setup.cfg
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-21 19:18:21.474238 socketcan-1.2.0/socketcan/
--rw-r--r--   0 zeero     (1000) zeero     (1000)      182 2021-10-14 14:14:40.000000 socketcan-1.2.0/socketcan/__init__.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    38747 2022-11-21 19:11:47.000000 socketcan-1.2.0/socketcan/socketcan.py
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-21 19:18:21.478238 socketcan-1.2.0/socketcan.egg-info/
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     7178 2022-11-21 19:18:21.000000 socketcan-1.2.0/socketcan.egg-info/PKG-INFO
--rw-rw-r--   0 zeero     (1000) zeero     (1000)      298 2022-11-21 19:18:21.000000 socketcan-1.2.0/socketcan.egg-info/SOURCES.txt
--rw-rw-r--   0 zeero     (1000) zeero     (1000)        1 2022-11-21 19:18:21.000000 socketcan-1.2.0/socketcan.egg-info/dependency_links.txt
--rw-rw-r--   0 zeero     (1000) zeero     (1000)       10 2022-11-21 19:18:21.000000 socketcan-1.2.0/socketcan.egg-info/requires.txt
--rw-rw-r--   0 zeero     (1000) zeero     (1000)       10 2022-11-21 19:18:21.000000 socketcan-1.2.0/socketcan.egg-info/top_level.txt
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-21 19:18:21.478238 socketcan-1.2.0/tests/
--rw-r--r--   0 zeero     (1000) zeero     (1000)        0 2021-02-05 18:25:38.000000 socketcan-1.2.0/tests/__init__.py
--rw-r--r--   0 zeero     (1000) zeero     (1000)      176 2021-02-26 19:42:59.000000 socketcan-1.2.0/tests/mocks.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    45263 2022-11-12 19:43:39.000000 socketcan-1.2.0/tests/test_socketcan.py
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-05-24 16:44:08.370061 socketcan-1.3.0/
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    35147 2018-06-01 10:17:25.000000 socketcan-1.3.0/LICENSE
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     7178 2023-05-24 16:44:08.370061 socketcan-1.3.0/PKG-INFO
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     6422 2022-05-16 16:50:02.000000 socketcan-1.3.0/README.md
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)      902 2023-05-24 16:41:14.000000 socketcan-1.3.0/pyproject.toml
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)       38 2023-05-24 16:44:08.370061 socketcan-1.3.0/setup.cfg
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-05-24 16:44:08.366061 socketcan-1.3.0/socketcan/
+-rw-r--r--   0 zeero     (1000) zeero     (1000)      182 2021-10-14 14:14:40.000000 socketcan-1.3.0/socketcan/__init__.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    38943 2023-05-24 16:37:39.000000 socketcan-1.3.0/socketcan/socketcan.py
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-05-24 16:44:08.366061 socketcan-1.3.0/socketcan.egg-info/
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     7178 2023-05-24 16:44:08.000000 socketcan-1.3.0/socketcan.egg-info/PKG-INFO
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)      298 2023-05-24 16:44:08.000000 socketcan-1.3.0/socketcan.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)        1 2023-05-24 16:44:08.000000 socketcan-1.3.0/socketcan.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)       10 2023-05-24 16:44:08.000000 socketcan-1.3.0/socketcan.egg-info/requires.txt
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)       10 2023-05-24 16:44:08.000000 socketcan-1.3.0/socketcan.egg-info/top_level.txt
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-05-24 16:44:08.366061 socketcan-1.3.0/tests/
+-rw-r--r--   0 zeero     (1000) zeero     (1000)        0 2021-02-05 18:25:38.000000 socketcan-1.3.0/tests/__init__.py
+-rw-r--r--   0 zeero     (1000) zeero     (1000)      176 2021-02-26 19:42:59.000000 socketcan-1.3.0/tests/mocks.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    39898 2023-05-24 16:38:41.000000 socketcan-1.3.0/tests/test_socketcan.py
```

### Comparing `socketcan-1.2.0/LICENSE` & `socketcan-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketcan-1.2.0/PKG-INFO` & `socketcan-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketcan
-Version: 1.2.0
+Version: 1.3.0
 Summary: A python 3 interface to socketcan
 Author-email: Patrick Menschel <menschel.p@posteo.de>
 Project-URL: Homepage, https://gitlab.com/menschel/socketcan
 Project-URL: Bug Tracker, https://gitlab.com/menschel/socketcan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `socketcan-1.2.0/README.md` & `socketcan-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `socketcan-1.2.0/pyproject.toml` & `socketcan-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketcan"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="Patrick Menschel", email="menschel.p@posteo.de" },
 ]
 description = "A python 3 interface to socketcan"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `socketcan-1.2.0/socketcan/socketcan.py` & `socketcan-1.3.0/socketcan/socketcan.py`

 * *Files 6% similar despite different names*

```diff
@@ -736,26 +736,30 @@
                  listen_only: bool = False,
                  use_padding: bool = False,
                  wait_tx_done: bool = False,
                  fc_bs: int = 0,
                  fc_stmin: int = 0,
                  use_canfd: bool = False,
                  enable_broadcast: bool = False,
+                 txpadding: int = 0xAA,
+                 rxpadding: int = 0xAA,
                  ):
         """
         :param interface: The interface name.
         :param rx_addr: The can_id for receive messages.
         :param tx_addr: The can_id for transmit messages.
         :param listen_only: Enable listen only socket option
         :param use_padding: Enable padding socket option.
         :param wait_tx_done: Enable blocking write socket option.
         :param fc_bs: Flow control block size value, i.e. number of consecutive frames to be sent.
         :param fc_stmin: Flow control frame separation time.
         :param use_canfd: Enable CAN FD usage instead of CAN 2.0
         :param enable_broadcast: A flag to enable CAN_ISOTP_SF_BROADCAST and CAN_ISOTP_CF_BROADCAST
+        :param txpadding: The fill byte as integer for padding tx messages.
+        :param rxpadding: The fill byte as integer for padding rx messages.
         """
 
         if tx_addr > 0x7FF:
             tx_addr = combine_can_id_and_flags(tx_addr, CanFlags.CAN_EFF_FLAG)
 
         if rx_addr > 0x7FF:
             rx_addr = combine_can_id_and_flags(rx_addr, CanFlags.CAN_EFF_FLAG)
@@ -768,15 +772,18 @@
         if use_padding:
             # To be added to options later.
             flags |= CAN_ISOTP_TX_PADDING | CAN_ISOTP_RX_PADDING
         if wait_tx_done:
             flags |= CAN_ISOTP_WAIT_TX_DONE
         if enable_broadcast:
             flags |= CAN_ISOTP_SF_BROADCAST | CAN_ISOTP_CF_BROADCAST
-        opts = IsoTpOpts(flags=flags)
+        opts = IsoTpOpts(flags=flags,
+                         txpadding=txpadding,
+                         rxpadding=rxpadding,
+                         )
         self._s.setsockopt(SOL_CAN_ISOTP, CAN_ISOTP_OPTS, opts.to_bytes())
 
         fc_opts = IsoTpFcOpts(bs=fc_bs,
                               stmin=fc_stmin)
         self._s.setsockopt(SOL_CAN_ISOTP, CAN_ISOTP_RECV_FC, fc_opts.to_bytes())
 
         if use_canfd:
@@ -813,72 +820,71 @@
 
 
 class IsoTpOpts:
     """
     A representation of isotp options
     """
 
-    FORMAT = "IIBccB"
+    FORMAT = "IIBBBB"
 
     def __init__(self,
                  flags=0,
                  frame_txtime=0,
                  ext_address=0,
-                 txpad_content=bytes(1),
-                 rxpad_content=bytes(1),
+                 txpadding: int = 0xAA,
+                 rxpadding: int = 0xAA,
                  rx_ext_address=0
                  ):
         """
         Constuctor
 
         :param flags: The flags in isotp options.
         :param frame_txtime: The time in between tx frames.
         :param ext_address: The external address if given.
-        :param txpad_content: The fill byte for padding tx messages.
-        :param rxpad_content: The fill byte for padding rx messages.
+        :param txpadding: The fill byte as integer for padding tx messages.
+        :param rxpadding: The fill byte as integer for padding rx messages.
         :param rx_ext_address: The external address for rx if given.
         """
         self.flags = flags
         self.frame_txtime = frame_txtime
         self.ext_address = ext_address
-        self.txpad_content = txpad_content
-        self.rxpad_content = rxpad_content
+        self.txpadding = txpadding
+        self.rxpadding = rxpadding
         self.rx_ext_address = rx_ext_address
 
     def to_bytes(self) -> bytes:
         """
         Convert to bytes representation.
 
         :return: The bytes representation of the object.
         """
         opts = struct.pack(self.FORMAT,
                            self.flags,
                            self.frame_txtime,
                            self.ext_address,
-                           self.txpad_content,
-                           self.rxpad_content,
+                           self.txpadding,
+                           self.rxpadding,
                            self.rx_ext_address)
         return opts
 
     @classmethod
     def from_bytes(cls, byte_repr: bytes):
         """
         Factory to create instance from bytes representation.
 
         :param byte_repr: The bytes representation of the object.
         :return: An instance of this class.
         """
         assert len(byte_repr) == cls.get_size()
-        flags, frame_txtime, ext_address, txpad_content, rxpad_content, rx_ext_address = struct.unpack(cls.FORMAT,
-                                                                                                       byte_repr)
+        flags, frame_txtime, ext_address, txpadding, rxpadding, rx_ext_address = struct.unpack(cls.FORMAT, byte_repr)
         return IsoTpOpts(flags=flags,
                          frame_txtime=frame_txtime,
                          ext_address=ext_address,
-                         txpad_content=txpad_content,
-                         rxpad_content=rxpad_content,
+                         txpadding=txpadding,
+                         rxpadding=rxpadding,
                          rx_ext_address=rx_ext_address)
 
     @classmethod
     def get_size(cls):
         """
         Get the calculated byte size of this class.
 
@@ -894,16 +900,16 @@
         :return: True if equal, False otherwise.
         """
         is_equal = False
         if isinstance(other, IsoTpOpts):
             is_equal = all((self.flags == other.flags,
                             self.frame_txtime == other.frame_txtime,
                             self.ext_address == other.ext_address,
-                            self.txpad_content == other.txpad_content,
-                            self.rxpad_content == other.rxpad_content,
+                            self.txpadding == other.txpadding,
+                            self.rxpadding == other.rxpadding,
                             self.rx_ext_address == other.rx_ext_address,
                             ))
         return is_equal
 
     def __ne__(self, other) -> bool:
         """
         Standard non equality operation
```

### Comparing `socketcan-1.2.0/socketcan.egg-info/PKG-INFO` & `socketcan-1.3.0/socketcan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketcan
-Version: 1.2.0
+Version: 1.3.0
 Summary: A python 3 interface to socketcan
 Author-email: Patrick Menschel <menschel.p@posteo.de>
 Project-URL: Homepage, https://gitlab.com/menschel/socketcan
 Project-URL: Bug Tracker, https://gitlab.com/menschel/socketcan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `socketcan-1.2.0/tests/test_socketcan.py` & `socketcan-1.3.0/tests/test_socketcan.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,76 +207,14 @@
     :param q: The queue where to put the received data into.
     :return: None.
     """
     s = CanJ1939Socket(interface=interface)
     q.put(s.recvfrom())
 
 
-# def generate_random_can_frame() -> CanFrame:
-#     can_id = randint(1, 0x1FFFFFFF)
-#     data_len = randint(0, 8)
-#     data = randbytes(data_len)
-#     frame = CanFrame(can_id=can_id, data=data)
-#     return frame
-#
-#
-# class RandomFrameGenerator:
-#     """
-#     An object that generates CanFrames
-#     sends these can frames on a given CAN interface
-#     and puts them into a queue, so the parent application
-#     can check every frame is received via interface.
-#     Note: This is actually an enhanced version of cangen command.
-#     """
-#
-#     def __init__(self,
-#                  interface: str,
-#                  q: Optional[Queue] = None,
-#                  wait_time: Optional[float] = None,
-#                  number_of_frames: Optional[int] = None,
-#                  ):
-#         """
-#         Constructor
-#         :param interface: The CAN interface.
-#         :param q: The queue to put the sent frames.
-#         """
-#         self.interface = interface
-#         self.q = q
-#         self.wait_time = wait_time
-#         self.timeout = 1
-#         self.number_of_frames = number_of_frames
-#         self.s = CanRawSocket(interface=interface)
-#         self.worker = Thread(target=self.generate_frames)
-#         self.worker.setDaemon(True)
-#         self.worker.start()
-#
-#     def generate_frames(self) -> None:
-#         """
-#         Worker thread to generate frames.
-#         :return: None.
-#         """
-#         len_of_can_frame = CanFrame.get_size()
-#         while self.number_of_frames is None \
-#                 or self.number_of_frames > 0:
-#             try:
-#                 ready_to_send = select.select([], [self.s, ], [], self.timeout)[1]
-#             except select.error:
-#                 pass
-#             else:
-#                 if ready_to_send:
-#                     frame = generate_random_can_frame()
-#                     if ready_to_send[0].send(frame) == len_of_can_frame:
-#                         if self.q is not None:
-#                             self.q.put(frame)
-#                         if self.wait_time is not None:
-#                             time.sleep(self.wait_time)
-#                         if self.number_of_frames is not None:
-#                             self.number_of_frames = self.number_of_frames - 1
-
-
 class TestObjectCreation:
     """
     A collection of tests for concat / parse objects.
     """
 
     def test_unequal_frames(self):
         can_id1 = 0x123
@@ -605,30 +543,30 @@
         assert len(bcm_as_bytes) == BcmMsg.get_size() + (CanFdFrame.get_size() * len(frames))
 
 
     def test_isotp_opts(self):
         opts = IsoTpOpts(flags=CAN_ISOTP_TX_PADDING | CAN_ISOTP_RX_PADDING,
                          frame_txtime=100,
                          ext_address=0xF1,
-                         txpad_content=b"\xAA",
-                         rxpad_content=b"\xCC",
+                         txpadding=0xAA,
+                         rxpadding=0xAA,
                          rx_ext_address=0xFA
                          )
         data = opts.to_bytes()
         opts2 = IsoTpOpts.from_bytes(data)
         assert opts == opts2
         assert not opts != opts2
 
     @pytest.mark.xfail
     def test_isotp_opts_should_fail(self):
         opts = IsoTpOpts(flags=CAN_ISOTP_TX_PADDING | CAN_ISOTP_RX_PADDING,
                          frame_txtime=100,
                          ext_address=0xF1,
-                         txpad_content=b"\xAA",
-                         rxpad_content=b"\xCC",
+                         txpadding=0xAA,
+                         rxpadding=0xAA,
                          rx_ext_address=0xFA
                          )
         data = opts.to_bytes()
         opts.ext_address = 0
         opts2 = IsoTpOpts.from_bytes(data)
         assert opts == opts2
 
@@ -1228,73 +1166,7 @@
         time.sleep(1)
         s.sendto(pgn=pgn, data=data, addr=dest)
         j1939_dict = q.get(timeout=10)
         p.join()
         LOGGER.info("{0}".format(j1939_dict))
         assert j1939_dict.get("data") == data
         assert j1939_dict.get("pgn") == pgn
-
-# @pytest.mark.long
-# @pytest.mark.skipif(not is_can_available(), reason="this test requires a can interface to be set up")
-# class TestPerformance:
-#
-#     @pytest.mark.skipif(not vcan0_available(),
-#                         reason="this test requires vcan0")
-#     def test_data_rate_via_can_raw_socket(self):
-#         interface = "vcan0"
-#         framecount = 0
-#         duration = datetime.timedelta(minutes=2)
-#         timeout = datetime.datetime.now() + duration
-#         q = Queue()
-#         s = CanRawSocket(interface=interface)
-#         framegen = RandomFrameGenerator(interface=interface,
-#                                         q=q,
-#                                         # wait_time=0.001,
-#                                         )
-#         while current_time := datetime.datetime.now() < timeout:
-#             next_frame = s.recv()
-#             queued_frame = q.get()
-#             assert next_frame == queued_frame
-#             framecount = framecount + 1
-#
-#         LOGGER.info("{0} frames in {1}".format(framecount, duration))
-#
-#     @pytest.mark.skipif(not mcp0_and_mcp1_available(),
-#                         reason="this test requires two connected interfaces, mcp0 and mcp1")
-#     @pytest.mark.timeout(3610)
-#     def test_data_rate_via_can_raw_socket_on_real_interface(self):
-#         interface = "mcp0"
-#         interface2 = "mcp1"
-#         framecount = 0
-#         dropped_frames_on_interface = 0
-#         duration = datetime.timedelta(minutes=60)
-#         timeout = datetime.datetime.now() + duration
-#         q = Queue()
-#         s = CanRawSocket(interface=interface)
-#         framegen = RandomFrameGenerator(interface=interface2,
-#                                         q=q,
-#                                         # wait_time=0.001,
-#                                         )
-#         while current_time := datetime.datetime.now() < timeout:
-#             next_frame = s.recv()  # blocking until a frame arrives
-#             try:
-#                 queued_frame = q.get(timeout=0.001)
-#             except Empty:
-#                 continue
-#             else:
-#                 if next_frame != queued_frame:
-#                     cnt = 0
-#                     while next_frame != queued_frame:
-#                         try:
-#                             queued_frame = q.get(timeout=0.001)
-#                         except Empty:
-#                             break
-#                         else:
-#                             cnt = cnt + 1
-#                     dropped_frames_on_interface = dropped_frames_on_interface + cnt
-#                     LOGGER.error(
-#                         "Re-synced queue after {0} dropped frames (overall {1})".format(
-#                         cnt, dropped_frames_on_interface))
-#                 framecount = framecount + 1
-#
-#         LOGGER.info("{0} frames in {1} (dropped frames by interface {2})".format(framecount, duration,
-#                                                                                  dropped_frames_on_interface))
```

