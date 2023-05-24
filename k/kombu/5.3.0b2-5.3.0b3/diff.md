# Comparing `tmp/kombu-5.3.0b2.tar.gz` & `tmp/kombu-5.3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kombu-5.3.0b2.tar", last modified: Wed Oct 19 14:02:11 2022, max compression
+gzip compressed data, was "kombu-5.3.0b3.tar", last modified: Mon Mar 20 11:02:46 2023, max compression
```

## Comparing `kombu-5.3.0b2.tar` & `kombu-5.3.0b3.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.232524 kombu-5.3.0b2/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5599 2022-10-19 13:47:58.000000 kombu-5.3.0b2/AUTHORS
--rw-rw-r--   0 asif      (1000) asif      (1000)      436 2021-09-07 04:22:35.000000 kombu-5.3.0b2/FAQ
--rw-rw-r--   0 asif      (1000) asif      (1000)      387 2021-09-07 04:22:35.000000 kombu-5.3.0b2/INSTALL
--rw-rw-r--   0 asif      (1000) asif      (1000)     1664 2021-09-07 04:22:35.000000 kombu-5.3.0b2/LICENSE
--rw-rw-r--   0 asif      (1000) asif      (1000)      515 2021-09-07 04:22:35.000000 kombu-5.3.0b2/MANIFEST.in
--rw-rw-r--   0 asif      (1000) asif      (1000)     1676 2022-10-19 14:02:11.232524 kombu-5.3.0b2/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    13195 2022-10-19 13:59:41.000000 kombu-5.3.0b2/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      980 2021-09-07 04:22:35.000000 kombu-5.3.0b2/THANKS
--rw-rw-r--   0 asif      (1000) asif      (1000)       82 2021-09-07 04:22:35.000000 kombu-5.3.0b2/TODO
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.120524 kombu-5.3.0b2/docs/
--rw-rw-r--   0 asif      (1000) asif      (1000)     8009 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/Makefile
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.120524 kombu-5.3.0b2/docs/_ext/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/_ext/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.120524 kombu-5.3.0b2/docs/_static/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/_static/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.120524 kombu-5.3.0b2/docs/_templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3082 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/_templates/sidebardonations.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.0b2/docs/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/faq.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.120524 kombu-5.3.0b2/docs/images/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5393 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/images/favicon.ico
--rw-rw-r--   0 asif      (1000) asif      (1000)   115481 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/images/kombu.jpg
--rw-rw-r--   0 asif      (1000) asif      (1000)    24746 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/images/kombusmall.jpg
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.124523 kombu-5.3.0b2/docs/includes/
--rw-rw-r--   0 asif      (1000) asif      (1000)      453 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/includes/installation.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)    10598 2022-10-19 13:57:25.000000 kombu-5.3.0b2/docs/includes/introduction.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      726 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/includes/resources.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/introduction.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7476 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/make.bat
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.148524 kombu-5.3.0b2/docs/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2078 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      301 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.abstract.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      354 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.aws.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.aws.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      353 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.aws.sqs.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      340 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.aws.sqs.message.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      332 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.aws.sqs.queue.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      327 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.aws.sqs.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      324 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.debug.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      347 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.http.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      338 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.http.curl.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      312 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.http.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      317 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.hub.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      320 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.semaphore.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.asynchronous.timer.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.clocks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.common.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      745 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.compat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      513 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.compression.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      884 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      461 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.exceptions.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.log.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.matcher.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.message.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      275 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.mixins.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2335 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.pidbox.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.pools.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      287 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.resource.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6031 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1118 2022-04-17 07:07:11.000000 kombu-5.3.0b2/docs/reference/kombu.serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2045 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.simple.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      446 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.SLMQ.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2736 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.SQS.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      533 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.azureservicebus.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      557 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.azurestoragequeues.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1883 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      605 2022-06-19 07:31:49.000000 kombu-5.3.0b2/docs/reference/kombu.transport.confluentkafka.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      459 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.consul.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      451 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.etcd.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      493 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.filesystem.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      741 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.librabbitmq.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      466 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.memory.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      465 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.mongodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      715 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.pyamqp.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      535 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.pyro.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      664 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.qpid.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      576 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.redis.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      543 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1152 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.sqlalchemy.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      772 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.virtual.exchange.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2271 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.virtual.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      484 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.transport.zookeeper.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.amq_manager.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      313 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.collections.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.compat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.debug.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.div.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      311 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.encoding.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      302 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.eventio.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      318 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.functional.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      309 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.imports.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.json.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.limits.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      308 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.objects.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.scheduling.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      289 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.text.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.time.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.url.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/reference/kombu.utils.uuid.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.148524 kombu-5.3.0b2/docs/templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1236 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/templates/readme.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.152524 kombu-5.3.0b2/docs/userguide/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7046 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/connections.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7298 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/consumers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1047 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/examples.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6726 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/failover.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      232 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3247 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/introduction.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5458 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/pools.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3635 2021-09-07 04:22:35.000000 kombu-5.3.0b2/docs/userguide/producers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6482 2022-08-01 07:19:26.000000 kombu-5.3.0b2/docs/userguide/serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3929 2022-03-06 04:55:41.000000 kombu-5.3.0b2/docs/userguide/simple.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.156524 kombu-5.3.0b2/examples/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1550 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/complete_receive.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1174 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/complete_send.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.156524 kombu-5.3.0b2/examples/experimental/
--rw-rw-r--   0 asif      (1000) asif      (1000)      745 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/experimental/async_consume.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      321 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/hello_consumer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      349 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/hello_publisher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      755 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/memory_transport.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.156524 kombu-5.3.0b2/examples/rpc-tut6/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1446 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/rpc-tut6/rpc_client.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1331 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/rpc-tut6/rpc_server.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1225 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_eventlet_receive.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1181 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_eventlet_send.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_receive.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1001 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_send.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.160524 kombu-5.3.0b2/examples/simple_task_queue/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/examples/simple_task_queue/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      994 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_task_queue/client.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      323 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_task_queue/queues.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       92 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_task_queue/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1276 2022-04-17 07:07:11.000000 kombu-5.3.0b2/examples/simple_task_queue/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.108523 kombu-5.3.0b2/extra/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.160524 kombu-5.3.0b2/extra/appveyor/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1844 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/appveyor/run_with_compiler.cmd
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.160524 kombu-5.3.0b2/extra/requirements/
--rw-rw-r--   0 asif      (1000) asif      (1000)      149 2022-10-19 13:47:58.000000 kombu-5.3.0b2/extra/requirements/default.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       95 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/dev.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      240 2021-11-07 23:46:52.000000 kombu-5.3.0b2/extra/requirements/docs.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.164524 kombu-5.3.0b2/extra/requirements/extras/
--rw-rw-r--   0 asif      (1000) asif      (1000)       24 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/azureservicebus.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/azurestoragequeues.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/brotli.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-08-01 07:19:26.000000 kombu-5.3.0b2/extra/requirements/extras/confluentkafka.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/consul.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/couchdb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/etcd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-11-08 00:17:43.000000 kombu-5.3.0b2/extra/requirements/extras/librabbitmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      135 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/lzma.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/mongodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        8 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/msgpack.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        6 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/pyro.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       35 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/qpid.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/redis.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/slmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       11 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/sqlalchemy.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       82 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/sqs.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/yaml.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/extras/zookeeper.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/extras/zstd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/funtest.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      116 2022-04-17 07:07:11.000000 kombu-5.3.0b2/extra/requirements/pkgutils.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       37 2021-09-07 04:22:35.000000 kombu-5.3.0b2/extra/requirements/test-ci-py2.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      279 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/test-ci-windows.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      292 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/test-ci.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       70 2022-06-19 07:31:49.000000 kombu-5.3.0b2/extra/requirements/test.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.172524 kombu-5.3.0b2/kombu/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3924 2022-10-19 13:57:03.000000 kombu-5.3.0b2/kombu/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4323 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/abstract.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.176524 kombu-5.3.0b2/kombu/asynchronous/
--rw-rw-r--   0 asif      (1000) asif      (1000)      237 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.180524 kombu-5.3.0b2/kombu/asynchronous/aws/
--rw-rw-r--   0 asif      (1000) asif      (1000)      475 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8538 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      522 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/ext.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.180524 kombu-5.3.0b2/kombu/asynchronous/aws/sqs/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/kombu/asynchronous/aws/sqs/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6808 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/sqs/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      131 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/sqs/ext.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      892 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/sqs/message.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4402 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/aws/sqs/queue.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1773 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/debug.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.180524 kombu-5.3.0b2/kombu/asynchronous/http/
--rw-rw-r--   0 asif      (1000) asif      (1000)      863 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/http/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9502 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/http/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9752 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/asynchronous/http/curl.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11932 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/asynchronous/hub.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3478 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/semaphore.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6868 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/asynchronous/timer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4799 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/clocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13416 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/common.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6752 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2942 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/compression.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    39601 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32807 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/entity.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2838 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/exceptions.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4066 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4269 2022-06-29 07:05:26.000000 kombu-5.3.0b2/kombu/matcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8059 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/message.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24047 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/messaging.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9667 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/mixins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14789 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/pidbox.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3975 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/pools.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7682 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/resource.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15533 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5302 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/simple.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.188524 kombu-5.3.0b2/kombu/transport/
--rw-rw-r--   0 asif      (1000) asif      (1000)     6215 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/SLMQ.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    34240 2022-08-01 07:19:26.000000 kombu-5.3.0b2/kombu/transport/SQS.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3328 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/transport/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16272 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/azureservicebus.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6448 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/transport/azurestoragequeues.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7663 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12106 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/transport/confluentkafka.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9308 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8485 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/etcd.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10416 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/transport/filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6022 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/librabbitmq.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2404 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/memory.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14989 2022-06-19 07:31:49.000000 kombu-5.3.0b2/kombu/transport/mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7752 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/pyamqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/pyro.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    71681 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/qpid.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    48179 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/transport/redis.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.188524 kombu-5.3.0b2/kombu/transport/sqlalchemy/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7428 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/sqlalchemy/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2294 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/sqlalchemy/models.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.192524 kombu-5.3.0b2/kombu/transport/virtual/
--rw-rw-r--   0 asif      (1000) asif      (1000)      476 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/virtual/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    34026 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/virtual/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4838 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/virtual/exchange.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/transport/zookeeper.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.196524 kombu-5.3.0b2/kombu/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)      698 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      716 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/amq_manager.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      942 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/collections.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3565 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/utils/compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      908 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/div.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2297 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/encoding.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10159 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/eventio.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10640 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2077 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3576 2022-10-19 13:47:58.000000 kombu-5.3.0b2/kombu/utils/json.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2497 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/limits.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1743 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2914 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/scheduling.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2214 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/text.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      272 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3804 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/url.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      315 2022-04-17 07:07:11.000000 kombu-5.3.0b2/kombu/utils/uuid.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.176524 kombu-5.3.0b2/kombu.egg-info/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1676 2022-10-19 14:02:10.000000 kombu-5.3.0b2/kombu.egg-info/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    10459 2022-10-19 14:02:10.000000 kombu-5.3.0b2/kombu.egg-info/SOURCES.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2022-10-19 14:02:10.000000 kombu-5.3.0b2/kombu.egg-info/dependency_links.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2021-09-07 06:13:24.000000 kombu-5.3.0b2/kombu.egg-info/not-zip-safe
--rw-rw-r--   0 asif      (1000) asif      (1000)      613 2022-10-19 14:02:10.000000 kombu-5.3.0b2/kombu.egg-info/requires.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        6 2022-10-19 14:02:10.000000 kombu-5.3.0b2/kombu.egg-info/top_level.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.196524 kombu-5.3.0b2/requirements/
--rw-rw-r--   0 asif      (1000) asif      (1000)      149 2022-10-19 13:47:58.000000 kombu-5.3.0b2/requirements/default.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       95 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/dev.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      240 2021-11-07 23:46:52.000000 kombu-5.3.0b2/requirements/docs.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.200524 kombu-5.3.0b2/requirements/extras/
--rw-rw-r--   0 asif      (1000) asif      (1000)       24 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/azureservicebus.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/azurestoragequeues.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/brotli.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-08-01 07:19:26.000000 kombu-5.3.0b2/requirements/extras/confluentkafka.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/consul.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/couchdb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/etcd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-11-08 00:17:43.000000 kombu-5.3.0b2/requirements/extras/librabbitmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      135 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/lzma.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/mongodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        8 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/msgpack.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        6 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/pyro.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       35 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/qpid.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/redis.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/slmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       11 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/sqlalchemy.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       82 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/sqs.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/yaml.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/extras/zookeeper.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/extras/zstd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/funtest.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      116 2022-04-17 07:07:11.000000 kombu-5.3.0b2/requirements/pkgutils.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       37 2021-09-07 04:22:35.000000 kombu-5.3.0b2/requirements/test-ci-py2.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      279 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/test-ci-windows.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      292 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/test-ci.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       70 2022-06-19 07:31:49.000000 kombu-5.3.0b2/requirements/test.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1152 2022-10-19 14:02:11.232524 kombu-5.3.0b2/setup.cfg
--rw-rw-r--   0 asif      (1000) asif      (1000)     4345 2022-08-01 07:19:26.000000 kombu-5.3.0b2/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.200524 kombu-5.3.0b2/t/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.204524 kombu-5.3.0b2/t/integration/
--rw-rw-r--   0 asif      (1000) asif      (1000)      120 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/integration/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17367 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/integration/common.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1464 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/integration/test_kafka.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3675 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/integration/test_mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1970 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/integration/test_py_amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4990 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/integration/test_redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6008 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/mocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      283 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/skip.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.208524 kombu-5.3.0b2/t/unit/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.212524 kombu-5.3.0b2/t/unit/asynchronous/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/asynchronous/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.212524 kombu-5.3.0b2/t/unit/asynchronous/aws/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      199 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/case.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.212524 kombu-5.3.0b2/t/unit/asynchronous/aws/sqs/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/sqs/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11941 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/sqs/test_connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7140 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/sqs/test_queue.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      318 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/test_aws.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9277 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/aws/test_connection.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.216524 kombu-5.3.0b2/t/unit/asynchronous/http/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/asynchronous/http/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5728 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/http/test_curl.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4221 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/http/test_http.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17161 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/asynchronous/test_hub.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1141 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/test_semaphore.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4247 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/asynchronous/test_timer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9493 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/conftest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2359 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/unit/test_clocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17580 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_common.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11181 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_compression.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    31855 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/test_connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13693 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/unit/test_entity.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      229 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/unit/test_exceptions.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4796 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1133 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_matcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1285 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_message.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24481 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_messaging.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7875 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_mixins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12543 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_pidbox.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7238 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/test_pools.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11162 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6704 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/test_simple.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.224524 kombu-5.3.0b2/t/unit/transport/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/transport/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    33591 2022-08-01 07:19:26.000000 kombu-5.3.0b2/t/unit/transport/test_SQS.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9505 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_azureservicebus.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2169 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/transport/test_azurestoragequeues.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5617 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2674 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2197 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_etcd.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10594 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/transport/test_filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4891 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_librabbitmq.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5643 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/transport/test_memory.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17045 2022-06-19 07:31:49.000000 kombu-5.3.0b2/t/unit/transport/test_mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7008 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_pyamqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2892 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/transport/test_pyro.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    71045 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_qpid.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    60297 2022-08-01 07:19:26.000000 kombu-5.3.0b2/t/unit/transport/test_redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1538 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_sqlalchemy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1014 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_transport.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1057 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/test_zookeeper.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.224524 kombu-5.3.0b2/t/unit/transport/virtual/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/transport/virtual/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    21252 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/transport/virtual/test_base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5530 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/transport/virtual/test_exchange.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-10-19 14:02:11.232524 kombu-5.3.0b2/t/unit/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b2/t/unit/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1281 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_amq_manager.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2637 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1630 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_div.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2962 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_encoding.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8800 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      967 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3156 2022-10-19 13:47:58.000000 kombu-5.3.0b2/t/unit/utils/test_json.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1064 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2769 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_scheduling.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      459 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2964 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_url.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      609 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_utils.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      289 2022-04-17 07:07:11.000000 kombu-5.3.0b2/t/unit/utils/test_uuid.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.668144 kombu-5.3.0b3/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5599 2022-10-19 13:47:58.000000 kombu-5.3.0b3/AUTHORS
+-rw-rw-r--   0 asif      (1000) asif      (1000)      436 2021-09-07 04:22:35.000000 kombu-5.3.0b3/FAQ
+-rw-rw-r--   0 asif      (1000) asif      (1000)      387 2021-09-07 04:22:35.000000 kombu-5.3.0b3/INSTALL
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1664 2021-09-07 04:22:35.000000 kombu-5.3.0b3/LICENSE
+-rw-rw-r--   0 asif      (1000) asif      (1000)      515 2021-09-07 04:22:35.000000 kombu-5.3.0b3/MANIFEST.in
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1685 2023-03-20 11:02:46.668144 kombu-5.3.0b3/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13224 2023-03-20 10:59:18.000000 kombu-5.3.0b3/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      980 2021-09-07 04:22:35.000000 kombu-5.3.0b3/THANKS
+-rw-rw-r--   0 asif      (1000) asif      (1000)       82 2021-09-07 04:22:35.000000 kombu-5.3.0b3/TODO
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.560142 kombu-5.3.0b3/docs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8009 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/Makefile
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.560142 kombu-5.3.0b3/docs/_ext/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/_ext/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.560142 kombu-5.3.0b3/docs/_static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/_static/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.560142 kombu-5.3.0b3/docs/_templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3082 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/_templates/sidebardonations.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.0b3/docs/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/faq.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.564143 kombu-5.3.0b3/docs/images/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5393 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/images/favicon.ico
+-rw-rw-r--   0 asif      (1000) asif      (1000)   115481 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/images/kombu.jpg
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24746 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/images/kombusmall.jpg
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.564143 kombu-5.3.0b3/docs/includes/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      453 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/includes/installation.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10598 2023-03-20 10:59:03.000000 kombu-5.3.0b3/docs/includes/introduction.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      726 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/includes/resources.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/introduction.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7476 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/make.bat
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.588143 kombu-5.3.0b3/docs/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2078 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      301 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.abstract.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      354 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.aws.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.aws.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      353 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.aws.sqs.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      340 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.aws.sqs.message.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      332 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.aws.sqs.queue.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      327 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.aws.sqs.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      324 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.debug.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      347 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.http.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      338 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.http.curl.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      312 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.http.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      317 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.hub.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      320 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.semaphore.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.asynchronous.timer.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.clocks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.common.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      745 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.compat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      513 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.compression.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      884 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      461 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.exceptions.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.log.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.matcher.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.message.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      275 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.mixins.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2335 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.pidbox.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.pools.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      287 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.resource.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6031 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1118 2022-04-17 07:07:11.000000 kombu-5.3.0b3/docs/reference/kombu.serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2045 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.simple.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      446 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.SLMQ.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2736 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.SQS.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      533 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.azureservicebus.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      557 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.azurestoragequeues.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1883 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      605 2022-06-19 07:31:49.000000 kombu-5.3.0b3/docs/reference/kombu.transport.confluentkafka.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      459 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.consul.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      451 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.etcd.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      493 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.filesystem.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      741 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.librabbitmq.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      466 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.memory.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      465 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.mongodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      715 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.pyamqp.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      535 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.pyro.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      664 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.qpid.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      576 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.redis.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      543 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1152 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.sqlalchemy.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      772 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.virtual.exchange.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2271 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.virtual.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      484 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.transport.zookeeper.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.amq_manager.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      313 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.collections.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.compat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.debug.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.div.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      311 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.encoding.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      302 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.eventio.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      318 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.functional.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      309 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.imports.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.json.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.limits.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      308 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.objects.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.scheduling.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      289 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.text.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.time.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.url.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/reference/kombu.utils.uuid.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.588143 kombu-5.3.0b3/docs/templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1262 2023-03-09 08:07:52.000000 kombu-5.3.0b3/docs/templates/readme.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.592143 kombu-5.3.0b3/docs/userguide/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7046 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/connections.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7298 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/consumers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1047 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/examples.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6726 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/failover.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      232 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3247 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/introduction.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5458 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/pools.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3635 2021-09-07 04:22:35.000000 kombu-5.3.0b3/docs/userguide/producers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6997 2023-03-09 08:07:52.000000 kombu-5.3.0b3/docs/userguide/serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3929 2022-03-06 04:55:41.000000 kombu-5.3.0b3/docs/userguide/simple.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.592143 kombu-5.3.0b3/examples/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1550 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/complete_receive.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1174 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/complete_send.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.592143 kombu-5.3.0b3/examples/experimental/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      745 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/experimental/async_consume.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      321 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/hello_consumer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      349 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/hello_publisher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      755 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/memory_transport.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.596143 kombu-5.3.0b3/examples/rpc-tut6/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1446 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/rpc-tut6/rpc_client.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1331 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/rpc-tut6/rpc_server.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1225 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_eventlet_receive.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1181 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_eventlet_send.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_receive.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1001 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_send.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.596143 kombu-5.3.0b3/examples/simple_task_queue/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/examples/simple_task_queue/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      994 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_task_queue/client.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      323 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_task_queue/queues.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       92 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_task_queue/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1276 2022-04-17 07:07:11.000000 kombu-5.3.0b3/examples/simple_task_queue/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.552142 kombu-5.3.0b3/extra/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.596143 kombu-5.3.0b3/extra/appveyor/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1844 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/appveyor/run_with_compiler.cmd
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.600143 kombu-5.3.0b3/extra/requirements/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      149 2022-10-19 13:47:58.000000 kombu-5.3.0b3/extra/requirements/default.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       93 2023-03-09 08:07:52.000000 kombu-5.3.0b3/extra/requirements/dev.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      240 2021-11-07 23:46:52.000000 kombu-5.3.0b3/extra/requirements/docs.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.604143 kombu-5.3.0b3/extra/requirements/extras/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       67 2023-03-20 10:18:51.000000 kombu-5.3.0b3/extra/requirements/extras/azureservicebus.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       51 2023-03-20 10:18:51.000000 kombu-5.3.0b3/extra/requirements/extras/azurestoragequeues.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/brotli.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-08-01 07:19:26.000000 kombu-5.3.0b3/extra/requirements/extras/confluentkafka.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b3/extra/requirements/extras/consul.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/couchdb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/etcd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-11-08 00:17:43.000000 kombu-5.3.0b3/extra/requirements/extras/librabbitmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      135 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/lzma.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b3/extra/requirements/extras/mongodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        8 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/msgpack.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-03-09 08:07:52.000000 kombu-5.3.0b3/extra/requirements/extras/pyro.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       35 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/qpid.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2023-03-09 08:07:52.000000 kombu-5.3.0b3/extra/requirements/extras/redis.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/slmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-03-20 10:18:51.000000 kombu-5.3.0b3/extra/requirements/extras/sqlalchemy.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       82 2022-06-19 07:31:49.000000 kombu-5.3.0b3/extra/requirements/extras/sqs.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/yaml.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0b3/extra/requirements/extras/zookeeper.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/extras/zstd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/funtest.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      116 2022-04-17 07:07:11.000000 kombu-5.3.0b3/extra/requirements/pkgutils.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       37 2021-09-07 04:22:35.000000 kombu-5.3.0b3/extra/requirements/test-ci-py2.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      279 2022-06-19 07:31:49.000000 kombu-5.3.0b3/extra/requirements/test-ci-windows.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      292 2022-06-19 07:31:49.000000 kombu-5.3.0b3/extra/requirements/test-ci.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       66 2023-03-09 08:07:52.000000 kombu-5.3.0b3/extra/requirements/test.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.612143 kombu-5.3.0b3/kombu/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3924 2023-03-20 10:58:46.000000 kombu-5.3.0b3/kombu/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4412 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/abstract.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.612143 kombu-5.3.0b3/kombu/asynchronous/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      237 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.612143 kombu-5.3.0b3/kombu/asynchronous/aws/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      475 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8538 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      522 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/ext.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.616143 kombu-5.3.0b3/kombu/asynchronous/aws/sqs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/kombu/asynchronous/aws/sqs/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6808 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/sqs/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      131 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/sqs/ext.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      892 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/sqs/message.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4402 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/aws/sqs/queue.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1773 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/debug.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.616143 kombu-5.3.0b3/kombu/asynchronous/http/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      863 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/http/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9502 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/http/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9752 2022-06-19 07:31:49.000000 kombu-5.3.0b3/kombu/asynchronous/http/curl.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11932 2022-10-19 13:47:58.000000 kombu-5.3.0b3/kombu/asynchronous/hub.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3478 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/semaphore.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6868 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/asynchronous/timer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4799 2022-06-19 07:31:49.000000 kombu-5.3.0b3/kombu/clocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13416 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/common.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6752 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2942 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/compression.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    40449 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32807 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/entity.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2838 2022-06-19 07:31:49.000000 kombu-5.3.0b3/kombu/exceptions.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4066 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4269 2022-06-29 07:05:26.000000 kombu-5.3.0b3/kombu/matcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8059 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/message.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24047 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/messaging.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9667 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/mixins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14789 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/pidbox.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3975 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/pools.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7682 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/resource.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15214 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5302 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/simple.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.624143 kombu-5.3.0b3/kombu/transport/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6215 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/SLMQ.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34240 2022-08-01 07:19:26.000000 kombu-5.3.0b3/kombu/transport/SQS.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3328 2022-06-19 07:31:49.000000 kombu-5.3.0b3/kombu/transport/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15933 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/transport/azureservicebus.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8894 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/transport/azurestoragequeues.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7663 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12106 2022-06-19 07:31:49.000000 kombu-5.3.0b3/kombu/transport/confluentkafka.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9308 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8485 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/etcd.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10416 2022-10-19 13:47:58.000000 kombu-5.3.0b3/kombu/transport/filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6022 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/librabbitmq.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2404 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/memory.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14989 2022-06-19 07:31:49.000000 kombu-5.3.0b3/kombu/transport/mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7752 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/pyamqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/pyro.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    71681 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/qpid.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    48179 2022-10-19 13:47:58.000000 kombu-5.3.0b3/kombu/transport/redis.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.624143 kombu-5.3.0b3/kombu/transport/sqlalchemy/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7440 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/transport/sqlalchemy/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2302 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/transport/sqlalchemy/models.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.628144 kombu-5.3.0b3/kombu/transport/virtual/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      476 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/virtual/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34026 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/virtual/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4838 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/virtual/exchange.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/transport/zookeeper.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.632144 kombu-5.3.0b3/kombu/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      698 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      716 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/amq_manager.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      942 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/collections.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3565 2023-03-12 08:03:46.000000 kombu-5.3.0b3/kombu/utils/compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      908 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/div.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2297 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/encoding.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10159 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/eventio.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10640 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2077 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3609 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/utils/json.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2497 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/limits.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1743 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2914 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/scheduling.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2190 2023-03-09 08:07:52.000000 kombu-5.3.0b3/kombu/utils/text.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      272 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3804 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/url.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      315 2022-04-17 07:07:11.000000 kombu-5.3.0b3/kombu/utils/uuid.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.612143 kombu-5.3.0b3/kombu.egg-info/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1685 2023-03-20 11:02:46.000000 kombu-5.3.0b3/kombu.egg-info/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10459 2023-03-20 11:02:46.000000 kombu-5.3.0b3/kombu.egg-info/SOURCES.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-03-20 11:02:46.000000 kombu-5.3.0b3/kombu.egg-info/dependency_links.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2021-09-07 06:13:24.000000 kombu-5.3.0b3/kombu.egg-info/not-zip-safe
+-rw-rw-r--   0 asif      (1000) asif      (1000)      719 2023-03-20 11:02:46.000000 kombu-5.3.0b3/kombu.egg-info/requires.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-03-20 11:02:46.000000 kombu-5.3.0b3/kombu.egg-info/top_level.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.636144 kombu-5.3.0b3/requirements/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      149 2022-10-19 13:47:58.000000 kombu-5.3.0b3/requirements/default.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       93 2023-03-09 08:07:52.000000 kombu-5.3.0b3/requirements/dev.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      240 2021-11-07 23:46:52.000000 kombu-5.3.0b3/requirements/docs.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.636144 kombu-5.3.0b3/requirements/extras/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       67 2023-03-20 10:18:51.000000 kombu-5.3.0b3/requirements/extras/azureservicebus.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       51 2023-03-20 10:18:51.000000 kombu-5.3.0b3/requirements/extras/azurestoragequeues.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/brotli.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-08-01 07:19:26.000000 kombu-5.3.0b3/requirements/extras/confluentkafka.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b3/requirements/extras/consul.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/couchdb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/etcd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-11-08 00:17:43.000000 kombu-5.3.0b3/requirements/extras/librabbitmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      135 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/lzma.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0b3/requirements/extras/mongodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        8 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/msgpack.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-03-09 08:07:52.000000 kombu-5.3.0b3/requirements/extras/pyro.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       35 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/qpid.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2023-03-09 08:07:52.000000 kombu-5.3.0b3/requirements/extras/redis.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/slmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-03-20 10:18:51.000000 kombu-5.3.0b3/requirements/extras/sqlalchemy.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       82 2022-06-19 07:31:49.000000 kombu-5.3.0b3/requirements/extras/sqs.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/yaml.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0b3/requirements/extras/zookeeper.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/extras/zstd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/funtest.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      116 2022-04-17 07:07:11.000000 kombu-5.3.0b3/requirements/pkgutils.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       37 2021-09-07 04:22:35.000000 kombu-5.3.0b3/requirements/test-ci-py2.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      279 2022-06-19 07:31:49.000000 kombu-5.3.0b3/requirements/test-ci-windows.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      292 2022-06-19 07:31:49.000000 kombu-5.3.0b3/requirements/test-ci.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       66 2023-03-09 08:07:52.000000 kombu-5.3.0b3/requirements/test.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1152 2023-03-20 11:02:46.672144 kombu-5.3.0b3/setup.cfg
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4354 2023-03-09 08:07:52.000000 kombu-5.3.0b3/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.640144 kombu-5.3.0b3/t/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.640144 kombu-5.3.0b3/t/integration/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      120 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/integration/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17367 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/integration/common.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1464 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/integration/test_kafka.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3675 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/integration/test_mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1970 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/integration/test_py_amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4990 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/integration/test_redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6008 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/mocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      283 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/skip.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.648144 kombu-5.3.0b3/t/unit/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.648144 kombu-5.3.0b3/t/unit/asynchronous/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/asynchronous/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.652144 kombu-5.3.0b3/t/unit/asynchronous/aws/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      199 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/case.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.652144 kombu-5.3.0b3/t/unit/asynchronous/aws/sqs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/sqs/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11941 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/sqs/test_connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7140 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/sqs/test_queue.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      318 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/test_aws.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9277 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/aws/test_connection.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.652144 kombu-5.3.0b3/t/unit/asynchronous/http/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/asynchronous/http/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5728 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/http/test_curl.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4221 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/http/test_http.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17161 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/unit/asynchronous/test_hub.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1141 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/test_semaphore.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4247 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/asynchronous/test_timer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9493 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/conftest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2359 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/unit/test_clocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17580 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_common.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11181 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_compression.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32824 2023-03-09 08:07:52.000000 kombu-5.3.0b3/t/unit/test_connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13693 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/unit/test_entity.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      229 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/unit/test_exceptions.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4796 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1133 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_matcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1285 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_message.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24481 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_messaging.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7875 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_mixins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12543 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_pidbox.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7238 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/unit/test_pools.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11162 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6704 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/test_simple.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.660144 kombu-5.3.0b3/t/unit/transport/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/transport/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    33591 2022-08-01 07:19:26.000000 kombu-5.3.0b3/t/unit/transport/test_SQS.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10020 2023-03-09 08:07:52.000000 kombu-5.3.0b3/t/unit/transport/test_azureservicebus.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3455 2023-03-09 08:07:52.000000 kombu-5.3.0b3/t/unit/transport/test_azurestoragequeues.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5617 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2674 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2197 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_etcd.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10594 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/unit/transport/test_filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4891 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_librabbitmq.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5643 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/unit/transport/test_memory.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17045 2022-06-19 07:31:49.000000 kombu-5.3.0b3/t/unit/transport/test_mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7008 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_pyamqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2892 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/unit/transport/test_pyro.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    71045 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_qpid.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    60297 2022-08-01 07:19:26.000000 kombu-5.3.0b3/t/unit/transport/test_redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1538 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_sqlalchemy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1014 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_transport.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1057 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/test_zookeeper.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.664144 kombu-5.3.0b3/t/unit/transport/virtual/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/transport/virtual/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21252 2022-10-19 13:47:58.000000 kombu-5.3.0b3/t/unit/transport/virtual/test_base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5530 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/transport/virtual/test_exchange.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-20 11:02:46.668144 kombu-5.3.0b3/t/unit/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0b3/t/unit/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1281 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_amq_manager.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2806 2023-03-20 10:18:52.000000 kombu-5.3.0b3/t/unit/utils/test_compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1630 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_div.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2962 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_encoding.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8800 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      967 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2772 2023-03-09 08:07:52.000000 kombu-5.3.0b3/t/unit/utils/test_json.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1064 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2769 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_scheduling.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      459 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2964 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_url.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      609 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_utils.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      289 2022-04-17 07:07:11.000000 kombu-5.3.0b3/t/unit/utils/test_uuid.py
```

### Comparing `kombu-5.3.0b2/AUTHORS` & `kombu-5.3.0b3/AUTHORS`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/LICENSE` & `kombu-5.3.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/MANIFEST.in` & `kombu-5.3.0b3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/PKG-INFO` & `kombu-5.3.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: kombu
-Version: 5.3.0b2
+Version: 5.3.0b3
 Summary: Messaging library for Python.
 Home-page: https://kombu.readthedocs.io
 Author: Ask Solem
 Author-email: auvipy@gmail.com, ask@celeryproject.org
-License: BSD
+License: BSD-3-Clause
 Project-URL: Source, https://github.com/celery/kombu
 Keywords: messaging message amqp rabbitmq redis actor producer consumer
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `kombu-5.3.0b2/README.rst` & `kombu-5.3.0b3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ========================================
  kombu - Messaging library for Python
 ========================================
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp| |downloads|
 
