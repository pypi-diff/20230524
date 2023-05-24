# Comparing `tmp/testery-1.6.6-py3-none-any.whl.zip` & `tmp/testery-1.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 11960 bytes, number of entries: 7
--rw-r--r--  2.0 unx    46724 b- defN 22-Aug-31 20:46 testery.py
--rw-r--r--  2.0 unx     1055 b- defN 22-Aug-31 20:46 testery-1.6.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1264 b- defN 22-Aug-31 20:46 testery-1.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-31 20:46 testery-1.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 22-Aug-31 20:46 testery-1.6.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 22-Aug-31 20:46 testery-1.6.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      548 b- defN 22-Aug-31 20:46 testery-1.6.6.dist-info/RECORD
-7 files, 49751 bytes uncompressed, 10988 bytes compressed:  77.9%
+Zip file size: 14256 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    48914 b- defN 23-May-12 01:26 testery.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 01:26 tests/__init__.py
+-rw-r--r--  2.0 unx     1631 b- defN 23-May-12 01:26 tests/conftest.py
+-rw-r--r--  2.0 unx     3314 b- defN 23-May-12 01:26 tests/test_integration.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-May-12 01:59 testery-1.6.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1264 b- defN 23-May-12 01:59 testery-1.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 01:59 testery-1.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-May-12 01:59 testery-1.6.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-May-12 01:59 testery-1.6.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      776 b- defN 23-May-12 01:59 testery-1.6.7.dist-info/RECORD
+10 files, 57120 bytes uncompressed, 12938 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
 Filename: testery.py
 Comment: 
 
-Filename: testery-1.6.6.dist-info/LICENSE
+Filename: tests/__init__.py
 Comment: 
 
-Filename: testery-1.6.6.dist-info/METADATA
+Filename: tests/conftest.py
 Comment: 
 
-Filename: testery-1.6.6.dist-info/WHEEL
+Filename: tests/test_integration.py
 Comment: 
 
-Filename: testery-1.6.6.dist-info/entry_points.txt
+Filename: testery-1.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: testery-1.6.6.dist-info/top_level.txt
+Filename: testery-1.6.7.dist-info/METADATA
 Comment: 
 
-Filename: testery-1.6.6.dist-info/RECORD
+Filename: testery-1.6.7.dist-info/WHEEL
+Comment: 
+
+Filename: testery-1.6.7.dist-info/entry_points.txt
+Comment: 
+
+Filename: testery-1.6.7.dist-info/top_level.txt
+Comment: 
+
+Filename: testery-1.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testery.py

