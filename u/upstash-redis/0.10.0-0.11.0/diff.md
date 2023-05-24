# Comparing `tmp/upstash_redis-0.10.0.tar.gz` & `tmp/upstash_redis-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.10.0.tar", max compression
+gzip compressed data, was "upstash_redis-0.11.0.tar", max compression
```

## Comparing `upstash_redis-0.10.0.tar` & `upstash_redis-0.11.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      363 2023-05-19 12:33:50.766534 upstash_redis-0.10.0/README.md
--rw-r--r--   0        0        0      386 2023-05-23 14:01:20.445390 upstash_redis-0.10.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_redis-0.10.0/upstash_redis/__init__.py
--rw-r--r--   0        0        0    87450 2023-05-23 13:49:50.609076 upstash_redis-0.10.0/upstash_redis/client.py
--rw-r--r--   0        0        0      308 2023-05-16 14:24:46.481207 upstash_redis-0.10.0/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_redis-0.10.0/upstash_redis/exception.py
--rw-r--r--   0        0        0      764 2023-05-23 13:55:57.244800 upstash_redis-0.10.0/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     2599 2023-05-23 13:56:34.201650 upstash_redis-0.10.0/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      444 2023-05-23 10:52:27.301846 upstash_redis-0.10.0/upstash_redis/play.py
--rw-r--r--   0        0        0      322 2023-05-23 09:30:15.343429 upstash_redis-0.10.0/upstash_redis/play2.py
--rw-r--r--   0        0        0        0 2023-05-22 11:36:04.331779 upstash_redis-0.10.0/upstash_redis/py.typed
--rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_redis-0.10.0/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_redis-0.10.0/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      729 2023-05-19 12:15:03.869929 upstash_redis-0.10.0/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-05-19 11:45:14.791080 upstash_redis-0.10.0/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_redis-0.10.0/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_redis-0.10.0/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3339 2023-05-23 13:55:57.249048 upstash_redis-0.10.0/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     4133 2023-05-23 13:56:34.207474 upstash_redis-0.10.0/upstash_redis/utils/format.py
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 upstash_redis-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 07:39:12.527702 upstash_redis-0.11.0/LICENSE
+-rw-r--r--   0        0        0     7404 2023-05-24 11:08:54.242823 upstash_redis-0.11.0/README.md
+-rw-r--r--   0        0        0      386 2023-05-24 11:14:14.993582 upstash_redis-0.11.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 07:40:32.115270 upstash_redis-0.11.0/upstash_redis/__init__.py
+-rw-r--r--   0        0        0    83519 2023-05-24 08:45:35.611261 upstash_redis-0.11.0/upstash_redis/client.py
+-rw-r--r--   0        0        0      288 2023-05-24 08:45:35.613502 upstash_redis-0.11.0/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-05-24 07:40:32.115728 upstash_redis-0.11.0/upstash_redis/exception.py
+-rw-r--r--   0        0        0      764 2023-05-24 07:40:32.115822 upstash_redis-0.11.0/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     2599 2023-05-24 07:40:32.115903 upstash_redis-0.11.0/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      214 2023-05-24 09:14:08.037410 upstash_redis-0.11.0/upstash_redis/play.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:40:32.115926 upstash_redis-0.11.0/upstash_redis/py.typed
+-rw-r--r--   0        0        0      409 2023-05-24 07:40:32.116182 upstash_redis-0.11.0/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1119 2023-05-24 07:40:32.116295 upstash_redis-0.11.0/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      729 2023-05-24 07:40:32.116372 upstash_redis-0.11.0/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-05-24 07:40:32.116436 upstash_redis-0.11.0/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      107 2023-05-24 07:40:32.116534 upstash_redis-0.11.0/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-05-24 07:40:32.116604 upstash_redis-0.11.0/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3339 2023-05-24 07:40:32.116678 upstash_redis-0.11.0/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     4133 2023-05-24 07:40:32.116752 upstash_redis-0.11.0/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     7883 1970-01-01 00:00:00.000000 upstash_redis-0.11.0/PKG-INFO
```

### Comparing `upstash_redis-0.10.0/upstash_redis/client.py` & `upstash_redis-0.11.0/upstash_redis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from upstash_redis.schema.http import RESTResult, RESTEncoding
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.config import (
     REST_ENCODING,
     REST_RETRIES,
     REST_RETRY_INTERVAL,
     ALLOW_TELEMETRY,
-    ALLOW_DEPRECATED,
     FORMAT_RETURN
 )
 from upstash_redis.utils.format import (
     format_geo_positions_return,
     format_geo_members_return,
     format_hash_return,
     format_pubsub_numsub_return,
@@ -43,56 +42,52 @@
 class Redis:
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
-        rest_retry_interval: int = REST_RETRY_INTERVAL,
-        allow_deprecated: bool = ALLOW_DEPRECATED,
+        rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
         telemetry_data: TelemetryData | None = None
     ):
         self.url = url
         self.token = token
 
         self.allow_telemetry = allow_telemetry
 