-:Version: 5.3.0b2
+:Version: 5.3.0b3
 :Documentation: https://kombu.readthedocs.io/
 :Download: https://pypi.org/project/kombu/
 :Source: https://github.com/celery/kombu/
 :Keywords: messaging, amqp, rabbitmq, redis, mongodb, python, queue
 
 About
 =====
@@ -324,20 +324,20 @@
 License
 =======
 
 This software is licensed under the `New BSD License`. See the `LICENSE`
 file in the top distribution directory for the full license text.
 
 
-.. |build-status| image:: https://api.travis-ci.com/celery/kombu.png?branch=master
+.. |build-status| image:: https://github.com/celery/kombu/actions/workflows/ci.yaml/badge.svg
     :alt: Build status
-    :target: https://travis-ci.com/celery/kombu
+    :target: https://github.com/celery/kombu/actions/workflows/ci.yml
 
-.. |coverage| image:: https://codecov.io/github/celery/kombu/coverage.svg?branch=master
-    :target: https://codecov.io/github/celery/kombu?branch=master
+.. |coverage| image:: https://codecov.io/github/celery/kombu/coverage.svg?branch=main
+    :target: https://codecov.io/github/celery/kombu?branch=main
 
 .. |license| image:: https://img.shields.io/pypi/l/kombu.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/kombu.svg
     :alt: Kombu can be installed via wheel
