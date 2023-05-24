# Comparing `tmp/dora_rs-0.2.3rc5.tar.gz` & `tmp/dora_rs-0.2.3rc6.tar.gz`

## Comparing `dora_rs-0.2.3rc5.tar` & `dora_rs-0.2.3rc6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-download/Cargo.toml
--rw-r--r--   0     1001      123     1285 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-download/src/lib.rs
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/Cargo.toml
--rw-r--r--   0     1001      123     2216 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      123     2082 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      123     2209 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/event_stream/event.rs
--rw-r--r--   0     1001      123     6168 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/event_stream/mod.rs
--rw-r--r--   0     1001      123     8588 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/event_stream/thread.rs
--rw-r--r--   0     1001      123      267 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/lib.rs
--rw-r--r--   0     1001      123     3153 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/node/control_channel.rs
--rw-r--r--   0     1001      123     4854 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/node/drop_stream.rs
--rw-r--r--   0     1001      123    10789 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/node/mod.rs
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-metrics/Cargo.toml
--rw-r--r--   0     1001      123     1483 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-metrics/src/lib.rs
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/Cargo.toml
--rw-r--r--   0     1001      123     9127 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/config.rs
--rw-r--r--   0     1001      123     1013 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/coordinator_messages.rs
--rw-r--r--   0     1001      123     6466 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/daemon_messages.rs
--rw-r--r--   0     1001      123     8967 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/descriptor/mod.rs
--rw-r--r--   0     1001      123     7313 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/descriptor/validate.rs
--rw-r--r--   0     1001      123     6705 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      123      974 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/lib.rs
--rw-r--r--   0     1001      123     1970 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-core/src/topics.rs
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-python/Cargo.toml
--rw-r--r--   0     1001      123     5862 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-python/src/lib.rs
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      123     3249 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      123     7334 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      123     2010 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/src/lib.rs
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-types/Cargo.toml
--rw-r--r--   0     1001      123     2396 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-types/src/lib.rs
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-message/Cargo.toml
--rw-r--r--   0     1001      123      360 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-message/build.rs
--rw-r--r--   0     1001      123      229 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-message/schema/message.capnp
--rw-r--r--   0     1001      123     3225 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-message/src/lib.rs
--rw-r--r--   0     1001      123     7447 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-message/src/message_capnp.rs
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-tracing/Cargo.toml
--rw-r--r--   0     1001      123     1620 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-tracing/src/lib.rs
--rw-r--r--   0     1001      123     2248 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-tracing/src/telemetry.rs
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/local_dependencies/dora-runtime/Cargo.toml
--rw-r--r--   0     1001      123    13111 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/lib.rs
--rw-r--r--   0     1001      123     4296 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/channel.rs
--rw-r--r--   0     1001      123     2461 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/mod.rs
--rw-r--r--   0     1001      123    12448 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/python.rs
--rw-r--r--   0     1001      123     9727 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/shared_lib.rs
--rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/Cargo.toml
--rw-r--r--   0     1001      123      204 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/README.md
--rw-r--r--   0     1001      123      372 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/dora/__init__.py
--rw-r--r--   0     1001      123      153 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/pyproject.toml
--rw-r--r--   0     1001      123     2076 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/src/lib.rs
--rw-r--r--   0     1001      123   144347 2023-05-04 09:32:46.000000 dora_rs-0.2.3rc5/Cargo.lock
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc5/PKG-INFO
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-download/Cargo.toml
+-rw-r--r--   0     1001      123     1285 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-download/src/lib.rs
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      123     3249 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      123     7334 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      123     2010 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/lib.rs
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-tracing/Cargo.toml
+-rw-r--r--   0     1001      123     1620 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/lib.rs
+-rw-r--r--   0     1001      123     2248 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/telemetry.rs
+-rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/Cargo.toml
+-rw-r--r--   0     1001      123    13111 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/lib.rs
+-rw-r--r--   0     1001      123     4296 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      123     2461 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      123    12448 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/python.rs
+-rw-r--r--   0     1001      123     9727 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/shared_lib.rs
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/Cargo.toml
+-rw-r--r--   0     1001      123     5862 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/src/lib.rs
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-metrics/Cargo.toml
+-rw-r--r--   0     1001      123     1483 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-metrics/src/lib.rs
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/Cargo.toml
+-rw-r--r--   0     1001      123     9127 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/config.rs
+-rw-r--r--   0     1001      123      957 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      123     6485 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/daemon_messages.rs
+-rw-r--r--   0     1001      123     8967 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      123     7313 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      123     6705 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      123      974 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/lib.rs
+-rw-r--r--   0     1001      123     1970 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/topics.rs
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-types/Cargo.toml
+-rw-r--r--   0     1001      123     2396 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-types/src/lib.rs
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/Cargo.toml
+-rw-r--r--   0     1001      123      360 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/build.rs
+-rw-r--r--   0     1001      123      229 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/schema/message.capnp
+-rw-r--r--   0     1001      123     3225 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/src/lib.rs
+-rw-r--r--   0     1001      123     7447 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/src/message_capnp.rs
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/Cargo.toml
+-rw-r--r--   0     1001      123     2216 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      123     2082 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      123     2209 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/event.rs
+-rw-r--r--   0     1001      123     6484 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/mod.rs
+-rw-r--r--   0     1001      123     8588 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/thread.rs
+-rw-r--r--   0     1001      123      267 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/lib.rs
+-rw-r--r--   0     1001      123     3153 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/control_channel.rs
+-rw-r--r--   0     1001      123     5186 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/drop_stream.rs
+-rw-r--r--   0     1001      123    10789 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/mod.rs
+-rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/Cargo.toml
+-rw-r--r--   0     1001      123      204 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/README.md
+-rw-r--r--   0     1001      123      372 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/dora/__init__.py
+-rw-r--r--   0     1001      123      153 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/pyproject.toml
+-rw-r--r--   0     1001      123     2076 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/src/lib.rs
+-rw-r--r--   0     1001      123   144347 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/PKG-INFO
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-download/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-download/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-download"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-download/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-node-api"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 [features]
 default = ["tracing"]
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/daemon_connection/mod.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/event_stream/event.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/event.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/event_stream/mod.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -55,19 +55,27 @@
     pub(crate) fn init_on_channel(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         mut channel: DaemonChannel,
         mut close_channel: DaemonChannel,
     ) -> eyre::Result<Self> {
         channel.register(dataflow_id, node_id.clone())?;
-        channel
+        let reply = channel
             .request(&DaemonRequest::Subscribe)
             .map_err(|e| eyre!(e))
             .wrap_err("failed to create subscription with dora-daemon")?;
 
+        match reply {
+            daemon_messages::DaemonReply::Result(Ok(())) => {}
+            daemon_messages::DaemonReply::Result(Err(err)) => {
+                eyre::bail!("subscribe failed: {err}")
+            }
+            other => eyre::bail!("unexpected subscribe reply: {other:?}"),
+        }
+
         close_channel.register(dataflow_id, node_id.clone())?;
 
         let (tx, rx) = flume::bounded(0);
         let thread_handle = thread::init(node_id.clone(), tx, channel)?;
 
         Ok(EventStream {
             node_id: node_id.clone(),
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/event_stream/thread.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/thread.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/node/control_channel.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/control_channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/node/drop_stream.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/drop_stream.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::time::Duration;
 
 use crate::daemon_connection::DaemonChannel;
 use dora_core::{
     config::NodeId,
     daemon_messages::{
-        DaemonCommunication, DaemonReply, DaemonRequest, DataflowId, DropToken, NodeDropEvent,
+        self, DaemonCommunication, DaemonReply, DaemonRequest, DataflowId, DropToken, NodeDropEvent,
     },
 };
 use eyre::{eyre, Context};
 use flume::RecvTimeoutError;
 
 pub struct DropStream {
     receiver: flume::Receiver<DropToken>,
@@ -41,19 +41,27 @@
     pub fn init_on_channel(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         mut channel: DaemonChannel,
     ) -> eyre::Result<Self> {
         channel.register(dataflow_id, node_id.clone())?;
 
-        channel
+        let reply = channel
             .request(&DaemonRequest::SubscribeDrop)
             .map_err(|e| eyre!(e))
             .wrap_err("failed to create subscription with dora-daemon")?;
 
+        match reply {
+            daemon_messages::DaemonReply::Result(Ok(())) => {}
+            daemon_messages::DaemonReply::Result(Err(err)) => {
+                eyre::bail!("drop subscribe failed: {err}")
+            }
+            other => eyre::bail!("unexpected drop subscribe reply: {other:?}"),
+        }
+
         let (tx, rx) = flume::bounded(0);
         let node_id_cloned = node_id.clone();
 
         let handle = std::thread::spawn(|| drop_stream_loop(node_id_cloned, tx, channel));
 
         Ok(Self {
             receiver: rx,
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-node-api/src/node/mod.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-metrics/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-metrics/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-metrics"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-metrics/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-metrics/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-core"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/config.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/coordinator_messages.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/coordinator_messages.rs`

 * *Files 21% similar despite different names*

```diff
@@ -15,20 +15,21 @@
     },
 }
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 pub enum DaemonEvent {
     AllNodesReady {
         dataflow_id: DataflowId,
+        success: bool,
     },
     AllNodesFinished {
         dataflow_id: DataflowId,
         result: Result<(), String>,
     },
-    Watchdog,
+    Heartbeat,
 }
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 pub enum RegisterResult {
     Ok,
     Err(String),
 }
@@ -37,10 +38,7 @@
     pub fn to_result(self) -> eyre::Result<()> {
         match self {
             RegisterResult::Ok => Ok(()),
             RegisterResult::Err(err) => Err(eyre!(err)),
         }
     }
 }
-
-#[derive(Debug, serde::Serialize, serde::Deserialize)]
-pub struct WatchdogAck;
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/daemon_messages.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/daemon_messages.rs`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         }
     }
 }
 
 type SharedMemoryId = String;
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
+#[must_use]
 pub enum DaemonReply {
     Result(Result<(), String>),
     PreparedMessage { shared_memory_id: SharedMemoryId },
     NextEvents(Vec<NodeEvent>),
     NextDropEvents(Vec<NodeDropEvent>),
     Empty,
 }
@@ -196,29 +197,30 @@
 }
 
 #[derive(Debug, serde::Deserialize, serde::Serialize)]
 pub enum DaemonCoordinatorEvent {
     Spawn(SpawnDataflowNodes),
     AllNodesReady {
         dataflow_id: DataflowId,
+        success: bool,
     },
     StopDataflow {
         dataflow_id: DataflowId,
     },
     ReloadDataflow {
         dataflow_id: DataflowId,
         node_id: NodeId,
         operator_id: Option<OperatorId>,
     },
     Logs {
         dataflow_id: DataflowId,
         node_id: NodeId,
     },
     Destroy,
-    Watchdog,
+    Heartbeat,
 }
 
 #[derive(Debug, serde::Deserialize, serde::Serialize)]
 pub enum InterDaemonEvent {
     Output {
         dataflow_id: DataflowId,
         node_id: NodeId,
@@ -234,15 +236,14 @@
 
 #[derive(Debug, serde::Deserialize, serde::Serialize)]
 pub enum DaemonCoordinatorReply {
     SpawnResult(Result<(), String>),
     ReloadResult(Result<(), String>),
     StopResult(Result<(), String>),
     DestroyResult(Result<(), String>),
-    WatchdogAck,
     Logs(Result<Vec<u8>, String>),
 }
 
 pub type DataflowId = Uuid;
 
 #[derive(Debug, serde::Deserialize, serde::Serialize)]
 pub struct SpawnDataflowNodes {
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/descriptor/mod.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/descriptor/validate.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/validate.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/descriptor/visualize.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-core/src/topics.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/topics.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-python/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-operator-api-python"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-python/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "shared-memory-server"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/src/channel.rs` & `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/shared-memory-server/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-operator-api-types/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-message/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-message/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-message"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # Building capnp schema script is disabled by default as it requires to install capnp.
 # To change the schema install capnp at: https://capnproto.org/install.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-message/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-message/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-message/src/message_capnp.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-message/src/message_capnp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-tracing/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-tracing/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-tracing"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-tracing/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-tracing/src/telemetry.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-runtime/Cargo.toml` & `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-runtime"
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/channel.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/mod.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/python.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/python.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/local_dependencies/dora-runtime/src/operator/shared_lib.rs` & `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/shared_lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/Cargo.toml` & `dora_rs-0.2.3rc6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [package]
-version= "0.2.3-rc5"
+version= "0.2.3-rc6"
 name = "dora-node-api-python"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc5/src/lib.rs` & `dora_rs-0.2.3rc6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc5/Cargo.lock` & `dora_rs-0.2.3rc6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -530,28 +530,28 @@
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -862,23 +862,23 @@
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "communication-layer-pub-sub"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "flume",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 
 [[package]]
 name = "concurrent-queue"
 version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30ed07550be01594c6026cff2a1d7fe9c8f683caa798e12b68694ac9e88286a3"
 dependencies = [
@@ -1266,15 +1266,15 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "atty",
  "bat",
  "clap 4.1.11",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-core",
@@ -1291,15 +1291,15 @@
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "clap 3.2.23",
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
@@ -1315,15 +1315,15 @@
  "uuid",
  "which",
  "zenoh",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
  "serde_yaml 0.9.19",
@@ -1331,15 +1331,15 @@
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "async-trait",
  "bincode",
  "clap 3.2.23",
  "ctrlc",
  "dora-core",
  "dora-download",
@@ -1358,15 +1358,15 @@
  "tracing",
  "tracing-opentelemetry",
  "uuid",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
@@ -1387,36 +1387,36 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "capnp",
  "capnpc",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "futures",
  "opentelemetry 0.17.0",
  "opentelemetry-otlp",
  "opentelemetry-system-metrics",
  "tokio",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "arrow",
  "bincode",
  "capnp",
  "dora-core",
  "dora-tracing",
  "eyre",
@@ -1431,101 +1431,101 @@
  "tokio",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
  "flume",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-runtime",
  "eyre",
  "flume",
  "pyo3",
  "serde_yaml 0.8.23",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "arrow",
  "dora-node-api",
  "eyre",
  "flume",
  "pyo3",
  "serde_yaml 0.8.23",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "clap 4.1.11",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
  "dora-operator-api-python",
@@ -1545,15 +1545,15 @@
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tokio",
  "tracing",
  "tracing-opentelemetry",
@@ -2826,33 +2826,33 @@
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "nanorand"
@@ -4030,33 +4030,33 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "rust-dataflow-example-operator"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "rust-dataflow-example-sink"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rustc-hash"
@@ -4353,15 +4353,15 @@
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
  "shared_memory",
  "tracing",
@@ -5938,15 +5938,15 @@
  "zenoh-link-commons",
  "zenoh-protocol-core",
  "zenoh-sync",
 ]
 
 [[package]]
 name = "zenoh-logger"
-version = "0.2.3-rc5"
+version = "0.2.3-rc6"
 dependencies = [
  "zenoh",
 ]
 
 [[package]]
 name = "zenoh-macros"
 version = "0.7.0-rc"
```

