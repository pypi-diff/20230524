# Comparing `tmp/thoughtful-1.9.0.tar.gz` & `tmp/thoughtful-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-1.9.0.tar", max compression
+gzip compressed data, was "thoughtful-2.0.0rc0.tar", max compression
```

## Comparing `thoughtful-1.9.0.tar` & `thoughtful-2.0.0rc0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0     4450 2022-10-21 22:43:49.374262 thoughtful-1.9.0/README.md
--rw-r--r--   0        0        0     2088 2022-10-21 22:43:49.405760 thoughtful-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      184 2022-10-21 22:43:49.375159 thoughtful-1.9.0/supervisor/__init__.py
--rw-r--r--   0        0        0       54 2022-10-21 22:43:49.375253 thoughtful-1.9.0/supervisor/__version__.py
--rw-r--r--   0        0        0     5370 2022-10-21 22:43:49.375384 thoughtful-1.9.0/supervisor/default_instances.py
--rw-r--r--   0        0        0      888 2022-10-21 22:43:49.375490 thoughtful-1.9.0/supervisor/dynamic.py
--rw-r--r--   0        0        0     7099 2022-10-21 22:43:49.375636 thoughtful-1.9.0/supervisor/main_context.py
--rw-r--r--   0        0        0    13010 2022-10-21 22:43:49.375863 thoughtful-1.9.0/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2022-10-21 22:43:49.375905 thoughtful-1.9.0/supervisor/py.typed
--rw-r--r--   0        0        0     6543 2022-10-21 22:43:49.376069 thoughtful-1.9.0/supervisor/recorder.py
--rw-r--r--   0        0        0        0 2022-10-21 22:43:49.376170 thoughtful-1.9.0/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     1010 2022-10-21 22:43:49.376288 thoughtful-1.9.0/supervisor/reporting/record.py
--rw-r--r--   0        0        0     2006 2022-10-21 22:43:49.376417 thoughtful-1.9.0/supervisor/reporting/report.py
--rw-r--r--   0        0        0     6809 2022-10-21 22:43:49.376554 thoughtful-1.9.0/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      659 2022-10-21 22:43:49.376648 thoughtful-1.9.0/supervisor/reporting/status.py
--rw-r--r--   0        0        0     1496 2022-10-21 22:43:49.376743 thoughtful-1.9.0/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2022-10-21 22:43:49.376843 thoughtful-1.9.0/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1870 2022-10-21 22:43:49.376932 thoughtful-1.9.0/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     8197 2022-10-21 22:43:49.377063 thoughtful-1.9.0/supervisor/step_context.py
--rw-r--r--   0        0        0     8140 2022-10-21 22:43:49.377227 thoughtful-1.9.0/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0     1764 2022-10-21 22:43:49.377339 thoughtful-1.9.0/supervisor/streaming_callback.py
--rw-r--r--   0        0        0     5653 2022-10-21 22:43:49.916624 thoughtful-1.9.0/setup.py
--rw-r--r--   0        0        0     5902 2022-10-21 22:43:49.916929 thoughtful-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-12-14 17:25:44.942523 thoughtful-2.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     2992 2023-03-22 17:30:28.308693 thoughtful-2.0.0rc0/README.md
+-rw-r--r--   0        0        0     1947 2023-05-24 19:52:08.900768 thoughtful-2.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-03-07 23:35:15.321689 thoughtful-2.0.0rc0/thoughtful/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-24 19:52:15.741990 thoughtful-2.0.0rc0/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-05-24 14:49:11.094869 thoughtful-2.0.0rc0/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2022-12-14 17:25:44.949518 thoughtful-2.0.0rc0/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-24 14:49:11.095347 thoughtful-2.0.0rc0/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0     8598 2023-05-24 14:25:56.931578 thoughtful-2.0.0rc0/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2022-12-14 17:25:44.949966 thoughtful-2.0.0rc0/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2022-12-14 17:25:44.949991 thoughtful-2.0.0rc0/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2022-12-14 17:25:44.950159 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2619 2023-05-24 14:48:54.309495 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1125 2023-05-24 14:48:54.309801 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2131 2023-02-23 21:00:49.643195 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10192 2023-05-24 14:48:54.310046 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      659 2022-12-14 17:25:44.950571 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      883 2023-05-24 14:25:56.932274 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2022-12-14 17:25:44.951007 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1870 2022-12-14 17:25:44.951071 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7643 2023-05-24 14:48:54.310467 thoughtful-2.0.0rc0/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     7462 2023-05-24 14:49:04.525171 thoughtful-2.0.0rc0/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-01-30 21:43:52.785761 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-06 19:41:20.157278 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     3087 2023-05-24 14:49:11.095696 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/callback.py
+-rw-r--r--   0        0        0     3184 2023-05-24 14:48:54.311303 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     4233 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc0/setup.py
+-rw-r--r--   0        0        0     4554 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc0/PKG-INFO
```

### Comparing `thoughtful-1.9.0/pyproject.toml` & `thoughtful-2.0.0rc0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,62 @@
 [tool.poetry]
 name = "thoughtful"
-version = "1.9.0"
-description = "Supervisor is a Workflow Engine for Digital Workers that generates a detailed telemetric log at runtime called a Work Report"
+version = "2.0.0rc0"
+description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <engineering@thoughtfulautomation.com>"]
-license = "MIT"
+license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtfulautomation.com"
-repository = "https://github.com/thoughtful-automation/supervisor"
-documentation = "https://thoughtful-automation.github.io/supervisor"
+repository = "https://github.com/thoughtful-automation/thoughtful"
+documentation = "https://readthedocs.com/projects/thoughtful-supervisor/"
 
 keywords = ['rpa', 'robot-framework', 'robocorp', 'automation']
 
 classifiers = [
   "Topic :: Security :: Cryptography",
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: Apache Software License",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Library",
   "Framework :: Robot Framework :: Tool",
 ]
 