```

### Comparing `kombu-5.3.0b2/THANKS` & `kombu-5.3.0b3/THANKS`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/Makefile` & `kombu-5.3.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/_templates/sidebardonations.html` & `kombu-5.3.0b3/docs/_templates/sidebardonations.html`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/conf.py` & `kombu-5.3.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/images/favicon.ico` & `kombu-5.3.0b3/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/images/kombu.jpg` & `kombu-5.3.0b3/docs/images/kombu.jpg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/images/kombusmall.jpg` & `kombu-5.3.0b3/docs/images/kombusmall.jpg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/includes/introduction.txt` & `kombu-5.3.0b3/docs/includes/introduction.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.3.0b2
+:Version: 5.3.0b3
 :Web: https://kombu.readthedocs.io/
 :Download: https://pypi.org/project/kombu/
 :Source: https://github.com/celery/kombu/
 :Keywords: messaging, amqp, rabbitmq, redis, mongodb, python, queue
 
 About
 =====
```

### Comparing `kombu-5.3.0b2/docs/includes/resources.txt` & `kombu-5.3.0b3/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/make.bat` & `kombu-5.3.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/index.rst` & `kombu-5.3.0b3/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.compat.rst` & `kombu-5.3.0b3/docs/reference/kombu.compat.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.compression.rst` & `kombu-5.3.0b3/docs/reference/kombu.compression.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.connection.rst` & `kombu-5.3.0b3/docs/reference/kombu.connection.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.pidbox.rst` & `kombu-5.3.0b3/docs/reference/kombu.pidbox.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.rst` & `kombu-5.3.0b3/docs/reference/kombu.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.serialization.rst` & `kombu-5.3.0b3/docs/reference/kombu.serialization.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.simple.rst` & `kombu-5.3.0b3/docs/reference/kombu.simple.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.SQS.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.SQS.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.azureservicebus.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.azureservicebus.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.azurestoragequeues.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.azurestoragequeues.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.base.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.base.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.confluentkafka.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.confluentkafka.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.librabbitmq.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.librabbitmq.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.pyamqp.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.pyamqp.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.pyro.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.pyro.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.qpid.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.qpid.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.redis.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.redis.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.sqlalchemy.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.virtual.exchange.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.virtual.exchange.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/reference/kombu.transport.virtual.rst` & `kombu-5.3.0b3/docs/reference/kombu.transport.virtual.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/templates/readme.txt` & `kombu-5.3.0b3/docs/templates/readme.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 .. include:: ../includes/introduction.txt
 
 .. include:: ../includes/installation.txt
 
 .. include:: ../includes/resources.txt
 
