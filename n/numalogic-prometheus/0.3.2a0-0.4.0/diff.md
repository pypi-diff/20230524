# Comparing `tmp/numalogic_prometheus-0.3.2a0.tar.gz` & `tmp/numalogic_prometheus-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.3.2a0.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.4.0.tar", max compression
```

## Comparing `numalogic_prometheus-0.3.2a0.tar` & `numalogic_prometheus-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-26 22:19:51.663205 numalogic_prometheus-0.3.2a0/LICENSE
--rw-r--r--   0        0        0      839 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/__init__.py
--rw-r--r--   0        0        0     1395 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1316 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/redis.py
--rw-r--r--   0        0        0     1342 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4483 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/factory.py
--rw-r--r--   0        0        0     8855 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      741 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4148 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/inference.py
--rw-r--r--   0        0        0     6982 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     1887 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     3431 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4321 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     5616 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/train.py
--rw-r--r--   0        0        0     7808 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5935 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/watcher.py
--rw-r--r--   0        0        0     1542 2023-04-26 22:19:51.671205 numalogic_prometheus-0.3.2a0/pyproject.toml
--rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.2a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/LICENSE
+-rw-r--r--   0        0        0      839 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3565 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1316 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2515 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4483 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/factory.py
+-rw-r--r--   0        0        0     7002 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4339 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     6836 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     2768 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     4193 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4148 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     6965 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     8095 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5935 2023-05-24 21:36:52.439238 numalogic_prometheus-0.4.0/numaprom/watcher.py
+-rw-r--r--   0        0        0     1550 2023-05-24 21:36:52.443238 numalogic_prometheus-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.0/PKG-INFO
```

### Comparing `numalogic_prometheus-0.3.2a0/LICENSE` & `numalogic_prometheus-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/__init__.py` & `numalogic_prometheus-0.4.0/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/_config.py` & `numalogic_prometheus-0.4.0/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/_constants.py` & `numalogic_prometheus-0.4.0/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.4.0/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/clients/redis.py` & `numalogic_prometheus-0.4.0/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.4.0/numaprom/clients/sentinel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,45 @@
+import os
 from typing import Optional
 
+from numalogic.tools.types import redis_client_t
 from redis.backoff import ExponentialBackoff
-from redis.client import Redis
 from redis.exceptions import RedisClusterException, RedisError
 from redis.retry import Retry
 from redis.sentinel import Sentinel, MasterNotFoundError
 
 from numaprom import get_logger
+from numaprom._config import RedisConf
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
-SENTINEL_MASTER_CLIENT: Optional[Redis] = None
+SENTINEL_MASTER_CLIENT: Optional[redis_client_t] = None
 
 
 def get_redis_client(
-    host: str, port: int, password: str, mastername: str, recreate: bool = False
-) -> Redis:
+    host: str,
+    port: int,
+    password: str,
+    mastername: str,
+    decode_responses: bool = False,
+    recreate: bool = False,
+) -> redis_client_t:
     """
     Return a master redis client for sentinel connections, with retry.
+
+    Args:
+        host: Redis host
+        port: Redis port
+        password: Redis password
+        mastername: Redis sentinel master name
+        decode_responses: Whether to decode responses
+        recreate: Whether to flush and recreate the client
+
+    Returns:
+        Redis client instance
     """
     global SENTINEL_MASTER_CLIENT
 
     if not recreate and SENTINEL_MASTER_CLIENT:
         return SENTINEL_MASTER_CLIENT
 
     retry = Retry(
@@ -30,16 +49,43 @@
             ConnectionError,
             TimeoutError,
             RedisClusterException,
             RedisError,
             MasterNotFoundError,
         ),
     )
-    sentinel_args = {"sentinels": [(host, port)], "socket_timeout": 0.1, "decode_responses": True}
+    sentinel_args = {
+        "sentinels": [(host, port)],
+        "socket_timeout": 0.1,
+        "decode_responses": decode_responses,
+    }
 
     _LOGGER.info("Sentinel redis params: %s", sentinel_args)
 
     sentinel = Sentinel(
         **sentinel_args, sentinel_kwargs=dict(password=password), password=password, retry=retry
     )
     SENTINEL_MASTER_CLIENT = sentinel.master_for(mastername)
     return SENTINEL_MASTER_CLIENT
+
+
+def get_redis_client_from_conf(redis_conf: RedisConf = None, **kwargs) -> redis_client_t:
+    """
+    Return a master redis client from config for sentinel connections, with retry.
+
+    Args:
+        redis_conf: RedisConf object with host, port, master_name, etc.
+        **kwargs: Additional arguments to pass to get_redis_client.
+
+    Returns:
+        Redis client instance
+    """
+    if not redis_conf:
+        redis_conf = ConfigManager.get_redis_config()
+
+    return get_redis_client(
+        redis_conf.host,
+        redis_conf.port,
+        password=os.getenv("REDIS_AUTH"),
+        mastername=redis_conf.master_name,
+        **kwargs
+    )
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/configs/config.yaml` & `numalogic_prometheus-0.4.0/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.4.0/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/entities.py` & `numalogic_prometheus-0.4.0/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/factory.py` & `numalogic_prometheus-0.4.0/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/tools.py` & `numalogic_prometheus-0.4.0/numaprom/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import socket
 import time
 from collections import OrderedDict
 from datetime import timedelta, datetime
 from functools import wraps
 from json import JSONDecodeError