```diff
@@ -477,14 +477,26 @@
 
     for environment in environments:
         if environment['key'] == environment_key:
             return environment
 
     raise Exception("Environment with key not found: " + environment_key)
 
+def find_test_plan_by_key(api_url, token, test_plan_key):
+    test_plans_response = requests.get(api_url + '/test-plans', headers=headers)
+
+    testplans = test_plans_response.json()
+
+    for test_plan in testplans:
+        if test_plan['key'] == test_plan_key:
+            return test_plan
+
+    raise Exception("Test Plan with key not found: " + test_plan_key)
+
+
 def find_pipeline_stage_by_name(api_url, token, pipeline_stage_name):
     stages_response = requests.get(api_url + '/pipeline-stages', headers=headers)
 
     stages = stages_response.json()
     lower_name = pipeline_stage_name.lower()
 
     for stage in stages:
@@ -778,39 +790,40 @@
             if (test_run['ended'] == False):
                 click.echo("test_run_id: %s" % test_run['id'])
             # click.echo("test_run_id: %s" % test_run['id'])
 
     if wait_for_results:
         api_wait_deploy(api_url, token, deploy_id, output, fail_on_failure)
 
+
 @click.command('cancel-test-run')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
-@click.option('--token', help='Your Testery API token.')
-@click.option('--test-run-id', help='The ID of the test run to cancel.')
+@click.option('--token', required=True, help='Your Testery API token.')
+@click.option('--test-run-id', required=True, help='The ID of the test run to cancel.')
 def cancel_test_run(testery_dev, token, test_run_id):
     """
     Cancels a test run.
     """
     headers['Authorization'] = "Bearer " + token
     api_url = get_api_url(testery_dev)
+    test_run = requests.get(f'{api_url}/test-runs/{test_run_id}', headers=headers).json()
+    status = test_run['status']
 
-    test_run = requests.get(
-        api_url + '/test-runs/' + str(test_run_id), headers=headers).json()
-
-    if test_run['status'] not in ['PASS', 'FAIL', 'CANCELED']:
-
-        test_run_response = requests.patch(api_url + '/test-runs/' + test_run_id,
+    if status not in ['PASS', 'FAIL', 'CANCELED']:
+        test_run_response = requests.patch(f'{api_url}/test-runs/{test_run_id}',
                                            headers=headers,
                                            json={"status": "CANCELED"})
 
-        print(test_run_response)
-
-        test_run = test_run_response.json()
-
-        print(test_run)
+        if test_run_response.status_code != 200:
+            raise Exception(
+                f'Failed to cancel test run {test_run_id}\n. Response: {test_run_response.status_code}'
+            )
+        click.echo(f'Canceled test run {test_run_id}')
+    else:
+        click.echo(f'Test run already done. Status: {status}')
 
 
 @click.command('add-file')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
 @click.option('--token', help='Your Testery API token.')
 @click.option('--test-run-id', help='The ID of the test run to add the file to.')
 @click.option('--kind', help='The kind of file you are uploading. For an DotCover JSON file put DotCover')
@@ -938,72 +951,106 @@
             scheduled_maintenances = status.get('scheduled_maintenances')
 
         print("Testery's scheduled maintenance is now complete. We'd like to thank you for your patience and for being such an awesome customer. Happy testing and good luck with this test run!")
 
 
 @click.command('report-test-run', help='Outputs individual test results for the entire run to the specified destination in the specified format.')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
-@click.option('--token', help='Your Testery API token.')
-@click.option('--test-run-id', help='The ID for the test run you would like to monitor and wait for.')
+@click.option('--token', required=True, help='Your Testery API token.')
+@click.option('--test-run-id', required=True, help='The ID for the test run you would like to monitor and wait for.')
 @click.option("--fail-on-failure", is_flag=True, help='When set, the testery command will return exit code 1 if there are test failures.')
 @click.option('--output', default="sonarcube", help='The format for outputting results [sonarcube]')
 @click.option('--outfile', default="results.xml", help='The filename to write the results to.')
 def report_test_run_cmd(testery_dev, token, test_run_id, fail_on_failure, output, outfile):
     api_url = get_api_url(testery_dev)
 
     api_wait_test_run(api_url, token, test_run_id, output, fail_on_failure)
 
     headers['Authorization'] = "Bearer " + token
 
-    test_run = requests.get(api_url + '/test-runs/' + str(test_run_id), headers=headers).json()
-
     test_run_results = requests.get(api_url + '/test-runs/' + str(test_run_id) + '/results', headers=headers).json()
 
     test_executions = ET.Element('testExecutions')
-    test_executions.set('version','1')
+    test_executions.set('version', '1')
 
     for test_run_result in test_run_results:
 
         file_node = ET.SubElement(test_executions, 'file')
-        file_node.set('path', test_run_result.get('fileFilter'))
+        file_node.set('path', test_run_result['projectTest']['fileFilter'])
 
         test_case_node = ET.SubElement(file_node, 'testCase')
-        test_case_node.set('name',test_run_result.get('name'))
-        test_case_node.set('duration','{0:g}'.format(test_run_result.get('duration')))
+        test_case_node.set('name', test_run_result['projectTest']['name'])
+        test_case_node.set('duration', '{0:g}'.format(test_run_result['duration']))
 
         if test_run_result.get('stackTrace'):
-            print("Stack trace: %s" % str(test_run_result.get('stackTrace')))
+            print(f"Stack trace: {test_run_result['stackTrace']}")
 
-        if test_run_result.get('status') == 'FAIL':
+        if test_run_result['status'] == 'FAIL':
             error_node = ET.SubElement(test_case_node, 'error')
             error_node.set('message', 'Failed')
             if test_run_result.get('stackTrace') is not None:
-                error_text = test_run_result.get('error') + test_run_result.get('stackTrace')
+                error_text = test_run_result['error'] + test_run_result['stackTrace']
             else:
-                error_text = test_run_result.get('error')
+                error_text = test_run_result['error']
             error_node.text = error_text
-        elif test_run_result.get('status') == 'IGNORED':
-            error_node.set('message', 'Skipped')
+        elif test_run_result['status'] == 'IGNORED':
             error_node = ET.SubElement(test_case_node, 'skipped')
+            error_node.set('message', 'Skipped')
             error_node.text = "Test was marked as ignored."
-        elif test_run_result.get('status') == 'PASS':
+        elif test_run_result['status'] == 'PASS':
             # No error node needed
             pass
         else:
-            error_node.set('message', 'Unrecognized test status')
             error_node = ET.SubElement(test_case_node, 'error')
-            error_node.text = "Unrecognized status: %s" % test_run_result.get('status')
+            error_node.set('message', 'Unrecognized test status')
+            error_node.text = f"Unrecognized status: {test_run_result['status']}"
 
+    xml_data = ET.tostring(test_executions)
+    with open(outfile, "wb") as xml_file:
+        xml_file.write(xml_data)
 
 
-    # Write output
+@click.command('run-test-plan')
+@click.option('--testery-dev', is_flag=True, default=False, hidden=True)
+@click.option('--token', required=True, help='Your Testery API token.')
+@click.option('--environment-key', default=None, help='Which environment you would like to run your tests against.')
+@click.option('--test-plan-key', required=True, default=None, help='The key of the test plan to run.')
+def run_test_plan(testery_dev, token, environment_key,  test_plan_key):
+    """
+    Submits a Test Plan run to the Testery platform.
+    """
+
+    wait_for_maintenance_window()
+
+    headers['Authorization'] = "Bearer " + token
+    api_url = get_api_url(testery_dev)
+
+    test_plan_run_request = {}
+
+    test_plan_id = find_test_plan_by_key(api_url, token, test_plan_key)["id"]
+
+    if environment_key is not None:
+        environment_id = find_environment_by_key(api_url, token, environment_key)["id"]
+        test_plan_run_request["environmentId"] = environment_id
+
+    test_run_response = requests.post(f'{api_url}/test-plans/{test_plan_id}/runs',
+                                      headers=headers,
+                                      json=test_plan_run_request)
+
+    if test_run_response.status_code != 200:
+        if test_run_response.status_code == 404:
+            message = f'Failed to create test run for test plan id {test_plan_id}.'
+        else:
+            message = f'Failed to create test run, status code:  {test_run_response.status_code}.'
+
+        raise Exception(message)
+    else:
+        test_run = test_run_response.json()
+        click.echo(f"test_plan_run_id: {test_run['id']} in status {test_run['status']}")
 
-    xml_data = ET.tostring(test_executions)
-    xml_file = open(outfile, "wb")
-    xml_file.write(xml_data)
 
 cli.add_command(create_environment)
 cli.add_command(update_environment)
 cli.add_command(upload_environment_file)
 cli.add_command(delete_environment)
 
 cli.add_command(create_schedule)
@@ -1016,10 +1063,11 @@
 cli.add_command(report_test_run_cmd)
 cli.add_command(add_file)
 cli.add_command(monitor_test_run)
 cli.add_command(monitor_test_runs)
 cli.add_command(verify_token)
 cli.add_command(load_users)
 cli.add_command(upload_build_artifacts)
+cli.add_command(run_test_plan)
 
 if __name__ == '__main__':
     cli()
```

## Comparing `testery-1.6.6.dist-info/LICENSE` & `testery-1.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `testery-1.6.6.dist-info/METADATA` & `testery-1.6.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testery
-Version: 1.6.6
+Version: 1.6.7
 Summary: Testery CLI
 Home-page: https://github.com/testery/testery-cli
 Author: Testery
 Author-email: chris.harbert@testery.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