-.. |build-status| image:: https://secure.travis-ci.org/celery/kombu.png?branch=master
+.. |build-status| image:: https://github.com/celery/kombu/actions/workflows/ci.yaml/badge.svg
     :alt: Build status
-    :target: https://travis-ci.org/celery/kombu
+    :target: https://github.com/celery/kombu/actions/workflows/ci.yml
 
-.. |coverage| image:: https://codecov.io/github/celery/kombu/coverage.svg?branch=master
-    :target: https://codecov.io/github/celery/kombu?branch=master
+.. |coverage| image:: https://codecov.io/github/celery/kombu/coverage.svg?branch=main
+    :target: https://codecov.io/github/celery/kombu?branch=main
 
 .. |license| image:: https://img.shields.io/pypi/l/kombu.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/kombu.svg
     :alt: Kombu can be installed via wheel
```

### Comparing `kombu-5.3.0b2/docs/userguide/connections.rst` & `kombu-5.3.0b3/docs/userguide/connections.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/consumers.rst` & `kombu-5.3.0b3/docs/userguide/consumers.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/examples.rst` & `kombu-5.3.0b3/docs/userguide/examples.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/failover.rst` & `kombu-5.3.0b3/docs/userguide/failover.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/introduction.rst` & `kombu-5.3.0b3/docs/userguide/introduction.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/pools.rst` & `kombu-5.3.0b3/docs/userguide/pools.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/producers.rst` & `kombu-5.3.0b3/docs/userguide/producers.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/docs/userguide/serialization.rst` & `kombu-5.3.0b3/docs/userguide/serialization.rst`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,31 @@
     encoding which supports native binary types. This will only happen
     if the bytes object can't be decoded into utf8.
 
     However, if your data fits inside the above constraints and
     you need cross-language support, the default setting of `JSON`
     is probably your best choice.
 
+    If you need support for custom types, you can write serialize/deserialize
+    functions and register them as follows:
+
+    .. code-block:: python
+
+        from kombu.utils.json import register_type
+        from django.db.models import Model
+        from django.apps import apps
+
+        # Allow serialization of django models:
+        register_type(
+            Model,
+            "model",
+            lambda o: [o._meta.label, o.pk],
+            lambda o: apps.get_model(o[0]).objects.get(pk=o[1]),
+        )
+
 `pickle` -- If you have no desire to support any language other than
     Python, then using the `pickle` encoding will gain you
     the support of all built-in Python data types (except class instances),
     smaller messages when sending binary files, and a slight speedup
     over `JSON` processing.
 
     .. admonition:: Pickle and Security
```

### Comparing `kombu-5.3.0b2/docs/userguide/simple.rst` & `kombu-5.3.0b3/docs/userguide/simple.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/complete_receive.py` & `kombu-5.3.0b3/examples/complete_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/complete_send.py` & `kombu-5.3.0b3/examples/complete_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/experimental/async_consume.py` & `kombu-5.3.0b3/examples/experimental/async_consume.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/memory_transport.py` & `kombu-5.3.0b3/examples/memory_transport.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/rpc-tut6/rpc_client.py` & `kombu-5.3.0b3/examples/rpc-tut6/rpc_client.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/rpc-tut6/rpc_server.py` & `kombu-5.3.0b3/examples/rpc-tut6/rpc_server.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/simple_eventlet_receive.py` & `kombu-5.3.0b3/examples/simple_eventlet_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/simple_eventlet_send.py` & `kombu-5.3.0b3/examples/simple_eventlet_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/simple_receive.py` & `kombu-5.3.0b3/examples/simple_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/simple_send.py` & `kombu-5.3.0b3/examples/simple_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/simple_task_queue/client.py` & `kombu-5.3.0b3/examples/simple_task_queue/client.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/examples/simple_task_queue/worker.py` & `kombu-5.3.0b3/examples/simple_task_queue/worker.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/extra/appveyor/run_with_compiler.cmd` & `kombu-5.3.0b3/extra/appveyor/run_with_compiler.cmd`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/__init__.py` & `kombu-5.3.0b3/kombu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 import re
 import sys
 from collections import namedtuple
 from typing import Any, cast
 
