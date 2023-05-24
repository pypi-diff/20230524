# Comparing `tmp/idpmodem-2.3.5.tar.gz` & `tmp/idpmodem-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idpmodem-2.3.5.tar", max compression
+gzip compressed data, was "idpmodem-2.3.6.tar", max compression
```

## Comparing `idpmodem-2.3.5.tar` & `idpmodem-2.3.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0    10763 2021-09-26 16:07:24.162483 idpmodem-2.3.5/LICENSE
--rw-r--r--   0        0        0      304 2023-03-26 17:53:16.586339 idpmodem-2.3.5/idpmodem/__init__.py
--rw-r--r--   0        0        0       40 2022-07-15 21:11:00.743064 idpmodem-2.3.5/idpmodem/asyncio/__init__.py
--rw-r--r--   0        0        0     8102 2022-04-19 10:57:07.964213 idpmodem-2.3.5/idpmodem/asyncio/atcommand.py
--rw-r--r--   0        0        0    48406 2022-04-19 10:56:23.766312 idpmodem-2.3.5/idpmodem/asyncio/atcommand_async.py
--rw-r--r--   0        0        0    38915 2023-03-26 17:30:16.859025 idpmodem-2.3.5/idpmodem/asyncio/modem.py
--rw-r--r--   0        0        0      616 2022-04-18 16:50:03.044139 idpmodem-2.3.5/idpmodem/aterror.py
--rw-r--r--   0        0        0       69 2022-06-21 22:04:05.752050 idpmodem-2.3.5/idpmodem/codecs/__init__.py
--rw-r--r--   0        0        0      217 2022-12-22 22:48:50.621272 idpmodem-2.3.5/idpmodem/codecs/common_mdf.py
--rw-r--r--   0        0        0      545 2022-12-22 22:41:12.204297 idpmodem-2.3.5/idpmodem/codecs/common_message_format/__init__.py
--rw-r--r--   0        0        0     3401 2022-12-22 22:35:49.340483 idpmodem-2.3.5/idpmodem/codecs/common_message_format/base.py
--rw-r--r--   0        0        0      616 2022-12-22 20:53:20.689493 idpmodem-2.3.5/idpmodem/codecs/common_message_format/constants.py
--rw-r--r--   0        0        0      242 2022-12-22 21:17:44.284480 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/__init__.py
--rw-r--r--   0        0        0     9064 2022-12-22 21:52:45.125084 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/array_field.py
--rw-r--r--   0        0        0     3556 2022-12-23 13:40:54.325794 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/base_field.py
--rw-r--r--   0        0        0     2597 2022-12-23 13:42:03.479625 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/boolean_field.py
--rw-r--r--   0        0        0     7592 2022-12-23 13:52:28.617274 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/data_field.py
--rw-r--r--   0        0        0     5744 2022-12-23 22:11:37.048422 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/enum_field.py
--rw-r--r--   0        0        0     1120 2022-12-22 20:09:24.081950 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/helpers.py
--rw-r--r--   0        0        0     9018 2022-12-23 15:07:32.713822 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/integer_field.py
--rw-r--r--   0        0        0     4915 2022-12-23 13:52:13.860341 idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/string_field.py
--rw-r--r--   0        0        0     3198 2022-12-22 21:58:21.526690 idpmodem-2.3.5/idpmodem/codecs/common_message_format/message_definitions.py
--rw-r--r--   0        0        0     7102 2022-12-22 22:17:34.077694 idpmodem-2.3.5/idpmodem/codecs/common_message_format/messages.py
--rw-r--r--   0        0        0     4858 2022-12-22 21:59:38.807257 idpmodem-2.3.5/idpmodem/codecs/common_message_format/services.py
--rw-r--r--   0        0        0    13754 2023-03-26 17:30:20.143711 idpmodem-2.3.5/idpmodem/constants.py
--rw-r--r--   0        0        0     3194 2022-06-22 21:25:43.836758 idpmodem-2.3.5/idpmodem/crcxmodem.py
--rw-r--r--   0        0        0     2576 2022-06-22 21:23:44.104600 idpmodem-2.3.5/idpmodem/helpers.py
--rw-r--r--   0        0        0    13509 2022-04-21 01:33:30.905231 idpmodem-2.3.5/idpmodem/location.py
--rw-r--r--   0        0        0     3424 2023-03-26 12:18:23.203745 idpmodem-2.3.5/idpmodem/propertycache.py
--rw-r--r--   0        0        0     7628 2022-04-19 10:47:54.958690 idpmodem-2.3.5/idpmodem/s_registers.py
--rw-r--r--   0        0        0       57 2022-06-21 22:05:00.325962 idpmodem-2.3.5/idpmodem/threaded/__init__.py
--rw-r--r--   0        0        0    15120 2023-03-26 03:53:24.878893 idpmodem-2.3.5/idpmodem/threaded/atcommand.py
--rw-r--r--   0        0        0    61161 2023-03-26 17:49:44.478931 idpmodem-2.3.5/idpmodem/threaded/modem.py
--rw-r--r--   0        0        0      777 2023-03-26 17:51:46.528656 idpmodem-2.3.5/pyproject.toml
--rw-r--r--   0        0        0      902 2023-03-26 17:54:03.586938 idpmodem-2.3.5/setup.py
--rw-r--r--   0        0        0      644 2023-03-26 17:54:03.587138 idpmodem-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0    10763 2021-09-26 16:07:24.162483 idpmodem-2.3.6/LICENSE
+-rw-r--r--   0        0        0     2017 2022-06-21 22:15:20.012649 idpmodem-2.3.6/README.md
+-rw-r--r--   0        0        0      304 2023-03-26 17:53:16.586339 idpmodem-2.3.6/idpmodem/__init__.py
+-rw-r--r--   0        0        0       40 2022-07-15 21:11:00.743064 idpmodem-2.3.6/idpmodem/asyncio/__init__.py
+-rw-r--r--   0        0        0     8102 2022-04-19 10:57:07.964213 idpmodem-2.3.6/idpmodem/asyncio/atcommand.py
+-rw-r--r--   0        0        0    48406 2022-04-19 10:56:23.766312 idpmodem-2.3.6/idpmodem/asyncio/atcommand_async.py
+-rw-r--r--   0        0        0    38915 2023-03-26 17:30:16.859025 idpmodem-2.3.6/idpmodem/asyncio/modem.py
+-rw-r--r--   0        0        0      616 2022-04-18 16:50:03.044139 idpmodem-2.3.6/idpmodem/aterror.py
+-rw-r--r--   0        0        0       69 2022-06-21 22:04:05.752050 idpmodem-2.3.6/idpmodem/codecs/__init__.py
+-rw-r--r--   0        0        0      217 2022-12-22 22:48:50.621272 idpmodem-2.3.6/idpmodem/codecs/common_mdf.py
+-rw-r--r--   0        0        0      545 2022-12-22 22:41:12.204297 idpmodem-2.3.6/idpmodem/codecs/common_message_format/__init__.py
+-rw-r--r--   0        0        0     3401 2022-12-22 22:35:49.340483 idpmodem-2.3.6/idpmodem/codecs/common_message_format/base.py
+-rw-r--r--   0        0        0      616 2022-12-22 20:53:20.689493 idpmodem-2.3.6/idpmodem/codecs/common_message_format/constants.py
+-rw-r--r--   0        0        0      242 2022-12-22 21:17:44.284480 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/__init__.py
+-rw-r--r--   0        0        0     9064 2022-12-22 21:52:45.125084 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/array_field.py
+-rw-r--r--   0        0        0     3556 2022-12-23 13:40:54.325794 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/base_field.py
+-rw-r--r--   0        0        0     2597 2022-12-23 13:42:03.479625 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/boolean_field.py
+-rw-r--r--   0        0        0     7592 2022-12-23 13:52:28.617274 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/data_field.py
+-rw-r--r--   0        0        0     5744 2022-12-23 22:11:37.048422 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/enum_field.py
+-rw-r--r--   0        0        0     1120 2022-12-22 20:09:24.081950 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/helpers.py
+-rw-r--r--   0        0        0     9018 2022-12-23 15:07:32.713822 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/integer_field.py
+-rw-r--r--   0        0        0     4915 2022-12-23 13:52:13.860341 idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/string_field.py
+-rw-r--r--   0        0        0     3198 2022-12-22 21:58:21.526690 idpmodem-2.3.6/idpmodem/codecs/common_message_format/message_definitions.py
+-rw-r--r--   0        0        0     7102 2022-12-22 22:17:34.077694 idpmodem-2.3.6/idpmodem/codecs/common_message_format/messages.py
+-rw-r--r--   0        0        0     4858 2022-12-22 21:59:38.807257 idpmodem-2.3.6/idpmodem/codecs/common_message_format/services.py
+-rw-r--r--   0        0        0    13754 2023-03-26 17:30:20.143711 idpmodem-2.3.6/idpmodem/constants.py
+-rw-r--r--   0        0        0     3194 2022-06-22 21:25:43.836758 idpmodem-2.3.6/idpmodem/crcxmodem.py
+-rw-r--r--   0        0        0     2576 2022-06-22 21:23:44.104600 idpmodem-2.3.6/idpmodem/helpers.py
+-rw-r--r--   0        0        0    13509 2022-04-21 01:33:30.905231 idpmodem-2.3.6/idpmodem/location.py
+-rw-r--r--   0        0        0     3527 2023-03-27 15:00:37.391287 idpmodem-2.3.6/idpmodem/propertycache.py
+-rw-r--r--   0        0        0     7628 2022-04-19 10:47:54.958690 idpmodem-2.3.6/idpmodem/s_registers.py
+-rw-r--r--   0        0        0       57 2022-06-21 22:05:00.325962 idpmodem-2.3.6/idpmodem/threaded/__init__.py
+-rw-r--r--   0        0        0    15120 2023-03-26 03:53:24.878893 idpmodem-2.3.6/idpmodem/threaded/atcommand.py
+-rw-r--r--   0        0        0    61332 2023-03-27 15:05:14.232939 idpmodem-2.3.6/idpmodem/threaded/modem.py
+-rw-r--r--   0        0        0      897 2023-03-27 15:07:32.108111 idpmodem-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3011 2023-03-27 15:07:42.237189 idpmodem-2.3.6/setup.py
+-rw-r--r--   0        0        0     2867 2023-03-27 15:07:42.237493 idpmodem-2.3.6/PKG-INFO
```

### Comparing `idpmodem-2.3.5/LICENSE` & `idpmodem-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/asyncio/atcommand.py` & `idpmodem-2.3.6/idpmodem/asyncio/atcommand.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/asyncio/atcommand_async.py` & `idpmodem-2.3.6/idpmodem/asyncio/atcommand_async.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/asyncio/modem.py` & `idpmodem-2.3.6/idpmodem/asyncio/modem.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/aterror.py` & `idpmodem-2.3.6/idpmodem/aterror.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/__init__.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/__init__.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/base.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/base.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/constants.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/constants.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/array_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/array_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/base_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/boolean_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/boolean_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/data_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/data_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/enum_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/enum_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/helpers.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/helpers.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/integer_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/integer_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/fields/string_field.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/fields/string_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/message_definitions.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/message_definitions.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/messages.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/messages.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/codecs/common_message_format/services.py` & `idpmodem-2.3.6/idpmodem/codecs/common_message_format/services.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/constants.py` & `idpmodem-2.3.6/idpmodem/constants.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/crcxmodem.py` & `idpmodem-2.3.6/idpmodem/crcxmodem.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/helpers.py` & `idpmodem-2.3.6/idpmodem/helpers.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/location.py` & `idpmodem-2.3.6/idpmodem/location.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/propertycache.py` & `idpmodem-2.3.6/idpmodem/propertycache.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,17 +76,20 @@
         Args:
             tag: The property name to be removed from the cache.
         
         Raises:
             `KeyError` if the tag is not in the cache.
             
         """
-        cached = self._cache.pop(tag)
+        cached = self._cache.pop(tag, None)
         if self._vlog():
-            _log.debug(f'Removed {tag} aged {cached.age} seconds')
+            if cached:
+                _log.debug(f'Removed {tag} aged {cached.age} seconds')
+            else:
+                _log.debug(f'{tag} was not cached')
     
     def get_cached(self, tag: str) -> Any:
         """Retrieves the cached property value if valid.
         
         If the property is aged/invalid, it is removed from the cache.
         
         Args:
