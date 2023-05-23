# Comparing `tmp/gkligo-0.0.9.tar.gz` & `tmp/gkligo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.0.9.tar", last modified: Fri Apr 28 13:12:21 2023, max compression
+gzip compressed data, was "gkligo-0.1.0.tar", last modified: Tue May 23 23:39:23 2023, max compression
```

## Comparing `gkligo-0.0.9.tar` & `gkligo-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.209688 gkligo-0.0.9/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.9/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.9/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 13:12:21.209123 gkligo-0.0.9/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.9/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.199647 gkligo-0.0.9/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.9/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:33:16.000000 gkligo-0.0.9/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.203371 gkligo-0.0.9/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.9/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.208300 gkligo-0.0.9/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.9/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:33:16.000000 gkligo-0.0.9/gkligo/scripts/python/__version__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.9/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.9/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.9/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     8999 2023-04-28 13:09:16.000000 gkligo-0.0.9/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.9/gkligo/scripts/python/generateGWReports.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.0.9/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.202732 gkligo-0.0.9/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      623 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-28 13:12:21.209890 gkligo-0.0.9/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.9/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.327611 gkligo-0.1.0/
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.0/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1669 2023-05-23 23:39:23.327029 gkligo-0.1.0/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.1.0/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.314180 gkligo-0.1.0/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.0/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-23 22:38:35.000000 gkligo-0.1.0/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.317675 gkligo-0.1.0/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.0/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.325653 gkligo-0.1.0/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.0/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.0/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.0/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.0/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)    13653 2023-05-23 23:09:22.000000 gkligo-0.1.0/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.1.0/gkligo/scripts/python/generateGWReports.py
+-rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.0/gkligo/scripts/python/test.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.0/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.317037 gkligo-0.1.0/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1669 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      610 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-23 23:39:23.327829 gkligo-0.1.0/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.0/setup.py
```

### Comparing `gkligo-0.0.9/PKG-INFO` & `gkligo-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.9
+Version: 0.1.0
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
+Description: # gkligo
+        Code to download GW Alert skymaps from Kafka, and optionally write them
+        out and/or convert them to MOC files at specified contours.
+        
+        The code is based on code written by Roy Williams and Leo Singer.
+        
+        It requires the following python packages:
+        
+        * gcn-kafka
+        * healpy
+        * gkutils
+        * docopt
+        * pyYAML
+        * numpy
+        * ligo.skymap
+        * astropy
+        * mocpy
+        
+        The command line utilities are:
+        * downloadGWAlert (Download the alert from Kafka)
+        
+        The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
+        Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
+        
+        The code has been daemonised so one of the parameters will be start|restart|stop.
+        
+        Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# gkligo
-Code to download GW Alert skymaps from Kafka, and optionally write them
-out and/or convert them to MOC files at specified contours.
-
-The code is based on code written by Roy Williams and Leo Singer.
-
-It requires the following python packages:
-
-* gcn-kafka
-* healpy
-* gkutils
-* docopt
-* pyYAML
-* numpy
-* ligo.skymap
-* astropy
-* mocpy
-
-The command line utilities are:
-* downloadGWAlert (Download the alert from Kafka)
-
-The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
-Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
-
-The code has been daemonised so one of the parameters will be start|restart|stop.
-
-Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
-
```

### Comparing `gkligo-0.0.9/README.md` & `gkligo-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.9/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.1.0/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Requires:
 numpy
 ligo.skymap
 astropy
 mocpy
 
 Usage:
-  %s <configFile> <action> [--writeMap] [--writeMOC] [--directory=<directory>] [--contours=<contours>] [--pidfile=<pidfile>] [--logfile=<logfile>] [--daemonErrFile=<deamonErrFile>] [--daemonOutFile=<deamonOutFile>] [--terminal]
+  %s <configFile> <action> [--writeMap] [--writeMOC] [--directory=<directory>] [--contours=<contours>] [--pidfile=<pidfile>] [--logfile=<logfile>] [--daemonErrFile=<deamonErrFile>] [--daemonOutFile=<deamonOutFile>] [--terminal] [--writemeta] [--superevents]
   %s (-h | --help)
   %s --version
 
 where action is start|stop|restart|listen
 
 If action is listen, start in non-daemon mode. Otherwise use daemon mode.
 
@@ -28,27 +28,30 @@
   --directory=<directory>           Directory to where the maps and MOCs will be written [default: /tmp].
   --contours=<contours>             Which MOC contours do you want? Multiple contours should be separated by commas, with no spaces [default: 90]
   --pidfile=<pidfile>               PID file [default: /tmp/ligo.pid]
   --logfile=<logfile>               PID file [default: /tmp/ligo.log]
   --daemonErrFile=<daemonErrFile>   Daemon Error File - for recording unexpected errors [default: /tmp/ligodaemonerr.log].
   --daemonOutFile=<daemonOutFile>   Daemon Out File - for recording unexpected output [default: /tmp/ligodaemonout.log].
   --terminal                        Override the Daemon error and out files and write to the terminal. 