-__version__ = '5.3.0b2'
+__version__ = '5.3.0b3'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com, ask@celeryproject.org'
 __homepage__ = 'https://kombu.readthedocs.io'
 __docformat__ = 'restructuredtext en'
 
 # -eof meta-
```

### Comparing `kombu-5.3.0b2/kombu/abstract.py` & `kombu-5.3.0b3/kombu/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
 from .connection import maybe_channel
 from .exceptions import NotBoundError
 from .utils.functional import ChannelPromise
 
 if TYPE_CHECKING:
+    from kombu.connection import Connection
     from kombu.transport.virtual import Channel
 
 
 __all__ = ('Object', 'MaybeChannelBound')
 
 _T = TypeVar("_T")
 _ObjectType = TypeVar("_ObjectType", bound="Object")
@@ -76,27 +77,27 @@
     _channel: Channel | None = None
     _is_bound = False
 
     #: Defines whether maybe_declare can skip declaring this entity twice.
     can_cache_declaration = False
 
     def __call__(
-        self: _MaybeChannelBoundType, channel: Channel
+        self: _MaybeChannelBoundType, channel: (Channel | Connection)
     ) -> _MaybeChannelBoundType:
         """`self(channel) -> self.bind(channel)`."""
         return self.bind(channel)
 
     def bind(
-        self: _MaybeChannelBoundType, channel: Channel
+        self: _MaybeChannelBoundType, channel: (Channel | Connection)
     ) -> _MaybeChannelBoundType:
         """Create copy of the instance that is bound to a channel."""
         return copy(self).maybe_bind(channel)
 
     def maybe_bind(
-        self: _MaybeChannelBoundType, channel: Channel
+        self: _MaybeChannelBoundType, channel: (Channel | Connection)
     ) -> _MaybeChannelBoundType:
         """Bind instance to channel if not already bound."""
         if not self.is_bound and channel:
             self._channel = maybe_channel(channel)
             self.when_bound()
             self._is_bound = True
         return self
```

### Comparing `kombu-5.3.0b2/kombu/asynchronous/aws/connection.py` & `kombu-5.3.0b3/kombu/asynchronous/aws/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/aws/ext.py` & `kombu-5.3.0b3/kombu/asynchronous/aws/ext.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/aws/sqs/connection.py` & `kombu-5.3.0b3/kombu/asynchronous/aws/sqs/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/aws/sqs/message.py` & `kombu-5.3.0b3/kombu/asynchronous/aws/sqs/message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/aws/sqs/queue.py` & `kombu-5.3.0b3/kombu/asynchronous/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/debug.py` & `kombu-5.3.0b3/kombu/asynchronous/debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/http/__init__.py` & `kombu-5.3.0b3/kombu/asynchronous/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/http/base.py` & `kombu-5.3.0b3/kombu/asynchronous/http/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/http/curl.py` & `kombu-5.3.0b3/kombu/asynchronous/http/curl.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/hub.py` & `kombu-5.3.0b3/kombu/asynchronous/hub.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/semaphore.py` & `kombu-5.3.0b3/kombu/asynchronous/semaphore.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/asynchronous/timer.py` & `kombu-5.3.0b3/kombu/asynchronous/timer.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/clocks.py` & `kombu-5.3.0b3/kombu/clocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/common.py` & `kombu-5.3.0b3/kombu/common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/compat.py` & `kombu-5.3.0b3/kombu/compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/compression.py` & `kombu-5.3.0b3/kombu/compression.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/connection.py` & `kombu-5.3.0b3/kombu/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,15 @@
         """Revive connection after connection re-established."""
         if self._default_channel and new_channel is not self._default_channel:
             self.maybe_close_channel(self._default_channel)
             self._default_channel = None
 
     def ensure(self, obj, fun, errback=None, max_retries=None,
                interval_start=1, interval_step=1, interval_max=1,
-               on_revive=None):
+               on_revive=None, retry_errors=None):
         """Ensure operation completes.
 
         Regardless of any channel/connection errors occurring.
 
         Retries by establishing the connection, and reapplying
         the function.
 
@@ -507,39 +507,56 @@
                 sleeping for.
             interval_step (float): How many seconds added to the interval
                 for each retry.
             interval_max (float): Maximum number of seconds to sleep between
                 each retry.
             on_revive (Callable): Optional callback called whenever
                 revival completes successfully
+            retry_errors (tuple): Optional list of errors to retry on
+                regardless of the connection state. Must provide max_retries
+                if this is specified.
 
         Examples:
             >>> from kombu import Connection, Producer
             >>> conn = Connection('amqp://')
             >>> producer = Producer(conn)
 
             >>> def errback(exc, interval):
             ...     logger.error('Error: %r', exc, exc_info=1)
             ...     logger.info('Retry in %s seconds.', interval)
 
             >>> publish = conn.ensure(producer, producer.publish,
             ...                       errback=errback, max_retries=3)
             >>> publish({'hello': 'world'}, routing_key='dest')
         """
+        if retry_errors is None:
+            retry_errors = tuple()
+        elif max_retries is None:
+            # If the retry_errors is specified, but max_retries is not,
+            # this could lead into an infinite loop potentially.
+            raise ValueError(
+                "max_retries must be specified if retry_errors is specified"
+            )
+
         def _ensured(*args, **kwargs):
             got_connection = 0
             conn_errors = self.recoverable_connection_errors
             chan_errors = self.recoverable_channel_errors
             has_modern_errors = hasattr(
                 self.transport, 'recoverable_connection_errors',
             )
             with self._reraise_as_library_errors():
                 for retries in count(0):  # for infinity
                     try:
                         return fun(*args, **kwargs)
+                    except retry_errors as exc:
+                        if max_retries is not None and retries >= max_retries:
+                            raise
+                        self._debug('ensure retry policy error: %r',
+                                    exc, exc_info=1)
                     except conn_errors as exc:
                         if got_connection and not has_modern_errors:
                             # transport can not distinguish between
                             # recoverable/irrecoverable errors, so we propagate
                             # the error if it persists after a new connection
                             # was successfully established.
                             raise
```

### Comparing `kombu-5.3.0b2/kombu/entity.py` & `kombu-5.3.0b3/kombu/entity.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/exceptions.py` & `kombu-5.3.0b3/kombu/exceptions.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/log.py` & `kombu-5.3.0b3/kombu/log.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/matcher.py` & `kombu-5.3.0b3/kombu/matcher.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/message.py` & `kombu-5.3.0b3/kombu/message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/messaging.py` & `kombu-5.3.0b3/kombu/messaging.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/mixins.py` & `kombu-5.3.0b3/kombu/mixins.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/pidbox.py` & `kombu-5.3.0b3/kombu/pidbox.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/pools.py` & `kombu-5.3.0b3/kombu/pools.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/resource.py` & `kombu-5.3.0b3/kombu/resource.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/serialization.py` & `kombu-5.3.0b3/kombu/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -380,26 +380,14 @@
 register_pickle()
 register_yaml()
 register_msgpack()
 
 # Default serializer is 'json'
 registry._set_default_serializer('json')
 
