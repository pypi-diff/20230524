# Comparing `tmp/qtwasmserver-0.0.6.tar.gz` & `tmp/qtwasmserver-0.1.0.tar.gz`

## Comparing `qtwasmserver-0.0.6.tar` & `qtwasmserver-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/build
--rwxr-xr-x   0        0        0     9468 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/src/qtwasmserver/qtwasmserver.py
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/src/qtwasmserver/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/LICENSE
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/README.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 qtwasmserver-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/build
+-rwxr-xr-x   0        0        0     9805 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/src/qtwasmserver/qtwasmserver.py
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/src/qtwasmserver/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/PKG-INFO
```

### Comparing `qtwasmserver-0.0.6/src/qtwasmserver/qtwasmserver.py` & `qtwasmserver-0.1.0/src/qtwasmserver/qtwasmserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from http.server import SimpleHTTPRequestHandler, ThreadingHTTPServer
 from subprocess import run
 
 import brotli
 import netifaces as ni
 from httpcompressionserver import HTTPCompressionRequestHandler
 
+
 def generate_mkcert_certificate(addresses):
     """ "Generates a https certificate for localhost and selected addresses. This
     requires that the mkcert utility is installed, and that a certificate
     authority key pair (rootCA-key.pem and rootCA.pem) has been generated. The
     certificates are written to /tmp, where the http server can find them
     ater on."""
 
@@ -34,54 +35,57 @@
     # check if mkcert is installed
     try:
         out = subprocess.check_output(["mkcert", "-CAROOT"])
         root_ca_path = out.decode("utf-8").strip()
         print(
             "Generating certificates with mkcert, using certificate authority files at:"
         )
-        print(f"   {root_ca_path}\n")
+        print(f"   {root_ca_path}       [from 'mkcert -CAROOT'] \n")
     except Exception as e:
         print("Warning: Unable to run mkcert. Will not start https server.")
         print(e)
         print(f"Install mkcert from github.com/FiloSottile/mkcert to fix this.\n")
         return False, None, None
 
-    # generate certificates
+    # generate certificates using mkcert
     addresses_string = f"localhost {' '.join(addresses)}"
+    print("=== begin mkcert output ===\n")
     ret = run(
         f"mkcert -cert-file {cert_file.name} -key-file {cert_key_file.name} {addresses_string}",
         shell=True,
     )
+    print("=== end mkcert output ===\n")
     has_certificate = ret.returncode == 0
     if not has_certificate:
         print(
             "Warning: mkcert is not installed or was unable to create a certificate. Will not start HTTPS server."
         )
     return has_certificate, cert_file, cert_key_file
 
 
-def send_site_isolation_headers(handler):
-    """Sends COOP and COEP site isolation headers"""
+def send_cross_origin_isolation_headers(handler):
+    """Sends COOP and COEP cross origin isolation headers"""
     handler.send_header("Cross-Origin-Opener-Policy", "same-origin")
     handler.send_header("Cross-Origin-Embedder-Policy", "require-corp")
     handler.send_header("Cross-Origin-Resource-Policy", "cross-origin")
 
 
 def send_empty_favicon(handle):
     """Sends an empty icon to surpess missing faviocon errors"""
     self.send_response(200)
     self.send_header("Content-Type", "image/x-icon")
     self.send_header("Content-Length", 0)
 
+
 class HttpRequestHandler(SimpleHTTPRequestHandler):
     protocol_version = "HTTP/1.1"
 
     def end_headers(self):
-        if self.site_isolation == True:
-            send_site_isolation_headers(self)
+        if self.cross_origin_isolation == True:
+            send_cross_origin_isolation_headers(self)
         super().end_headers()
 
 
 class CompressionHttpRequesthandler(HTTPCompressionRequestHandler):
     protocol_version = "HTTP/1.1"
 
     # Add wasm to the list of compressed types.
@@ -112,50 +116,57 @@
     # Ideally, we would like to use the default gzip/deflate support as well,
     # however that makes gzip take precedence over brotli. In practice, all
     # browsers support brotli, so we can just use that.
     compressions = {}  # HTTPCompressionRequestHandler.compressions.copy()
     compressions["br"] = brotli_producer
 
     def end_headers(self):