-from typing import Optional, Sequence, List
+from typing import List
 
-import boto3
 import numpy as np
 import pandas as pd
 import pytz
-from botocore.session import get_session
-from mlflow.entities.model_registry import ModelVersion
-from mlflow.exceptions import RestException
 from numalogic.config import PostprocessFactory
 from numalogic.models.threshold import SigmoidThreshold
-from numalogic.registry import MLflowRegistry, ArtifactData
 from pynumaflow.function import Messages, Message
 
 from numaprom import get_logger, MetricConf
-from numaprom.entities import TrainerPayload, StreamPayload
 from numaprom.clients.prometheus import Prometheus
+from numaprom.entities import TrainerPayload, StreamPayload
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def catch_exception(func):
     @wraps(func)
@@ -42,44 +37,44 @@
 def msgs_forward(handler_func):
     @wraps(handler_func)
     def inner_function(*args, **kwargs):
         json_list = handler_func(*args, **kwargs)
         msgs = Messages()
         for json_data in json_list:
             if json_data:
-                msgs.append(Message.to_all(json_data))
+                msgs.append(Message(json_data))
             else:
                 msgs.append(Message.to_drop())
         return msgs
 
     return inner_function
 
 
 def msg_forward(handler_func):
     @wraps(handler_func)
     def inner_function(*args, **kwargs):
         json_data = handler_func(*args, **kwargs)
         msgs = Messages()
         if json_data:
-            msgs.append(Message.to_all(value=json_data))
+            msgs.append(Message(value=json_data))
         else:
             msgs.append(Message.to_drop())
         return msgs
 
     return inner_function
 
 
 def conditional_forward(hand_func):
     @wraps(hand_func)
     def inner_function(*args, **kwargs) -> Messages:
         data = hand_func(*args, **kwargs)
         msgs = Messages()
         for vertex, json_data in data:
             if json_data and vertex:
-                msgs.append(Message.to_vtx(key=vertex.encode(), value=json_data))
+                msgs.append(Message(value=json_data, tags=[vertex.encode()]))
             else:
                 msgs.append(Message.to_drop())
         return msgs
 
     return inner_function
 
 
@@ -117,45 +112,14 @@
             time.sleep(sleep_sec)
         else:
             return True
     _LOGGER.error("Failed to resolve hostname: %s even after retries!")
     return False
 
 
-def load_model(
-    skeys: Sequence[str], dkeys: Sequence[str], artifact_type: str = "pytorch"
-) -> Optional[ArtifactData]:
-    set_aws_session()
-    try:
-        registry_conf = ConfigManager.get_registry_config()
-        ml_registry = MLflowRegistry(
-            tracking_uri=registry_conf.tracking_uri, artifact_type=artifact_type
-        )
-        return ml_registry.load(skeys=skeys, dkeys=dkeys)
-    except RestException as warn:
-        if warn.error_code == 404:
-            return None
-        _LOGGER.warning("Non 404 error from mlflow: %r", warn)
-    except Exception as ex:
-        _LOGGER.error("Unexpected error while loading model from MLflow database: %r", ex)
-        return None
-
-
-def save_model(
-    skeys: Sequence[str], dkeys: Sequence[str], model, artifact_type="pytorch", **metadata
-) -> Optional[ModelVersion]:
-    set_aws_session()
-    registry_conf = ConfigManager.get_registry_config()
-    ml_registry = MLflowRegistry(
-        tracking_uri=registry_conf.tracking_uri, artifact_type=artifact_type
-    )
-    version = ml_registry.save(skeys=skeys, dkeys=dkeys, artifact=model, **metadata)
-    return version
-
-
 def fetch_data(
     payload: TrainerPayload,
     metric_config: MetricConf,
     labels: dict,
     return_labels=None,
     hours: int = 36,
 ) -> pd.DataFrame:
@@ -179,30 +143,14 @@
         payload.uuid,
         time.time() - _start_time,
         df.shape,
     )
     return df
 
 
-def set_aws_session() -> None:
-    """
-    Setup default aws session by refreshing credentials.
-    """
-    session = get_session()
-    credentials = session.get_credentials()
-    if not credentials:
-        _LOGGER.debug("No AWS credentials object returned")
-        return
-    boto3.setup_default_session(
-        aws_access_key_id=credentials.access_key,
-        aws_secret_access_key=credentials.secret_key,
-        aws_session_token=credentials.token,
-    )
-
-
 def calculate_static_thresh(payload: StreamPayload, upper_limit: float):
     """
     Calculates anomaly scores using static thresholding.
     """
     x = payload.get_stream_array(original=True)
     static_clf = SigmoidThreshold(upper_limit=upper_limit)
     static_scores = static_clf.score_samples(x)
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udf/filter.py` & `numalogic_prometheus-0.4.0/numaprom/udf/filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from numaprom.tools import catch_exception, msg_forward
 
 _LOGGER = get_logger(__name__)
 
 
 @catch_exception
 @msg_forward