-        self.allow_deprecated = allow_deprecated
         self.format_return = format_return
 
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
         self.telemetry_data = telemetry_data
 
     @classmethod
     def from_env(
         cls,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
-        allow_deprecated: bool = ALLOW_DEPRECATED,
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
         telemetry_data: TelemetryData | None = None
     ):
         """
         Load the credentials from environment.
         """
 
         return cls(
             environ["UPSTASH_REDIS_REST_URL"],
             environ["UPSTASH_REDIS_REST_TOKEN"],
             rest_encoding,
             rest_retries,
             rest_retry_interval,
-            allow_deprecated,
             format_return,
             allow_telemetry,
             telemetry_data
         )
 
     async def __aenter__(self) -> ClientSession:
         """
@@ -575,19 +570,14 @@
 
         :param store_as: replacement for "STORE"
         :param store_distance_as: replacement for "STORE_DIST"
 
         :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 6.2.0, this command is deprecated.
-It can be replaced by "geosearch" and "geosearchstore" with the "radius" argument.
-Source: https://redis.io/commands/georadius""")
-
         handle_georadius_write_exceptions(
             with_distance,
             with_hash,
             with_coordinates,
             count,
             count_any,
             store_as,
@@ -645,19 +635,14 @@
         See https://redis.io/commands/georadius_ro
 
         :param count_any: replacement for "ANY"
 
         :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 6.2.0, this command is deprecated.
-It can be replaced by "geosearch" with the "radius" argument.
-Source: https://redis.io/commands/georadius_ro""")
-
         if count_any and count is None:
             raise Exception("\"count_any\" can only be used together with \"count\".")
 
         command: list = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
 
         if with_distance:
             command.append("WITHDIST")
@@ -706,19 +691,14 @@
 
         :param store_as: replacement for "STORE"
         :param store_distance_as: replacement for "STORE_DIST"
 
         :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 6.2.0, this command is deprecated.
-It can be replaced by "geosearch" and "geosearchstore" with the "radius" and "member" arguments.
-Source: https://redis.io/commands/georadiusbymember""")
-
         handle_georadius_write_exceptions(
             with_distance,
             with_hash,
             with_coordinates,
             count,
             count_any,
             store_as,
@@ -775,19 +755,14 @@
         See https://redis.io/commands/georadiusbymember
 
         :param count_any: replacement for "ANY"
 
         :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 6.2.0, this command is deprecated.
-        It can be replaced by "geosearch" with the "radius" and "member" arguments.
-        Source: https://redis.io/commands/georadiusbymember""")
-
         if count_any and count is None:
             raise Exception("\"count_any\" can only be used together with \"count\".")
 
         command: list = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
 
         if with_distance:
             command.append("WITHDIST")
@@ -1057,19 +1032,14 @@
         return await self.run(command)
 
     async def hmset(self, key: str, fields_and_values: dict) -> str:
         """
         See https://redis.io/commands/hmset
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 4.0.0, this command is deprecated.
-It can be replaced by "hset".
-Source: https://redis.io/commands/hmset""")
-
         command: list = ["HMSET", key]
 
         for field, value in fields_and_values.items():
             command.extend([field, value])
 
         return await self.run(command)
 
@@ -1384,19 +1354,14 @@
         return await self.run(command)
 
     async def rpoplpush(self, source_key: str, destination_key: str) -> str | None:
         """
         See https://redis.io/commands/rpoplpush
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 6.2.0, this command is deprecated.
-It can be replaced by "lmove" with "source_position" set to "RIGHT" and the "destination_position" set to "LEFT".
-Source: https://redis.io/commands/rpoplpush""")
-
         command: list = ["RPOPLPUSH", source_key, destination_key]
 
         return await self.run(command)
 
     async def rpush(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/rpush
@@ -1520,15 +1485,15 @@
         command: list = ["FLUSHDB"]
 
         if mode:
             command.append(mode)
 
         return await self.run(command)
 
-    async def server_time(self) -> list[str] | dict[str, int]:
+    async def time(self) -> list[str] | dict[str, int]:
         """
         See https://redis.io/commands/time
 
         :return: A dict with the keys "seconds" and "microseconds" if self.format_return is True.
         """
 
         command: list = ["TIME"]
@@ -2096,20 +2061,14 @@
         offset: int | None = None,
         count: int | None = None
     ) -> list[str | None]:
         """
         See https://redis.io/commands/zrangebylex
         """
 