-        if self.site_isolation == True:
-            send_site_isolation_headers(self)
+        if self.cross_origin_isolation == True:
+            send_cross_origin_isolation_headers(self)
         super().end_headers()
 
 
 class CompressionMode(Enum):
-    AUTO = 1
-    ALWAYS = 2
-    NEVER = 3
+    AUTO = "Auto"
+    ALWAYS = "Always"
+    NEVER = "Never"
 
 
 def select_http_handler_class(compression_mode, address):
+
     """Returns the http handler class to use, based on the compression mode,
     and the address of the server for the auto mode."""
     if compression_mode == CompressionMode.ALWAYS:
         return CompressionHttpRequesthandler
     elif compression_mode == CompressionMode.NEVER:
         return HttpRequestHandler
     else:
         # Select http request handler based on addrees. If the address is
         # localhost then compression is typically not worth it since the
         # localhost connection is very fast. For other addresses we assume
-        # normal network bandwidth and enable compression to reduce the download
+        # typical network bandwidth and enable compression to reduce the download
         # size.
         if address == "127.0.0.1":
             return HttpRequestHandler
         else:
             return CompressionHttpRequesthandler
 
 
 # Serve cwd from http(s)://address:port, with certificates from certdir if set
 def serve_on_thread(
-    address, port, secure, cert_file, cert_key_file, compression_mode, site_isolation
+    address,
+    port,
+    secure,
+    cert_file,
+    cert_key_file,
+    compression_mode,
+    cross_origin_isolation,
 ):
     handler = select_http_handler_class(compression_mode, address)