-def metric_filter(_: str, datum: Datum) -> Optional[Messages]:
+def metric_filter(_: list[str], datum: Datum) -> Optional[Messages]:
     """
     UDF to filter metrics by labels
     """
     _LOGGER.debug("Received Msg: %s ", datum.value)
 
     msg = datum.value.decode("utf-8")
     data = json.loads(msg)
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udf/inference.py` & `numalogic_prometheus-0.4.0/numaprom/udf/inference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import time
-from datetime import datetime, timedelta
-
 from numalogic.config import NumalogicConf
 from numalogic.models.autoencoder import AutoencoderTrainer
-from numalogic.registry import ArtifactData
+from numalogic.registry import ArtifactData, RedisRegistry
 from numalogic.tools.data import StreamingDataset
+from numalogic.tools.exceptions import RedisRegistryError
 from orjson import orjson
 from pynumaflow.function import Datum
 from torch.utils.data import DataLoader
 
-from numaprom import get_logger, MetricConf
+from numaprom import get_logger
+from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import PayloadFactory
 from numaprom.entities import Status, StreamPayload, Header
-from numaprom.tools import load_model, msg_forward
+from numaprom.tools import msg_forward
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
+REDIS_CLIENT = get_redis_client_from_conf()
 
 
 def _run_inference(
     payload: StreamPayload, artifact_data: ArtifactData, numalogic_conf: NumalogicConf
 ) -> StreamPayload:
     model = artifact_data.artifact
     stream_data = payload.get_stream_array()
@@ -36,27 +37,16 @@
 
     payload.set_win_arr(recon_err.numpy())
     payload.set_status(Status.INFERRED)
     payload.set_metadata("version", artifact_data.extras.get("version"))
     return payload
 
 
-def _is_model_stale(
-    payload: StreamPayload, artifact_data: ArtifactData, metric_config: MetricConf
-) -> bool:
-    date_updated = artifact_data.extras["last_updated_timestamp"] / 1000
-    stale_date = (datetime.now() - timedelta(hours=int(metric_config.retrain_freq_hr))).timestamp()
-    if date_updated < stale_date:
-        _LOGGER.info("%s - Model found is stale for %s", payload.uuid, payload.composite_keys)
-        return True
-    return False
-
-
 @msg_forward
-def inference(_: str, datum: Datum) -> bytes:
+def inference(_: list[str], datum: Datum) -> bytes:
     _start_time = time.perf_counter()
 
     _in_msg = datum.value.decode("utf-8")
 
     # Construct payload object
     payload = PayloadFactory.from_json(_in_msg)
 
@@ -70,30 +60,43 @@
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     # Load config
     metric_config = ConfigManager.get_metric_config(payload.composite_keys)
     numalogic_conf = metric_config.numalogic_conf
 
     # Load inference model
-    artifact_data = load_model(
-        skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
-        dkeys=[numalogic_conf.model.name],
-    )
+    model_registry = RedisRegistry(client=REDIS_CLIENT)
+    try:
+        artifact_data = model_registry.load(
+            skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
+            dkeys=[numalogic_conf.model.name],
+        )
+    except RedisRegistryError as err:
+        _LOGGER.exception(
+            "%s - Error while fetching inference artifact, keys: %s, err: %r",
+            payload.uuid,
+            payload.composite_keys,
+            err,
+        )
+        payload.set_header(Header.STATIC_INFERENCE)
+        payload.set_status(Status.RUNTIME_ERROR)
+        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
+
     if not artifact_data:
         _LOGGER.info(
             "%s - Inference artifact not found, forwarding for static thresholding. Keys: %s",
             payload.uuid,
             payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.ARTIFACT_NOT_FOUND)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     # Check if current model is stale
-    if _is_model_stale(payload, artifact_data, metric_config):
+    if RedisRegistry.is_artifact_stale(artifact_data, int(metric_config.retrain_freq_hr)):
         payload.set_header(Header.MODEL_STALE)
 
     # Generate predictions
     try:
         payload = _run_inference(payload, artifact_data, numalogic_conf)
     except RuntimeError:
         _LOGGER.info(
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.4.0/numaprom/udf/postprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 import os
 import time
-import numpy as np
 from typing import List
-from orjson import orjson
-from redis.exceptions import RedisError, RedisClusterException
 
+import numpy as np
+from orjson import orjson
 from pynumaflow.function import Datum
+from redis.exceptions import RedisError, RedisClusterException
 from redis.sentinel import MasterNotFoundError
 
 from numaprom import get_logger, UnifiedConf
+from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import Status, PrometheusPayload, StreamPayload, Header
-from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import msgs_forward, WindowScorer
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 AUTH = os.getenv("REDIS_AUTH")
 
 
 def __save_to_redis(
     payload: StreamPayload, final_score: float, recreate: bool, unified_config: UnifiedConf
 ):
-    redis_conf = ConfigManager.get_redis_config()
-    r = get_redis_client(
-        redis_conf.host,
-        redis_conf.port,
-        password=AUTH,
-        mastername=redis_conf.master_name,
-        recreate=recreate,
-    )
+    r = get_redis_client_from_conf(recreate=recreate)
 
     metric_name = payload.composite_keys["name"]
 
     r_keys = payload.composite_keys
     r_keys.pop("name")
     r_key = f"{':'.join(r_keys.values())}:{payload.end_ts}"
 
@@ -46,15 +39,15 @@
         metric_name,
         final_score,
     )
 
     anomalies = []
     for m in unified_config.unified_metrics:
         if r.hexists(name=r_key, key=m):