```

### Comparing `idpmodem-2.3.5/idpmodem/s_registers.py` & `idpmodem-2.3.6/idpmodem/s_registers.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/threaded/atcommand.py` & `idpmodem-2.3.6/idpmodem/threaded/atcommand.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.5/idpmodem/threaded/modem.py` & `idpmodem-2.3.6/idpmodem/threaded/modem.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,16 +529,16 @@
     
     @power_mode.setter
     def power_mode(self, value: 'str|int|PowerMode'):
         CACHE_TAG = 'power_mode'
         try:
             self.power_mode_set(value)
             self._property_cache.remove(CACHE_TAG)
-        except:
-            _log.error(f'Failed to set power_mode {value}')
+        except Exception as err:
+            _log.error(f'Failed to set power_mode {value}: {err}')
     
     def wakeup_period_get(self) -> 'WakeupPeriod|None':
         """The modem wakeup period setting (enumerated) in `S51`."""
         response = self.atcommand('ATS51?')
         if response[0] != 'ERROR':
             return WakeupPeriod(int(response[0]))
         self._handle_at_error(response)
@@ -575,16 +575,16 @@
 
     @wakeup_period.setter
     def wakeup_period(self, value: 'str|int|WakeupPeriod'):
         CACHE_TAG = 'wakeup_period'
         try:
             self.wakeup_period_set(value)
             self._property_cache.remove(CACHE_TAG)