-    handler.site_isolation = site_isolation
+    handler.cross_origin_isolation = cross_origin_isolation
     httpd = ThreadingHTTPServer((address, port), handler)
     if secure:
         context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
         context.load_cert_chain(cert_file.name, cert_key_file.name)
         httpd.socket = context.wrap_socket(
             httpd.socket,
             server_side=True,
@@ -180,20 +191,22 @@
         "--address",
         "-a",
         help="Bind to additional address, in addition to localhost",
         action="append",
     )
     parser.add_argument(
         "--all-interfaces",
+        "-A",
         help="Bind to all local interfaces, instead of locahost only",
         action="store_true",
     )
     parser.add_argument(
-        "--site-isolation",
-        help="Enables site isolation mode, required for WebAssembly threads",
+        "--cross-origin-isolation",
+        "-i",
+        help="Enables cross-origin isolation mode, required for WebAssembly threads",
         action="store_true",
     )
     parser.add_argument(
         "--compress-auto",
         help="Enables file compression on non-localhost addresses",
         action="store_true",
         default=True,
@@ -214,15 +227,15 @@
 
     args = parser.parse_args()
     http_port = args.port
     https_port = http_port + 1
     all_interfaces = args.all_interfaces
     cmd_addresses = args.address or []
     serve_path = args.path
-    site_isolation = args.site_isolation
+    cross_origin_isolation = args.cross_origin_isolation
 
     compression_mode = CompressionMode.AUTO
     if args.compress_always:
         compression_mode = CompressionMode.ALWAYS
     elif args.compress_never:
         compression_mode = CompressionMode.NEVER
 
@@ -242,41 +255,41 @@
     print("Serving at addresses:")
     print(f"   {addresses}\n")
 
     has_certificate, cert_file, cert_key_file = generate_mkcert_certificate(addresses)
 
     print("Options:")
     print(f"   Secure server:          {has_certificate}")
-    print(f"   Site isolation mode:    {site_isolation}")
-    print(f"   Compression:            {compression_mode}")
+    print(f"   Cross Origin Isolation: {cross_origin_isolation}")
+    print(f"   Compression:            {compression_mode.value}")
     print("")
 
     # Start servers
     print(f"Serving at:")
     for address in addresses:
         print(f"    http://{address}:{http_port}")
         serve_on_thread(
             address,
             http_port,
             False,
             cert_file,
             cert_key_file,
             compression_mode,
-            site_isolation,
+            cross_origin_isolation,
         )
 
     if has_certificate:
         for address in addresses:
             print(f"    https://{address}:{https_port}")
             serve_on_thread(
                 address,
                 https_port,
                 True,
                 cert_file,
                 cert_key_file,
                 compression_mode,
-                site_isolation,
+                cross_origin_isolation,
             )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `qtwasmserver-0.0.6/LICENSE` & `qtwasmserver-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.0.6/README.md` & `qtwasmserver-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,53 +17,47 @@
 * Support for generating https certificates using the mkcert utility. Many web features
   require a secure context. While "localhost" is considered a secure context (also when plain
   http is used), other addresses are not. Clicking through the "not secure" warnings is
   an option, but using a valid certificate improves flow.
 
 * Support for compression using brotli. By default, the server compresses when serving over a
   public, non-localhost address. (localhost is fast, enabling compression here usualually increases
-  download time instead of the opposite). Compression be controlled with the --compress-always and 
+  download time instead of doing the opposite). Compression be controlled with the --compress-always and
   --compress-never options.
 
-* Support for enabling site isolation mode. This sets the so-called COOP and COEP headers,
-  which are required to enable SharedArrayBuffer and multithreading. Enable with the --site-isolation option.
-  While there is little reason to not enable SharedArrayBuffer, site isolation mode also enables
-  additional restrictions for cross origin requests, which may come as a surprise.
-
-It also has a couple of non-features:
-
-* Support for starting/stopping web browsers.
-
-* Support for forwarding standard output to the console.
-
-If you are looking to use features like the above, then emrun from Emscripten is a better choice.
+* Support for enabling cross-origin isolation mode. This sets the so-called COOP and COEP headers,
+  which are required to enable SharedArrayBuffer and multithreading. Enable with the --cross-origin-isolation
+  option. Note that this may impose additional restrictions on cross-origin requests.
 
 TODO:
 
  * ipv6 support
 
 # Installation and Usage
 
 pip install qtwasmserver
 
-    qtwasmserver                        # Start server on localhost, serve $CWD
-    qtwasmserver /path/to/wasm/builds   # Specify web root path
-    qtwasmserver --all-interfaces       # Start server(s) on all network interfaces
-    qtwasmserver -a 10.0.0.2            # Start server on specific address, in addition to localhost
-    qtwasmserver --site-isolation       # Enable site isolation mode for multithreading
-    qtwasmserver -h                     # Show help
+Usage exmaples:
+
+    qtwasmserver                            # Start server on localhost, serve $CWD
+    qtwasmserver /path/to/wasm/builds       # Specify web root path
+    qtwasmserver -p 1080                    # Start server(s) on a spesific port
+    qtwasmserver --all-interfaces           # Start server(s) on all network interfaces
+    qtwasmserver -a 10.0.0.2                # Start server on specific address, in addition to localhost
+    qtwasmserver --cross-origin-isolation   # Enable cross-origin isolation mode for multithreading
+    qtwasmserver -h                         # Show help
 
 # Using mkcert
 
 qtwasmserver can optinally use mkcert to generate https certifacates. See https://github.com/FiloSottile/mkcert for
 installation and getting started instructions.
 
 The basic flow is:
 
  1. Gereate a certificate authority (CA), and install that on all devices and browsers.
     This is a one time operation. mkcert will use thuis CA to sign certificates.
  2. Generate a certificate for each address you want to use. This is done automatically
     by this server.
 
-The main beneifits of this appraoch is that certificates can be freely generated if/when
-the network address for the server changes, for example when moving between home and office
-networks, and that it does not requie reqeusting certificates from a third party.
+The main beneifit of this appraoch is that certificates can be generated locally on demand,
+which can be useful when for instance when moving a development machine between home and office
+networks.
```

### Comparing `qtwasmserver-0.0.6/pyproject.toml` & `qtwasmserver-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qtwasmserver"
-version = "0.0.6"
+version = "0.1.0"
 authors = [
   { name="Morten Sørvig", email="msorvig@gmail.com" },
 ]
 description = "Development Web Server for Qt for Webassembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "brotli >= 1",
+  "brotlipy >= 0.7",
   "netifaces >= 0.10",
   "httpcompressionserver >= 0.5",
 ]
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src"]
 sources = ["src"]
