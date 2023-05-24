# Comparing `tmp/klab-client-py-0.1.1.tar.gz` & `tmp/klab-client-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klab-client-py-0.1.1.tar", last modified: Mon Feb 20 07:09:40 2023, max compression
+gzip compressed data, was "klab-client-py-0.1.2.tar", last modified: Wed May 24 14:25:50 2023, max compression
```

## Comparing `klab-client-py-0.1.1.tar` & `klab-client-py-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34523 2023-02-06 09:54:55.204480 klab-client-py-0.1.1/LICENSE
--rw-r--r--   0        0        0     2619 2023-02-20 06:42:40.030476 klab-client-py-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:54:55.204480 klab-client-py-0.1.1/klab/__init__.py
--rw-r--r--   0        0        0    11905 2023-02-18 11:14:19.402969 klab-client-py-0.1.1/klab/engine.py
--rw-r--r--   0        0        0      636 2023-02-18 07:09:20.214218 klab-client-py-0.1.1/klab/exceptions.py
--rw-r--r--   0        0        0    20920 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/klab/geometry.py
--rw-r--r--   0        0        0     6448 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/klab/klab.py
--rw-r--r--   0        0        0     4212 2023-02-20 07:04:43.041133 klab-client-py-0.1.1/klab/observable.py
--rw-r--r--   0        0        0    14864 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/klab/observation.py
--rw-r--r--   0        0        0    21000 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/klab/references.py
--rw-r--r--   0        0        0     4420 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/klab/ticket.py
--rw-r--r--   0        0        0     8111 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/klab/types.py
--rw-r--r--   0        0        0     8970 2023-02-18 10:55:10.474545 klab-client-py-0.1.1/klab/utils.py
--rw-r--r--   0        0        0      667 2023-02-20 07:08:58.935912 klab-client-py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    15973 2023-02-20 07:06:08.920729 klab-client-py-0.1.1/tests/test_connection.py
--rw-r--r--   0        0        0      533 2023-02-17 15:10:49.981233 klab-client-py-0.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 klab-client-py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-06 09:54:55.204480 klab-client-py-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2618 2023-05-24 14:19:13.085175 klab-client-py-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:54:55.204480 klab-client-py-0.1.2/klab/__init__.py
+-rw-r--r--   0        0        0    12359 2023-05-24 13:05:29.651569 klab-client-py-0.1.2/klab/engine.py
+-rw-r--r--   0        0        0      641 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/exceptions.py
+-rw-r--r--   0        0        0    20931 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/geometry.py
+-rw-r--r--   0        0        0     7621 2023-05-24 14:05:34.904483 klab-client-py-0.1.2/klab/klab.py
+-rw-r--r--   0        0        0     4206 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/observable.py
+-rw-r--r--   0        0        0    14872 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/observation.py
+-rw-r--r--   0        0        0    21021 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/references.py
+-rw-r--r--   0        0        0     4420 2023-02-17 15:10:49.981233 klab-client-py-0.1.2/klab/ticket.py
+-rw-r--r--   0        0        0     8118 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/types.py
+-rw-r--r--   0        0        0     8958 2023-05-24 12:06:19.749578 klab-client-py-0.1.2/klab/utils.py
+-rw-r--r--   0        0        0      667 2023-05-24 14:19:32.277169 klab-client-py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14968 2023-05-24 13:48:34.587816 klab-client-py-0.1.2/tests/test_connection.py
+-rw-r--r--   0        0        0      533 2023-02-17 15:10:49.981233 klab-client-py-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 klab-client-py-0.1.2/PKG-INFO
```

### Comparing `klab-client-py-0.1.1/LICENSE` & `klab-client-py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `klab-client-py-0.1.1/README.md` & `klab-client-py-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # k.LAB CLient Python
 
 A Python client library to interact with a running (local or remote) k.LAB Engine.
 
-This package is a python client for [k.LAB](https://github.com/integratedmodelling/klab). It allows registered users of k.LAB to make observations on the k.LAB semantic web from a Java program using the REST API. After creating a spatial/temporal context root observation as a context, you can submit concepts to be observed in it and the relative observations will be made at the server side and returned. Depending on the semantics submitted, the results will consists of different scientific artifacts that can be exported or inspected as needed through the API.
+This package is a python client for [k.LAB](https://github.com/integratedmodelling/klab). It allows registered users of k.LAB to make observations on the k.LAB semantic web from a Python program using the REST API. After creating a spatial/temporal context root observation as a context, you can submit concepts to be observed in it and the relative observations will be made at the server side and returned. Depending on the semantics submitted, the results will consists of different scientific artifacts that can be exported or inspected as needed through the API.
 
 While the API (both k.LAB's public REST API and the interfaces in this package) should be stable, this code is young - features are still missing and bugs certainly remain. Please submit Github issues as needed.
 
 This README assumes knowledge of k.LAB and semantic modeling. An introduction to both is available as a [technical note](https://docs.integratedmodelling.org/technote/index.html) while more extensive documentation is developed.
 
 
 ## Installation
@@ -63,12 +63,12 @@
 elevation = await ticketHandler.get()
 ```
 
 6. export the observation to a geotiff
 
 ```
 path = "your path here"
-elevation.exportToFile(Export.DATA, ExportFormat.GEOTIFF_RASTER, path)
+elevation.exportToFile(Export.DATA, ExportFormat.BYTESTREAM, path)
 ```
 
 
