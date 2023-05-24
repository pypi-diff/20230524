# Comparing `tmp/octodns-bind-0.0.3.tar.gz` & `tmp/octodns-bind-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-bind-0.0.3.tar", last modified: Sun May 14 05:14:36 2023, max compression
+gzip compressed data, was "octodns-bind-0.0.4.tar", last modified: Wed May 24 02:33:11 2023, max compression
```

## Comparing `octodns-bind-0.0.3.tar` & `octodns-bind-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.975699 octodns-bind-0.0.3/
--rw-r--r--   0 yzguy      (501) staff       (20)     5141 2023-05-14 05:14:36.975565 octodns-bind-0.0.3/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)     4809 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/README.md
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.974623 octodns-bind-0.0.3/octodns_bind/
--rw-r--r--   0 yzguy      (501) staff       (20)     7516 2023-05-14 05:08:21.000000 octodns-bind-0.0.3/octodns_bind/__init__.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.975150 octodns-bind-0.0.3/octodns_bind.egg-info/
--rw-r--r--   0 yzguy      (501) staff       (20)     5141 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)      273 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/SOURCES.txt
--rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/dependency_links.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      210 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/requires.txt
--rw-r--r--   0 yzguy      (501) staff       (20)       13 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/top_level.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      305 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/pyproject.toml
--rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-05-14 05:14:36.975732 octodns-bind-0.0.3/setup.cfg
--rw-r--r--   0 yzguy      (501) staff       (20)     1791 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/setup.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.975255 octodns-bind-0.0.3/tests/
--rw-r--r--   0 yzguy      (501) staff       (20)     9035 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/tests/test_provider_octodns_bind.py
+drwxrwxr-x   0 yzguy     (1000) yzguy     (1000)        0 2023-05-24 02:33:11.530618 octodns-bind-0.0.4/
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)     6172 2023-05-24 02:33:11.526618 octodns-bind-0.0.4/PKG-INFO
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)     5840 2023-05-21 02:23:30.000000 octodns-bind-0.0.4/README.md
+drwxrwxr-x   0 yzguy     (1000) yzguy     (1000)        0 2023-05-24 02:33:11.526618 octodns-bind-0.0.4/octodns_bind/
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)     7930 2023-05-24 02:31:50.000000 octodns-bind-0.0.4/octodns_bind/__init__.py
+drwxrwxr-x   0 yzguy     (1000) yzguy     (1000)        0 2023-05-24 02:33:11.526618 octodns-bind-0.0.4/octodns_bind.egg-info/
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)     6172 2023-05-24 02:33:11.000000 octodns-bind-0.0.4/octodns_bind.egg-info/PKG-INFO
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)      273 2023-05-24 02:33:11.000000 octodns-bind-0.0.4/octodns_bind.egg-info/SOURCES.txt
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)        1 2023-05-24 02:33:11.000000 octodns-bind-0.0.4/octodns_bind.egg-info/dependency_links.txt
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)      210 2023-05-24 02:33:11.000000 octodns-bind-0.0.4/octodns_bind.egg-info/requires.txt
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)       13 2023-05-24 02:33:11.000000 octodns-bind-0.0.4/octodns_bind.egg-info/top_level.txt
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)      305 2023-05-21 02:23:30.000000 octodns-bind-0.0.4/pyproject.toml
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)       38 2023-05-24 02:33:11.530618 octodns-bind-0.0.4/setup.cfg
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)     1791 2023-05-21 02:23:30.000000 octodns-bind-0.0.4/setup.py
+drwxrwxr-x   0 yzguy     (1000) yzguy     (1000)        0 2023-05-24 02:33:11.526618 octodns-bind-0.0.4/tests/
+-rw-rw-r--   0 yzguy     (1000) yzguy     (1000)     9505 2023-05-21 02:23:30.000000 octodns-bind-0.0.4/tests/test_provider_octodns_bind.py
```

### Comparing `octodns-bind-0.0.3/PKG-INFO` & `octodns-bind-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: octodns-bind
-Version: 0.0.3
-Summary:  RFC compliant (Bind9) provider for octoDNS
-Home-page: https://github.com/octodns/octodns-bind
-Author: Adam Smith
-Author-email: zero1three@gmail.com
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-
 ## RFC compliant (Bind9) provider for octoDNS
 
 An [octoDNS](https://github.com/octodns/octodns/) provider that targets [Bind](https://www.isc.org/bind/) and other standards compliant servers. It includes support for sourcing records via AXFR, reading zone files, and fully managing records with [RFC 2136](https://datatracker.ietf.org/doc/html/rfc2136).
 
 ### Installation
 
 #### Command line
@@ -74,14 +61,18 @@
 providers:
   axfr:
       class: octodns_bind.AxfrSource
       # The address of nameserver to perform zone transfer against
       host: ns1.example.com
       # The port that the nameserver is listening on. Optional. Default: 53
       port: 53
+      # Use IPv6 to perform operations. Optional. Default: False
+      ipv6: False
+      # The number of seconds to wait until timing out. Optional. Default: 15
+      timeout: 15
       # optional, default: non-authed
       key_name: env/AXFR_KEY_NAME
       # optional, default: non-authed
       key_secret: env/AXFR_KEY_SECRET
       # optional, see https://github.com/rthalley/dnspython/blob/master/dns/tsig.py#L78
       # for available algorithms
       key_algorithm: hmac-sha1
@@ -105,14 +96,18 @@
   rfc2136:
       # also available as octodns_bind.BindProvider
       class: octodns_bind.Rfc2136Provider
       # The address of nameserver to perform zone transfer against
       host: ns1.example.com
       # The port that the nameserver is listening on. Optional. Default: 53
       port: 53
+      # Use IPv6 to perform operations. Optional. Default: False
+      ipv6: False
+      # The number of seconds to wait until timing out. Optional. Default: 15
+      timeout: 15
       # optional, default: non-authed
       key_name: env/AXFR_KEY_NAME
       # optional, default: non-authed
       key_secret: env/AXFR_KEY_SECRET
       # optional, see https://github.com/rthalley/dnspython/blob/master/dns/tsig.py#L78
       # for available algorithms
       key_algorithm: hmac-sha1
@@ -151,8 +146,29 @@
 
 This module does not support dynamic records.
 
 ### Development
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
 
-There is a [docker-compose.yml](/docker-compose.yml) file included in the repo that will set up a Bind9 server with AXFR transfers and RFC 2136 updates enabled for use in development. The secret for the server can be found in [docker/etc/bind/named.conf](docker/etc/bind/named.conf).
+#### Local Server
+
+A local server is included in the repo via [docker-compose.yml](/docker-compose.yml). This will set up a Bind9 server with AXFR transfers and RFC 2136 updates enabled for use in development on IPv4 and IPv6. Configuration for the server can be found in [docker/etc/bind/named.conf](docker/etc/bind/named.conf), including the TSIG secret which can be used to perform authenticated operations. Zonefiles can be found in [docker/var/lib/bind](docker/var/lib/bind). All logs are written to STDOUT and can be viewed by running `docker-compose logs -f`
+
+An example octodns configuration to interact with the local server is below:
+
+```yaml
+providers:
+  rfc2136:
+    class: octodns_bind.Rfc2136Provider
+    host: localhost
+    key_name: 'octodns.exxampled.com.'
+    key_secret: 'vZew5TtZLTZKTCl00xliGt+1zzsuLWQWFz48bRbPnZU='
+    key_algorithm: 'hmac-sha256'
+
+zones:
+  exxampled.com.:
+    sources:
+      - config
+    targets:
+      - rfc2136
+```
```

### Comparing `octodns-bind-0.0.3/octodns_bind/__init__.py` & `octodns-bind-0.0.4/octodns_bind/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 #
 #
 
+import socket
 from logging import getLogger
 from os import listdir
 from os.path import join
 
 import dns.name
 import dns.query
 import dns.rdatatype
@@ -15,15 +16,15 @@
 from dns.exception import DNSException
 from dns.update import Update as DnsUpdate
 
 from octodns.provider.base import BaseProvider
 from octodns.record import Create, Record, Rr, Update
 from octodns.source.base import BaseSource
 
-__VERSION__ = '0.0.3'
+__VERSION__ = '0.0.4'
 
 
 class RfcPopulate:
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = False
     SUPPORTS = set(
         (
@@ -143,45 +144,55 @@
 
 class AxfrPopulate(RfcPopulate):
     def __init__(
         self,
         id,
         host,
         port=53,
+        ipv6=False,
+        timeout=15,
         key_name=None,
         key_secret=None,
         key_algorithm=None,
     ):
         self.log = getLogger(f'{self.__class__.__name__}[{id}]')
         self.log.debug(
-            '__init__: id=%s, host=%s, port=%d, key_name=%s, key_secret=%s, key_algorithm=%s',
+            '__init__: id=%s, host=%s, port=%d, ipv6=%s, timeout=%d, key_name=%s, key_secret=%s, key_algorithm=%s',
             id,
             host,
             port,
+            ipv6,
+            timeout,
             key_name,
             key_secret is not None,
             key_algorithm is not None,
         )
         super().__init__(id)
-        self.host = self._host(host)
+        self.host = self._host(host, ipv6)
         self.port = int(port)
+        self.ipv6 = ipv6
+        self.timeout = float(timeout)
         self.key_name = key_name
         self.key_secret = key_secret
         self.key_algorithm = key_algorithm
 
-    def _host(self, host):
+    def _host(self, host, ipv6):
         h = host
         try:
             # Determine if IPv4/IPv6 address
             dns.inet.af_for_address(host)
         except ValueError:
+            address_family = socket.AF_INET
+            if ipv6:
+                address_family = socket.AF_INET6
+
             try:
-                h = dns.resolver.resolve(host)[0].address
-            except DNSException as err:
-                raise AxfrSourceZoneTransferFailed(err) from None
+                h = socket.getaddrinfo(host, None, address_family)[0][4][0]
+            except OSError as err:
+                raise AxfrSourceZoneTransferFailed(err)
 
         return h
 
     def _auth_params(self):
         params = {}
         if self.key_name is not None:
             params['keyring'] = tsigkeyring.from_text(
@@ -195,14 +206,16 @@
         auth_params = self._auth_params()
         try:
             z = dns.zone.from_xfr(
                 dns.query.xfr(
                     self.host,
                     zone.name,
                     port=self.port,
+                    timeout=self.timeout,
+                    lifetime=self.timeout,
                     relativize=False,
                     **auth_params,
                 ),
                 relativize=False,
             )
         except DNSException as err:
             raise AxfrSourceZoneTransferFailed(err) from None
@@ -253,15 +266,15 @@
                 update.add(name, ttl, _type, *rdatas)
             elif isinstance(change, Update):
                 update.replace(name, ttl, _type, *rdatas)
             else:  # isinstance(change, Delete):
                 update.delete(name, _type, *rdatas)
 
         r: dns.message.Message = dns.query.tcp(
-            update, self.host, port=self.port
+            update, self.host, port=self.port, timeout=self.timeout
         )
         if r.rcode() != dns.rcode.NOERROR:
             raise Rfc2136ProviderUpdateFailed(dns.rcode.to_text(r.rcode()))
 
         self.log.debug(
             '_apply: zone=%s, num_records=%d', name, len(plan.changes)
         )
```

### Comparing `octodns-bind-0.0.3/octodns_bind.egg-info/PKG-INFO` & `octodns-bind-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-bind
-Version: 0.0.3
+Version: 0.0.4
 Summary:  RFC compliant (Bind9) provider for octoDNS
 Home-page: https://github.com/octodns/octodns-bind
 Author: Adam Smith
 Author-email: zero1three@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -74,14 +74,18 @@
 providers:
   axfr:
       class: octodns_bind.AxfrSource
       # The address of nameserver to perform zone transfer against
       host: ns1.example.com
       # The port that the nameserver is listening on. Optional. Default: 53
       port: 53
+      # Use IPv6 to perform operations. Optional. Default: False
+      ipv6: False
+      # The number of seconds to wait until timing out. Optional. Default: 15
+      timeout: 15
       # optional, default: non-authed
       key_name: env/AXFR_KEY_NAME
       # optional, default: non-authed
       key_secret: env/AXFR_KEY_SECRET
       # optional, see https://github.com/rthalley/dnspython/blob/master/dns/tsig.py#L78
       # for available algorithms
       key_algorithm: hmac-sha1
@@ -105,14 +109,18 @@
   rfc2136:
       # also available as octodns_bind.BindProvider
       class: octodns_bind.Rfc2136Provider
       # The address of nameserver to perform zone transfer against
       host: ns1.example.com
       # The port that the nameserver is listening on. Optional. Default: 53
       port: 53
+      # Use IPv6 to perform operations. Optional. Default: False
+      ipv6: False
+      # The number of seconds to wait until timing out. Optional. Default: 15
+      timeout: 15
       # optional, default: non-authed
       key_name: env/AXFR_KEY_NAME
       # optional, default: non-authed
       key_secret: env/AXFR_KEY_SECRET
       # optional, see https://github.com/rthalley/dnspython/blob/master/dns/tsig.py#L78
       # for available algorithms
       key_algorithm: hmac-sha1
@@ -151,8 +159,29 @@
 
 This module does not support dynamic records.
 
 ### Development
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
 
-There is a [docker-compose.yml](/docker-compose.yml) file included in the repo that will set up a Bind9 server with AXFR transfers and RFC 2136 updates enabled for use in development. The secret for the server can be found in [docker/etc/bind/named.conf](docker/etc/bind/named.conf).
+#### Local Server
+
+A local server is included in the repo via [docker-compose.yml](/docker-compose.yml). This will set up a Bind9 server with AXFR transfers and RFC 2136 updates enabled for use in development on IPv4 and IPv6. Configuration for the server can be found in [docker/etc/bind/named.conf](docker/etc/bind/named.conf), including the TSIG secret which can be used to perform authenticated operations. Zonefiles can be found in [docker/var/lib/bind](docker/var/lib/bind). All logs are written to STDOUT and can be viewed by running `docker-compose logs -f`
+
+An example octodns configuration to interact with the local server is below:
+
+```yaml
+providers:
+  rfc2136:
+    class: octodns_bind.Rfc2136Provider
+    host: localhost
+    key_name: 'octodns.exxampled.com.'
+    key_secret: 'vZew5TtZLTZKTCl00xliGt+1zzsuLWQWFz48bRbPnZU='
+    key_algorithm: 'hmac-sha256'
+
+zones:
+  exxampled.com.:
+    sources:
+      - config
+    targets:
+      - rfc2136
+```
```

### Comparing `octodns-bind-0.0.3/setup.py` & `octodns-bind-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `octodns-bind-0.0.3/tests/test_provider_octodns_bind.py` & `octodns-bind-0.0.4/tests/test_provider_octodns_bind.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 #
 #
 
+import socket
 from os.path import exists
 from shutil import copyfile
 from unittest import TestCase
 from unittest.mock import patch
 
 import dns.resolver
 import dns.zone
@@ -22,15 +23,15 @@
     ZoneFileSource,
     ZoneFileSourceLoadFailure,
     ZoneFileSourceNotFound,
 )
 
 
 class TestAxfrSource(TestCase):
-    source = AxfrSource('test', 'localhost')
+    source = AxfrSource('test', '127.0.0.1')
 
     forward_zonefile = dns.zone.from_file(
         './tests/zones/unit.tests.tst', 'unit.tests', relativize=False
     )
 
     reverse_zonefile = dns.zone.from_file(
         './tests/zones/2.0.192.in-addr.arpa.',
@@ -130,56 +131,66 @@
             'The DNS zone has no NS RRset at its origin.', str(ctx.exception)
         )
 
         # Records are not to RFC (lenient=False)
         with self.assertRaises(ValidationError) as ctx:
             zone = Zone('invalid.records.', [])
             self.source.populate(zone)
+        # quotes were added to the record name 1.0.0rc1, this makes it work with
+        # both version
+        reason = str(ctx.exception).replace('"', '')
         self.assertEqual(
-            'Invalid record _invalid.invalid.records.\n'
-            '  - invalid name for SRV record',
-            str(ctx.exception),
+            'Invalid record _invalid.invalid.records.\n  - invalid name for SRV record',
+            reason,
         )
 
         # Records are not to RFC, but load anyhow (lenient=True)
         invalid = Zone('invalid.records.', [])
         self.source.populate(invalid, lenient=True)
         self.assertEqual(12, len(invalid.records))
 
 
 class TestRfc2136Provider(TestCase):
     def test_host_ip(self):
         provider = Rfc2136Provider('test', '192.0.2.1')
         self.assertEqual('192.0.2.1', provider.host)
 
-    @patch('dns.resolver.resolve')
+    @patch('socket.getaddrinfo')
     def test_host_dns(self, resolve_mock):
-        host, ip = 'axfr.unit.tests.', '192.0.2.2'
+        host, ipv4, ipv6 = 'axfr.unit.tests.', '192.0.2.2', '2001:db8::1'
 
-        # Query success
-        resolve_mock.return_value = dns.rrset.from_text(
-            host, 300, 'IN', 'A', ip
-        )
+        # Query success IPv4
+        resolve_mock.return_value = [
+            (socket.AF_INET, socket.SOCK_STREAM, 6, '', (ipv4, 0))
+        ]
         provider = Rfc2136Provider('test', host)
-        self.assertEqual(ip, provider.host)
+        self.assertEqual(ipv4, provider.host)
+
+        # Query success IPv6
+        resolve_mock.reset_mock()
+        resolve_mock.return_value = [
+            (socket.AF_INET6, socket.SOCK_STREAM, 6, '', (ipv6, 0, 0, 0))
+        ]
+        provider = Rfc2136Provider('test', host, ipv6=True)
+        self.assertEqual(ipv6, provider.host)
 
         # Query failure
         resolve_mock.reset_mock()
-        resolve_mock.side_effect = DNSException
+        resolve_mock.side_effect = OSError
         with self.assertRaises(AxfrSourceZoneTransferFailed):
             provider = Rfc2136Provider('test', host)
 
     def test_auth(self):
-        provider = Rfc2136Provider('test', 'localhost')
+        provider = Rfc2136Provider('test', '127.0.0.1')
         self.assertEqual({}, provider._auth_params())
 
         key_secret = 'vZew5TtZLTZKTCl00xliGt+1zzsuLWQWFz48bRbPnZU='
         provider = Rfc2136Provider(
             'test',
-            'localhost',
+            '127.0.0.1',
             key_name='key-name',
             key_secret=key_secret,
             key_algorithm='hmac-sha1',
         )
         self.assertTrue('keyring' in provider._auth_params())
         self.assertTrue('keyalgorithm' in provider._auth_params())
 
@@ -192,15 +203,15 @@
         self,
         zone_records_mock,
         dns_query_tcp_mock,
         add_mock,
         replace_mock,
         delete_mock,
     ):
-        provider = Rfc2136Provider('test', 'localhost')
+        provider = Rfc2136Provider('test', '127.0.0.1')
 
         desired = Zone('unit.tests.', [])
         record = Record.new(
             desired, 'a', {'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
         )
         desired.add_record(record)
```