-
-_setupfuns = {
-    'json': register_json,
-    'pickle': register_pickle,
-    'yaml': register_yaml,
-    'msgpack': register_msgpack,
-    'application/json': register_json,
-    'application/x-yaml': register_yaml,
-    'application/x-python-serialize': register_pickle,
-    'application/x-msgpack': register_msgpack,
-}
-
 NOTSET = object()
 
 
 def enable_insecure_serializers(choices=NOTSET):
     """Enable serializers that are considered to be unsafe.
 
     Note:
```

### Comparing `kombu-5.3.0b2/kombu/simple.py` & `kombu-5.3.0b3/kombu/simple.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/SLMQ.py` & `kombu-5.3.0b3/kombu/transport/SLMQ.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/SQS.py` & `kombu-5.3.0b3/kombu/transport/SQS.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/__init__.py` & `kombu-5.3.0b3/kombu/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/azureservicebus.py` & `kombu-5.3.0b3/kombu/transport/azureservicebus.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,44 +83,42 @@
 
 class SendReceive:
     """Container for Sender and Receiver."""
 
     def __init__(self,
                  receiver: ServiceBusReceiver | None = None,
                  sender: ServiceBusSender | None = None):
-        self.receiver = receiver  # type: ServiceBusReceiver
-        self.sender = sender  # type: ServiceBusSender
+        self.receiver: ServiceBusReceiver = receiver
+        self.sender: ServiceBusSender = sender
 
     def close(self) -> None:
         if self.receiver:
             self.receiver.close()
             self.receiver = None
         if self.sender:
             self.sender.close()
             self.sender = None
 
 
 class Channel(virtual.Channel):
     """Azure Service Bus channel."""
 
-    default_wait_time_seconds = 5  # in seconds
-    default_peek_lock_seconds = 60  # in seconds (default 60, max 300)
+    default_wait_time_seconds: int = 5  # in seconds
+    default_peek_lock_seconds: int = 60  # in seconds (default 60, max 300)
     # in seconds (is the default from service bus repo)
-    default_uamqp_keep_alive_interval = 30
+    default_uamqp_keep_alive_interval: int = 30
     # number of retries (is the default from service bus repo)
-    default_retry_total = 3
+    default_retry_total: int = 3
     # exponential backoff factor (is the default from service bus repo)
-    default_retry_backoff_factor = 0.8
+    default_retry_backoff_factor: float = 0.8
     # Max time to backoff (is the default from service bus repo)
-    default_retry_backoff_max = 120
-    domain_format = 'kombu%(vhost)s'
-    _queue_service = None  # type: ServiceBusClient
-    _queue_mgmt_service = None  # type: ServiceBusAdministrationClient
-    _queue_cache = {}  # type: Dict[str, SendReceive]
-    _noack_queues = set()  # type: Set[str]
+    default_retry_backoff_max: int = 120
+    domain_format: str = 'kombu%(vhost)s'
+    _queue_cache: Dict[str, SendReceive] = {}
+    _noack_queues: Set[str] = set()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._namespace = None
         self._policy = None
         self._sas_key = None
@@ -225,15 +223,15 @@
                 pass
             return self._add_queue_to_cache(queue)
 
     def _delete(self, queue: str, *args, **kwargs) -> None:
         """Delete queue by name."""
         queue = self.entity_name(self.queue_name_prefix + queue)
 
-        self._queue_mgmt_service.delete_queue(queue)
+        self.queue_mgmt_service.delete_queue(queue)
         send_receive_obj = self._queue_cache.pop(queue, None)
         if send_receive_obj:
             send_receive_obj.close()
 
     def _put(self, queue: str, message, **kwargs) -> None:
         """Put message onto queue."""
         queue = self.entity_name(self.queue_name_prefix + queue)
@@ -296,15 +294,15 @@
     def _size(self, queue: str) -> int:
         """Return the number of messages in a queue."""
         queue = self.entity_name(self.queue_name_prefix + queue)
         props = self.queue_mgmt_service.get_queue_runtime_properties(queue)
 
         return props.total_message_count
 
-    def _purge(self, queue):
+    def _purge(self, queue) -> int:
         """Delete all current messages in a queue."""
         # Azure doesn't provide a purge api yet
         n = 0
         max_purge_count = 10
         queue = self.entity_name(self.queue_name_prefix + queue)
 
         # By default all the receivers will be in PEEK_LOCK receive mode
@@ -335,32 +333,27 @@
             for queue_obj in self._queue_cache.values():
                 queue_obj.close()
             self._queue_cache.clear()
 
             if self.connection is not None:
                 self.connection.close_channel(self)
 
-    @property
+    @cached_property
     def queue_service(self) -> ServiceBusClient:
-        if self._queue_service is None:
-            self._queue_service = ServiceBusClient.from_connection_string(
-                self._connection_string,
-                retry_total=self.retry_total,
-                retry_backoff_factor=self.retry_backoff_factor,
-                retry_backoff_max=self.retry_backoff_max
-            )
-        return self._queue_service
+        return ServiceBusClient.from_connection_string(
+            self._connection_string,
+            retry_total=self.retry_total,
+            retry_backoff_factor=self.retry_backoff_factor,
+            retry_backoff_max=self.retry_backoff_max
+        )
 
-    @property
+    @cached_property
     def queue_mgmt_service(self) -> ServiceBusAdministrationClient:
-        if self._queue_mgmt_service is None:
-            self._queue_mgmt_service = \
-                ServiceBusAdministrationClient.from_connection_string(
+        return ServiceBusAdministrationClient.from_connection_string(
                     self._connection_string)
-        return self._queue_mgmt_service
 
     @property
     def conninfo(self):
         return self.connection.client
 
     @property
     def transport_options(self):
```

### Comparing `kombu-5.3.0b2/kombu/transport/azurestoragequeues.py` & `kombu-5.3.0b3/kombu/transport/azurestoragequeues.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,63 +11,90 @@
 * Supports Fanout: *Unreviewed*
 * Supports Priority: *Unreviewed*
 * Supports TTL: *Unreviewed*
 
 Connection String
 =================
 
-Connection string has the following format:
+Connection string has the following formats:
 
 .. code-block::
 
-    azurestoragequeues://STORAGE_ACCOUNT_ACCESS_KEY@STORAGE_ACCOUNT_URL
-    azurestoragequeues://SAS_TOKEN@STORAGE_ACCOUNT_URL
+    azurestoragequeues://<STORAGE_ACCOUNT_ACCESS_KEY>@<STORAGE_ACCOUNT_URL>
+    azurestoragequeues://<SAS_TOKEN>@<STORAGE_ACCOUNT_URL>
+    azurestoragequeues://DefaultAzureCredential@<STORAGE_ACCOUNT_URL>
+    azurestoragequeues://ManagedIdentityCredential@<STORAGE_ACCOUNT_URL>
+
+Note that if the access key for the storage account contains a forward slash
+(``/``), it will have to be regenerated before it can be used in the connection
+URL.
 
-Note that if the access key for the storage account contains a slash, it will
-have to be regenerated before it can be used in the connection URL.
+.. code-block::
+
+    azurestoragequeues://DefaultAzureCredential@<STORAGE_ACCOUNT_URL>
+    azurestoragequeues://ManagedIdentityCredential@<STORAGE_ACCOUNT_URL>
+
+If you wish to use an `Azure Managed Identity` you may use the
+``DefaultAzureCredential`` format of the connection string which will use
+``DefaultAzureCredential`` class in the azure-identity package. You may want to
+read the `azure-identity documentation` for more information on how the
+``DefaultAzureCredential`` works.
+
+.. _azure-identity documentation:
+https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python
+.. _Azure Managed Identity:
+https://learn.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/overview
 
 Transport Options
 =================
 
 * ``queue_name_prefix``
 """
 
 from __future__ import annotations
 
 import string
 from queue import Empty
+from typing import Any, Optional
 
 from azure.core.exceptions import ResourceExistsError
 
 from kombu.utils.encoding import safe_str
 from kombu.utils.json import dumps, loads
 from kombu.utils.objects import cached_property
 
 from . import virtual
 
 try:
     from azure.storage.queue import QueueServiceClient
 except ImportError:  # pragma: no cover
     QueueServiceClient = None
 
+try:
+    from azure.identity import (DefaultAzureCredential,
+                                ManagedIdentityCredential)
+except ImportError:
+    DefaultAzureCredential = None
+    ManagedIdentityCredential = None
+
 # Azure storage queues allow only alphanumeric and dashes
 # so, replace everything with a dash
 CHARS_REPLACE_TABLE = {
     ord(c): 0x2d for c in string.punctuation
 }
 
 
 class Channel(virtual.Channel):
     """Azure Storage Queues channel."""
 
-    domain_format = 'kombu%(vhost)s'
-    _queue_service = None
-    _queue_name_cache = {}
-    no_ack = True
-    _noack_queues = set()
+    domain_format: str = 'kombu%(vhost)s'
+    _queue_service: Optional[QueueServiceClient] = None
+    _queue_name_cache: dict[Any, Any] = {}
+    no_ack: bool = True
+    _noack_queues: set[Any] = set()
 
     def __init__(self, *args, **kwargs):
         if QueueServiceClient is None:
             raise ImportError('Azure Storage Queues transport requires the '
                               'azure-storage-queue library')
 
         super().__init__(*args, **kwargs)
@@ -82,15 +109,15 @@
     def basic_consume(self, queue, no_ack, *args, **kwargs):
         if no_ack:
             self._noack_queues.add(queue)
 
         return super().basic_consume(queue, no_ack,
                                      *args, **kwargs)
 
-    def entity_name(self, name, table=CHARS_REPLACE_TABLE):
+    def entity_name(self, name, table=CHARS_REPLACE_TABLE) -> str:
         """Format AMQP queue name into a valid Azure Storage Queue name."""
         return str(safe_str(name)).translate(table)
 
     def _ensure_queue(self, queue):
         """Ensure a queue exists."""
         queue = self.entity_name(self.queue_name_prefix + queue)
         try:
@@ -143,15 +170,15 @@
         """Delete all current messages in a queue."""
         q = self._ensure_queue(queue)
         n = self._size(q.queue_name)
         q.clear_messages()
         return n
 
     @property
-    def queue_service(self):
+    def queue_service(self) -> QueueServiceClient:
         if self._queue_service is None:
             self._queue_service = QueueServiceClient(
                 account_url=self._url, credential=self._credential
             )
 
         return self._queue_service
 
@@ -160,59 +187,77 @@
         return self.connection.client
 
     @property
     def transport_options(self):
         return self.connection.client.transport_options
 
     @cached_property
-    def queue_name_prefix(self):
+    def queue_name_prefix(self) -> str:
         return self.transport_options.get('queue_name_prefix', '')
 
 
 class Transport(virtual.Transport):
     """Azure Storage Queues transport."""
 
     Channel = Channel
 
-    polling_interval = 1
-    default_port = None
-    can_parse_url = True
+    polling_interval: int = 1
+    default_port: Optional[int] = None
+    can_parse_url: bool = True
 
     @staticmethod
     def parse_uri(uri: str) -> tuple[str | dict, str]:
         # URL like:
-        #  azurestoragequeues://STORAGE_ACCOUNT_ACCESS_KEY@STORAGE_ACCOUNT_URL
-        #  azurestoragequeues://SAS_TOKEN@STORAGE_ACCOUNT_URL
+        #  azurestoragequeues://<STORAGE_ACCOUNT_ACCESS_KEY>@<STORAGE_ACCOUNT_URL>
+        #  azurestoragequeues://<SAS_TOKEN>@<STORAGE_ACCOUNT_URL>
+        #  azurestoragequeues://DefaultAzureCredential@<STORAGE_ACCOUNT_URL>
+        #  azurestoragequeues://ManagedIdentityCredential@<STORAGE_ACCOUNT_URL>
 
         # urllib parse does not work as the sas key could contain a slash
         # e.g.: azurestoragequeues://some/key@someurl
 
         try:
             # > 'some/key@url'
             uri = uri.replace('azurestoragequeues://', '')
             # > 'some/key',  'url'
             credential, url = uri.rsplit('@', 1)
 
-            # parse credential as a dict if Azurite is being used
-            if "devstoreaccount1" in url and ".core.windows.net" not in url:
+            if "DefaultAzureCredential".lower() == credential.lower():
+                if DefaultAzureCredential is None:
+                    raise ImportError('Azure Storage Queues transport with a '
+                                      'DefaultAzureCredential requires the '
+                                      'azure-identity library')
+                credential = DefaultAzureCredential()
+            elif "ManagedIdentityCredential".lower() == credential.lower():
+                if ManagedIdentityCredential is None:
+                    raise ImportError('Azure Storage Queues transport with a '
+                                      'ManagedIdentityCredential requires the '
+                                      'azure-identity library')
+                credential = ManagedIdentityCredential()
+            elif "devstoreaccount1" in url and ".core.windows.net" not in url:
+                # parse credential as a dict if Azurite is being used
                 credential = {
                     "account_name": "devstoreaccount1",
                     "account_key": credential,
                 }
 
             # Validate parameters
             assert all([credential, url])
         except Exception:
             raise ValueError(
                 'Need a URI like '
-                'azurestoragequeues://{SAS or access key}@{URL}'
+                'azurestoragequeues://{SAS or access key}@{URL}, '
+                'azurestoragequeues://DefaultAzureCredential@{URL}, '
+                ', or '
+                'azurestoragequeues://ManagedIdentityCredential@{URL}'
             )
 
         return credential, url
 
     @classmethod
-    def as_uri(cls, uri: str, include_password=False, mask='**') -> str:
+    def as_uri(
+        cls, uri: str, include_password: bool = False, mask: str = "**"
+    ) -> str:
         credential, url = cls.parse_uri(uri)