-            anomalies.append(float(r.hget(name=r_key, key=m)))
+            anomalies.append(float(r.hget(name=r_key, key=m).decode()))
         else:
             _LOGGER.debug(
                 "%s - Unable to generate unified anomaly, missing metric: %s, redis_key: %s",
                 payload.uuid,
                 m,
                 r_key,
             )
@@ -159,15 +152,15 @@
             "%s - Unified anomaly payload sent to publisher: %s", payload.uuid, unified_json
         )
         return [publisher_json, unified_json]
     return [publisher_json]
 
 
 @msgs_forward
-def postprocess(_: str, datum: Datum) -> List[bytes]:
+def postprocess(_: List[str], datum: Datum) -> List[bytes]:
     """
     UDF for performing the following steps:
 
     1. Postprocess the raw scores, e.g. bring the scores into a range of 0 - 10
     2. Calculate a unified anomaly score by combining multiple metrics
     3. Construct and publish a Prometheus Payload object
     """
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.4.0/numaprom/udf/preprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,65 @@
+import os
 import time
+from typing import List
 
 import orjson
+from numalogic.registry import RedisRegistry
+from numalogic.tools.exceptions import RedisRegistryError
 from pynumaflow.function import Datum
 
 from numaprom import get_logger
+from numaprom.clients.sentinel import get_redis_client
 from numaprom.entities import Status, StreamPayload, Header
-from numaprom.tools import msg_forward, load_model
+from numaprom.tools import msg_forward
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
+AUTH = os.getenv("REDIS_AUTH")
+REDIS_CONF = ConfigManager.get_redis_config()
+REDIS_CLIENT = get_redis_client(
+    REDIS_CONF.host,
+    REDIS_CONF.port,
+    password=AUTH,
+    mastername=REDIS_CONF.master_name,
+    recreate=False,
+)
+
 
 @msg_forward
-def preprocess(_: str, datum: Datum) -> bytes:
+def preprocess(_: List[str], datum: Datum) -> bytes:
     _start_time = time.perf_counter()
     _in_msg = datum.value.decode("utf-8")
 
     payload = StreamPayload(**orjson.loads(_in_msg))
     _LOGGER.info("%s - Received Payload: %r ", payload.uuid, payload)
 
     # Load config
     metric_config = ConfigManager.get_metric_config(payload.composite_keys)
     preprocess_cfgs = metric_config.numalogic_conf.preprocess
 
     # Load preprocess artifact