-        if not self.allow_deprecated:
-            raise Exception(
-                """From version 6.2.0, this command is deprecated.
-It can be replaced by "zrange" with "range_method" set to "BYLEX".
-Source: https://redis.io/commands/zrangebylex""")
-
         handle_zrangebylex_exceptions(min_score, max_score, offset, count)
 
         command: list = ["ZRANGEBYLEX", key, min_score, max_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
 
@@ -2132,20 +2091,14 @@
         See https://redis.io/commands/zrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
         :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception(
-                """From 6.2.0, this command is deprecated.
-It can be replaced by "zrange" with "range_method" set to "BYSCORE".
-Source: https://redis.io/commands/zrangebyscore""")
-
         if number_are_not_none(offset, count, number=1):
             raise Exception("Both \"offset\" and \"count\" must be specified.")
 
         command: list = ["ZRANGEBYSCORE", key, min_score, max_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
@@ -2262,19 +2215,14 @@
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zrevrange
 
         :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From 6.2.0, this command is deprecated.
-It can be replaced by "zrange" with "rev" set to True.
-Source: https://redis.io/commands/zrevrange""")
-
         command: list = ["ZREVRANGE", key, start, stop]
 
         if with_scores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
@@ -2290,19 +2238,14 @@
         offset: int | None = None,
         count: int | None = None
     ) -> list[str]:
         """
         See https://redis.io/commands/zrevrangebylex
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From 6.2.0, this command is deprecated.
-It can be replaced by "zrange" with "rev" set to True and "range_method" set to "BYLEX".
-Source: https://redis.io/commands/zrevrangebylex""")
-
         handle_zrangebylex_exceptions(min_score, max_score, offset, count)
 
         command: list = ["ZREVRANGEBYLEX", key, max_score, min_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
 
@@ -2325,19 +2268,14 @@
         See https://redis.io/commands/zrevrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
         :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From 6.2.0, this command is deprecated.
-It can be replaced by "zrange" with "rev" set to True and "range_method" set to "BYSCORE".
-Source: https://redis.io/commands/zrevrangebyscore""")
-
         if number_are_not_none(offset, count, number=1):
             raise Exception("Both \"offset\" and \"count\" must be specified.")
 
         command: list = ["ZREVRANGEBYSCORE", key, max_score, min_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
@@ -2573,19 +2511,14 @@
         return await self.run(command)
 
     async def getset(self, key: str, value: Any) -> str | None:
         """
         See https://redis.io/commands/getset
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 6.2.0, this command is deprecated.
-It can be replaced by "set" with "get".
-Source: https://redis.io/commands/getset""")
-
         command: list = ["GETSET", key, value]
 
         return await self.run(command)
 
     async def incr(self, key: str) -> int:
         """
         See https://redis.io/commands/incr
@@ -2654,19 +2587,14 @@
         return await self.run(command)
 
     async def psetex(self, key: str, milliseconds: int, value: Any) -> str:
         """
         See https://redis.io/commands/psetex
         """
 
-        if not self.allow_deprecated:
-            raise Exception(""" From version 2.6.12, this command is deprecated.
-It can be replaced by "set" with "milliseconds".
-Source: https://redis.io/commands/psetex""")
-
         command: list = ["PSETEX", key, milliseconds, value]
 
         return await self.run(command)
 
     async def set(
         self,
         key: str,
@@ -2729,33 +2657,23 @@
         return await self.run(command)
 
     async def setex(self, key: str, seconds: int, value: Any) -> str:
         """
         See https://redis.io/commands/setex
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 2.6.12, this command is deprecated.
-It can be replaced by "set" with "seconds".
-Source: https://redis.io/commands/setex""")
-
         command: list = ["SETEX", key, seconds, value]
 
         return await self.run(command)
 
     async def setnx(self, key: str, value: Any) -> Literal[1, 0]:
         """
         See https://redis.io/commands/setnx
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 2.6.12, this command is deprecated.
-It can be replaced by "set" with "nx".
-Source: https://redis.io/commands/setnx""")
-
         command: list = ["SETNX", key, value]
 
         return await self.run(command)
 
     async def setrange(self, key: str, offset: int, value: Any) -> int:
         """
         See https://redis.io/commands/setrange
@@ -2775,19 +2693,14 @@
         return await self.run(command)
 
     async def substr(self, key: str, start: int, end: int) -> str:
         """
         See https://redis.io/commands/substr
         """
 
-        if not self.allow_deprecated:
-            raise Exception("""From version 2.0.0, this command is deprecated.
-It can be replaced by "getrange".
-Source: https://redis.io/commands/substr""")
-
         command: list = ["SUBSTR", key, start, end]
 
         return await self.run(command)
 
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
```

### Comparing `upstash_redis-0.10.0/upstash_redis/http/decode.py` & `upstash_redis-0.11.0/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.10.0/upstash_redis/http/execute.py` & `upstash_redis-0.11.0/upstash_redis/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.10.0/upstash_redis/schema/commands/returns.py` & `upstash_redis-0.11.0/upstash_redis/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.10.0/upstash_redis/schema/http.py` & `upstash_redis-0.11.0/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.10.0/upstash_redis/utils/exception.py` & `upstash_redis-0.11.0/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.10.0/upstash_redis/utils/format.py` & `upstash_redis-0.11.0/upstash_redis/utils/format.py`

 * *Files identical despite different names*

