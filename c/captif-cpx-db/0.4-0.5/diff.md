# Comparing `tmp/captif_cpx_db-0.4.tar.gz` & `tmp/captif_cpx_db-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.4.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.5.tar", max compression
```

## Comparing `captif_cpx_db-0.4.tar` & `captif_cpx_db-0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/LICENSE
--rw-r--r--   0        0        0       16 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/README.md
--rw-r--r--   0        0        0      257 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0       30 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/constants.py
--rw-r--r--   0        0        0     3284 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/__init__.py
--rw-r--r--   0        0        0      244 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/sa_helpers.py
--rw-r--r--   0        0        0    11287 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/segment.py
--rw-r--r--   0        0        0     7437 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/session.py
--rw-r--r--   0        0        0      504 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/LICENSE
+-rw-r--r--   0        0        0       16 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/README.md
+-rw-r--r--   0        0        0      257 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/captif_cpx_db/constants.py
+-rw-r--r--   0        0        0     3284 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/captif_cpx_db/models/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/captif_cpx_db/models/sa_helpers.py
+-rw-r--r--   0        0        0    11303 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/captif_cpx_db/models/segment.py
+-rw-r--r--   0        0        0     7437 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/captif_cpx_db/models/session.py
+-rw-r--r--   0        0        0      504 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.5/PKG-INFO
```

### Comparing `captif_cpx_db-0.4/LICENSE` & `captif_cpx_db-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.4/captif_cpx_db/models/__init__.py` & `captif_cpx_db-0.5/captif_cpx_db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.4/captif_cpx_db/models/segment.py` & `captif_cpx_db-0.5/captif_cpx_db/models/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,20 +166,20 @@
     wheel_bay_name: str = Field(
         primary_key=True,
         description="wheel_bay name ('left' or 'right')",
     )
     ir_temperatures: List["IRTemperature"] = Relationship()
     microphone_details: List["SegmentMicrophoneDetails"] = Relationship()
     wheel_bay_third_octave_levels: List["WheelBayThirdOctaveLevels"] = Relationship()
-    laeq_db: float = Field(
-        nullable=False,
+    laeq_db: Optional[float] = Field(
+        default=None,
         description="LAeq for the wheel bay in dB (no CPX corrections applied)",
     )
-    lcpx_db: float = Field(
-        nullable=False,
+    lcpx_db: Optional[float] = Field(
+        default=None,
         description="LCPX for the wheel bay in dB",
     )
 
 
 class IRTemperature(SQLModel, table=True):
     """
     Average tyre or road temperature across a road segment for a wheel bay
```

### Comparing `captif_cpx_db-0.4/captif_cpx_db/models/session.py` & `captif_cpx_db-0.5/captif_cpx_db/models/session.py`

 * *Files identical despite different names*