-        except:
-            _log.error(f'Failed to set wakeup_period {value}')
+        except Exception as err:
+            _log.error(f'Failed to set wakeup_period {value}: {err}')
     
     def temperature_get(self) -> int:
         response = self.atcommand('ATS85?')
         if response[0] != 'ERROR':
             return int(float(response[0]) / 10)
         self._handle_at_error(response)
     
@@ -628,16 +628,16 @@
 
     @gnss_refresh_interval.setter
     def gnss_refresh_interval(self, value: int):
         CACHE_TAG = 'gnss_refresh_interval'
         try:
             self.gnss_refresh_interval_set(value)
             self._property_cache.remove(CACHE_TAG)
-        except:
-            _log.error(f'Failed to set gnss_refresh_interval {value}')
+        except Exception as err:
+            _log.error(f'Failed to set gnss_refresh_interval {value}: {err}')
 
     def gnss_continuous_set(self,
                             interval: int = 0,
                             doppler: bool = True,
                             ) -> bool:
         """Sets the GNSS continous mode (0 = on-demand).
         
@@ -792,16 +792,16 @@
 
     @gnss_mode.setter
     def gnss_mode(self, mode: 'GnssMode|int'):
         CACHE_TAG = 'gnss_mode'
         try:
             self.gnss_mode_set(mode)
             self._property_cache.remove(CACHE_TAG)
-        except:
-            _log.error(f'Failed to set gnss_mode {mode}')
+        except Exception as err:
+            _log.error(f'Failed to set gnss_mode {mode}: {err}')
 
     def transmitter_status_get(self) -> TransmitterStatus:
         """The transmitter status reported by `S54`"""
         response = self.atcommand('ATS54?')
         if response[0] != 'ERROR':
             return TransmitterStatus(int(response[0]))
         self._handle_at_error(response)
@@ -1298,16 +1298,16 @@
         
     @trace_event_monitor.setter
     def trace_event_monitor(self, events: 'list[tuple[int, int]]'):
         CACHE_TAG = 'trace_event_monitor'
         try:
             self.trace_event_monitor_set(events)
             self._property_cache.remove(CACHE_TAG)
-        except:
-            _log.error(f'Failed to set trace_event_monitor {events}')
+        except Exception as err:
+            _log.error(f'Failed to set trace_event_monitor {events}: {err}')
 
     @property
     def trace_events_cached(self) -> 'list[tuple[int, int]]':
         """The list of trace events cached for retrieval.
         
         Cached for 1 second.
         """
@@ -1456,16 +1456,17 @@
     
     @event_notification_monitor.setter
     def event_notification_monitor(self, event_list: 'list[EventNotification]'):
         CACHE_TAG = 'event_notification_monitor'
         try:
             self.event_notification_monitor_set(event_list)
             self._property_cache.remove(CACHE_TAG)
-        except:
-            _log.error(f'Failed to set event_notification_monitor {event_list}')
+        except Exception as err:
+            _log.error(f'Failed to set event_notification_monitor {event_list}'
+                       f': {err}')
 
     def event_notifications_get(self) -> 'list[EventNotification]':
         """The list of active events reported in `S89`."""
         response = self.atcommand('ATS89?')
         if response[0] != 'ERROR':
             return self._list_events(int(response[0]))
         self._handle_at_error(response)
```

### Comparing `idpmodem-2.3.5/pyproject.toml` & `idpmodem-2.3.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "idpmodem"
-version = "2.3.5"
+version = "2.3.6"
 description = "A library for interfacing with an Inmarsat IsatData Pro satellite IoT modem using serial AT commands."
 authors = ["geoffbrucepayne <geoff.bruce-payne@inmarsat.com>"]
 license = "Apache2.0"
+repository = "https://github.com/inmarsat-enterprise.com/idpmodem"
+readme = "README.md"
+keywords = ["satellite", "iot"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
 aioserial = "1.3.0"
 pyserial-asyncio = "^0.6"
```