-        return 'azurestoragequeues://{}@{}'.format(
-            credential if include_password else mask,
-            url
+        return "azurestoragequeues://{}@{}".format(
+            credential if include_password else mask, url
         )
```

### Comparing `kombu-5.3.0b2/kombu/transport/base.py` & `kombu-5.3.0b3/kombu/transport/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/confluentkafka.py` & `kombu-5.3.0b3/kombu/transport/confluentkafka.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/consul.py` & `kombu-5.3.0b3/kombu/transport/consul.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/etcd.py` & `kombu-5.3.0b3/kombu/transport/etcd.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/filesystem.py` & `kombu-5.3.0b3/kombu/transport/filesystem.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/librabbitmq.py` & `kombu-5.3.0b3/kombu/transport/librabbitmq.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/memory.py` & `kombu-5.3.0b3/kombu/transport/memory.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/mongodb.py` & `kombu-5.3.0b3/kombu/transport/mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/pyamqp.py` & `kombu-5.3.0b3/kombu/transport/pyamqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/pyro.py` & `kombu-5.3.0b3/kombu/transport/pyro.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/qpid.py` & `kombu-5.3.0b3/kombu/transport/qpid.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/redis.py` & `kombu-5.3.0b3/kombu/transport/redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/sqlalchemy/__init__.py` & `kombu-5.3.0b3/kombu/transport/sqlalchemy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 """
 from __future__ import annotations
 
 import threading
 from json import dumps, loads
 from queue import Empty
 
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, text
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import sessionmaker
 
 from kombu.transport import virtual
 from kombu.utils import cached_property
 from kombu.utils.encoding import bytes_to_str
 
@@ -165,15 +165,15 @@
             self.session.commit()
         except OperationalError:
             self.session.rollback()
 
     def _get(self, queue):
         obj = self._get_or_create(queue)
         if self.session.bind.name == 'sqlite':
-            self.session.execute('BEGIN IMMEDIATE TRANSACTION')
+            self.session.execute(text('BEGIN IMMEDIATE TRANSACTION'))
         try:
             msg = self.session.query(self.message_cls) \
                 .with_for_update() \
                 .filter(self.message_cls.queue_id == obj.id) \
                 .filter(self.message_cls.visible != False) \
                 .order_by(self.message_cls.sent_at) \
                 .order_by(self.message_cls.id) \
```

### Comparing `kombu-5.3.0b2/kombu/transport/sqlalchemy/models.py` & `kombu-5.3.0b3/kombu/transport/sqlalchemy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import datetime
 
 from sqlalchemy import (Boolean, Column, DateTime, ForeignKey, Index, Integer,
                         Sequence, SmallInteger, String, Text)
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import MetaData
 
 try:
     from sqlalchemy.orm import declarative_base, declared_attr
 except ImportError:
     # TODO: Remove this once we drop support for SQLAlchemy < 1.4.
     from sqlalchemy.ext.declarative import declarative_base, declared_attr
@@ -33,15 +33,15 @@
         self.name = name
 
     def __str__(self):
         return f'<Queue({self.name})>'
 
     @declared_attr
     def messages(cls):
-        return relation('Message', backref='queue', lazy='noload')
+        return relationship('Message', backref='queue', lazy='noload')
 
 
 class Message:
     """The message class."""
 
     __table_args__ = (
         Index('ix_kombu_message_timestamp_id', 'timestamp', 'id'),
```

### Comparing `kombu-5.3.0b2/kombu/transport/virtual/base.py` & `kombu-5.3.0b3/kombu/transport/virtual/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/virtual/exchange.py` & `kombu-5.3.0b3/kombu/transport/virtual/exchange.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/transport/zookeeper.py` & `kombu-5.3.0b3/kombu/transport/zookeeper.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/__init__.py` & `kombu-5.3.0b3/kombu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/amq_manager.py` & `kombu-5.3.0b3/kombu/utils/amq_manager.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/collections.py` & `kombu-5.3.0b3/kombu/utils/collections.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/compat.py` & `kombu-5.3.0b3/kombu/utils/compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/debug.py` & `kombu-5.3.0b3/kombu/utils/debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/div.py` & `kombu-5.3.0b3/kombu/utils/div.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/encoding.py` & `kombu-5.3.0b3/kombu/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/eventio.py` & `kombu-5.3.0b3/kombu/utils/eventio.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/functional.py` & `kombu-5.3.0b3/kombu/utils/functional.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/imports.py` & `kombu-5.3.0b3/kombu/utils/imports.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/limits.py` & `kombu-5.3.0b3/kombu/utils/limits.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/objects.py` & `kombu-5.3.0b3/kombu/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/scheduling.py` & `kombu-5.3.0b3/kombu/utils/scheduling.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu/utils/text.py` & `kombu-5.3.0b3/kombu/utils/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Text Utilities."""
 # flake8: noqa
 
 
 from __future__ import annotations
 
 from difflib import SequenceMatcher
-from typing import Iterable, Iterator, Optional, Tuple, Union
+from typing import Iterable, Iterator
 
 from kombu import version_info_t
 
 
 def escape_regex(p, white=''):
     # type: (str, str) -> str
     """Escape string for use within a regular expression."""
```

### Comparing `kombu-5.3.0b2/kombu/utils/url.py` & `kombu-5.3.0b3/kombu/utils/url.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/kombu.egg-info/PKG-INFO` & `kombu-5.3.0b3/kombu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: kombu
-Version: 5.3.0b2
+Version: 5.3.0b3
 Summary: Messaging library for Python.
 Home-page: https://kombu.readthedocs.io
 Author: Ask Solem
 Author-email: auvipy@gmail.com, ask@celeryproject.org
-License: BSD
+License: BSD-3-Clause
 Project-URL: Source, https://github.com/celery/kombu
 Keywords: messaging message amqp rabbitmq redis actor producer consumer
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `kombu-5.3.0b2/kombu.egg-info/SOURCES.txt` & `kombu-5.3.0b3/kombu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/setup.cfg` & `kombu-5.3.0b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/setup.py` & `kombu-5.3.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     author_email=meta['contact'],
     url=meta['homepage'],
     project_urls={
         'Source': 'https://github.com/celery/kombu'
     },
     platforms=['any'],
     zip_safe=False,
-    license='BSD',
+    license='BSD-3-Clause',
     cmdclass={'test': pytest},
     python_requires=">=3.7",
     install_requires=reqs('default.txt'),
     tests_require=reqs('test.txt'),
     extras_require={
         'msgpack': extras('msgpack.txt'),
         'yaml': extras('yaml.txt'),
```

### Comparing `kombu-5.3.0b2/t/integration/common.py` & `kombu-5.3.0b3/t/integration/common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/integration/test_kafka.py` & `kombu-5.3.0b3/t/integration/test_kafka.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/integration/test_mongodb.py` & `kombu-5.3.0b3/t/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/integration/test_py_amqp.py` & `kombu-5.3.0b3/t/integration/test_py_amqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/integration/test_redis.py` & `kombu-5.3.0b3/t/integration/test_redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/mocks.py` & `kombu-5.3.0b3/t/mocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/aws/sqs/test_connection.py` & `kombu-5.3.0b3/t/unit/asynchronous/aws/sqs/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/aws/sqs/test_queue.py` & `kombu-5.3.0b3/t/unit/asynchronous/aws/sqs/test_queue.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/aws/test_connection.py` & `kombu-5.3.0b3/t/unit/asynchronous/aws/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/http/test_curl.py` & `kombu-5.3.0b3/t/unit/asynchronous/http/test_curl.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/http/test_http.py` & `kombu-5.3.0b3/t/unit/asynchronous/http/test_http.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/test_hub.py` & `kombu-5.3.0b3/t/unit/asynchronous/test_hub.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/test_semaphore.py` & `kombu-5.3.0b3/t/unit/asynchronous/test_semaphore.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/asynchronous/test_timer.py` & `kombu-5.3.0b3/t/unit/asynchronous/test_timer.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/conftest.py` & `kombu-5.3.0b3/t/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_clocks.py` & `kombu-5.3.0b3/t/unit/test_clocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_common.py` & `kombu-5.3.0b3/t/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_compat.py` & `kombu-5.3.0b3/t/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_compression.py` & `kombu-5.3.0b3/t/unit/test_compression.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_connection.py` & `kombu-5.3.0b3/t/unit/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,14 +493,51 @@
             raise _ConnectionError('failed connection')
 
         self.conn.get_transport_cls().connection_errors = (_ConnectionError,)
         ensured = self.conn.ensure(self.conn, publish)
         with pytest.raises(OperationalError):
             ensured()
 
+    def test_ensure_retry_errors_is_not_looping_infinitely(self):
+        class _MessageNacked(Exception):
+            pass
+
+        def publish():
+            raise _MessageNacked('NACK')
+
+        with pytest.raises(ValueError):
+            self.conn.ensure(
+                self.conn,
+                publish,
+                retry_errors=(_MessageNacked,)
+            )
+
+    def test_ensure_retry_errors_is_limited_by_max_retries(self):
+        class _MessageNacked(Exception):
+            pass
+
+        tries = 0
+
+        def publish():
+            nonlocal tries
+            tries += 1
+            if tries <= 3:
+                raise _MessageNacked('NACK')
+            # On the 4th try, we let it pass
+            return 'ACK'
+
+        ensured = self.conn.ensure(
+            self.conn,
+            publish,
+            max_retries=3,  # 3 retries + 1 initial try = 4 tries
+            retry_errors=(_MessageNacked,)
+        )
+
+        assert ensured() == 'ACK'
+
     def test_autoretry(self):
         myfun = Mock()
 
         self.conn.get_transport_cls().connection_errors = (KeyError,)
 
         def on_call(*args, **kwargs):
             myfun.side_effect = None
```

### Comparing `kombu-5.3.0b2/t/unit/test_entity.py` & `kombu-5.3.0b3/t/unit/test_entity.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_log.py` & `kombu-5.3.0b3/t/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_matcher.py` & `kombu-5.3.0b3/t/unit/test_matcher.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_message.py` & `kombu-5.3.0b3/t/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_messaging.py` & `kombu-5.3.0b3/t/unit/test_messaging.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_mixins.py` & `kombu-5.3.0b3/t/unit/test_mixins.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_pidbox.py` & `kombu-5.3.0b3/t/unit/test_pidbox.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_pools.py` & `kombu-5.3.0b3/t/unit/test_pools.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_serialization.py` & `kombu-5.3.0b3/t/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/test_simple.py` & `kombu-5.3.0b3/t/unit/test_simple.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_SQS.py` & `kombu-5.3.0b3/t/unit/transport/test_SQS.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_azureservicebus.py` & `kombu-5.3.0b3/t/unit/transport/test_azureservicebus.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,22 +199,43 @@
 
 MockQueue = namedtuple(
     'MockQueue',
     ['queue_name', 'asb', 'asb_mgmt', 'conn', 'channel', 'producer', 'queue']
 )
 
 
+@pytest.fixture(autouse=True)
+def sbac_class_patch():
+    with patch('kombu.transport.azureservicebus.ServiceBusAdministrationClient') as sbac: # noqa
+        yield sbac
+
+
+@pytest.fixture(autouse=True)
+def sbc_class_patch():
+    with patch('kombu.transport.azureservicebus.ServiceBusClient') as sbc: # noqa
+        yield sbc
+
+
+@pytest.fixture(autouse=True)
+def mock_clients(
+    sbc_class_patch,
+    sbac_class_patch,
+    mock_asb,
+    mock_asb_management
+):
+    sbc_class_patch.from_connection_string.return_value = mock_asb
+    sbac_class_patch.from_connection_string.return_value = mock_asb_management
+
+
 @pytest.fixture
 def mock_queue(mock_asb, mock_asb_management, random_queue) -> MockQueue:
     exchange = Exchange('test_servicebus', type='direct')
     queue = Queue(random_queue, exchange, random_queue)
     conn = Connection(URL_CREDS, transport=azureservicebus.Transport)
     channel = conn.channel()
-    channel._queue_service = mock_asb
-    channel._queue_mgmt_service = mock_asb_management
 
     queue(channel).declare()
     producer = messaging.Producer(channel, exchange, routing_key=random_queue)
 
     return MockQueue(
         random_queue,
         mock_asb,
```

### Comparing `kombu-5.3.0b2/t/unit/transport/test_azurestoragequeues.py` & `kombu-5.3.0b3/t/unit/transport/test_azurestoragequeues.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 from unittest.mock import patch
 
 import pytest
+from azure.identity import DefaultAzureCredential, ManagedIdentityCredential
 
 from kombu import Connection
 
 pytest.importorskip('azure.storage.queue')
 from kombu.transport import azurestoragequeues  # noqa
 
 URL_NOCREDS = 'azurestoragequeues://'
 URL_CREDS = 'azurestoragequeues://sas/key%@https://STORAGE_ACCOUNT_NAME.queue.core.windows.net/' # noqa
 AZURITE_CREDS = 'azurestoragequeues://Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==@http://localhost:10001/devstoreaccount1'  # noqa
 AZURITE_CREDS_DOCKER_COMPOSE = 'azurestoragequeues://Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==@http://azurite:10001/devstoreaccount1'  # noqa
+DEFAULT_AZURE_URL_CREDS = 'azurestoragequeues://DefaultAzureCredential@https://STORAGE_ACCOUNT_NAME.queue.core.windows.net/' # noqa
+MANAGED_IDENTITY_URL_CREDS = 'azurestoragequeues://ManagedIdentityCredential@https://STORAGE_ACCOUNT_NAME.queue.core.windows.net/' # noqa
 
 
 def test_queue_service_nocredentials():
     conn = Connection(URL_NOCREDS, transport=azurestoragequeues.Transport)
     with pytest.raises(
         ValueError,
         match='Need a URI like azurestoragequeues://{SAS or access key}@{URL}'
@@ -48,7 +51,35 @@
         channel = conn.channel()
 
         assert channel._credential == {
             'account_name': 'devstoreaccount1',
             'account_key': 'Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw=='  # noqa
         }
         assert channel._url == f'http://{hostname}:10001/devstoreaccount1' # noqa
+
+
+def test_queue_service_works_for_default_azure_credentials():
+    conn = Connection(
+        DEFAULT_AZURE_URL_CREDS, transport=azurestoragequeues.Transport
+    )
+    with patch("kombu.transport.azurestoragequeues.QueueServiceClient"):
+        channel = conn.channel()
+
+        assert isinstance(channel._credential, DefaultAzureCredential)
+        assert (
+            channel._url
+            == "https://STORAGE_ACCOUNT_NAME.queue.core.windows.net/"
+        )
+
+
+def test_queue_service_works_for_managed_identity_credentials():
+    conn = Connection(
+        MANAGED_IDENTITY_URL_CREDS, transport=azurestoragequeues.Transport
+    )
+    with patch("kombu.transport.azurestoragequeues.QueueServiceClient"):
+        channel = conn.channel()
+
+        assert isinstance(channel._credential, ManagedIdentityCredential)
+        assert (
+            channel._url
+            == "https://STORAGE_ACCOUNT_NAME.queue.core.windows.net/"
+        )
```

### Comparing `kombu-5.3.0b2/t/unit/transport/test_base.py` & `kombu-5.3.0b3/t/unit/transport/test_base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_consul.py` & `kombu-5.3.0b3/t/unit/transport/test_consul.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_etcd.py` & `kombu-5.3.0b3/t/unit/transport/test_etcd.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_filesystem.py` & `kombu-5.3.0b3/t/unit/transport/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_librabbitmq.py` & `kombu-5.3.0b3/t/unit/transport/test_librabbitmq.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_memory.py` & `kombu-5.3.0b3/t/unit/transport/test_memory.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_mongodb.py` & `kombu-5.3.0b3/t/unit/transport/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_pyamqp.py` & `kombu-5.3.0b3/t/unit/transport/test_pyamqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_pyro.py` & `kombu-5.3.0b3/t/unit/transport/test_pyro.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_qpid.py` & `kombu-5.3.0b3/t/unit/transport/test_qpid.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_redis.py` & `kombu-5.3.0b3/t/unit/transport/test_redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_sqlalchemy.py` & `kombu-5.3.0b3/t/unit/transport/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_transport.py` & `kombu-5.3.0b3/t/unit/transport/test_transport.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/test_zookeeper.py` & `kombu-5.3.0b3/t/unit/transport/test_zookeeper.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/virtual/test_base.py` & `kombu-5.3.0b3/t/unit/transport/virtual/test_base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/transport/virtual/test_exchange.py` & `kombu-5.3.0b3/t/unit/transport/virtual/test_exchange.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_amq_manager.py` & `kombu-5.3.0b3/t/unit/utils/test_amq_manager.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_compat.py` & `kombu-5.3.0b3/t/unit/utils/test_compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 
 
 def test_entrypoints():
     with patch(
         'kombu.utils.compat.importlib_metadata.entry_points', create=True
     ) as iterep:
         eps = [Mock(), Mock()]
-        iterep.return_value = {'kombu.test': eps}
+        iterep.return_value = (
+            {'kombu.test': eps} if sys.version_info < (3, 10) else eps)
 
         assert list(entrypoints('kombu.test'))
-        iterep.assert_called_with()
+        if sys.version_info < (3, 10):
+            iterep.assert_called_with()
+        else:
+            iterep.assert_called_with(group='kombu.test')
         eps[0].load.assert_called_with()
         eps[1].load.assert_called_with()
 
 
 def test_maybe_fileno():
     assert maybe_fileno(3) == 3
     f = Mock(name='file')
```

### Comparing `kombu-5.3.0b2/t/unit/utils/test_debug.py` & `kombu-5.3.0b3/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_div.py` & `kombu-5.3.0b3/t/unit/utils/test_div.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_encoding.py` & `kombu-5.3.0b3/t/unit/utils/test_encoding.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_functional.py` & `kombu-5.3.0b3/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_imports.py` & `kombu-5.3.0b3/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_json.py` & `kombu-5.3.0b3/t/unit/utils/test_json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 import uuid
 from collections import namedtuple
-from datetime import date, datetime
+from datetime import datetime
 from decimal import Decimal
-from unittest.mock import MagicMock, Mock
 
 import pytest
 import pytz
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from kombu.utils.encoding import str_to_bytes
-from kombu.utils.json import _DecodeError, dumps, loads
+from kombu.utils.json import dumps, loads
 
 
 class Custom:
 
     def __init__(self, data):
         self.data = data
 
@@ -25,40 +24,41 @@
 
 
 class test_JSONEncoder:
     @pytest.mark.freeze_time("2015-10-21")
     def test_datetime(self):
         now = datetime.utcnow()
         now_utc = now.replace(tzinfo=pytz.utc)
-        serialized = loads(dumps({
+
+        original = {
             'datetime': now,
             'tz': now_utc,
             'date': now.date(),
-            'time': now.time()},
-        ))
-        assert serialized == {
-            'datetime': now,
-            'tz': now_utc,
-            'time': now.time().isoformat(),
-            'date':  date(now.year, now.month, now.day),
+            'time': now.time(),
         }
 
+        serialized = loads(dumps(original))
+
+        assert serialized == original
+
     @given(message=st.binary())
     @settings(print_blob=True)
     def test_binary(self, message):
         serialized = loads(dumps({
             'args': (message,),
         }))
         assert serialized == {
             'args': [message],
         }
 
     def test_Decimal(self):
-        d = Decimal('3314132.13363235235324234123213213214134')
-        assert loads(dumps({'d': d})), {'d': str(d)}
+        original = {'d': Decimal('3314132.13363235235324234123213213214134')}
+        serialized = loads(dumps(original))
+
+        assert serialized == original
 
     def test_namedtuple(self):
         Foo = namedtuple('Foo', ['bar'])
         assert loads(dumps(Foo(123))) == [123]
 
     def test_UUID(self):
         constructors = [
@@ -66,15 +66,15 @@
             lambda: uuid.uuid3(uuid.NAMESPACE_URL, "https://example.org"),
             uuid.uuid4,
             lambda: uuid.uuid5(uuid.NAMESPACE_URL, "https://example.org"),
         ]
         for constructor in constructors:
             id = constructor()
             loaded_value = loads(dumps({'u': id}))
-            assert loaded_value, {'u': id}
+            assert loaded_value == {'u': id}
             assert loaded_value["u"].version == id.version
 
     def test_default(self):
         with pytest.raises(TypeError):
             dumps({'o': object()})
 
 
@@ -99,13 +99,7 @@
             bytearray(dumps({'x': 'z'}), encoding='utf-8')
         ) == {'x': 'z'}
 
     def test_loads_bytes(self):
         assert loads(
             str_to_bytes(dumps({'x': 'z'})),
             decode_bytes=True) == {'x': 'z'}
-
-    def test_loads_DecodeError(self):
-        _loads = Mock(name='_loads')
-        _loads.side_effect = _DecodeError(
-            MagicMock(), MagicMock(), MagicMock())
-        assert loads(dumps({'x': 'z'}), _loads=_loads) == {'x': 'z'}
```

### Comparing `kombu-5.3.0b2/t/unit/utils/test_objects.py` & `kombu-5.3.0b3/t/unit/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_scheduling.py` & `kombu-5.3.0b3/t/unit/utils/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_url.py` & `kombu-5.3.0b3/t/unit/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0b2/t/unit/utils/test_utils.py` & `kombu-5.3.0b3/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