```

### Comparing `qtwasmserver-0.0.6/PKG-INFO` & `qtwasmserver-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: qtwasmserver
-Version: 0.0.6
+Version: 0.1.0
 Summary: Development Web Server for Qt for Webassembly
 Project-URL: Homepage, https://github.com/msorvig/qtwasmserver
 Project-URL: Bug Tracker, https://github.com/msorvig/qtwasmserver/issues
 Author-email: Morten Sørvig <msorvig@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: brotli>=1
+Requires-Dist: brotlipy>=0.7
 Requires-Dist: httpcompressionserver>=0.5
 Requires-Dist: netifaces>=0.10
 Description-Content-Type: text/markdown
 
 ## Qt for WebAssembly development server. 
 
 This server is intented to be used while developing and testing WebAssembly applications on a
@@ -34,53 +34,47 @@
 * Support for generating https certificates using the mkcert utility. Many web features
   require a secure context. While "localhost" is considered a secure context (also when plain
   http is used), other addresses are not. Clicking through the "not secure" warnings is
   an option, but using a valid certificate improves flow.
 
 * Support for compression using brotli. By default, the server compresses when serving over a
   public, non-localhost address. (localhost is fast, enabling compression here usualually increases
-  download time instead of the opposite). Compression be controlled with the --compress-always and 
+  download time instead of doing the opposite). Compression be controlled with the --compress-always and
   --compress-never options.
 
-* Support for enabling site isolation mode. This sets the so-called COOP and COEP headers,
-  which are required to enable SharedArrayBuffer and multithreading. Enable with the --site-isolation option.
-  While there is little reason to not enable SharedArrayBuffer, site isolation mode also enables
-  additional restrictions for cross origin requests, which may come as a surprise.
-
-It also has a couple of non-features:
-
-* Support for starting/stopping web browsers.
-
-* Support for forwarding standard output to the console.
-
-If you are looking to use features like the above, then emrun from Emscripten is a better choice.
+* Support for enabling cross-origin isolation mode. This sets the so-called COOP and COEP headers,
+  which are required to enable SharedArrayBuffer and multithreading. Enable with the --cross-origin-isolation
+  option. Note that this may impose additional restrictions on cross-origin requests.
 
 TODO:
 
  * ipv6 support
 
 # Installation and Usage
 
 pip install qtwasmserver
 
-    qtwasmserver                        # Start server on localhost, serve $CWD
-    qtwasmserver /path/to/wasm/builds   # Specify web root path
-    qtwasmserver --all-interfaces       # Start server(s) on all network interfaces
-    qtwasmserver -a 10.0.0.2            # Start server on specific address, in addition to localhost
-    qtwasmserver --site-isolation       # Enable site isolation mode for multithreading
-    qtwasmserver -h                     # Show help
+Usage exmaples:
+
+    qtwasmserver                            # Start server on localhost, serve $CWD
+    qtwasmserver /path/to/wasm/builds       # Specify web root path
+    qtwasmserver -p 1080                    # Start server(s) on a spesific port
+    qtwasmserver --all-interfaces           # Start server(s) on all network interfaces
+    qtwasmserver -a 10.0.0.2                # Start server on specific address, in addition to localhost
+    qtwasmserver --cross-origin-isolation   # Enable cross-origin isolation mode for multithreading
+    qtwasmserver -h                         # Show help
 
 # Using mkcert
 
 qtwasmserver can optinally use mkcert to generate https certifacates. See https://github.com/FiloSottile/mkcert for
 installation and getting started instructions.
 
 The basic flow is:
 
  1. Gereate a certificate authority (CA), and install that on all devices and browsers.
     This is a one time operation. mkcert will use thuis CA to sign certificates.
  2. Generate a certificate for each address you want to use. This is done automatically
     by this server.
 
-The main beneifits of this appraoch is that certificates can be freely generated if/when
-the network address for the server changes, for example when moving between home and office
-networks, and that it does not requie reqeusting certificates from a third party.
+The main beneifit of this appraoch is that certificates can be generated locally on demand,
+which can be useful when for instance when moving a development machine between home and office
+networks.
```