-**For more examples have a look at [the testcases in the repository](https://github.com/integratedmodelling/klab-client-python/tree/main/tests).**
+**For more examples have a look at [the testcases in the repository](https://github.com/integratedmodelling/klab-client-python/tree/main/tests).**
```

### Comparing `klab-client-py-0.1.1/klab/engine.py` & `klab-client-py-0.1.2/klab/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 
 class Engine:
     """
 
     """
 
     def __init__(self, url):
-        self.token = None
+        self.session = None
+        self.authorization = None
         self.url = url
         self.acceptHeader = None
 
         while self.url.endswith("/"):
             self.url = self.url[0:-1]
 
-    def authenticate(self, username = None, password = None):
+    def authenticate(self, username=None, password=None):
         """Local engine login, no auth necessary."""
 
         if username and password:
             requestUrl = self.makeUrl(EndPoint.AUTHENTICATE_USER.value)
             userAgent = self.getUserAgent()
             headers = {
                 "User-Agent": userAgent,
@@ -42,17 +43,19 @@
             try:
                 response = requests.post(requestUrl, headers=headers, data=json.dumps(data))
                 response.raise_for_status()
             except Exception as err:
                 raise err
             else:
                 jsonResponse = response.json()
-                session = jsonResponse.get("session")
-                if session:
-                    self.token = session
+                sessionId = jsonResponse.get("session")
+                auth = jsonResponse.get("authorization")
+                if sessionId and auth:
+                    self.session = sessionId
+                    self.authorization = auth
                 else:
                     raise KlabIllegalStateException(f"Unable to authenticate for user: {username}.")
         else:
             requestUrl = self.makeUrl(EndPoint.PING.value)
             userAgent = self.getUserAgent()
             headers = {
                 "User-Agent": userAgent,
@@ -61,17 +64,16 @@
             try:
                 response = requests.get(requestUrl, headers=headers)
                 response.raise_for_status()
             except Exception as err:
                 raise err
             else:
                 jsonResponse = response.json()
-                self.token = jsonResponse.get("localSessionId")
+                self.session = jsonResponse.get("localSessionId")
 
-        return self.token
 
     def deauthenticate(self):
         # TODO this doesn't have a backend implementation yet, for now return true
         # headers = {
         #     "Authorization":self.token
         # }
         # requestUrl = self.makeUrl(EndPoint.DEAUTHENTICATE_USER.value)
@@ -80,33 +82,33 @@
         #     response.raise_for_status()
         # except Exception:
         #     return False
         # else:
         return True
 
     def isOnline(self):
-        return self.token != None
+        return self.session != None
     
-    def accept(self, mediaType:str):
+    def accept(self, mediaType: str):
         self.acceptHeader = mediaType
         return self
-	
 
-    def get(self, endpoint:str, parameters:list=None):
+    def get(self, endpoint: str, parameters: list = None):
         mediaType = "application/json"
         if self.acceptHeader:
             mediaType = self.acceptHeader
             self.acceptHeader = None
         
         requestUrl = self.makeUrl(endpoint, parameters)
         userAgent = self.getUserAgent()
         headers = {
             "User-Agent": userAgent,
             "Accept": mediaType,
-            "Authorization": self.token
+            "Authorization": self.session,
+            "Authentication": self.authorization
         }
         try:
             response = requests.get(requestUrl, headers=headers)
             response.raise_for_status()
         except Exception as err:
             raise err
         else:
@@ -114,16 +116,15 @@
                 jsonResponse = response.json()
                 return jsonResponse
             elif mediaType == 'text/plain':
                 return response.text
             else:
                 return response.content
 
-
-    def post(self, endpoint:str, request:any, pathVariables:list = None):
+    def post(self, endpoint:str, request: any, pathVariables:list = None):
         mediaType = "application/json"
         if self.acceptHeader:
             mediaType = self.acceptHeader
             self.acceptHeader = None
         
         # TODO
         # if (pathVariables != null) {
@@ -134,27 +135,26 @@
 
         requestUrl = self.makeUrl(endpoint)
         userAgent = self.getUserAgent()
         headers = {
             "User-Agent": userAgent,
             "Content-Type": "application/json",
             "Accept": mediaType,
-            "Authorization": self.token
+            "Authorization": self.session,
+            "Authentication": self.authorization
         }
 
         try:
-            response = requests.post(requestUrl, headers=headers, data=request.toJson() )
+            response = requests.post(requestUrl, headers=headers, data=request.toJson())
             response.raise_for_status()
         except Exception as err:
             raise err
         else:
             jsonResponse = response.json()
             return jsonResponse
-    
-
 
     def makeUrl(self, endpoint, parameters=[]):
         parms = ""
         if parameters:
             for i in range(0, len(parameters)):
                 if parms == "":
                     parms += "?"
@@ -182,22 +182,25 @@
 
         return f"{endpoint}{parms}"
 
     def getUserAgent(self):
         return "k.LAB/" + KLAB_VERSION + " (" + USER_AGENT_PLATFORM + ")"
 
     def getObservation(self, artifactId: str) -> ObservationReference:
-        endpoint = EndPoint.EXPORT_DATA.value.replace(P_EXPORT, Export.STRUCTURE.name.lower()).replace(P_OBSERVATION, artifactId)
+        endpoint = EndPoint.EXPORT_DATA.value.replace(P_EXPORT, Export.STRUCTURE.name.lower()).replace(P_OBSERVATION,
+                                                                                                       artifactId)
         ret = self.get(endpoint)
         if not ret or 'id' not in ret:
             return None
         return ObservationReference.fromDict(ret)
 
-    def streamExport(self, observationId: str, target: Export,  format: ExportFormat, output: io.BytesIO, parameters: list = []) -> bool:
-        endpoint = EndPoint.EXPORT_DATA.value.replace(P_EXPORT, target.name.lower()).replace(P_OBSERVATION, observationId)
+    def streamExport(self, observationId: str, target: Export,  format: ExportFormat, output: io.BytesIO,
+                     parameters: list = []) -> bool:
+        endpoint = EndPoint.EXPORT_DATA.value.replace(P_EXPORT, target.name.lower()).replace(P_OBSERVATION,
+                                                                                             observationId)
         endpoint = self.addParams(endpoint, parameters)
 
         self.accept(format.getMediaType())
 
         ret = self.get(endpoint)
         if ret:
             if format == ExportFormat.GEOJSON_FEATURES or format == ExportFormat.JSON_CODE or format == ExportFormat.ELK_GRAPH_JSON:
@@ -219,51 +222,45 @@
             elif format == ExportFormat.PNG_IMAGE or ExportFormat.BYTESTREAM:
                 output.write(ret)
                     
             return True
         else:
             return False
 
-
     def submitObservation(self, request: ObservationRequest) -> Ticket:
         """Submit context request, return ticket number or null in case of error"""
         endpoint = EndPoint.OBSERVE_IN_CONTEXT.value.replace(P_CONTEXT, request.contextId)
 
         response = self.post(endpoint, request)
         if response:
             return Ticket.fromDict(response)
         
         return None
 
-
-
-    def submitContext(self, request:ContextRequest) -> Ticket:
+    def submitContext(self, request: ContextRequest) -> Ticket:
         """Submit context request, return ticket number or null in case of error"""
         LOGGER.debug(f"submit context...")
         response = self.post(EndPoint.CREATE_CONTEXT.value, request)
         if response:
             return Ticket.fromDict(response)
         
         return None
-	
 
     def submitEstimate(self, estimateId: str) -> Ticket:
         endpoint = EndPoint.SUBMIT_ESTIMATE.value.replace(P_ESTIMATE, estimateId)
         response = self.get(endpoint)
         if response:
             return Ticket.fromDict(response)
-	
 
     def getTicket(self, ticketId: str) -> Ticket:
         LOGGER.debug(f"get ticket info...")
         ret = self.get(EndPoint.TICKET_INFO.value.replace(P_TICKET, ticketId))
         if ret and 'id' in ret:
             return Ticket.fromDict(ret)
         return None  
-        
 
 
 class TicketHandler():
     def __init__(self,  engine: Engine, ticketId: str, context: Context) -> None:
         self.engine = engine
         self.ticketId = ticketId
         self.context = context
@@ -276,15 +273,15 @@
 
     def isCancelled(self) -> bool:
         return self.cancelled
 
     def isDone(self) -> bool:
         return self.result != None
 
-    async def get(self, timeoutSeconds:int = 900):
+    async def get(self, timeoutSeconds: int = 900):
         if self.isCancelled():
             return None
         time = 0
         while not self.result:
             if time > timeoutSeconds:
                 break
             bean = self.poll(self.engine)
@@ -305,26 +302,25 @@
             return None
 
         if ticket.status == TicketStatus.RESOLVED:
             return self.processTicket(ticket)
         return None
 
     def processTicket(self, ticket: Ticket):
-        match ticket.type:
-            case TicketType.ContextEstimate:
-                return self.makeEstimate(ticket)
-            case TicketType.ObservationEstimate:
-                return self.makeEstimate(ticket)
-            case TicketType.ContextObservation:
-                return self.makeContext(ticket)
-            case TicketType.ObservationInContext:
-                return self.makeObservation(ticket)
-
-        raise KlabInternalErrorException(
-            f"unexpected ticket type: {ticket.type}")
+        if ticket.type == TicketType.ContextEstimate:
+            return self.makeEstimate(ticket)
+        elif ticket.type == TicketType.ObservationEstimate:
+            return self.makeEstimate(ticket)
+        elif ticket.type == TicketType.ContextObservation:
+            return self.makeContext(ticket)
+        elif ticket.type == TicketType.ObservationInContext:
+            return self.makeObservation(ticket)
+        else:
+            raise KlabInternalErrorException(
+                f"unexpected ticket type: {ticket.type}")
 
     def makeObservation(self,  ticket: Ticket) -> any:
         if "artifacts" in ticket.data:
             artSplit = ticket.data["artifacts"].split(",")
             for oid in artSplit:
                 bean = self.engine.getObservation(oid)
                 ret = Observation(bean, self.engine)
@@ -338,10 +334,10 @@
         context = Context(bean, self.engine)
         if "artifacts" in ticket.data:
             artSplit = ticket.data["artifacts"].split(",")
             for oid in artSplit:
                 context.notifyObservation(oid)
         return context
 
-    def makeEstimate(self,  ticket:Ticket):
+    def makeEstimate(self,  ticket: Ticket):
         return Estimate(ticket.data.get("estimate"), float(ticket.data.get("cost")),
                 ticket.data.get("currency"), ticket.type, ticket.data.get("feasible"))
```

### Comparing `klab-client-py-0.1.1/klab/exceptions.py` & `klab-client-py-0.1.2/klab/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 
 
 class KlabIllegalArgumentException(Exception):
     """Custom exception for klab illegal argument, to be extended if necessary."""
 
+
 class KlabIllegalStateException(Exception):
     """Custom exception for klab illegal state, to be extended if necessary."""
 
+
 class KlabRemoteException(Exception):
     """Custom exception for klab remote, to be extended if necessary."""
 
+
 class KlabInternalErrorException(Exception):
     """Custom exception for klab internal error, to be extended if necessary."""
 
+
 class KlabResourceNotFoundException(Exception):
-    """Custom exception for klab resources not found error, to be extended if necessary."""
+    """Custom exception for klab resources not found error, to be extended if necessary."""
```

### Comparing `klab-client-py-0.1.1/klab/geometry.py` & `klab-client-py-0.1.2/klab/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,16 +185,14 @@
     # // geometry
     # // dimensions");
     # // }
 
     def getParameters(self) -> dict:
         return self.parameters
 
-
-
     # public void setType(Type type) {
     #     this.type = type;
     # }
 
     # public void setRegular(boolean regular) {
     #     this.regular = regular;
     # }
@@ -624,15 +622,16 @@
         """
         if KlabSpace.isWKT(urn):
             self.space().shape(urn).size(1).build()
         else:
             self.space().urn(urn).size(1).build()
         return self
 
-    def grid(self, x1: float = None, x2: float = None, y1: float = None, y2: float = None, resolution: str = None, urn: str = None):
+    def grid(self, x1: float = None, x2: float = None, y1: float = None, y2: float = None, resolution: str = None,
+             urn: str = None):
         """
         A grid can be created from:
 
         1) Create a spatial polygon of multiplicity 1 from a lat/lon bounding box. 
         The box is "straight" with the X axis specifying longitude.
 
         2) same as 1 but with a resolution object (a string in the format "1 km")
```

### Comparing `klab-client-py-0.1.1/klab/klab.py` & `klab-client-py-0.1.2/klab/klab.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from .utils import DEFAULT_LOCAL_ENGINE_URL
 from .observable import Observable
 from .observation import Context, ContextRequest
 from .geometry import KlabGeometry
 from .exceptions import *
 from .ticket import Estimate, TicketType
 import asyncio
+import os
 
 import logging
 
 LOGGER = logging.getLogger(__name__)
 
 
-
 class Klab:
     """
     The main k.LAB client class. A client object represents a user session in a local or remote
     engine.
 
     Instantiate a k.LAB client using the create* methods to connect to a local or remote engine. 
     After creation, isOnline() should always be called to ensure the connection was successful. 
@@ -25,120 +25,150 @@
     on the resulting context. Using estimate provides a pattern to obtain a cost estimate for each
     operation, which depends on the size of the job and the user agreement.
     """
 
     def __init__(self, url, username=None, password=None):
         if username and password:
             self.engine = Engine(url)
-            self.session = self.engine.authenticate(username, password);
+            self.engine.authenticate(username, password)
         else:
             self.engine = Engine(url)
-            self.session = self.engine.authenticate();
-
+            self.engine.authenticate()
 
     @staticmethod
-    def create(remoteOrLocalEngineUrl = DEFAULT_LOCAL_ENGINE_URL, username = None, password = None):
+    def create(remoteOrLocalEngineUrl=DEFAULT_LOCAL_ENGINE_URL, username=None, password=None, credentialsFile=None):
         """
         Authenticate with a local or remote engine and open a new user session. Call `close()` to free
         remote resources.
 
         Parameters
         ----------
         remoteOrLocalEngineUrl: str
             the url to the remote or local engine, something like: http://127.0.0.1:8283/modeler.
             This defaults to DEFAULT_LOCAL_ENGINE_URL
         username:str
             necessary only for remote engines.
         password:str
             necessary only for remote engines.
+        credentialsFile:str
+            an optional properties file of credentials to override authentication. The format of the 
+            file is like:
             
+            ```
+            # hash is comment
+            username=myuser
+            password=mypwd
+            engine=https://myurl.org/modeler
+            ```
+
         Returns
         -------
         Klab:
             The created remote Klab instance.
         """
+
+        if credentialsFile:
+            if os.path.exists(credentialsFile):
+                with open(credentialsFile, 'r') as file:
+                    lines = file.readlines()
+                for line in lines:
+                    line = line.strip()
+                    if not line.startswith("#"):
+                        lineSplit = line.split("=")
+                        key = lineSplit[0].strip()
+                        value = lineSplit[1].strip()
+                        if key == "username":
+                            username = value
+                        elif key == "password":
+                            password = value
+                        elif key == "engine":
+                            remoteOrLocalEngineUrl = value
+
+        if not remoteOrLocalEngineUrl:
+            raise KlabIllegalArgumentException(f"No engine url has been set for user: {username}.")
+
         return Klab(remoteOrLocalEngineUrl, username, password)
 
     def isOnline(self):
         """
         Checks if the engine is online. Should always be called after creation to check on the engine status.
-        
+
         Returns
         -------
         bool:
             true is the engine is online..
         """
-        return self.engine.isOnline();
-    
+        return self.engine.isOnline()
+
     def close(self):
         if self.engine.isOnline():
-            return self.engine.deauthenticate();
+            return self.engine.deauthenticate()
         return True
-        
-    def submit(self, contextType:Observable,  geometry:KlabGeometry, *arguments:list ) -> TicketHandler:
+
+    def submit(self, contextType: Observable,  geometry: KlabGeometry, *arguments: list) -> TicketHandler:
         """
         Call with a concept and geometry to create the context observation (accepting all costs) and
         optionally further observations as semantic types or options.
-        
+
         @param contextType the type of the context. The Explorer sets that as earth:Region by
             default.
         @param geometry the geometry for the context. Use {@link GeometryBuilder} to create fluently.
         @param arguments pass semantic types for further observations to be made in the context (if
             passed, the task will finish after all have been computed). Strings will be
             interpreted as scenario URNs.
         """
 
-
         request = ContextRequest()
         request.contextType = str(contextType)
         request.geometry = geometry.encode()
         request.estimate = False
 
         LOGGER.debug(f"klab submit with: {request}")
 
         for o in arguments:
             if isinstance(o, Observable):
                 request.observables.append(o)
             elif isinstance(o, str):
                 request.scenarios.append(o)
-            
+
         if request.geometry != None and request.contextType != None:
             ticket = self.engine.submitContext(request)
             if ticket:
                 LOGGER.debug(f"got ticket: {ticket}")
                 return TicketHandler(self.engine, ticket.id, None)
 
-        raise KlabIllegalArgumentException(f"Cannot build observation request from arguments: {arguments}")
-    
-    def submitEstimate(self, estimate:Estimate) -> TicketHandler:
+        raise KlabIllegalArgumentException(
+            f"Cannot build observation request from arguments: {arguments}")
+
+    def submitEstimate(self, estimate: Estimate) -> TicketHandler:
         if estimate.ticketType != TicketType.ContextEstimate:
-            raise KlabIllegalArgumentException("the estimate passed is not a context estimate");
+            raise KlabIllegalArgumentException(
+                "the estimate passed is not a context estimate")
 
         LOGGER.debug(f"klab submit estimate with: {estimate}")
         ticket = self.engine.submitEstimate(estimate.estimateId)
         if ticket:
             LOGGER.debug(f"got ticket: {ticket}")
             return TicketHandler(self.engine, ticket.id, None)
-        
-        raise KlabIllegalStateException("estimate cannot be used");
 
+        raise KlabIllegalStateException("estimate cannot be used")
 
-    def estimate(self, contextType:Observable,  geometry:KlabGeometry, *arguments:list ) -> TicketHandler:
+    def estimate(self, contextType: Observable,  geometry: KlabGeometry, *arguments: list) -> TicketHandler:
         """
         Call with a concept and geometry to retrieve an estimate of the cost of making the context
         observation described. Add any observations to be made in the context as semantic types or
         options.
-        
+
         @param contextType the type of the context. The Explorer sets that as earth:Region by
                default.
         @param geometry the geometry for the context. Use {@link GeometryBuilder} to create fluently.
         @param arguments pass observables for further observations to be made in the context (if
                passed, the task will finish after all have been computed). Strings will be
                interpreted as scenario URNs.
-        
+
         @return a TicketHandler; call get() to wait until the estimate is ready and retrieve it.
         """
         request = ContextRequest()
         request.contextType = str(contextType)
         request.geometry = geometry.encode()
         request.estimate = True
 
@@ -152,9 +182,9 @@
 
         if request.geometry != None and request.contextType != None:
             ticket = self.engine.submitContext(request)
             if ticket:
                 LOGGER.debug(f"got estimate ticket: {ticket}")
                 return TicketHandler(self.engine, ticket.id, None)
 
-        raise KlabIllegalArgumentException(f"Cannot build estimate request from arguments: {arguments}")
-
+        raise KlabIllegalArgumentException(
+            f"Cannot build estimate request from arguments: {arguments}")
```

### Comparing `klab-client-py-0.1.1/klab/observable.py` & `klab-client-py-0.1.2/klab/observable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .exceptions import KlabIllegalStateException
 from .utils import NumberUtils
 
+
 class Range():
 
-    def __init__(self, lower:float = None, upper:float = None, lowerExclusive:bool = None, upperExclusive:bool = None):
+    def __init__(self, lower: float = None, upper: float = None, lowerExclusive: bool = None,
+                 upperExclusive: bool = None):
         self.lowerInfinite = True
         self.upperInfinite = True
         self.lowerBound = NumberUtils.NEGATIVE_INFINITY
         if lower:
             self.lowerBound = lower
             self.lowerInfinite = False
 
@@ -54,64 +56,61 @@
         if self == other:
             return True
         
         if not self.lowerInfinite and not other.lowerInfinite:
             # check lower
             if self.lowerBound >= other.lowerBound if self.lowerExclusive else self.lowerBound > other.lowerBound:
                 return False
-            
-        
+
         if not self.upperInfinite and not other.upperInfinite:
             if self.upperBound <= other.upperBound if self.upperExclusive else self.upperBound < other.upperBound:
                 return False
         
         if not self.upperInfinite and other.upperInfinite:
             return False
         
         if not self.lowerInfinite and other.lowerInfinite:
             return False
         
         return True
     
 
-
 class Observable():
     """
     Textual peer of a true observable with fluent API and minimal validation.
     Used to discriminate observables in inputs of the observation functions.
     """
 
-    def __init__(self, s:str):
+    def __init__(self, s: str):
         self._semantics = s
         self._name = None
         self._unit = None
         self._value = None
         self._range = None
 
     @staticmethod
     def create(s):
         return Observable(s)
-    
 
     def named(self, name):
         if self._name:
             raise KlabIllegalStateException("cannot add modifiers more than once")
         
         self._name = name
         return self
     
-    def range(self, range:Range):
+    def range(self, range: Range):
         if self._unit or self._range:
             raise KlabIllegalStateException("cannot add modifiers more than once")
 
         self._range = range
         return self
     
 
-    def value(self, value:any):
+    def value(self, value: any):
         if self._value:
             raise KlabIllegalStateException("cannot add modifiers more than once")
         
         self._value = value
         return self
 
     def unit(self, unit):
@@ -133,11 +132,7 @@
             string += f" in {self._unit}"
         if self._name:
             string += f" named {self._name}"
         return string
 
     def getName(self):
         return self._name
-
-
-
-
```

### Comparing `klab-client-py-0.1.1/klab/observation.py` & `klab-client-py-0.1.2/klab/observation.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,39 +75,38 @@
         names = self.reference.childIds.keys()
         for name in names:
             if id == self.reference.childIds.get(name):
                 self.catalogIds[name] = id
                 self.getObservation(name)
                 break
 
-    def exportToFile(self, target:Export,  format: ExportFormat,  path:str, parameters:list = []) -> bool:
+    def exportToFile(self, target: Export, eformat: ExportFormat,  path: str, parameters: list = []) -> bool:
         stream = io.BytesIO()
-        self.export(target, format, stream, parameters)
+        self.export(target, eformat, stream, parameters)
         with open(path, 'wb') as file:
             file.write(stream.getbuffer())
         
         return True 
 
-    def exportToString(self, target: Export, format: ExportFormat) -> str:
-        if not format.isText():
-            raise KlabIllegalArgumentException(f"illegal export format {format} for string export of {target.name}")
+    def exportToString(self, target: Export, eformat: ExportFormat) -> str:
+        if not eformat.isText():
+            raise KlabIllegalArgumentException(f"illegal export format {eformat} for string export of {target.name}")
         
         stream = io.BytesIO()
-        self.export(target, format, stream)
+        self.export(target, eformat, stream)
 
         bytesBuffer = stream.getvalue()
         return bytesBuffer.decode("utf-8")
 
-
-    def export(self, target: Export,  format: ExportFormat,  output:io.BytesIO,  parameters: list = []) -> bool:
-        if not format.isExportAllowed(target):
+    def export(self, target: Export, eformat: ExportFormat,  output:io.BytesIO,  parameters: list = []) -> bool:
+        if not eformat.isExportAllowed(target):
             raise KlabIllegalArgumentException(
                 "export format is incompatible with target")
 
-        return self.engine.streamExport(self.reference.id, target, format, output, parameters)
+        return self.engine.streamExport(self.reference.id, target, eformat, output, parameters)
 
     def getObservation(self, name: str):
         id = self.catalogIds.get(name)
         if id:
             ret = self.catalog.get(id)
             if not ret:
                 ref = self.engine.getObservation(id)
@@ -131,19 +130,19 @@
                 "getDataRange called on a non-state or null observation")
 
         return Range(lower=self.reference.dataSummary.minValue, upper=self.reference.dataSummary.maxValue)
 
     def getScalarValue(self):
         literalValue = self.reference.overallValue
         if literalValue:
-            match self.reference.valueType:
-                case ValueType.BOOLEAN:
-                    return bool(literalValue)
-                case ValueType.NUMBER:
-                    return float(literalValue)
+            if self.reference.valueType == ValueType.BOOLEAN:
+                return bool(literalValue)
+            elif self.reference.valueType == ValueType.NUMBER:
+                return float(literalValue)
+
         return literalValue
 
     def getAggregatedValue(self):
         if not self.reference or self.reference.observationType != ObservationType.STATE:
             raise KlabIllegalStateException(
                 "getDataRange called on a non-state or null observation")
 
@@ -402,16 +401,14 @@
         ticket = self.engine.submitObservation(request)
         if ticket:
             return E.TicketHandler(self.engine, ticket.id, self)
 
         raise KlabIllegalArgumentException(
             f"Cannot build observation request from arguments: {arguments}")
 
-    
-
     # @Override
     # public Future<Observation> submit(Estimate estimate) {
 
     #     if (((EstimateImpl) estimate).getTicketType() != Type.ObservationEstimate) {
     #         throw new KlabIllegalArgumentException("the estimate passed is not a context estimate");
     #     }
     #     String ticket = engine.submitEstimate(((EstimateImpl) estimate).getEstimateId());
@@ -420,37 +417,36 @@
     #         return new TicketHandler<Observation>(engine, ticket, this);
     #     }
 
     #     throw new KlabIllegalStateException("estimate cannot be used");
 
     # }
 
-    def getDataflow(self, format:ExportFormat) -> str:
-        if format != ExportFormat.ELK_GRAPH_JSON and format != ExportFormat.KDL_CODE:
-            raise KlabIllegalArgumentException(f"cannot export a dataflow to {format.name}")
+    def getDataflow(self, eformat: ExportFormat) -> str:
+        if eformat != ExportFormat.ELK_GRAPH_JSON and eformat != ExportFormat.KDL_CODE:
+            raise KlabIllegalArgumentException(f"cannot export a dataflow to {eformat.name}")
         
         stream = io.BytesIO()
-        self.engine.streamExport(self.reference.id, Export.DATAFLOW, format, stream)
+        self.engine.streamExport(self.reference.id, Export.DATAFLOW, eformat, stream)
         bytesBuffer = stream.getvalue()
         return bytesBuffer.decode("utf-8")
     
-    def getProvenance(self, simplified:bool, format:ExportFormat) -> str:
-        if format != ExportFormat.ELK_GRAPH_JSON and format != ExportFormat.KIM_CODE:
-            raise KlabIllegalArgumentException(f"cannot export the provenance graph to {format.name}")
+    def getProvenance(self, simplified: bool, eformat: ExportFormat) -> str:
+        if eformat != ExportFormat.ELK_GRAPH_JSON and eformat != ExportFormat.KIM_CODE:
+            raise KlabIllegalArgumentException(f"cannot export the provenance graph to {eformat.name}")
         
         exp = Export.PROVENANCE_FULL
         if simplified:
             exp = Export.PROVENANCE_SIMPLIFIED
 
         stream = io.BytesIO()
-        self.engine.streamExport(self.reference.id, exp, format, stream)
+        self.engine.streamExport(self.reference.id, exp, eformat, stream)
         bytesBuffer = stream.getvalue()
         return bytesBuffer.decode("utf-8")
 
-
     # @Override
     # public Context with(Observable concept, Object value) {
 
     #     if (value instanceof IGeometry) {
     #         if (concept.getName() == null) {
     #             throw new KlabIllegalStateException("observables that create objects must be given an explicit name");
     #         }
@@ -469,9 +465,8 @@
         """
         self.reference = self.engine.getObservation(self.reference.id)
         names = list(self.reference.childIds.keys())
         for name in names:
             if ret.reference.id == self.reference.childIds.get(name):
                 self.catalogIds[name] = ret.reference.id
                 self.catalog[ret.reference.id] = ret
-                break;
-
+                break
```

### Comparing `klab-client-py-0.1.1/klab/references.py` & `klab-client-py-0.1.2/klab/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .types import KimConceptType, ShapeType, ValueType, ObservationType, GeometryType, TimeResolutionType
 from .utils import NumberUtils, ExportFormat
 
+
 class ActionReference():
     """
     Describes a possible action to be performed on an observation. The engine
     sends all possible actions with each new observation and handles
     ActionRequest with action reference ID.
     
     Actions may be regular ones (with the ID to communicate to the back end along
@@ -13,40 +14,40 @@
     but a non-null downloadUrl and downloadFileExtension, which should be handled
     by the front end to produce a file download).
     
     Actions may also have sub-actions, in which case they correspond to
     sub-menus.
     """
 
-    def __init__(self, label:str = None, id:str = None) -> None:
+    def __init__(self, label:str = None, id: str = None) -> None:
         self._actionLabel = label
         self._actionId = id
         self._downloadUrl = None
         self._downloadFileExtension = None
         self._enabled = True
         self._separator = False
         self._submenu = []
 
     @staticmethod
-    def fromDict(dataMap:dict):
+    def fromDict(dataMap: dict):
         if not dataMap:
             return None
         ar = ActionReference()
         ar._actionLabel = dataMap.get('actionLabel')
         ar._actionId = dataMap.get('actionId')
         ar._downloadUrl = dataMap.get('downloadUrl')
         ar._downloadFileExtension = dataMap.get('downloadFileExtension')
         ar._enabled = dataMap.get('enabled')
         ar._separator = dataMap.get('separator')
         ar._submenu = dataMap.get('submenu')
         return ar
     
     @staticmethod
-    def fromList(dataList:list):
-        return [ ActionReference.fromDict(obj) for obj in dataList ]
+    def fromList(dataList: list):
+        return [ActionReference.fromDict(obj) for obj in dataList]
 
 
 class ScaleReference():
     """
     Used to communicate spatio/temporal regions of interest. Space values should
     be in decimal latitude and longitude.
 
@@ -84,15 +85,15 @@
         self._featureUrn = None
         self._metadata = {}
         # // FIXME REMOVE
         # private String resolutionDescription;
         # private int year = -1;
 
     @staticmethod
-    def fromDict(dataMap:dict):
+    def fromDict(dataMap: dict):
         if not dataMap:
             return None
         sr = ScaleReference()
         sr._name = dataMap.get('name')
         sr._east = dataMap.get('east')
         sr._west = dataMap.get('west')
         sr._north = dataMap.get('north')
@@ -116,42 +117,41 @@
         sr._spaceExtension = dataMap.get('spaceExtension')
         sr._spaceEnumerated = dataMap.get('spaceEnumerated')
         sr._contextId = dataMap.get('contextId')
         sr._featureUrn = dataMap.get('featureUrn')
         sr._metadata = dataMap.get('metadata')
         return sr
 
-
-
     # TODO add properties
 
     def __str__(self) -> str:
-        return f"ScaleReference [east={self.east}, west={self.west}, north={self.north}, south={self.south}, spaceScale={self.spaceScale}, resolutionDescription={self.spaceResolutionDescription}]"
+        return f"ScaleReference [east={self.east}, west={self.west}, north={self.north}, south={self.south}, " \
+               f"spaceScale={self.spaceScale}, resolutionDescription={self.spaceResolutionDescription}]"
 
 
 class ObservationExportFormat():
-    def __init__(self, label:str = None, value:str = None, adapter:str = None, extension:str = None) -> None:
+    def __init__(self, label: str = None, value: str = None, adapter: str = None, extension: str = None) -> None:
         self._label = label
         self._value = value
         self._adapter = adapter
         self._extension = extension
 
     @staticmethod
-    def fromDict(dataMap:dict):
+    def fromDict(dataMap: dict):
         if not dataMap:
             return None
         oef = ObservationExportFormat()
         oef._label = dataMap.get('label')
         oef._value = dataMap.get('value')
         oef._adapter = dataMap.get('adapter')
         oef._extension = dataMap.get('extension')
         return oef
     
     @staticmethod
-    def fromList(dataList:list):
+    def fromList(dataList: list):
         if not dataList:
             return None
         oefList = [ObservationExportFormat.fromDict(oef) for oef in dataList]
         return oefList
     
     @property
     def label(self):
@@ -181,30 +181,28 @@
     def extension(self):
         return self._extension
     
     @extension.setter
     def extension(self, extension):
         self._extension = extension
 
-        
-
 
 class DataSummary():
 
     def __init__(self) -> None:
         self._nodataProportion = 0.0
         self._minValue = NumberUtils.NaN
         self._maxValue = NumberUtils.NaN
         self._mean = NumberUtils.NaN
         self._categorized = False
         self._histogram = []
         self._categories = []
 
     @staticmethod
-    def fromDict(dataMap:dict):
+    def fromDict(dataMap: dict):
         if not dataMap:
             return None
         ds = DataSummary()
         ds._nodataProportion = dataMap.get('nodataProportion')
         ds._minValue = dataMap.get('minValue')
         ds._maxValue = dataMap.get('maxValue')
         ds._mean = dataMap.get('mean')
@@ -265,14 +263,15 @@
     def mean(self):
         return self._mean
 
     @mean.setter
     def mean(self, mean):
         self._mean = mean
 
+
 class ObservationReference():
 
     def __init__(self) -> None:
         self._shapeType = ShapeType.EMPTY
         self._encodedShape = None
         self._spatialProjection = None
         self._id = None
@@ -366,16 +365,16 @@
         obr._creationTime = dataMap.get('creationTime')  # 0
         obr._urn = dataMap.get('urn')  # None
         obr._valueCount = dataMap.get('valueCount')  # 0
         obr._previouslyNotified = dataMap.get('previouslyNotified')  # False
         obr._contextualized = dataMap.get('contextualized')  # False
         obr._lastUpdate = dataMap.get('lastUpdate')  # 0
         obr._key = dataMap.get('key')  # None
-        obr._scaleReference = ScaleReference.fromDict(dataMap.get('scaleReference') ) # None
-        obr._actions = ActionReference.fromList(dataMap.get('actions') ) # None
+        obr._scaleReference = ScaleReference.fromDict(dataMap.get('scaleReference'))   # None
+        obr._actions = ActionReference.fromList(dataMap.get('actions'))   # None
 
         return obr
 
     @property
     def shapeType(self) -> ShapeType:
         return self._shapeType
 
@@ -722,8 +721,7 @@
     @property
     def actions(self) -> str:
         return self._actions
 
     @actions.setter
     def actions(self, actions):
         self._actions = actions
-
```

### Comparing `klab-client-py-0.1.1/klab/ticket.py` & `klab-client-py-0.1.2/klab/ticket.py`

 * *Files identical despite different names*

### Comparing `klab-client-py-0.1.1/klab/types.py` & `klab-client-py-0.1.2/klab/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from .exceptions import KlabIllegalArgumentException
 from enum import Enum
 
+
 class Granularity(Enum):
         SINGLE = "SINGLE"
         MULTIPLE = "MULTIPLE"
 
+
 class DimensionType(Enum):
         NUMEROSITY = "NUMEROSITY"
         TIME = "TIME"
         SPACE = "SPACE"
 
+
 class ShapeType(Enum):
     EMPTY="EMPTY" 
     POINT="POINT" 
     LINESTRING="LINESTRING" 
     POLYGON="POLYGON" 
     MULTIPOINT="MULTIPOINT" 
     MULTILINESTRING="MULTILINESTRING" 
@@ -241,45 +244,46 @@
     """
     Corresponding to geometry #... - a folder, empty or ready to receive other
     observations. Communicated always with childrenCount == 0, children may
     arrive later.
     """
 
     @staticmethod
-    def fromValue(value:str):
+    def fromValue(value: str):
         if not value:
             return None
         for gt in GeometryType:
             if gt.value.lower() == value.lower():
                 return gt
         raise KlabIllegalArgumentException(f"No GeometryType available by the value: {value}")
 
     @staticmethod
-    def fromListToSet(value:list):
+    def fromListToSet(value: list):
         gts = set()
         for v in value:
             gt = GeometryType.fromValue(v)
             if gt:
                 gts.add(gt)
         return gts
 
+
 class TimeResolutionType(Enum):
     MILLENNIUM=0
     CENTURY=1
     DECADE=2
     YEAR=3
     MONTH=4
     WEEK=5
     DAY=6
     HOUR=7
     MINUTE=8
     SECOND=9
     MILLISECOND=10
 
     @staticmethod
-    def fromValue(value:int):
+    def fromValue(value: int):
         if not value:
             return None
         for trt in TimeResolutionType:
             if trt.value == value:
                 return trt
         raise KlabIllegalArgumentException(f"No TimeResolutionType available by the value: {value}")
```

### Comparing `klab-client-py-0.1.1/klab/utils.py` & `klab-client-py-0.1.2/klab/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 
 P_EXPORT = "{export}"
 P_CONTEXT = "{context}"
 P_OBSERVATION = "{observation}"
 P_TICKET = "{ticket}"
 P_ESTIMATE = "{estimate}"
 
+
 class Export(Enum):
     STRUCTURE = "structure"
     DATA = "data"
     VIEW = "view"
     LEGEND = "legend"
     REPORT = "report"
     DATAFLOW = "dataflow"
     PROVENANCE_FULL = "provenance_full"
     PROVENANCE_SIMPLIFIED = "provenance_simplified"
 
+
 class ExportFormat(Enum):
     PNG_IMAGE = ("image/png", [Export.DATA, Export.LEGEND, Export.VIEW])
     GEOTIFF_RASTER = ("image/tiff", [Export.DATA])
     GEOJSON_FEATURES = ("application/json", [Export.DATA])
     JSON_CODE = ("application/json", [Export.LEGEND, Export.STRUCTURE])
     KDL_CODE = ("text/plain", [Export.DATAFLOW])
     KIM_CODE = ("text/plain", [Export.PROVENANCE_FULL, Export.PROVENANCE_SIMPLIFIED])
@@ -52,53 +54,56 @@
     def getMediaType(self) -> str:
         return self.value[0]
     
     def isText(self) -> bool:
         mt = self.value[0]
         return "text/plain" == mt or "application/json" == mt or "text/csv" == mt
     
-    def isExportAllowed( self, export:Export ) -> bool:
+    def isExportAllowed(self, export: Export) -> bool:
         allowedList = self.value[1]
         return export in allowedList
     
     def __str__(self) -> str:
         return f"{self.value[0]}"
 
     @staticmethod
-    def fromMediaType(value:str):
+    def fromMediaType(value: str):
         if not value:
             return None
         for ef in ExportFormat:
             if ef.value.lower() == value.lower():
                 return ef
         raise KlabIllegalArgumentException(f"No ExportFormat available by the value: {value}")
 
     @staticmethod
-    def fromMediaTypeList(value:list):
+    def fromMediaTypeList(value: list):
         efl = []
         for v in value:
             ef = ExportFormat.fromValue(v)
             if ef:
                 efl.append(ef)
             
         return efl
         
     
 class EndPoint(Enum):
     AUTHENTICATE_USER = API_BASE + "/users/log-in"
-    """Called by users to log in and receive an authentication token for a remote engine. Duplicate from HUB. POST with username and password in data."""
+    """Called by users to log in and receive an authentication token for a remote engine. Duplicate from HUB. 
+    POST with username and password in data."""
 
     DEAUTHENTICATE_USER = API_BASE + "/users/log-out"
     """Called by users to log off from a remote engine. Duplicate from HUB."""
 
     CREATE_CONTEXT = PUBLIC_BASE + "/submit/context"
-    """Post a `ContextRequest` to create a context or get an estimate for it. Returns a ticket to poll and retrieve the outcome when done."""
+    """Post a `ContextRequest` to create a context or get an estimate for it. Returns a ticket to poll and retrieve 
+    the outcome when done."""
 
     OBSERVE_IN_CONTEXT = PUBLIC_BASE + "/submit/observation/" + P_CONTEXT
-    """Post a `ObservationRequest` to make an observation in an existing context or get an estimate for it. Returns a a ticket to poll and retrieve the outcome when done."""
+    """Post a `ObservationRequest` to make an observation in an existing context or get an estimate for it. Returns 
+    a ticket to poll and retrieve the outcome when done."""
 
     SUBMIT_ESTIMATE = PUBLIC_BASE + "/submit/estimate/" + P_ESTIMATE
     """Call as GET with an estimate ID to accept the estimate and start an observation (context
     or observation) for which an estimation was previously made. Returns the ticket
     corresponding to the running task."""
 
     EXPORT_DATA = PUBLIC_BASE + "/export/" + P_EXPORT + "/" + P_OBSERVATION
@@ -154,15 +159,14 @@
 #     P_QUERY = "{query}"
 #     """Parameter: query for any GET call used to search"""
 
 #     P_CODELIST = "{codelist}"
 #     """Parameter: a codelist name for GET requests."""
 
 
-
 #     AUTHENTICATE_USER = "/api/v2/users/log-in"
 #     """
 #     Called by users to log in and receive an authentication token for a remote engine.
 #     POST with username and password in data.
 #     """
 
 #     DEAUTHENTICATE_USER = "/api/v2/users/log-out"
@@ -188,15 +192,15 @@
         try:
             float(val)
             return True
         except ValueError:
             return False
 
     @staticmethod
-    def objectArrayFromString( array:str,  splitRegex:str, cls:type) -> list:
+    def objectArrayFromString(array: str,  splitRegex: str, cls: type) -> list:
 
         if array.startswith("["):
             array = array[1:]
         
         if array.endswith("]"):
             array = array[:-1]
         
@@ -222,39 +226,38 @@
                 #     ret[i] = Integer.parseInt(s[i].trim());
                 # } else {
                 #     ret[i] = s[i];
                 # }
         return ret
 
     @staticmethod
-    def podArrayFromString(array:str, splitRegex:str, cls):
-        pods = NumberUtils.objectArrayFromString(array, splitRegex, cls);
+    def podArrayFromString(array: str, splitRegex: str, cls):
+        pods = NumberUtils.objectArrayFromString(array, splitRegex, cls)
         iret = [None]*len(pods)
         fret = [None]*len(pods)
         bret = [None]*len(pods)
         nd = 0
         ni = 0
         cl = 0
 
         for i in  range(0, len(pods)):
             if isinstance(pods[i], float):
-                cl = 4;
+                cl = 4
                 fret[i] = pods[i]
                 nd+=1
             elif isinstance(pods[i], int):
                 cl = 2
-                iret[i] = pods[i];
+                iret[i] = pods[i]
                 ni+=1
             elif isinstance(pods[i],bool):
-                cl = 5;
+                cl = 5
                 bret[i] = pods[i]
                 ni+=1
             
-        match cl:
-            case 2:
-                return iret
-            case 4:
-                return fret
-            case 5:
-                return bret
+        if cl == 2:
+            return iret
+        elif cl == 4:
+            return fret
+        elif cl == 5:
+            return bret
         
-        raise KlabIllegalArgumentException("cannot turn array into PODs: type not handled");
+        raise KlabIllegalArgumentException("cannot turn array into PODs: type not handled")
```

### Comparing `klab-client-py-0.1.1/pyproject.toml` & `klab-client-py-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "klab-client-py"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python client to interact with a running k.LAB Engine."
 authors = [
     { name = "Ferdinando Villa" },
     { name = "Andrea Antonello" },
 ]
 dependencies = [
     "requests>=2.28.2",
```

### Comparing `klab-client-py-0.1.1/tests/test_connection.py` & `klab-client-py-0.1.2/tests/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,38 +367,17 @@
 
 
 class TestRemoteConnection(BaseTestClass, IsolatedAsyncioTestCase):
     
     def setUp(self):
         home = os.path.expanduser('~')
         credentialsFile = os.path.join(home, ".klab", "testcredentials.properties")
-        username = None
-        password = None
-        testEngine = "https://developers.integratedmodelling.org/modeler"
-        if os.path.exists(credentialsFile):
-            with open(credentialsFile, 'r') as file:
-                lines = file.readlines()
-            for line in lines:
-                line = line.strip().split("=")
-                key = line[0].strip()
-                value = line[1].strip()
-                if key == "username":
-                    username = value
-                elif key == "password":
-                    password = value
-                elif key == "engine":
-                    testEngine = value
-        else:
-            raise KlabResourceNotFoundException("Can't open ~/.klab/testcredentials.properties with username and passwords for test engine.")
-
-
-        if username and password and testEngine:
-            self.klab = Klab.create(remoteOrLocalEngineUrl=testEngine, username=username, password=password)
-        else:
-            raise KlabIllegalArgumentException("Credentials for remote mode testing not found.")
+
+        self.klab = Klab.create(credentialsFile=credentialsFile)
+
 
     def tearDown(self) -> None:
         if self.klab:
             self.assertTrue(self.klab.close())
 
 
 if __name__ == "__main__":
```

### Comparing `klab-client-py-0.1.1/tests/test_utils.py` & `klab-client-py-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `klab-client-py-0.1.1/PKG-INFO` & `klab-client-py-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: klab-client-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client to interact with a running k.LAB Engine.
 License: AGPLv3
 Author: Ferdinando Villa,Andrea Antonello
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Project-URL: homepage, https://integratedmodelling.org/
 Project-URL: repository, https://github.com/integratedmodelling/klab-client-python.git
 Description-Content-Type: text/markdown
 
 # k.LAB CLient Python
 
 A Python client library to interact with a running (local or remote) k.LAB Engine.
 
-This package is a python client for [k.LAB](https://github.com/integratedmodelling/klab). It allows registered users of k.LAB to make observations on the k.LAB semantic web from a Java program using the REST API. After creating a spatial/temporal context root observation as a context, you can submit concepts to be observed in it and the relative observations will be made at the server side and returned. Depending on the semantics submitted, the results will consists of different scientific artifacts that can be exported or inspected as needed through the API.
+This package is a python client for [k.LAB](https://github.com/integratedmodelling/klab). It allows registered users of k.LAB to make observations on the k.LAB semantic web from a Python program using the REST API. After creating a spatial/temporal context root observation as a context, you can submit concepts to be observed in it and the relative observations will be made at the server side and returned. Depending on the semantics submitted, the results will consists of different scientific artifacts that can be exported or inspected as needed through the API.
 
 While the API (both k.LAB's public REST API and the interfaces in this package) should be stable, this code is young - features are still missing and bugs certainly remain. Please submit Github issues as needed.
 
 This README assumes knowledge of k.LAB and semantic modeling. An introduction to both is available as a [technical note](https://docs.integratedmodelling.org/technote/index.html) while more extensive documentation is developed.
 
 
 ## Installation
@@ -76,12 +76,13 @@
 elevation = await ticketHandler.get()
 ```
 
 6. export the observation to a geotiff
 
 ```
 path = "your path here"
-elevation.exportToFile(Export.DATA, ExportFormat.GEOTIFF_RASTER, path)
+elevation.exportToFile(Export.DATA, ExportFormat.BYTESTREAM, path)
 ```
 
 
 **For more examples have a look at [the testcases in the repository](https://github.com/integratedmodelling/klab-client-python/tree/main/tests).**
+
```