-packages = [{ include = "supervisor" }]
-include = [{ path = "supervisor/py.typed" }]
-
-[[tool.poetry.source]]
-name = "codeartifact"
-url = "https://thoughtful-automation-975753646808.d.codeartifact.us-east-1.amazonaws.com/pypi/thoughtful-automation/"
-secondary = true
+packages = [{ include = "thoughtful" }]
+include = [{ path = "thoughtful/py.typed" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8,<3.12"
 pyyaml = ">=5.4.1"
 chevron = "^0.14.0"
 pyconfs = "^0.5.5"
 pydantic = "^1.8.2"
 pre-commit = "^2.17.0"
 pydantic-yaml = "^0.6.3"
 isodate = "^0.6.1"
 boto3 = "^1.24.64"
 aws-requests-auth = "^0.4.3"
 moto = "^4.0.5"
+requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
 mkdocs = "^1.2.3"
 datamodel-code-generator = "^0.11.14"
 mkdocstrings = "^0.16.2"
-pytest = "^6.2.5"
+pytest = "^7.2.0"
 pytest-cov = "^2.12.1"
 pytest-watch = "^4.2.0"
 pytest-sugar = "^0.9.4"
 pytest-timeout = "^2.0.2"
 syrupy = "^1.5.0"
 tox = "^3.2.3"
 yapf = "^0.31.0"
 pylint = "^2.11.1"
-pre-commit = "^2.15.0"
+pre-commit = "^2.21.0"
 devtools = "^0.8.0"
-isort = "^5.10.1"
-autoflake = "^1.4"
+isort = "^5.12.0"
+autoflake = "^1.7.8"
 # This specifically needs to be exactly 1.0.0
 bump2version = "1.0.0"
 Sphinx = "^4.4.0"
 sphinx-rtd-theme = "^1.0.0"
 requests-mock = "^1.10.0"
 
 [tool.datamodel-codegen]
```

### Comparing `thoughtful-1.9.0/supervisor/default_instances.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/default_instances.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,127 +15,99 @@
     - a ``StepContext`` named ``step_context``,
     - a function to set step statuses called ``set_step_status``,
     - and a function to set record statuses called ``set_record_status``.
 
 See the quickstart for, well, quickstarts on each of these methods.
 """
 
-
 import logging
-import os
 import pathlib
-import warnings
 from typing import Optional, Union
-from urllib.parse import urlparse
-
-import boto3
-from aws_requests_auth.aws_auth import AWSRequestsAuth
 
-from supervisor.main_context import MainContext
-from supervisor.recorder import Recorder
-from supervisor.reporting.report_builder import ReportBuilder
-from supervisor.step_context import StepContext
-from supervisor.step_decorator_factory import create_step_decorator
-from supervisor.streaming_callback import StreamingCallback
+from thoughtful.environment_variables import EnvironmentVariables
+from thoughtful.supervisor.main_context import MainContext
+from thoughtful.supervisor.manifest import Manifest
+from thoughtful.supervisor.reporting.report_builder import ReportBuilder
+from thoughtful.supervisor.step_context import StepContext
+from thoughtful.supervisor.step_decorator_factory import create_step_decorator
+from thoughtful.supervisor.streaming.callback import StreamingCallback
 
 logger = logging.getLogger(__name__)
 
+# Share a streaming callback variable, but we can't set it until a user
+# provides a JWT token.
+streamer = StreamingCallback(
+    run_id=EnvironmentVariables().run_id,
+    callback_url=EnvironmentVariables().callback_url,
+    # The JWT token is set by the user later. If steamer is set to None,
+    # then the step decorators can't be updated to stream if streamer is
+    # changed to a new instance.
+    #
+    # See CX-2368 for the proper fix by lifting the streamer out of the contexts
+    jwt_token="",
+)
+
 #: A shared ``ReportBuilder`` for steps and step contexts to add step reports
 #: to.
 report_builder = ReportBuilder()
 
-#: A shared ``Recorder`` for steps and step contexts to record messages to.
-recorder = Recorder()
-
 #: Use this decorator on your own functions to mark what workflow step each
 #: Python function is matched to.
-step = create_step_decorator(report_builder, recorder)
+step = create_step_decorator(report_builder, streamer)
 
 #: Use this function to mark a step as failed.
 #: This is just a shortcut for ``set_step_status(step_id, "failed")``.
 #: Exposes ``report_builder.fail_step``.
 fail_step = report_builder.fail_step
 
 #: Expose the report builder's ability to override a step's status as a
 #: top-level call. Exposes ``report_builder.set_step_status``.
 set_step_status = report_builder.set_step_status
 
 #: Expose the report builder's ability to override a step's record's status as a
 #: top-level call. Exposes ``report_builder.set_record_status``.
 set_record_status = report_builder.set_record_status
 
-# If callback url is in environment, we will stream to that url
-streaming_callback: Optional[StreamingCallback] = None
-if callback_url := os.environ.get("SUPERVISOR_CALLBACK_URL"):
-    credentials = boto3.Session().get_credentials()
-    host = urlparse(callback_url).hostname
-    aws_auth = AWSRequestsAuth(
-        aws_access_key=credentials.access_key,
-        aws_secret_access_key=credentials.secret_key,
-        aws_token=credentials.token,
-        aws_host=host,
-        aws_region="us-east-1",
-        aws_service="execute-api",
-    )
-    streaming_callback = StreamingCallback.from_env_defaults(aws_auth)
+#: Expose the report builder's ability to override a run's status as a
+#: top-level call. Exposes ``report_builder.set_run_status``.
+set_run_status = report_builder.set_run_status
 
 
 # noinspection PyPep8Naming
 class step_scope(StepContext):
     """
     It's a context manager that provides a scope for a step using the
     aforementioned default instances of ``report_builder`` and ``recorder``.
     """
 
-    def __init__(self, *step_id, record_id: Optional[str] = None):
+    def __init__(self, step_id: str):
         """
         A default `StepContext` that uses the root level `report_builder` and
         `recorder`.
 
         Args:
             *step_id: The list of integers that represent the step ID.
-            record_id: An optional ID of the record being actively processed
         """
         super().__init__(
             report_builder,
-            recorder,
-            *step_id,
-            streaming_callback=streaming_callback,
-            record_id=record_id,
-        )
-
-
-# noinspection PyPep8Naming
-class substep(step_scope):
-    """
-    The deprecated version of ``step_scope``.
-    """
-
-    def __init__(self, *step_id):
-        warnings.simplefilter("once", DeprecationWarning)
-        warnings.warn(
-            f"`{self.__class__.__name__}` has been renamed to `step_scope`. "
-            f"Please use that class name instead.",
-            DeprecationWarning,
-            stacklevel=2,
+            step_id,
+            streaming_callback=streamer,
         )
-        warnings.simplefilter("default", DeprecationWarning)
-        super().__init__(*step_id)
 
 
 # noinspection PyPep8Naming
 class supervise(MainContext):
     """
     It's a context manager that provides a scope for the main context using the
     aforementioned default instances of ``report_builder`` and ``recorder``.
     """
 
     def __init__(
         self,
-        manifest: Union[str, pathlib.Path] = "manifest.yaml",
+        manifest: Union[Manifest, str, pathlib.Path] = "manifest.yaml",
         output_dir: Union[str, pathlib.Path] = "output/",
         *args,
         **kwargs,
     ):
         """
         A default `MainContext` that uses the root level `report_builder` and
         `recorder`.
@@ -145,13 +117,14 @@
             **kwargs: Extra keyword arguments to the `MainContext` constructor.
             manifest (str): The digital worker's manifest definition
             output_dir (str): Where the work report and drift report will
                 be written to
         """
         super().__init__(
             report_builder=report_builder,
-            recorder=recorder,
             manifest=manifest,
             output_dir=output_dir,
+            upload_uri=EnvironmentVariables().s3_bucket_uri,
+            streaming_callback=streamer,
             *args,
             **kwargs,
         )
```

### Comparing `thoughtful-1.9.0/supervisor/main_context.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/main_context.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from __future__ import annotations
 
 import datetime
 import logging
 import os
 import pathlib
 from types import TracebackType
-from typing import Callable, List, Optional, Type, Union
+from typing import Callable, Optional, Type, Union
 from urllib.parse import urlparse
 
 import boto3
 
-from supervisor.manifest import Manifest
-from supervisor.recorder import Recorder
-from supervisor.reporting.report_builder import ReportBuilder
-from supervisor.reporting.status import Status
+from thoughtful.supervisor.manifest import Manifest
+from thoughtful.supervisor.reporting.report_builder import ReportBuilder
+from thoughtful.supervisor.reporting.status import Status
+from thoughtful.supervisor.streaming.callback import StreamingCallback
 
 logger = logging.getLogger(__name__)
 
 
 class MainContext:
     """
     Supervises an entire digital worker run and generates a work report
@@ -59,60 +59,85 @@
         with supervise(callback=print_work_report):
             main()
     """
 
     def __init__(
         self,
         report_builder: ReportBuilder,
-        recorder: Recorder,
-        manifest: Union[str, pathlib.Path],
+        manifest: Union[Manifest, str, pathlib.Path],
         output_dir: Union[str, pathlib.Path],
+        upload_uri: Optional[str] = None,
         callback: Optional[Callable] = None,
+        streaming_callback: Optional[StreamingCallback] = None,
     ):
         """
         Args:
             report_builder (ReportBuilder): A ReportBuilder object that will
                 receive the step reports and provide the run report.
-            recorder (Recorder): A Recorder object that will record optional
                 messages and logs throughout the process execution.
             manifest (str, Path): A pathlike object that points to the manifest
                 file for the process.
             output_dir (str, Path): A pathlike object that points to the output
                 directory for the process. This will receive the run report and
                 output manifest.
+            upload_uri (str, optional): A URI to upload the output files to.
             callback (callable, optional): a function that is invoked with three
                 parameters: the current context (as the `MainContext` instance)
                 and the `Report` generated from this digital worker's run.
         """
         self.report_builder = report_builder
-        self.recorder = recorder
-        self.manifest_path = pathlib.Path(manifest)
         self.output_path = pathlib.Path(output_dir)
+        self.upload_uri = upload_uri
 
+        self.manifest_path = (
+            manifest if isinstance(manifest, (str, pathlib.Path)) else None
+        )
+        self.manifest = self._parse_manifest(manifest)
         self.callback = callback
+        self.streaming_callback = streaming_callback
+
+    @staticmethod
+    def _parse_manifest(
+        manifest: Union[Manifest, str, pathlib.Path]
+    ) -> Optional[Manifest]:
+        if isinstance(manifest, Manifest):
+            return manifest
+        manifest_path = pathlib.Path(manifest)
+        try:
+            manifest = Manifest.from_file(manifest_path)
+            return manifest
+        except Exception:
+            logger.exception("warning: could not read manifest")
+        return None
 
     def __enter__(self) -> MainContext:
         """
         Logic for when this context is first started. Attempts to load the
         manifest and returns itself as the context.
 
         Returns:
             MainContext: This instance.
         """
-        # Check if the manifest exists and warn if it doesn't
-        if self.manifest_path.exists():
-            # Check if manifest is valid, and warn if it isn't
-            try:
-                _ = Manifest.from_file(self.manifest_path)
-            except Exception as e:
-                logger.exception("warning: could not read manifest")
-        else:
-            logger.warning(f"{self.manifest_path=} does not exist")
+        if self.manifest and self.streaming_callback:
+            self.streaming_callback.post_manifest(self.manifest)
+        self._stream_run_status_change(Status.RUNNING)
+
         return self
 
+    def set_run_status(self, status: Union[Status, str]) -> None:
+        """
+        Sets the run status of the process. This is the final status of the
+        process, and will be used to determine the status of the run report.
+
+        Args:
+            status (Union[Status, str]): The status to set.
+        """
+        self.report_builder.set_run_status(status)
+        self._stream_run_status_change(status)
+
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> bool:
         """
@@ -120,67 +145,84 @@
         by a raised Exception or now.
 
         Returns:
             bool: True if the parent caller should ignore the
                 Exception raised before entering this function
                 (if any), False otherwise.
         """
-        self.report_builder.status = Status.FAILED if exc_type else Status.SUCCEEDED
+        if exc_type:
+            self.report_builder.run_had_exception = True
         work_report = self.report_builder.to_report()
 
+        self._stream_run_status_change(work_report.status)
+
         # Create the output directory if it doesn't already exist
         self.output_path.mkdir(parents=True, exist_ok=True)
 
         # Write the work report
         work_report_path = self._safe_report_path(file_prefix="run-report")
         work_report.write(work_report_path)
 
         # Write the manifest back out as a JSON file
-        manifest_json_path = self.output_path / "manifest.json"
-        Manifest.yaml_to_json(self.manifest_path, manifest_json_path)
+        if self.manifest:
+            manifest_json_path = self.output_path / "manifest.json"
+            self.manifest.write_to_json_file(manifest_json_path)
 
         # Run the user-defined callback
         if self.callback:
             self.callback(self, work_report)
 
         # Upload output files to S3
-        if upload_uri := os.getenv("SUPERVISOR_ARTIFACT_UPLOAD_URI"):
+        if self.upload_uri:
             try:
-                self.upload_output_files_to_s3(upload_uri)
+                self._upload_output_files_to_s3(self.upload_uri)
             except Exception:
                 logger.exception("Failed to upload output files to S3")
-        else:
+        elif os.environ.get("ROBOCORP_HOME") is None:
             logger.warning(
                 "SUPERVISOR_ARTIFACT_UPLOAD_URI is not set. Artifacts"
                 " will not be uploaded to S3."
             )
 
         # Explicitly return false so that the parent caller above
         # this context sees the exception (if any)
         return False
 
-    def upload_output_files_to_s3(self, upload_uri: str) -> None:
+    def _stream_run_status_change(self, status: Status) -> None:
+        """
+        Post a status change to the stream callback if it exists.
+        """
+        if self.streaming_callback:
+            self.streaming_callback.post_status_change(status)
+
+    def _upload_output_files_to_s3(self, upload_uri: str) -> None:
         """
         It uploads all files in the output directory to S3. It requires the
         environment variable `SUPERVISOR_ARTIFACT_UPLOAD_URI` to be set with
         the S3 URI to upload the files to.
+
+        Args:
+            upload_uri (str): The S3 URI to upload the files to.
         """
         s3_client = boto3.client("s3")
-        upload_uri = urlparse(upload_uri.strip())
-        bucket = upload_uri.hostname
-        path = upload_uri.path.strip("/")
+        parsed_upload_uri = urlparse(upload_uri.strip())
+        bucket = parsed_upload_uri.hostname
+        path = parsed_upload_uri.path.strip("/")
 
         for file in self.output_path.glob("*"):
             try:
                 if file.is_file():
                     obj = f"{path}/{file.name}" if path else file.name
                     s3_client.upload_file(str(file), bucket, obj)
             except Exception:
                 logger.exception(f"Failed to upload {file} to S3")
 
+        if self.streaming_callback:
+            self.streaming_callback.post_artifacts_uploaded(output_uri=upload_uri)
+
     def _safe_report_path(self, file_prefix: str) -> pathlib.Path:
         """
         A ``pathlib.Path`` instance that points to a new work report writable
         location that is safe across all OSes.
 
         Returns:
             pathlib.Path: The path to the new report to be written.
```

### Comparing `thoughtful-1.9.0/supervisor/manifest.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/manifest.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,82 +24,55 @@
       succeeded: Finished
       failed: Error
 
     workflow:
       - step_id: 1
         title: Prepare for Process
         description: do this
-        step_type: sequential
         steps:
           - step_id: 1.1
             title: Get Credentials from Bitwarden
             description: do that
-            step_type: sequential
           - step_id: 1.2
             title: Get mapping files
             description: |-
               Get the mapping files from the server
-            step_type: sequential
             columns:
               succeeded: Done
               warning: Warning!
             steps:
               - step_id: 1.2.1
                 title: Get mapping file from S3
       - step_id: 2
         title: Populate job postings
         description: do this
-        step_type: sequential
         steps:
           - step_id: 2.1
             title: Aya Connect
             description: Just your average step
-            step_type: sequential
 
 The columns attributes are optional, as are each of their three values. If you
 choose to override the record status column titles at the base, it will be the
 default throughout the entire workflow. If you choose to override the record
 status column titles at the step level, it will be the default for that step
 only.
 """
 
 from __future__ import annotations
 
 import json
 import pathlib
 from collections import defaultdict
-from enum import Enum
-from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing import Any, List, Optional, TypeVar, Union
 
 import pydantic
 import yaml
 from pydantic import validator
 from pydantic_yaml import YamlModel
 
-
-class StepType(str, Enum):
-    """
-    This enum was relevant in the past, but is no longer used. It will soon
-    be removed. Originally it would identify the flow that Supervisor would
-    follow when choosing what step to execute next, but as supervisor no longer
-    manages the flow, this is no longer relevant.
-    """
-
-    SEQUENTIAL = "sequential"
-    """at this point, sequential steps are the only type of step that
-    Supervisor supports."""
-    CONDITIONAL = "conditional"
-    """str, Deprecated: conditional steps are no longer supported."""
-    BRANCH = "branch"
-    """str, Deprecated: branch steps are no longer supported."""
-    # Use "unknown" for steps indicated by the dev that aren't in the manifest
-    UNKNOWN = "unknown"
-    """str, Deprecated: unknown steps are no longer supported."""
-
-
 StepId = TypeVar("StepId", bound=str)
 
 
 class RecordStatusColumns(YamlModel):
     """
     Columns is a list of column names that are used to display the
     output of a step in a table. When left blank, the default values
@@ -109,42 +82,45 @@
     default for that step only.
     """
 
     succeeded: Optional[str]
     """
     str, optional: The name of the column that contains the succeeded records.
     """
+
     failed: Optional[str]
     """
     str, optional: The name of the column that contains the failed records.
     """
+
     warning: Optional[str]
     """
     str, optional: The name of the column that contains the warning records.
     """
 
+    def __json__(self):
+        return {
+            "succeeded": self.succeeded,
+            "failed": self.failed,
+            "warning": self.warning,
+        }
+
 
 class Step(YamlModel):
     """
     A step to execute in a manifest workflow. This is an attribute of the
     ``Manifest`` yaml model. Each step can contain a list of ``Step`` yaml
     models, allowing for a tree of sub-steps to be defined.
     """
 
     step_id: str
     """
     str: The ID of the step.
     """
 
-    step_type: StepType
-    """
-    StepType, Deprecated: The type of step. This was relevant in the past when
-    Supervisor managed process flow, but is no longer used.
-    """
-
     title: str
     """
     str: The name of the step.
     """
 
     description: Optional[str]
     """
@@ -152,34 +128,14 @@
     """
 
     steps: Optional[List[Step]] = None
     """
     List[Step], optional: A list of children steps. Empty list if no children.
     """
 
-    branches: Optional[Dict[Any, Any]]
-    """
-    dict, optional, Deprecated: A dictionary of branches to execute. This was
-    used in the past to support conditional steps, but is no longer used.
-    """
-
-    when_false: Optional[str]
-    """
-    str, optional, Deprecated: The next step ID if the previous step returned
-    `False`. This was used in the past to support conditional steps, but is no
-    longer used.
-    """
-
-    when_true: Optional[str]
-    """
-    str, optional, Deprecated: The next step ID if the previous step returned
-    `True`. This was used in the past to support conditional steps, but is no
-    longer used.
-    """
-
     columns: Optional[RecordStatusColumns]
     """
     RecordStatusColumns, optional: The columns to display in the UI for record
     statuses. If none, it will use manifest defaults.
     """
 
     # PyCharm can't recognize that `@validator` creates a class method
@@ -187,45 +143,22 @@
     @validator("steps", pre=True, always=True)
     def set_steps(cls, steps):
         """
         Validator: Set the steps attribute to an empty list if it is None.
         """
         return steps or []
 
-    @classmethod
-    def to_flat_dict(cls, steps: List[Step]) -> Dict[str, Step]:
-        """
-        Creates a flat dictionary of a list of steps, where each step's children
-        is added to the flat dictionary.
-
-        Args:
-            steps (List[Step]): The steps to flatten.
-
-        Returns:
-            Dict[str, Step]: The steps as a flat dict. The keys are the step IDs
-                and the values are the ``Step`` s.
-        """
-        flat = {}
-        for step in steps:
-            flat[step.step_id] = step
-            child_values = Step.to_flat_dict(step.steps)
-            flat.update(child_values)
-
-        return flat
-
-    @property
-    def has_children(self) -> bool:
-        """
-        Says whether this instance has children ``Step`` s.
-
-        Returns:
-            bool: True if this instance has children, False otherwise.
-
-        """
-        return True if self.steps and len(self.steps) else False
+    def __json__(self):
+        return {
+            "step_id": self.step_id,
+            "title": self.title,
+            "description": self.description,
+            "steps": [step.__json__() for step in self.steps],
+            "columns": self.columns.__json__() if self.columns else self.columns,
+        }
 
 
 class Manifest(YamlModel):
     """
     A digital worker manifest, typically read from a `manifest.yaml` file.
     """
 
@@ -261,27 +194,14 @@
     """
 
     workflow: List[Step]
     """
     List[Step]: The list of steps to execute.
     """
 
-    steps_by_id: Optional[Dict]
-    """
-    dict, optional: The same ``Step`` s as `self.workflow`, but as a dictionary,
-    where the keys are the ``Step`` IDs.
-    """
-
-    def set_steps_by_id(self) -> None:
-        """
-        After loading from a YAML/dict, this function creates a dictionary
-        that maps step IDs to steps.
-        """
-        self.steps_by_id = Step.to_flat_dict(self.workflow)
-
     @classmethod
     def from_file(cls, filename: Union[str, pathlib.Path]) -> Manifest:
         """
         Creates an instance of this class from a YAML file.
 
         Args:
             filename: The name of the manifest .yaml file.
@@ -302,15 +222,14 @@
             raise ValueError(error_message) from ex
 
         # The base importer loads the steps as dicts, so convert them into
         # proper steps
         step_dicts = manifest_in_flight.workflow
         final_steps: List[Step] = cls._load_manifest_file_steps(step_dicts)
         manifest_in_flight.workflow = final_steps
-        manifest_in_flight.set_steps_by_id()
 
         return manifest_in_flight
 
     @classmethod
     def yaml_to_json(
         cls,
         manifest_path: Union[str, pathlib.Path],
@@ -336,22 +255,29 @@
         Returns the values of this instance as a dictionary that are needed
         for a report.
         Returns:
             dict: The JSON-able dictionary (of only primitives) representation
                 of this instance.
         """
         # Only return the keys we want in the report
-        keys = ["uid", "name", "description", "author", "source"]
-        value = {k: v for k, v in self.__dict__.items() if k in keys}
-        return value
+        keys = ["uid", "name", "description", "author", "source", "columns"]
+        manifest_json = {k: v for k, v in self.__dict__.items() if k in keys}
+        manifest_json["workflow"] = [step.__json__() for step in self.workflow]
+        return manifest_json
+
+    def write_to_json_file(self, json_path):
+        _json = self.__json__()
+        with open(json_path, "w+") as json_file:
+            json.dump(_json, json_file)
 
     # Private implementation
-
     @classmethod
-    def _load_manifest_file_steps(cls, step_dicts: List[dict]) -> List[Step]:
+    def _load_manifest_file_steps(
+        cls, step_dicts: List[Union[dict, Step]]
+    ) -> List[Step]:
         """
         Creates a list of Step instances based on a list of steps in dictionary
         format (usually loaded from a raw YAML file).
 
         Args:
             step_dicts: The steps as dictionaries to parse.
```

### Comparing `thoughtful-1.9.0/supervisor/reporting/report.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from __future__ import annotations
 
 import json
 import pathlib
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
-from supervisor.__version__ import __version__
-from supervisor.reporting.status import Status
-from supervisor.reporting.step_report import StepReport
-from supervisor.reporting.timed_report import TimedReport
+from thoughtful.__version__ import __version__
+from thoughtful.supervisor.reporting.record_report import RecordReport
+from thoughtful.supervisor.reporting.status import Status
+from thoughtful.supervisor.reporting.step_report import StepReport
+from thoughtful.supervisor.reporting.timed_report import TimedReport
 
 
 @dataclass
 class Report(TimedReport):
     """
     Report: A report is a representation of a run's execution. This dataclass
     contains all the information that will be stored in the run report,
@@ -27,15 +28,15 @@
     """
 
     supervisor_version = str(__version__)
     """
     str: The version of the supervisor that generated the report.
     """
 
-    workflow: List[StepReport] = field(default_factory=list)
+    workflow: List[Union[StepReport, RecordReport]] = field(default_factory=list)
     """
     List[StepReport]: The list of steps that were executed.
     """
 
     status: Optional[Status] = None
     """
     Status, optional: The status of the run.
```

### Comparing `thoughtful-1.9.0/supervisor/reporting/report_builder.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,62 @@
 to a ``Report`` object containing the list of ``StepReport`` objects.
 
 It returns this ``Report`` object as the final product of the run.
 """
 
 from __future__ import annotations
 
+import copy
 import datetime
 import time
-from collections import defaultdict
+import warnings
+from collections import OrderedDict, defaultdict
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Tuple, Union
 
-from supervisor.manifest import StepId
-from supervisor.recorder import DataLog, MessageLog
-from supervisor.reporting.record import Record
-from supervisor.reporting.report import Report
-from supervisor.reporting.status import Status
-from supervisor.reporting.step_report import StepReport
-from supervisor.reporting.timer import Timer
+from thoughtful.supervisor.manifest import StepId
+from thoughtful.supervisor.reporting.record import Record
+from thoughtful.supervisor.reporting.record_report import RecordReport
+from thoughtful.supervisor.reporting.report import Report
+from thoughtful.supervisor.reporting.status import Status
+from thoughtful.supervisor.reporting.step_report import StepReport
+from thoughtful.supervisor.reporting.timer import Timer
+
+
+@dataclass
+class RecordAccumulator:
+    records_by_id: Dict[RecordId, Record] = field(default_factory=OrderedDict)
+
+    def upsert(self, record: Record):
+        """Insert a new Record, or update the record if it already exists."""
+        self.records_by_id[record.record_id] = record
+
+    def exists(self, _id: RecordId) -> bool:
+        return _id in self.records_by_id.keys()
+
+    def soft_update(self, record: Record):
+        """
+        Update a record *only* if it doesn't exist *or* the current status is
+        RUNNING, otherwise do nothing.
+        """
+        if (
+            self.exists(record.record_id)
+            and self.records_by_id[record.record_id].status != Status.RUNNING
+        ):
+            return
+        self.upsert(record)
+
+    def to_reports(self, base_step_report: StepReport) -> List[RecordReport]:
+        return [
+            RecordReport.from_step_report(base_step_report, record)
+            for record in self.records_by_id.values()
+        ]
+
+    def __iter__(self) -> Iterable[Record]:
+        return iter(self.records_by_id.values())
 
 
 @dataclass
 class StepReportBuilder:
     """
     Builds a dynamic digital worker step. This is similar to the ``StepReport``
     except that this is higher level in that it contains unflattened data
@@ -48,46 +83,62 @@
     """
 
     end_time: Optional[datetime.datetime] = None
     """
     datetime.datetime: The end time of the step.
     """
 
-    message_log: MessageLog = field(default_factory=list)
+    _record_accumulator: RecordAccumulator = field(default_factory=RecordAccumulator)
     """
-    MessageLog: The message log of the step.
+    RecordAccumulator: Holds records that were processed by this step.
     """
 
-    data_log: DataLog = field(default_factory=list)
-    """
-    DataLog: The data log of the step.
-    """
+    def to_reports(self) -> List[StepReport]:
+        step_report = self._to_report()
+        record_reports: List[StepReport] = self._record_accumulator.to_reports(
+            step_report
+        )
+        return record_reports + [step_report]
 
-    record: Optional[Record] = None
-    """
-    Record, optional: The record of the step.
-    """
+    # NOTE: optional fields for message & metadata
+    # use **metadata instead?
+    def set_record_status(
+        self,
+        record_id: RecordId,
+        status: Status,
+        message: Optional[str] = None,
+        metadata: Optional[dict] = None,
+        is_soft_update: bool = False,
+    ):
+        message = message or ""
+        metadata = metadata or {}
+        new_record = Record(record_id, status, message, metadata)
+        if is_soft_update:
+            self._record_accumulator.soft_update(new_record)
+        else:
+            self._record_accumulator.upsert(new_record)
+
+    @property
+    def records(self) -> Tuple[Record]:
+        return tuple(self._record_accumulator)
 
-    def to_report(self) -> StepReport:
+    def _to_report(self) -> StepReport:
         """
         An easily "jsonable" final report on this step's execution.
 
         Returns:
             StepReport: A final report on this step's execution.
         """
 
         # Build the report
         return StepReport(
             step_id=self.step_id,
             status=self.status,
             start_time=self.start_time,
             end_time=self.end_time,
-            message_log=self.message_log,
-            data_log=self.data_log,
-            record=self.record,
         )
 
 
 RecordId = str
 
 
 @dataclass
@@ -98,15 +149,15 @@
     """
 
     timer: Timer = field(default_factory=Timer)
     """
     Timer: The timer used to time the execution of the workflow.
     """
 
-    workflow: List[StepReportBuilder] = field(default_factory=list)
+    step_report_builders: List[StepReportBuilder] = field(default_factory=list)
     """
     List[StepReportBuilder]: The list of step reports.
     """
 
     timer_start: float = time.perf_counter()
     """
     float: The start time of the workflow.
@@ -119,23 +170,32 @@
 
     # These steps will be overridden with the specified status when the
     # `Report` is written
     _step_statuses_to_override: Dict[StepId, Status] = field(default_factory=dict)
     """
     Dict[StepId, Status]: The statuses to override for each step
     """
-
-    _record_statuses_to_override: Dict[StepId, Dict[RecordId, Status]] = field(
+    _records_to_override: Dict[StepId, Dict[RecordId, Record]] = field(
         default_factory=lambda: defaultdict(dict)
     )
     """
     Dict[StepId, Dict[RecordId, Status]]: The statuses to override for each
     record
     """
 
+    run_had_exception: bool = False
+    """
+    Boolean value to indicate if the run terminated on an exception.
+    """
+
+    _run_status_override: Optional[Status] = None
+    """
+    Override the status of the run to be in the status of `status`.
+    """
+
     def __post_init__(self):
         self.timer.start()
 
     def fail_step(self, step_id: str) -> None:
         """
         Override a step to be in the `StepStatus.ERROR` state. Note: this
         overrides every step with this ID, so if the step ran multiple times
@@ -157,57 +217,89 @@
             status (Status | str): The status to override the step to.
         """
         # Convert the status to the correct type if necessary
         safe_status = Status(status)
         self._step_statuses_to_override[step_id] = safe_status
 
     def set_record_status(
-        self, step_id: str, record_id: str, status: Union[Status, str]
+        self,
+        step_id: str,
+        record_id: str,
+        status: Union[Status, str],
+        message: Optional[str] = None,
+        metadata: Optional[dict] = None,
     ) -> None:
         """
         Override a record to be in the status of `status`. Note: this
         overrides every step with this step ID and this record ID, so if the
         step ran multiple times in the workflow, they will all be marked as
         this `status`.
 
         Args:
             step_id (str): The step id a specific step that contains this record
             record_id (str): The id of the record to override.
             status (Status | str): The status to override the record to.
         """
         # Convert the status to the correct type if necessary
+        message = message or ""
+        metadata = metadata or {}
+        safe_status = Status(status)
+        self._records_to_override[step_id][record_id] = Record(
+            record_id=record_id, status=safe_status, message=message, metadata=metadata
+        )
+
+    def set_run_status(self, status: Union[Status, str]) -> None:
+        """
+        Manually set the status of the bot run. If not set, the run
+        status will be determined automatically
+
+        Args:
+            status (Union[Status, str]): The status to override the run to.
+        """
+        # Convert the status to the correct type if necessary
         safe_status = Status(status)
-        self._record_statuses_to_override[step_id][record_id] = safe_status
+        self._run_status_override = safe_status
 
     def to_report(self) -> Report:
         """
         Convert supervisor workflow to work report. It is here that we
         convert the entire workflow to a list of ``StepReport`` objects.
         After which, we pass over the entire list overriding the record
         and step statuses according to the ``_step_statuses_to_override``
-        and ``_record_statuses_to_override`` dictionaries.
+        and ``_records_to_override`` dictionaries.
 
         Returns:
             Report: The finalized work report.
         """
         timed = self.timer.end()
 
-        # Update step reports with any overridden statuses
-        steps = [x.to_report() for x in self.workflow]
-        for step_report in steps:
-            # Update step statuses
-            if step_report.step_id in self._step_statuses_to_override:
-                new_status = self._step_statuses_to_override[step_report.step_id]
-                step_report.status = new_status
-            # Update the record statuses
-            if step_report.step_id in self._record_statuses_to_override:
-                records = self._record_statuses_to_override[step_report.step_id]
-                if step_report.record.record_id in records:
-                    new_status = records[step_report.record.record_id]
-                    step_report.record.status = new_status
+        for step_builder in self.step_report_builders:
+            # Override the step status if requested
+            if step_builder.step_id in self._step_statuses_to_override:
+                new_status = self._step_statuses_to_override[step_builder.step_id]
+                step_builder.status = new_status
+            # Override any of the step's record statuses if requested
+            if step_builder.step_id in self._records_to_override:
+                records = self._records_to_override[step_builder.step_id]
+                # NOTE: need to make change here from status - ReportBuilder saving
+                # Records instead of just status - in self._records_to_override
+                for record_id, record in records.items():
+                    step_builder.set_record_status(
+                        record_id, record.status, record.message, record.metadata
+                    )
+
+        # Merge all the step reports together
+        final_workflow = [
+            report for step in self.step_report_builders for report in step.to_reports()
+        ]
+
+        # Set the run status
+        self.status = Status.FAILED if self.run_had_exception else Status.SUCCEEDED
+        if self._run_status_override is not None:
+            self.status = self._run_status_override
 
         return Report(
             start_time=timed.start,
             end_time=timed.end,
-            workflow=steps,
+            workflow=final_workflow,
             status=self.status,
         )
```

### Comparing `thoughtful-1.9.0/supervisor/reporting/status.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.9.0/supervisor/reporting/timed_report.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.9.0/supervisor/reporting/timer.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.9.0/supervisor/step_context.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/step_context.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The step context is a context manager that is used to supervise a single step
 of a digital worker. It is used in lieu of the ``@step`` decorator for
 situations when you do not want to write a function for a step. For example,
 it is very useful when iterating over a list of items:
 
 .. code-block:: python
 
-    from supervisor import supervise, step_scope
+    from thoughtful.supervisor import supervise, step_scope
 
     def times_two(integers: list) -> None:
         return integers * 2
 
     def times_three(integer: int) -> None:
         return integer * 3
 
@@ -37,80 +37,66 @@
 
 from __future__ import annotations
 
 import warnings
 from types import TracebackType
 from typing import Optional, Type, Union
 
-from supervisor.recorder import Recorder
-from supervisor.reporting.record import Record
-from supervisor.reporting.report_builder import ReportBuilder, StepReportBuilder
-from supervisor.reporting.status import Status
-from supervisor.reporting.timer import Timer
-from supervisor.streaming_callback import StreamingCallback
+from thoughtful.supervisor.reporting.report_builder import ReportBuilder
+from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
+from thoughtful.supervisor.reporting.status import Status
+from thoughtful.supervisor.reporting.timer import Timer
+from thoughtful.supervisor.streaming.callback import StreamingCallback
 
 
 class StepContext:
     """
     A context manager for a step that is running inside another step.
     This is an alternative to ``@step`` decorator when you don't want
     to write an entire function for a step.
     """
 
     def __init__(
         self,
         builder: ReportBuilder,
-        recorder: Recorder,
-        *step_id,
-        record_id: Optional[str] = None,
+        step_id: Union[str, int],
         streaming_callback: Optional[StreamingCallback] = None,
     ):
         """
         Args:
             builder: Where the step report will be written.
-            recorder: Where messages and data logs will be written.
             *step_id: The step id of this step, ie `"1.1"`
-            record_id: An optional ID of the record being actively processed
             streaming_callback (StreamingCallback, optional): If set, streams
                 the status of work report steps to that callback handler.
                 Defaults to `None`.
         """
-        if len(step_id) > 1:
-            warnings.warn(
-                "Passing multiple step ids to StepContext is deprecated. "
-                "Instead, pass a single step id string with dots, ie '1.1'",
-                DeprecationWarning,
-            )
-
-        self.uuid = ".".join([str(n) for n in step_id])
+        self.step_id = str(step_id)
         self.report_builder = builder
-        self.recorder = recorder
         self.timer = Timer()
         self._status_override: Optional[Status] = None
-        self.record_id: Optional[str] = record_id
-        self._record_status_override: Optional[Status] = None
-        self._streaming_callback = streaming_callback
+        self.streaming_callback = streaming_callback
+        self.step_report_builder: StepReportBuilder
 
     def __enter__(self):
         """
         Logic for when this context is first started.
 
         Returns:
             MainContext: This instance.
         """
         start_time = self.timer.start()
-        self.step_report = StepReportBuilder(
-            step_id=self.uuid,
+        self.step_report_builder = StepReportBuilder(
+            step_id=self.step_id,
             start_time=start_time,
             status=Status.RUNNING,
-            message_log=self.recorder.messages,
-            data_log=self.recorder.data,
         )
-        if self._streaming_callback:
-            self._streaming_callback.post_step_update(self.step_report.to_report())
+
+        if self.streaming_callback:
+            for report in self.step_report_builder.to_reports():
+                self.streaming_callback.post_step_update(report)
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
@@ -126,33 +112,24 @@
         """
         timed_info = self.timer.end()
         if self._status_override:
             step_status = self._status_override
         else:
             step_status = Status.FAILED if exc_type else Status.SUCCEEDED
 
-        if self._record_status_override:
-            record_status = self._record_status_override
-        else:
-            record_status = Status.FAILED if exc_type else Status.SUCCEEDED
+        # Update step report with finished step details
+        self.step_report_builder.end_time = timed_info.end
+        self.step_report_builder.status = step_status
+
+        # Stream reports if requested
+        if self.streaming_callback:
+            for report in self.step_report_builder.to_reports():
+                self.streaming_callback.post_step_update(report)
 
-        record = Record(self.record_id, record_status) if self.record_id else None
-
-        new_report = StepReportBuilder(
-            step_id=self.uuid,
-            start_time=timed_info.start,
-            end_time=timed_info.end,
-            status=step_status,
-            message_log=self.recorder.messages,
-            data_log=self.recorder.data,
-            record=record,
-        )
-        self.report_builder.workflow.append(new_report)
-        if self._streaming_callback:
-            self._streaming_callback.post_step_update(self.step_report.to_report())
+        self.report_builder.step_report_builders.append(self.step_report_builder)
 
         # Return False so that any exceptions inside this context
         # are still raised after this function ends
         return False
 
     def error(self) -> None:
         """
@@ -201,26 +178,33 @@
                 ]
             }
         """
         # Convert the status to the correct type if necessary
         safe_status = Status(status)
         self._status_override = safe_status
 
-    def set_record_status(self, status: Union[str, Status]) -> None:
+    def set_record_status(
+        self,
+        status: Union[str, Status],
+        record_id: str = "",
+        message: Optional[str] = None,
+        metadata: Optional[dict] = None,
+    ) -> None:
         """
         Override a step context's record to be in the status of ``status``
 
         Args:
             status (str, Status): The status to set the record to
+            record_id (str): The ID of the record
 
         .. code-block:: python
 
-            with step_scope("1.1", record_id="kaleb_cool_guy") as s:
+            with step_scope("1.1") as s:
                 ...  # do some stuff
-                s.set_record_status("warning")
+                s.set_record_status("warning", "record01")
 
         .. code-block:: json
 
             {
                 "workflow": [
                     {
                         "step_id": "1.1",
@@ -231,30 +215,32 @@
                         }
                     }
                 ]
             }
 
         """
         # Convert the status to the correct type if necessary
-        if not self.record_id:
-            warnings.warn(
-                "Setting a record status for a step without "
-                "a record ID will have no effect",
-                UserWarning,
-            )
+        if message is not None and not type(message) == str:
+            raise ValueError("Record message must be a string")
+        if metadata is not None and not type(metadata) == dict:
+            raise ValueError("Record metadata must be a dict")
+
+        message = message or ""
+        metadata = metadata or {}
         safe_status = Status(status)
-        self._record_status_override = safe_status
+        self.step_report_builder.set_record_status(
+            record_id, safe_status, message, metadata
+        )
 
 
 if __name__ == "__main__":
     report_builder = ReportBuilder()
-    r = Recorder()
 
     substep = StepContext
 
-    with substep(report_builder, r, 1) as s:
+    with substep(report_builder, 1) as s:
         print("hello world")
 
-        with substep(report_builder, r, 1, 1) as s2:
+        with substep(report_builder, "1.1") as s2:
             print("inner step")
 
-    print(report_builder.workflow)
+    print(report_builder.step_report_builders)
```

### Comparing `thoughtful-1.9.0/supervisor/step_decorator_factory.py` & `thoughtful-2.0.0rc0/thoughtful/supervisor/step_decorator_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains the functions necessary to fuel the step decorator
 factory function ``create_step_decorator``. This step decorator—``@step``—is
 used to supervise the execution of a function in a digital worker.
 
 .. code-block:: python
 
-    from supervisor import supervise, step
+    from thoughtful.supervisor import supervise, step
 
     @step("1.1")
     def times_two(integers: list) -> None:
         return integers * 2
 
     @step("1.2")
     def times_three(integer: int) -> None:
@@ -57,50 +57,51 @@
 
 from __future__ import annotations
 
 import contextlib
 import functools
 import json
 import logging
-import warnings
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, Union
 
-from supervisor.recorder import Recorder
-from supervisor.reporting.record import Record
-from supervisor.reporting.report_builder import ReportBuilder, StepReportBuilder
-from supervisor.reporting.status import Status
-from supervisor.reporting.timer import Timer
+from thoughtful.supervisor.reporting.report_builder import ReportBuilder
+from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
+from thoughtful.supervisor.reporting.status import Status
+from thoughtful.supervisor.reporting.timer import Timer
+from thoughtful.supervisor.streaming.callback import StreamingCallback
 
 
 def create_step_decorator(
-    report_builder: ReportBuilder, recorder: Recorder
+    report_builder: ReportBuilder,
+    streaming_callback: Optional[StreamingCallback] = None,
 ) -> Callable:
     """
     A step decorator generator that as input receives a ``ReportBuilder``
     object and a ``Recorder`` object. The returned decorator will use these
     objects to record the execution of the decorated function.
 
     Note that the return type here is `Any`, because proper type hinting
     for decorators is not yet obvious. PEP 612 specifies a way to type
     hint decorators starting in 3.10, but this project supports >= 3.7. See
     more here: https://stackoverflow.com/a/68290080/2597913.
 
     Args:
         report_builder (ReportBuilder): The report builder to use to record
             the execution of the decorated function.
-        recorder (Recorder): The recorder to use to record the execution of
-            the decorated function.
+        streaming_callback (StreamingCallback, optional): If set, streams
+            the status of work report steps to that callback handler.
+            Defaults to `None`.
 
     Returns:
         Any: A decorator to attach to functions.
     """
 
     # The decorator to be returned as the property
     # This handles the inputs to the decorator itself
-    def returned_decorator(*step_id):
+    def returned_decorator(step_id: Union[str, int]):
         """
         A decorator to mark a function as the implementation of a step in a
         digital worker's manifest.
 
         To include a `supervisor_record_id`, pass it to the decorated function
         as a kwarg. For example,
         ```
@@ -108,38 +109,42 @@
             def my_func(*args, supervisor_record_id: str):
                 do stuff
                 ...
 
             my_func(supervisor_record_id="my_record_id")
         ```
         """
-        step_id = _step_id_from_args(step_id)
 
         # The decorator to grab the function callable itself
         def inner_decorator(fn):
             # And the wrapper around the function to call it with its
             # args and kwargs arguments
             @functools.wraps(fn)
             def wrapper(*fn_args, **fn_kwargs):
                 return _run_wrapped_func(
-                    fn, step_id, report_builder, recorder, *fn_args, **fn_kwargs
+                    fn,
+                    str(step_id),
+                    report_builder,
+                    streaming_callback,
+                    *fn_args,
+                    **fn_kwargs,
                 )
 
             return wrapper
 
         return inner_decorator
 
     return returned_decorator
 
 
 def _run_wrapped_func(
     fn: Callable,
     step_id: str,
     report_builder: ReportBuilder,
-    recorder: Recorder,
+    streaming_callback: StreamingCallback,
     *fn_args: Optional[Any],
     **fn_kwargs: Optional[Any],
 ) -> Any:
     """
     Runs `fn` with the given args `args` and `kwargs`, times how long it
     takes to run, and records the execution of this function under `step_id`
     in the work report.
@@ -153,95 +158,60 @@
 
     Returns:
     Any: Whatever is returned by executing the function
     """
 
     """Set up the step"""
     caught_exception: Optional[Exception] = None
-    step_final_status: Status
+    final_status: Status
 
     # Time the function
     func_timer = Timer()
     func_timer.start()
 
+    this_steps_report_builder = StepReportBuilder(
+        step_id=step_id,
+        start_time=func_timer.start_time,
+        end_time=None,
+        status=Status.RUNNING,
+    )
+
+    if streaming_callback:
+        for report in this_steps_report_builder.to_reports():
+            streaming_callback.post_step_update(report)
+
     """Run the step"""
     try:
         fn_result = fn(*fn_args, **fn_kwargs)
-        step_final_status = Status.SUCCEEDED
-        record_final_status = Status.SUCCEEDED
+        final_status = Status.SUCCEEDED
     except Exception as ex:
         fn_result = None
         caught_exception = ex
-        step_final_status = Status.FAILED
-        record_final_status = Status.FAILED
+        final_status = Status.FAILED
     timer_result = func_timer.end()
 
-    """Step teardown"""
-    # this checks if a record id was passed to the function and sets record_id
-    # as none if it is not included in the kwargs
-    record_id: str = fn_kwargs.get("supervisor_record_id")
-    record = Record(record_id, record_final_status) if record_id else None
-
-    # Create a new step report
-    new_report = StepReportBuilder(
-        step_id=step_id,
-        start_time=timer_result.start,
-        end_time=timer_result.end,
-        status=step_final_status,
-        message_log=recorder.messages,
-        data_log=recorder.data,
-        record=record,
-    )
-    report_builder.workflow.append(new_report)
-
-    # Reset the recorder for the next step
-    recorder.messages = []
-    recorder.data = []
+    # Finish the report
+    this_steps_report_builder.end_time = timer_result.end
+    this_steps_report_builder.status = final_status
+    report_builder.step_report_builders.append(this_steps_report_builder)
+
+    if streaming_callback:
+        for report in this_steps_report_builder.to_reports():
+            streaming_callback.post_step_update(report)
 
     """Passthrough the step's return value or raised exception"""
     # If the step failed and raised an exception, raise that instead
     # of returning None
     if caught_exception:
         raise caught_exception
 
     # Passthrough the function's returned data back up
     return fn_result
 
 
-def _step_id_from_args(args: tuple) -> str:
-    """
-    Joins decorator number args into a step ID string. This was more necessary
-    when the user was expected to pass in a series of integers as the step ID,
-    but now it's just a string. This is still here for backwards compatibility.
-
-    For example,
-    ```
-        @step(1, 2, 3)
-        def my_func():
-            ...
-    ```
-    would return "1.2.3".
-
-
-    Args:
-        args (tuple): The arguments to the decorator.
-
-    Returns:
-        str: The step ID.
-    """
-    if len(args) > 1:
-        warnings.warn(
-            "Passing multiple step ids to StepContext is deprecated. "
-            "Instead, pass a single step id string with dots, ie '1.1'",
-            DeprecationWarning,
-        )
-
-    return ".".join([str(arg) for arg in args])
-
-
 def to_safe_jsonable(value: Any) -> Any:
     """
     Returns a version of `value` that can be converted into JSON
     format using the `json` library.
 
     Args:
         value: The value to ensure is safe to JSON serialize.
```