+  --writemeta                       Attempt to write the event meta into a file.
+  --superevents                     Only deal with superevents. Ignore Mock and Test events.
 
 E.g.:
   %s config.yaml start --directory=/home/atls/ligo --writeMap
   %s config.yaml start --writeMap --writeMOC --directory=/tmp --contours=90
   %s config.yaml start --writeMOC --directory=/tmp --contours=90,50,10
+  %s /home/ligo/maps_gkligo/config_downloads.yaml start --directory=/home/ligo/maps_gkligo --writeMap --writeMOC --writemeta --contours=90,50,10 --superevents
 
 """
 import sys
-__doc__ = __doc__ % (sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0])
+__doc__ = __doc__ % (sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0])
 from docopt import docopt
-from __version__ import __version__
 
 from gcn_kafka import Consumer
+import yaml
 import json
 import base64
 from gkutils.commonutils import Struct, cleanOptions
 from io import BytesIO
 import daemon
 from daemon import pidfile
 import signal
@@ -113,14 +116,124 @@
     skymap = skymap[:i]
     skymap = skymap['UNIQ',]
     logger.info(skymap.info)
     skymap.write(outputMOCName, format='fits', overwrite=True)
     logger.info('MOC file %s written' % outputMOCName)
 
 
+def writeMeta(options, dataDict, logger):
+    #import MySQLdb
+    from astropy.io import fits
+
+    eventid = dataDict['superevent_id']
+    url = dataDict['urls']['gracedb']
+    far = None
+    instruments = None
+
+    mjd = None
+    distance = None
+    distanceStd = None
+    classification = None
+    properties = None
+    significant = None
+    time = None
+    group = None
+    pipeline = None
+    alertType = dataDict['alert_type']
+    timeCreated = dataDict['time_created']
+
+    try:
+        time = dataDict['event']['time']
+    except KeyError as e:
+        logger.error("Can't find the time info.")
+
+    try:
+        group = dataDict['event']['group']
+    except KeyError as e:
+        logger.error("Can't find the group info.")
+
+    try:
+        pipeline = dataDict['event']['pipeline']
+    except KeyError as e:
+        logger.error("Can't find the pipeline info.")
+
+    try:
+        classification = dataDict['event']['classification']
+    except KeyError as e:
+        logger.error("Can't find the classification info.")
+
+    try:
+        significant = dataDict['event']['significant']
+    except KeyError as e:
+        logger.error("Can't find the significance info.")
+
+    try:
+        properties = dataDict['event']['properties']
+    except KeyError as e:
+        logger.error("Can't find the properties info.")
+
+    eventMeta = {}
+
+    try:
+        far = float(dataDict['event']['far'])
+        # years = 1/(far*(24*3600*365.2425))
+    except ValueError as e:
+        logger.error("Can't find the FAR info.")
+    except KeyError as e:
+        logger.error("Can't find the FAR info.")
+
+    try:
+        instruments = dataDict['event']['instruments']
+    except KeyError as e:
+        logger.error("Can't find the instuments info.")
+
+
+    # Some info (e.g. distance) only in the FITS file
+    h = fits.open(BytesIO(base64.b64decode(dataDict['event']['skymap'])))
+    header = h[1].header
+
+    try:
+        mjd = header['MJD-OBS']
+    except KeyError as e:
+        logger.error("The MJD-OBS variable is missing.")
+
+    try:
+        distance = header['DISTMEAN']
+    except KeyError as e:
+        logger.error("The DISTMEAN variable is missing.")
+
+    try:
+        distanceStd = header['DISTSTD']
+    except KeyError as e:
+        logger.error("The DISTSTD variable is missing.")
+
+    # Do NOT write to the database, which could potentially be locked and crash the
+    # daemon. Write another script (e.g the reports script) that does that. Just
+    # record the metadata for loading.
+
+    eventMeta = {'ALERT': {'event': {'far': far,
+                                     'instruments': instruments,
+                                     'significant': significant,
+                                     'classification': classification,
+                                     'properties': properties,
+                                     'time': time,
+                                     'group': group,
+                                     'pipeline': pipeline},
+                           'urls': {'gracedb': url},
+                           'superevent_id': eventid},
+                           'alert_type': alertType,
+                           'time_created': timeCreated,
+                 'HEADER': {'MJD-OBS': mjd,
+                            'DISTMEAN': distance,
+                            'DISTSTD': distanceStd},
+                }
+
+    return eventMeta
+
+ 
 def listen(options):
     """listen.
 
     Args:
         options:
     """
     pid = os.getpid()
@@ -134,15 +247,14 @@
     formatstr = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
     formatter = logging.Formatter(formatstr)
 
     fh.setFormatter(formatter)
 
     logger.addHandler(fh)
 
-    import yaml
     with open(options.configFile) as yaml_file:
         config = yaml.safe_load(yaml_file)
 
     client_id = config['client_id']
     client_secret = config['client_secret']
     topic = config['topics']
 
@@ -153,18 +265,38 @@
 
     while True:
         # Non zero timeout is required, otherwise consume blocks termination signals.
         for message in consumer.consume(timeout=5):
             dataDict = json.loads(message.value().decode('utf-8'))
             try:
                 superEventId = dataDict['superevent_id']
+                eventType = superEventId[0] # M, T or S
+
                 alertTimeStamp = dataDict['time_created'].replace(' ','T')
                 alertType = dataDict['alert_type']
                 alertName = superEventId + '_' + alertType + '_' + alertTimeStamp
                 logger.info("Alert Received: %s" % alertName) # Future version of this script will log the output.
+
+                # Act on all events unless we only want superevents. Need to think about the logic!
+                if eventType != 'S' and options.superevents:
+                    logger.info("Skipping over this event.")
+                    # Skip to the next event
+                    continue
+
+                # Write the event meta into the databases
+                if dataDict['event'] is not None and options.writemeta:
+                    meta = writeMeta(options, dataDict, logger)
+                    if meta:
+                        for k,v in meta.items():
+                            logger.info("%s = %s" % (k, str(v)))
+                        # Overwrite the superevent info every time a new update arrives.
+                        with open(options.directory + '/' + superEventId + '.yaml', 'w') as yamlFile:
+                            yamlFile.write(yaml.dump(meta))
+
+
                 if dataDict['event'] is not None and options.writeMap:
                     skymap = dataDict['event']['skymap']
                     with open(options.directory + '/' + alertName + '.fits', 'wb') as fitsFile:
                         fitsFile.write(base64.b64decode(skymap))
 
                 if dataDict['event'] is not None and options.writeMOC:
                     for contour in options.contours.split(','):
@@ -206,15 +338,15 @@
         ) as context:
         listen(options)
 
 
 def main():
     """main.
     """
-    opts = docopt(__doc__, version=__version__)
+    opts = docopt(__doc__, version='0.0.10')
     opts = cleanOptions(opts)
 
     # Use utils.Struct to convert the dict into an object for compatibility with old optparse code.
     options = Struct(**opts)
 
 
     if options.action not in ['start', 'stop', 'restart', 'listen']:
```

### Comparing `gkligo-0.0.9/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.1.0/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.9/gkligo/scripts/python/testDaemon.py` & `gkligo-0.1.0/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.9/gkligo.egg-info/PKG-INFO` & `gkligo-0.1.0/gkligo.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.9
+Version: 0.1.0
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
+Description: # gkligo
+        Code to download GW Alert skymaps from Kafka, and optionally write them
+        out and/or convert them to MOC files at specified contours.
+        
+        The code is based on code written by Roy Williams and Leo Singer.
+        
+        It requires the following python packages:
+        
+        * gcn-kafka
+        * healpy
+        * gkutils
+        * docopt
+        * pyYAML
+        * numpy
+        * ligo.skymap
+        * astropy
+        * mocpy
+        
+        The command line utilities are:
+        * downloadGWAlert (Download the alert from Kafka)
+        
+        The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
+        Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
+        
+        The code has been daemonised so one of the parameters will be start|restart|stop.
+        
+        Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# gkligo
-Code to download GW Alert skymaps from Kafka, and optionally write them
-out and/or convert them to MOC files at specified contours.
-
-The code is based on code written by Roy Williams and Leo Singer.
-
-It requires the following python packages:
-
-* gcn-kafka
-* healpy
-* gkutils
-* docopt
-* pyYAML
-* numpy
-* ligo.skymap
-* astropy
-* mocpy
-
-The command line utilities are:
-* downloadGWAlert (Download the alert from Kafka)
-
-The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
-Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
-
-The code has been daemonised so one of the parameters will be start|restart|stop.
-
-Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
-
```

### Comparing `gkligo-0.0.9/gkligo.egg-info/SOURCES.txt` & `gkligo-0.1.0/gkligo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-LICENSE
 MANIFEST.in
 README.md
 setup.py
 gkligo/__init__.py
 gkligo/__version__.py
 gkligo.egg-info/PKG-INFO
 gkligo.egg-info/SOURCES.txt
 gkligo.egg-info/dependency_links.txt
 gkligo.egg-info/entry_points.txt
 gkligo.egg-info/requires.txt
 gkligo.egg-info/top_level.txt
 gkligo/scripts/__init__.py
 gkligo/scripts/python/__init__.py
-gkligo/scripts/python/__version__.py
 gkligo/scripts/python/config_download_example.yaml
 gkligo/scripts/python/config_reports.yaml
 gkligo/scripts/python/config_reports_example.yaml
 gkligo/scripts/python/downloadGWAlerts.py
 gkligo/scripts/python/generateGWReports.py
+gkligo/scripts/python/test.yaml
 gkligo/scripts/python/testDaemon.py
```

### Comparing `gkligo-0.0.9/setup.py` & `gkligo-0.1.0/setup.py`

 * *Files identical despite different names*