-    preproc_artifact = load_model(
-        skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
-        dkeys=[_conf.name for _conf in preprocess_cfgs],
-        artifact_type="sklearn",
-    )
+    model_registry = RedisRegistry(client=REDIS_CLIENT)
+    try:
+        preproc_artifact = model_registry.load(
+            skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
+            dkeys=[_conf.name for _conf in preprocess_cfgs],
+        )
+    except RedisRegistryError as err:
+        _LOGGER.exception(
+            "%s - Error while fetching preproc artifact, keys: %s, err: %r",
+            payload.uuid,
+            payload.composite_keys,
+            err,
+        )
+        payload.set_header(Header.STATIC_INFERENCE)
+        payload.set_status(Status.RUNTIME_ERROR)
+        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
+
     if not preproc_artifact:
         _LOGGER.info(
             "%s - Preprocess artifact not found, forwarding for static thresholding. Keys: %s",
             payload.uuid,
             payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udf/threshold.py` & `numalogic_prometheus-0.4.0/numaprom/udf/threshold.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import time
 from collections import OrderedDict
+from typing import List
 
+from numalogic.registry import RedisRegistry
+from numalogic.tools.exceptions import RedisRegistryError
 from orjson import orjson
 from pynumaflow.function import Datum
 
 from numaprom import get_logger
 from numaprom._constants import TRAIN_VTX_KEY, POSTPROC_VTX_KEY
+from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import Status, TrainerPayload, PayloadFactory, Header
-from numaprom.tools import conditional_forward, calculate_static_thresh, load_model
+from numaprom.tools import conditional_forward, calculate_static_thresh
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def _get_static_thresh_payload(payload, metric_config) -> bytes:
     """
@@ -25,15 +29,15 @@
     payload.set_metadata("version", -1)
 
     _LOGGER.info("%s - Static thresholding complete for payload: %s", payload.uuid, payload)
     return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
 
 @conditional_forward
-def threshold(_: str, datum: Datum) -> list[tuple[str, bytes]]:
+def threshold(_: List[str], datum: Datum) -> list[tuple[str, bytes]]:
     _start_time = time.perf_counter()
     _in_msg = datum.value.decode("utf-8")
 
     # Construct payload objects
     payload = PayloadFactory.from_json(_in_msg)
     train_payload = TrainerPayload(
         uuid=payload.uuid, composite_keys=OrderedDict(payload.composite_keys)
@@ -52,19 +56,33 @@
         )
         return [
             (TRAIN_VTX_KEY, orjson.dumps(train_payload)),
             (POSTPROC_VTX_KEY, _get_static_thresh_payload(payload, metric_config)),
         ]
 
     # load threshold artifact
-    thresh_artifact = load_model(
-        skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
-        dkeys=[thresh_cfg.name],
-        artifact_type="sklearn",
-    )
+    model_registry = RedisRegistry(client=get_redis_client_from_conf())
+    try:
+        thresh_artifact = model_registry.load(
+            skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
+            dkeys=[thresh_cfg.name],
+        )
+    except RedisRegistryError as err:
+        _LOGGER.exception(
+            "%s - Error while fetching threshold artifact, keys: %s, err: %r",
+            payload.uuid,
+            payload.composite_keys,
+            err,
+        )
+        payload.set_header(Header.STATIC_INFERENCE)
+        payload.set_status(Status.RUNTIME_ERROR)
+        return [
+            (TRAIN_VTX_KEY, orjson.dumps(train_payload)),
+            (POSTPROC_VTX_KEY, _get_static_thresh_payload(payload, metric_config)),
+        ]
     if not thresh_artifact:
         _LOGGER.info(
             "%s - Threshold artifact not found, performing static thresholding. Keys: %s",
             payload.uuid,
             payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udf/window.py` & `numalogic_prometheus-0.4.0/numaprom/udf/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import os
 import time
 import uuid
-from typing import Optional
+from typing import Optional, List
 
 import numpy as np
 import numpy.typing as npt
 from orjson import orjson
 from pynumaflow.function import Datum
 from redis.exceptions import RedisError, RedisClusterException
 
 from numaprom import get_logger
+from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import StreamPayload, Status, Header
-from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import msg_forward, create_composite_keys
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-AUTH = os.getenv("REDIS_AUTH")
-
 
 # TODO get the replacement value from config
 def _clean_arr(
     id_: str,
     ckeys: dict,
     arr: npt.NDArray[float],
     replace_val: float = 0.0,
@@ -40,37 +38,29 @@
 ) -> list[tuple[float, float]]:
     """
     Adds an element to the sliding window using a redis sorted set.
 
     Returns an empty list if adding the element does not create a new entry
     to the set.
     """
-    redis_conf = ConfigManager.get_redis_config()
-    redis_client = get_redis_client(
-        redis_conf.host,
-        redis_conf.port,
-        password=AUTH,
-        mastername=redis_conf.master_name,
-        recreate=recreate,
-    )
-
+    redis_client = get_redis_client_from_conf(recreate=recreate)
     with redis_client.pipeline() as pl:
         pl.zadd(key, {f"{value}::{ts}": ts})
         pl.zremrangebyrank(key, -(buff_size + 10), -buff_size)
         pl.zrange(key, -win_size, -1, withscores=True, score_cast_func=int)
         out = pl.execute()
     _is_new, _, _window = out
     if not _is_new:
         return []
-    _window = list(map(lambda x: (float(x[0].split("::")[0]), x[1]), _window))
+    _window = list(map(lambda x: (float(x[0].decode().split("::")[0]), x[1]), _window))
     return _window
 
 
 @msg_forward
-def window(_: str, datum: Datum) -> Optional[bytes]:
+def window(_: List[str], datum: Datum) -> Optional[bytes]:
     """
     UDF to construct windowing of the streaming input data, required by ML models.
     """
     _LOGGER.debug("Received Msg: %s ", datum.value)
 
     _start_time = time.perf_counter()
     msg = orjson.loads(datum.value)
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udsink/train.py` & `numalogic_prometheus-0.4.0/numaprom/udsink/train.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import os
 import time
-import numpy as np
-import pandas as pd
 from typing import List
-from orjson import orjson
-from sklearn.pipeline import make_pipeline
-from torch.utils.data import DataLoader
 
+import numpy as np
+import pandas as pd
 from numalogic.config import PreprocessFactory, ModelInfo, ThresholdFactory, ModelFactory
 from numalogic.models.autoencoder import AutoencoderTrainer
+from numalogic.registry import RedisRegistry
 from numalogic.tools.data import StreamingDataset
+from numalogic.tools.exceptions import RedisRegistryError
+from numalogic.tools.types import redis_client_t
+from orjson import orjson
 from pynumaflow.sink import Datum, Responses, Response
+from sklearn.pipeline import make_pipeline
+from torch.utils.data import DataLoader
 
 from numaprom import get_logger
+from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import TrainerPayload
-from numaprom.clients.sentinel import get_redis_client
-from numaprom.tools import save_model, fetch_data
+from numaprom.tools import fetch_data
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-AUTH = os.getenv("REDIS_AUTH")
+
+REQUEST_EXPIRY = int(os.getenv("REQUEST_EXPIRY", 300))
 
 
 def clean_data(df: pd.DataFrame, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
     df = df.fillna(method="bfill", limit=limit)
     if df.columns[df.isna().any()].tolist():
@@ -67,44 +71,36 @@
 def _find_threshold(x_reconerr, thresh_cfg: ModelInfo):
     thresh_factory = ThresholdFactory()
     thresh_clf = thresh_factory.get_instance(thresh_cfg)
     thresh_clf.fit(x_reconerr)
     return thresh_clf
 
 
-def _is_new_request(payload: TrainerPayload) -> bool:
-    redis_conf = ConfigManager.get_redis_config()
-    redis_client = get_redis_client(
-        redis_conf.host,
-        redis_conf.port,
-        password=AUTH,
-        mastername=redis_conf.master_name,
-        recreate=False,
-    )
-
+def _is_new_request(redis_client: redis_client_t, payload: TrainerPayload) -> bool:
     _ckeys = ":".join([payload.composite_keys["namespace"], payload.composite_keys["name"]])
     r_key = f"train::{_ckeys}"
 
     value = redis_client.get(r_key)
     if value:
         return False
 
-    redis_client.setex(r_key, time=redis_conf.expiry, value=1)
+    redis_client.setex(r_key, time=REQUEST_EXPIRY, value=1)
     return True
 
 
 def train(datums: List[Datum]) -> Responses:
     responses = Responses()
+    redis_client = get_redis_client_from_conf()
 
     for _datum in datums:
         payload = TrainerPayload(**orjson.loads(_datum.value))
 
         _LOGGER.debug("%s - Starting Training for keys: %s", payload.uuid, payload.composite_keys)
 
-        is_new = _is_new_request(payload)
+        is_new = _is_new_request(redis_client, payload)
         if not is_new:
             _LOGGER.debug(
                 "%s - Skipping train request with keys: %s", payload.uuid, payload.composite_keys
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
@@ -125,44 +121,85 @@
                 payload.uuid,
                 metric_config.min_train_size,
                 train_df.shape,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        preproc_cfg = metric_config.numalogic_conf.preprocess
-        x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfg)
+        preproc_cfgs = metric_config.numalogic_conf.preprocess
+        x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfgs)
 
         trainer_cfg = metric_config.numalogic_conf.trainer
         x_reconerr, anomaly_model = _train_model(payload.uuid, x_train, model_cfg, trainer_cfg)
 
         thresh_cfg = metric_config.numalogic_conf.threshold
         thresh_clf = _find_threshold(x_reconerr, thresh_cfg)
 
         # TODO change this to just use **composite_keys
         skeys = [payload.composite_keys["namespace"], payload.composite_keys["name"]]
 
-        version = save_model(
-            skeys=skeys, dkeys=["preproc"], model=preproc_clf, artifact_type="sklearn"
-        )
-        _LOGGER.info(
-            "%s - Preproc model saved with skeys: %s with version: %s", payload.uuid, skeys, version
-        )
-
-        version = save_model(skeys=skeys, dkeys=[model_cfg.name], model=anomaly_model)
-        _LOGGER.info(
-            "%s - Model saved with skeys: %s with version: %s", payload.uuid, skeys, version
-        )
-
-        version = save_model(
-            skeys=skeys, dkeys=["thresh"], model=thresh_clf, artifact_type="sklearn"
-        )
-        _LOGGER.info(
-            "%s - Threshold model saved with skeys: %s with version: %s",
-            payload.uuid,
-            skeys,
-            version,
-        )
+        # Save main model
+        model_registry = RedisRegistry(client=redis_client)
+        try:
+            version = model_registry.save(
+                skeys=skeys,
+                dkeys=[model_cfg.name],
+                artifact=anomaly_model,
+                uuid=payload.uuid,
+                train_size=train_df.shape[0],
+            )
+        except RedisRegistryError as err:
+            _LOGGER.exception(
+                "%s - Error while saving Model with skeys: %s, err: %r", payload.uuid, skeys, err
+            )
+        else:
+            _LOGGER.info(
+                "%s - Model saved with skeys: %s with version: %s", payload.uuid, skeys, version
+            )
+        # Save preproc model
+        try:
+            version = model_registry.save(
+                skeys=skeys,
+                dkeys=[_conf.name for _conf in preproc_cfgs],
+                artifact=preproc_clf,
+                uuid=payload.uuid,
+            )
+        except RedisRegistryError as err:
+            _LOGGER.exception(
+                "%s - Error while saving Preproc model with skeys: %s, err: %r",
+                payload.uuid,
+                skeys,
+                err,
+            )
+        else:
+            _LOGGER.info(
+                "%s - Preproc model saved with skeys: %s with version: %s",
+                payload.uuid,
+                skeys,
+                version,
+            )
+        # Save threshold model
+        try:
+            version = model_registry.save(
+                skeys=skeys,
+                dkeys=[thresh_cfg.name],
+                artifact=thresh_clf,
+                uuid=payload.uuid,
+            )
+        except RedisRegistryError as err:
+            _LOGGER.error(
+                "%s - Error while saving Threshold model with skeys: %s, err: %r",
+                payload.uuid,
+                skeys,
+                err,
+            )
+        else:
+            _LOGGER.info(
+                "%s - Threshold model saved with skeys: %s with version: %s",
+                payload.uuid,
+                skeys,
+                version,
+            )
 
         responses.append(Response.as_success(_datum.id))
 
     return responses
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.4.0/numaprom/udsink/train_rollout.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 import time
 from typing import List, Iterator
 
 import numpy as np
 import pandas as pd
 from numalogic.config import PreprocessFactory, ModelInfo, ThresholdFactory, ModelFactory
 from numalogic.models.autoencoder import AutoencoderTrainer
+from numalogic.registry import RedisRegistry
 from numalogic.tools.data import StreamingDataset
+from numalogic.tools.exceptions import RedisRegistryError
+from numalogic.tools.types import redis_client_t
 from orjson import orjson
 from pynumaflow.sink import Datum, Responses, Response
 from sklearn.pipeline import make_pipeline
 from torch.utils.data import DataLoader
 
-from numaprom import get_logger
+from numaprom import get_logger, MetricConf
+from numaprom.clients.sentinel import get_redis_client_from_conf
 from numaprom.entities import TrainerPayload
-from numaprom.clients.sentinel import get_redis_client
-from numaprom.tools import save_model, fetch_data
+from numaprom.tools import fetch_data
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-AUTH = os.getenv("REDIS_AUTH")
+REQUEST_EXPIRY = int(os.getenv("REQUEST_EXPIRY", 300))
 
 
 # TODO: extract all good hashes, including when there are 2 hashes at a time
 # TODO avoid filling inf with nan, or at least throw warning
 def clean_data(df: pd.DataFrame, hash_col: str, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
@@ -80,56 +83,47 @@
 def _find_threshold(x_reconerr, thresh_cfg: ModelInfo):
     thresh_factory = ThresholdFactory()
     thresh_clf = thresh_factory.get_instance(thresh_cfg)
     thresh_clf.fit(x_reconerr)
     return thresh_clf
 
 
-def _is_new_request(payload: TrainerPayload) -> bool:
-    redis_conf = ConfigManager.get_redis_config()
-    redis_client = get_redis_client(
-        redis_conf.host,
-        redis_conf.port,
-        password=AUTH,
-        mastername=redis_conf.master_name,
-        recreate=False,
-    )
-
+def _is_new_request(redis_client: redis_client_t, payload: TrainerPayload) -> bool:
     _ckeys = ":".join([payload.composite_keys["namespace"], payload.composite_keys["name"]])
     r_key = f"trainrollout::{_ckeys}"
     value = redis_client.get(r_key)
     if value:
         return False
 
-    redis_client.setex(r_key, time=redis_conf.expiry, value=1)
+    redis_client.setex(r_key, time=REQUEST_EXPIRY, value=1)
     return True
 
 
 def train_rollout(datums: Iterator[Datum]) -> Responses:
     responses = Responses()
+    redis_client = get_redis_client_from_conf()
 
     for _datum in datums:
         payload = TrainerPayload(**orjson.loads(_datum.value))
 
         _LOGGER.debug("%s - Starting Training for keys: %s", payload.uuid, payload.composite_keys)
 
-        is_new = _is_new_request(payload)
+        is_new = _is_new_request(redis_client, payload)
         if not is_new:
             _LOGGER.debug(
                 "%s - Skipping rollouts train request with keys: %s",
                 payload.uuid,
                 payload.composite_keys,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         metric_config = ConfigManager.get_metric_config(payload.composite_keys)
-        model_cfg = metric_config.numalogic_conf.model
 
-        # ToDo: standardize the label name
+        # TODO: standardize the label name
         if "rollouts_pod_template_hash" in payload.composite_keys:
             hash_label = "rollouts_pod_template_hash"
         else:
             hash_label = "hash_id"
 
         train_df = fetch_data(
             payload,
@@ -153,82 +147,96 @@
                 payload.uuid,
                 metric_config.min_train_size,
                 train_df.shape,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        preproc_cfgs = metric_config.numalogic_conf.preprocess
-        x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfgs)
-
-        trainer_cfg = metric_config.numalogic_conf.trainer
-        x_reconerr, anomaly_model, trainer = _train_model(
-            payload.uuid, x_train, model_cfg, trainer_cfg
-        )
+        _train_and_save(metric_config, payload, redis_client, train_df)
 
-        thresh_cfg = metric_config.numalogic_conf.threshold
-        thresh_clf = _find_threshold(x_reconerr, thresh_cfg)
+        responses.append(Response.as_success(_datum.id))
 
-        skeys = [payload.composite_keys["namespace"], payload.composite_keys["name"]]
+    return responses
 
-        # TODO 1. catch mlflow exception
-        # TODO 2. if one of the models fail to save,
-        #  delete the previously saved models and transition stage
 
-        # Save main model
-        version = save_model(
+def _train_and_save(
+    metric_config: MetricConf,
+    payload: TrainerPayload,
+    redis_client: redis_client_t,
+    train_df: pd.DataFrame,
+) -> None:
+    model_cfg = metric_config.numalogic_conf.model
+    preproc_cfgs = metric_config.numalogic_conf.preprocess
+
+    x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfgs)
+
+    trainer_cfg = metric_config.numalogic_conf.trainer
+    x_reconerr, anomaly_model, trainer = _train_model(payload.uuid, x_train, model_cfg, trainer_cfg)
+
+    thresh_cfg = metric_config.numalogic_conf.threshold
+    thresh_clf = _find_threshold(x_reconerr, thresh_cfg)
+
+    skeys = [payload.composite_keys["namespace"], payload.composite_keys["name"]]
+
+    # TODO if one of the models fail to save, delete the previously saved models and transition stage
+    # Save main model
+    model_registry = RedisRegistry(client=redis_client)
+    try:
+        version = model_registry.save(
             skeys=skeys,
             dkeys=[model_cfg.name],
-            model=anomaly_model,
+            artifact=anomaly_model,
             uuid=payload.uuid,
             train_size=train_df.shape[0],
         )
-        if version:
-            _LOGGER.info(
-                "%s - Model saved with skeys: %s with version: %s", payload.uuid, skeys, version
-            )
-        else:
-            _LOGGER.error("%s - Error while saving Model with skeys: %s", payload.uuid, skeys)
-
-        # Save preproc model
-        version = save_model(
+    except RedisRegistryError as err:
+        _LOGGER.exception(
+            "%s - Error while saving Model with skeys: %s, err: %r", payload.uuid, skeys, err
+        )
+    else:
+        _LOGGER.info(
+            "%s - Model saved with skeys: %s with version: %s", payload.uuid, skeys, version
+        )
+    # Save preproc model
+    try:
+        version = model_registry.save(
             skeys=skeys,
             dkeys=[_conf.name for _conf in preproc_cfgs],
-            model=preproc_clf,
-            artifact_type="sklearn",
+            artifact=preproc_clf,
             uuid=payload.uuid,
         )
-        if version:
-            _LOGGER.info(
-                "%s - Preproc model saved with skeys: %s with version: %s",
-                payload.uuid,
-                skeys,
-                version,
-            )
-        else:
-            _LOGGER.error(
-                "%s - Error while saving Preproc model with skeys: %s", payload.uuid, skeys
-            )
-
-        # Save threshold model
-        version = save_model(
+    except RedisRegistryError as err:
+        _LOGGER.exception(
+            "%s - Error while saving Preproc model with skeys: %s, err: %r",
+            payload.uuid,
+            skeys,
+            err,
+        )
+    else:
+        _LOGGER.info(
+            "%s - Preproc model saved with skeys: %s with version: %s",
+            payload.uuid,
+            skeys,
+            version,
+        )
+    # Save threshold model
+    try:
+        version = model_registry.save(
             skeys=skeys,
             dkeys=[thresh_cfg.name],
-            model=thresh_clf,
-            artifact_type="sklearn",
+            artifact=thresh_clf,
             uuid=payload.uuid,
         )
-        if version:
-            _LOGGER.info(
-                "%s - Threshold model saved with skeys: %s with version: %s",
-                payload.uuid,
-                skeys,
-                version,
-            )
-        else:
-            _LOGGER.error(
-                "%s - Error while saving Threshold model with skeys: %s", payload.uuid, skeys
-            )
-
-        responses.append(Response.as_success(_datum.id))
-
-    return responses
+    except RedisRegistryError as err:
+        _LOGGER.error(
+            "%s - Error while saving Threshold model with skeys: %s, err: %r",
+            payload.uuid,
+            skeys,
+            err,
+        )
+    else:
+        _LOGGER.info(
+            "%s - Threshold model saved with skeys: %s with version: %s",
+            payload.uuid,
+            skeys,
+            version,
+        )
```

### Comparing `numalogic_prometheus-0.3.2a0/numaprom/watcher.py` & `numalogic_prometheus-0.4.0/numaprom/watcher.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2a0/pyproject.toml` & `numalogic_prometheus-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.3.2a0"
+version = "0.4.0"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
@@ -15,36 +15,34 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Programming Language :: Python :: 3.10"
 ]
 repository = "https://github.com/numaproj/numalogic-prometheus"
 
 [tool.poetry.dependencies]
 python = "~3.10"
-redis = "^4.3.1"
-pynumaflow = "~0.3"
-numalogic = {version = "~0.3.7", extras = ["mlflow"]}
-boto3 = "^1.25.2"
+redis = {extras = ["hiredis"], version = "^4.5" }
+pynumaflow = "~0.4.1"
+numalogic = {version = "0.4a0", extras = ["redis"], allow-prereleases = true}
 orjson = "^3.8.4"
 omegaconf = "^2.3.0"
 watchdog = "^3.0.0"
 
 [tool.poetry.group.mlflowserver]
 optional = true
 
 [tool.poetry.group.mlflowserver.dependencies]
-mlflow = "^1.30.0"
+mlflow = "^2.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pytorch-lightning = "^1.8.6"
 coverage = "^6.3"
-black = "^22.1"
-fakeredis = "^1.8"
+black = "^23.1"
+fakeredis = "^2.11"
 flake8 = "^5.0"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 freezegun = "^1.2.2"
 
 [tool.black]
 line-length = 100
```

### Comparing `numalogic_prometheus-0.3.2a0/PKG-INFO` & `numalogic_prometheus-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.3.2a0
+Version: 0.4.0
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: boto3 (>=1.25.2,<2.0.0)
-Requires-Dist: numalogic[mlflow] (>=0.3.7,<0.4.0)
+Requires-Dist: numalogic[redis] (==0.4a0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: orjson (>=3.8.4,<4.0.0)
-Requires-Dist: pynumaflow (>=0.3,<0.4)
-Requires-Dist: redis (>=4.3.1,<5.0.0)
+Requires-Dist: pynumaflow (>=0.4.1,<0.5.0)
+Requires-Dist: redis[hiredis] (>=4.5,<5.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/numaproj/numalogic-prometheus
```

