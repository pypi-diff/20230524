# Comparing `tmp/googleads-8.1.0.tar.gz` & `tmp/googleads-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/googleads-8.1.0.tar", last modified: Wed Oct 11 22:05:15 2017, max compression
+gzip compressed data, was "dist/googleads-9.0.0.tar", last modified: Tue Nov 14 21:49:55 2017, max compression
```

## Comparing `googleads-8.1.0.tar` & `googleads-9.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-x---   0 msaniscalchi (185017) eng       (5000)        0 2017-10-11 22:05:15.000000 googleads-8.1.0/
-drwxr-x---   0 msaniscalchi (185017) eng       (5000)        0 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads.egg-info/
--rw-r-----   0 msaniscalchi (185017) eng       (5000)        1 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads.egg-info/dependency_links.txt
--rw-r-----   0 msaniscalchi (185017) eng       (5000)      117 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads.egg-info/requires.txt
--rw-r-----   0 msaniscalchi (185017) eng       (5000)     2325 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads.egg-info/PKG-INFO
--rw-r-----   0 msaniscalchi (185017) eng       (5000)       10 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads.egg-info/top_level.txt
--rw-r-----   0 msaniscalchi (185017) eng       (5000)      317 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads.egg-info/SOURCES.txt
--rw-r-----   0 msaniscalchi (185017) eng       (5000)     8947 2017-10-11 22:04:05.000000 googleads-8.1.0/README
-drwxr-x---   0 msaniscalchi (185017) eng       (5000)        0 2017-10-11 22:05:15.000000 googleads-8.1.0/googleads/
--rw-r-----   0 msaniscalchi (185017) eng       (5000)    74879 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/adwords.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)    11435 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/util.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)      710 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/__init__.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)    12682 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/oauth2.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)    34593 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/dfp.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)    32890 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/common.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)     4005 2017-10-11 22:04:05.000000 googleads-8.1.0/googleads/errors.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)     2325 2017-10-11 22:05:15.000000 googleads-8.1.0/PKG-INFO
--rwxr-x---   0 msaniscalchi (185017) eng       (5000)     3571 2017-10-11 22:04:05.000000 googleads-8.1.0/setup.py
--rw-r-----   0 msaniscalchi (185017) eng       (5000)       38 2017-10-11 22:05:15.000000 googleads-8.1.0/setup.cfg
+drwxr-x---   0 grivescorbett (454203) eng       (5000)        0 2017-11-14 21:49:55.000000 googleads-9.0.0/
+-rw-r-----   0 grivescorbett (454203) eng       (5000)     8947 2017-11-14 21:44:46.000000 googleads-9.0.0/README
+-rwxr-x--x   0 grivescorbett (454203) eng       (5000)     3733 2017-11-14 21:44:46.000000 googleads-9.0.0/setup.py
+drwxr-x---   0 grivescorbett (454203) eng       (5000)        0 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads.egg-info/
+-rw-r-----   0 grivescorbett (454203) eng       (5000)        1 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads.egg-info/dependency_links.txt
+-rw-r-----   0 grivescorbett (454203) eng       (5000)       10 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads.egg-info/top_level.txt
+-rw-r-----   0 grivescorbett (454203) eng       (5000)      148 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads.egg-info/requires.txt
+-rw-r-----   0 grivescorbett (454203) eng       (5000)      317 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads.egg-info/SOURCES.txt
+-rw-r-----   0 grivescorbett (454203) eng       (5000)     2325 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads.egg-info/PKG-INFO
+-rw-r-----   0 grivescorbett (454203) eng       (5000)     2325 2017-11-14 21:49:55.000000 googleads-9.0.0/PKG-INFO
+drwxr-x---   0 grivescorbett (454203) eng       (5000)        0 2017-11-14 21:49:55.000000 googleads-9.0.0/googleads/
+-rw-r-----   0 grivescorbett (454203) eng       (5000)    12682 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/oauth2.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)    11435 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/util.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)      710 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/__init__.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)    33099 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/common.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)    35482 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/dfp.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)    98494 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/adwords.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)     4005 2017-11-14 21:44:46.000000 googleads-9.0.0/googleads/errors.py
+-rw-r-----   0 grivescorbett (454203) eng       (5000)       38 2017-11-14 21:49:55.000000 googleads-9.0.0/setup.cfg
```

### Comparing `googleads-8.1.0/googleads.egg-info/PKG-INFO` & `googleads-9.0.0/googleads.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: googleads
-Version: 8.1.0
+Version: 9.0.0
 Summary: Google Ads Python Client Library
 Home-page: https://github.com/googleads/googleads-python-lib
 Author: Mark Saniscalchi
 Author-email: api.msaniscalchi@gmail.com
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description:
```

### Comparing `googleads-8.1.0/README` & `googleads-9.0.0/README`

 * *Files identical despite different names*

### Comparing `googleads-8.1.0/googleads/adwords.py` & `googleads-9.0.0/googleads/adwords.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Client library for the AdWords API."""
 
 from collections import namedtuple
+import datetime
 import io
 import logging
 import os
 import re
 import sys
 import urllib
 import urllib2
@@ -278,16 +279,16 @@
   _YAML_KEY = 'adwords'
   # A tuple containing values which must be provided to use AdWords.
   _REQUIRED_INIT_VALUES = ('developer_token',)
   # A tuple containing values which may optionally be provided when using
   # AdWords.
   _OPTIONAL_INIT_VALUES = (
       'validate_only', 'partial_failure', 'client_customer_id', 'user_agent',
-      'report_downloader_headers',
-      googleads.common.ENABLE_COMPRESSION_KEY)
+  'report_downloader_headers',
+  googleads.common.ENABLE_COMPRESSION_KEY)
 
   # The format of SOAP service WSDLs. A server, namespace, version, and service
   # name need to be formatted in.
   _SOAP_SERVICE_FORMAT = '%s/api/adwords/%s/%s/%s?wsdl'
 
   @classmethod
   def LoadFromString(cls, yaml_doc):
@@ -449,15 +450,16 @@
 
     client = suds.client.Client(
         self._SOAP_SERVICE_FORMAT %
         (server, version_service_mapping, version, service_name),
         **kwargs)
 
     return googleads.common.SudsServiceProxy(
-        client, _AdWordsHeaderHandler(self, version, self.enable_compression))
+        client, _AdWordsHeaderHandler(self, version, self.enable_compression),
+        packer=_AdWordsPacker)
 
   def GetBatchJobHelper(self, version=sorted(_SERVICE_MAP.keys())[-1],
                         server=None):
     """Returns a BatchJobHelper to work with the BatchJobService.
 
       This is a convenience method. It is functionally identical to calling
       BatchJobHelper(adwords_client, version).
@@ -619,14 +621,34 @@
         raise googleads.errors.GoogleAdsValueError(
             'The provided keyword "%s" is invalid. Accepted keywords are: %s'
             % (kw, _REPORT_HEADER_KWARGS.keys()))
 
     return headers
 
 
+class _AdWordsPacker(googleads.common.SudsPacker):
+  """A utility applying customized packing logic for AdWords."""
+
+  @classmethod
+  def Pack(cls, obj):
+    """Pack the given object using AdWords-specific logic.
+
+    Args:
+      obj: an object to be packed for suds using AdWords-specific logic, if
+          applicable.
+
+    Returns:
+      The given object packed with AdWords-specific logic for suds, if
+      applicable. Otherwise, returns the given object unmodified.
+    """
+    if isinstance(obj, ServiceQuery):
+      return str(obj)
+    return obj
+
+
 @googleads.common.RegisterUtility('BatchJobHelper')
 class BatchJobHelper(object):
   """A utility that simplifies working with the BatchJobService."""
 
   class AbstractResponseParser(object):
     """Interface for parsing responses from the BatchJobService."""
 
@@ -890,15 +912,15 @@
       Returns:
         A str containing the XML for only the operations, formatted to work with
         the BatchJobService.
 
       Raises:
         GoogleAdsValueError: if no xsi_type is specified for the operations.
       """
-        # Verify that all operations included specify an xsi_type.
+      # Verify that all operations included specify an xsi_type.
       if operations:
         if any('xsi_type' not in operation for operation in operations):
           raise googleads.errors.AdWordsBatchJobServiceInvalidOperationError(
               'Operations have no xsi_type specified.')
         return self._ExtractOperations(self._GenerateRawRequestXML(operations))
       else:
         return ''
@@ -1525,16 +1547,16 @@
   def DownloadReportWithAwql(self, query, file_format, output=sys.stdout,
                              **kwargs):
     """Downloads an AdWords report using an AWQL query.
 
     The report contents will be written to the given output.
 
     Args:
-      query: A string containing the query which specifies the data you want
-          your report to include.
+      query: A string or ReportQuery object containing the query which
+          specifies the data you want your report to include.
       file_format: A string representing the output format for your report.
           Acceptable values can be found in our API documentation:
           https://developers.google.com/adwords/api/docs/guides/reporting
       [optional]
       output: A writable object where the contents of the report will be written
           to. If the report is gzip compressed, you need to specify an output
           that can write binary data.
@@ -1751,23 +1773,24 @@
 
     return summary_fields
 
   def _SerializeAwql(self, query, file_format):
     """Serializes an AWQL query and file format for transport.
 
     Args:
-      query: A string representing the AWQL query used in the report.
+      query: A string or ReportQuery object representing the AWQL query used in
+          the report.
       file_format: A string representing the file format of the generated
           report.
 
     Returns:
       The given query and format URL encoded into the format needed for an
       AdWords report request as a string. This is intended to be a POST body.
     """
-    return urllib.urlencode({'__fmt': file_format, '__rdquery': query})
+    return urllib.urlencode({'__fmt': file_format, '__rdquery': str(query)})
 
   def _SerializeReportDefinition(self, report_definition):
     """Serializes a report definition for transport.
 
     Args:
       report_definition: A dictionary or ReportDefinition object to be
           serialized.
@@ -1804,7 +1827,717 @@
             tree.find('./ApiError/trigger').text,
             tree.find('./ApiError/fieldPath').text,
             error.code, error, content)
       except ElementTree.ParseError:
         pass
     return googleads.errors.AdWordsReportError(
         error.code, error, content)
+
+
+class _QueryBuilder(object):
+  """A query builder for building AWQL (AdWords Query Language) queries."""
+
+  def __init__(self, query_builder=None):
+    """Creates the query builder with the optional specified query builder.
+
+    This class shouldn't be instantiated directly or extended. Use
+    ReportQueryBuilder if you want to create a query for reporting or
+    ServiceQueryBuilder if you want to create a query for services.
+
+    Args:
+      query_builder: An optional query builder whose properties will be copied
+          over to this instance.
+
+    Returns:
+      The query builder.
+
+    Raises:
+      GoogleAdsValueError: If the passed query_builder isn't of the QueryBuilder
+          type.
+    """
+    if query_builder is None:
+      self.where_builders = []
+    else:
+      try:
+        self.where_builders = list(query_builder.where_builders)
+      except (AttributeError, TypeError):
+        raise googleads.errors.GoogleAdsValueError(
+            'The passed query builder should be of the QueryBuilder type.')
+
+  def Select(self, *fields):
+    """Sets a provided list of fields as selected fields for the query.
+
+    Args:
+      *fields: The specified list of fields to be added to a SELECT clause.
+
+    Returns:
+      This query builder.
+    """
+    raise NotImplementedError('You must subclass _QueryBuilder.')
+
+  def Where(self, field):
+    """Creates a WHERE builder using a provided field.
+
+    Args:
+      field: the field to be added as an argument in the WHERE clause.
+
+    Returns:
+      The created WHERE builder.
+    """
+    where_builder = _WhereBuilder(self, field)
+    self.where_builders.append(where_builder)
+    return where_builder
+
+
+class _WhereBuilder(object):
+  """A WHERE builder for building a WHERE clause in AWQL queries."""
+
+  def __init__(self, query_builder, field):
+    """Creates the WHERE builder with specified query builder and field.
+
+    This class should be instantiated through _QueryBuilder.Where. Don't call
+    this constructor directly.
+
+    Args:
+      query_builder: The query builder that this WHERE builder links to.
+      field: The field to be used in the WHERE condition.
+
+    Returns:
+      The WHERE builder.
+    """
+    self._field = field
+    self._query_builder = query_builder
+    self._awql = None
+
+  def EqualTo(self, value):
+    """Sets the type of the WHERE clause as "equal to".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, '=')
+    return self._query_builder
+
+  def NotEqualTo(self, value):
+    """Sets the type of the WHERE clause as "not equal to".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, '!=')
+    return self._query_builder
+
+  def GreaterThan(self, value):
+    """Sets the type of the WHERE clause as "greater than".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, '>')
+    return self._query_builder
+
+  def GreaterThanOrEqualTo(self, value):
+    """Sets the type of the WHERE clause as "greater than or equal to".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, '>=')
+    return self._query_builder
+
+  def LessThan(self, value):
+    """Sets the type of the WHERE clause as "less than".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, '<')
+    return self._query_builder
+
+  def LessThanOrEqualTo(self, value):
+    """Sets the type of the WHERE clause as "less than or equal to.
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, '<=')
+    return self._query_builder
+
+  def StartsWith(self, value):
+    """Sets the type of the WHERE clause as "starts with".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, 'STARTS_WITH')
+    return self._query_builder
+
+  def StartsWithIgnoreCase(self, value):
+    """Sets the type of the WHERE clause as "starts with ignore case".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value,
+                                                  'STARTS_WITH_IGNORE_CASE')
+    return self._query_builder
+
+  def Contains(self, value):
+    """Sets the type of the WHERE clause as "contains".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, 'CONTAINS')
+    return self._query_builder
+
+  def ContainsIgnoreCase(self, value):
+    """Sets the type of the WHERE clause as "contains ignore case".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, 'CONTAINS_IGNORE_CASE')
+    return self._query_builder
+
+  def DoesNotContain(self, value):
+    """Sets the type of the WHERE clause as "does not contain".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(value, 'DOES_NOT_CONTAIN')
+    return self._query_builder
+
+  def DoesNotContainIgnoreCase(self, value):
+    """Sets the type of the WHERE clause as "doesn not contain ignore case".
+
+    Args:
+      value: The value to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateSingleValueCondition(
+        value, 'DOES_NOT_CONTAIN_IGNORE_CASE')
+    return self._query_builder
+
+  def In(self, *values):
+    """Sets the type of the WHERE clause as "in".
+
+    Args:
+      *values: The values to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateMultipleValuesCondition(values, 'IN')
+    return self._query_builder
+
+  def NotIn(self, *values):
+    """Sets the type of the WHERE clause as "in".
+
+    Args:
+      *values: The values to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateMultipleValuesCondition(values, 'NOT_IN')
+    return self._query_builder
+
+  def ContainsAny(self, *values):
+    """Sets the type of the WHERE clause as "contains any".
+
+    Args:
+      *values: The values to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateMultipleValuesCondition(values, 'CONTAINS_ANY')
+    return self._query_builder
+
+  def ContainsNone(self, *values):
+    """Sets the type of the WHERE clause as "contains none".
+
+    Args:
+      *values: The values to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateMultipleValuesCondition(values, 'CONTAINS_NONE')
+    return self._query_builder
+
+  def ContainsAll(self, *values):
+    """Sets the type of the WHERE clause as "contains all".
+
+    Args:
+      *values: The values to be used in the WHERE condition.
+
+    Returns:
+      The query builder that this WHERE builder links to.
+    """
+    self._awql = self._CreateMultipleValuesCondition(values, 'CONTAINS_ALL')
+    return self._query_builder
+
+  def Build(self):
+    """Builds the WHERE clause by returning the stored AWQL.
+
+    Returns:
+      The resulting WHERE clause in AWQL format.
+    """
+    return self._awql
+
+  def _CreateSingleValueCondition(self, value, operator):
+    """Creates a single-value condition with the provided value and operator."""
+    if isinstance(value, str) or isinstance(value, unicode):
+      value = '"%s"' % value
+    return '%s %s %s' % (self._field, operator, value)
+
+  def _CreateMultipleValuesCondition(self, values, operator):
+    """Creates a condition with the provided list of values and operator."""
+    values = ['"%s"' % value if isinstance(value, str) or
+              isinstance(value, unicode) else str(value) for value in values]
+    return '%s %s [%s]' % (self._field, operator, ', '.join(values))
+
+
+@googleads.common.RegisterUtility('ReportQueryBuilder')
+class ReportQueryBuilder(_QueryBuilder):
+  """A query builder for building AWQL queries for reporting."""
+
+  def __init__(self, query_builder=None):
+    """Creates the report query builder with the optionally specified builder.
+
+    Creates the report query builder by initializing all attributes including
+    the report name, time range, start and end date. If the optional query
+    builder are specified, copy all its attributes to this instance.
+
+    Args:
+      query_builder: An optional query builder whose attributes will be copied
+          over to this instance.
+
+    Returns:
+      This report query builder.
+
+    Raises:
+      GoogleAdsValueError: If the passed query_builder isn't of the QueryBuilder
+          type.
+    """
+    _QueryBuilder.__init__(self, query_builder)
+    if query_builder is None:
+      self.select = None
+      self.from_report = None
+      self.date_range = None
+      self.start_date = None
+      self.end_date = None
+    else:
+      try:
+        self.select = list(query_builder.select)
+        self.from_report = query_builder.from_report
+        self.date_range = query_builder.date_range
+        self.start_date = query_builder.start_date
+        self.end_date = query_builder.end_date
+      except (AttributeError, TypeError):
+        raise googleads.errors.GoogleAdsValueError(
+            'The passed query builder should be of ReportQueryBuilder type.')
+
+  def Select(self, *fields):
+    """Sets a provided list of fields as selected fields for the query.
+
+    Subsequent calls to this method overwrite the entire set of selected fields
+    with the new one.
+
+    Args:
+      *fields: The specified list of fields to be added to a SELECT clause.
+
+    Returns:
+      This report query builder.
+    """
+    self.select = list(fields)
+    return self
+
+  def From(self, report_name):
+    """Sets a provided report name as the argument to FROM clause.
+
+    Args:
+      report_name: The specified report name.
+
+    Returns:
+      This report query builder.
+    """
+    self.from_report = report_name
+    return self
+
+  def During(self, date_range=None, start_date=None, end_date=None):
+    """Sets arguments for the DURING clause of the query.
+
+    Sets arguments for the DURING clause using the provided date range or start
+    and end dates. Only the date range or start and end date should be
+    specified. If both are supplied, an error will be thrown. A valid date range
+    string can be found at
+    https://developers.google.com/adwords/api/docs/guides/reporting#date_ranges.
+    Start and end dates should be in 'YYYYMMDD' format.
+
+    Args:
+      date_range: The specified date range string, e.g., YESTERDAY.
+      start_date: The start date string in 'YYYYMMDD' format or an instance of
+          datetime.date.
+      end_date: The end date string in 'YYYYMMDD' format or an instance of
+          datetime.date.
+
+    Returns:
+      This report query builder.
+
+    Raises:
+      ValueError: If all the arguments are None or both date_range and start
+          and end dates have values or if start_date has value but end_date
+          doesn't (and vice versa).
+    """
+    if date_range is None and (start_date is None or end_date is None):
+      raise ValueError(
+          'Either date_range or both start_date and end_date must not be None.')
+    if date_range is not None and (start_date is not None
+                                   or end_date is not None):
+      raise ValueError(
+          'If date_range is not None, start_date and end_date must be None '
+          '(and vice versa).')
+    self.date_range = date_range
+    self.start_date = start_date
+    self.end_date = end_date
+    return self
+
+  def Build(self):
+    """Builds a ReportQuery object containing the created AWQL query.
+
+    Returns:
+      The created ReportQuery object.
+
+    Raises:
+      ValueError: If the selected fields or report name is not specified.
+    """
+    if self.select is None:
+      raise ValueError('Must use Select() to specify SELECT clause for valid'
+                       ' AWQL first.')
+    if self.from_report is None:
+      raise ValueError('Must use From() to specify FROM clause for valid AWQL'
+                       ' first.')
+
+    parts = ['SELECT ', (', '.join(self.select))]
+    parts.extend([' FROM ', self.from_report])
+    where_clause = (' WHERE %s' % ' AND '.join([builder.Build() for builder
+                                                in self.where_builders])
+                    if self.where_builders else '')
+    parts += where_clause
+
+    if self.date_range:
+      parts.extend([' DURING ', self.date_range])
+    elif self._start_date and self._end_date:
+      parts.extend([' DURING ', '%s,%s' % (self._start_date, self._end_date)])
+    awql = ''.join(parts)
+
+    return ReportQuery(awql)
+
+  @property
+  def start_date(self):
+    """Gets the start date of the query."""
+    return self._start_date
+
+  @start_date.setter
+  def start_date(self, start_date):
+    """Sets the start date of the query to the provided value."""
+    if isinstance(start_date, datetime.date):
+      self._start_date = '{:%Y%m%d}'.format(start_date)
+    else:
+      self._start_date = start_date
+
+  @property
+  def end_date(self):
+    """Gets the end date of the query."""
+    return self._end_date
+
+  @end_date.setter
+  def end_date(self, end_date):
+    """Sets the end date of the query to the provided value."""
+    if isinstance(end_date, datetime.date):
+      self._end_date = '{:%Y%m%d}'.format(end_date)
+    else:
+      self._end_date = end_date
+
+
+class ReportQuery(object):
+  """A report query storing an AWQL query."""
+
+  def __init__(self, awql):
+    """Creates a report query instance storing the provided AWQL query."""
+    self._awql = awql
+
+  def __str__(self):
+    """Returns the stored AWQL query."""
+    return self._awql
+
+
+@googleads.common.RegisterUtility('ServiceQueryBuilder')
+class ServiceQueryBuilder(_QueryBuilder):
+  """A query builder for building AWQL queries for services."""
+
+  _ORDER_BY_CLAUSE = namedtuple('OrderByClause', ['field', 'direction'])
+
+  def __init__(self, query_builder=None):
+    """Creates the service query builder with the optionally specified builder.
+
+    Creates the service query builder by initializing all attributes including
+    oder by list, start index, and page size.
+    If the optional query builder are specified, copy all its attributes to this
+    instance.
+
+    Args:
+      query_builder: An optional query builder whose attributes will be copied
+          over to this instance.
+
+    Returns:
+      This service query builder.
+
+    Raises:
+      GoogleAdsValueError: If the passed query_builder isn't of the QueryBuilder
+          type.
+    """
+    _QueryBuilder.__init__(self, query_builder)
+    if query_builder is None:
+      self.select = set()
+      self.order_by_list = []
+      self.start_index = None
+      self.page_size = None
+    else:
+      try:
+        self.select = query_builder.select
+        self.order_by_list = query_builder.order_by_list
+        self.start_index = query_builder.start_index
+        self.page_size = query_builder.page_size
+      except (AttributeError, TypeError):
+        raise googleads.errors.GoogleAdsValueError(
+            'The passed query builder should be of ServiceQueryBuilder type.')
+
+  def Select(self, *fields):
+    """Sets a provided list of fields as selected fields for the query.
+
+    Subsequent calls to this method overwrite the entire set of selected fields
+    with the new one. Duplicate field names will be treated as one field.
+
+    Args:
+      *fields: The specified list of fields to be added to a SELECT clause.
+
+    Returns:
+      This service query builder.
+    """
+    self.select.update(fields)
+    return self
+
+  def OrderBy(self, field, ascending=True):
+    """Adds the provided field to the order-by list with the provided direction.
+
+    Args:
+      field: The specified field to be added to the order-by list.
+      ascending: If true, the newly created order-by clause will be in ascending
+          order. Otherwise, it will be in descending order.
+
+    Returns:
+      This service query builder.
+    """
+    order_by = self._ORDER_BY_CLAUSE(field, 'ASC' if ascending else 'DESC')
+    self.order_by_list.append(order_by)
+    return self
+
+  def Limit(self, start_index, page_size):
+    """Sets the LIMIT clause using the provided start index and page size.
+
+    Args:
+      start_index: The specified start index for the LIMIT clause.
+      page_size: The optional page size for the LIMIT clause.
+
+    Returns:
+      This service query builder.
+
+    Raises:
+      ValueError: If start_index is None but the page_size is not None or vice
+          versa.
+    """
+    if ((start_index is None and page_size is not None)
+        or (start_index is not None and page_size is None)):
+      raise ValueError('Either both start_index and page_size must be None, or'
+                       ' neither')
+    self.start_index = start_index
+    self.page_size = page_size
+    return self
+
+  def Build(self):
+    """Builds a ServiceQuery object containing AWQL queries.
+
+    Returns:
+      The created ServiceQuery object.
+
+    Raises:
+      ValueError: If the selected fields or service name is not specified.
+    """
+    if not self.select:
+      raise ValueError('Must use Select() to specify SELECT clause for valid'
+                       ' AWQL first')
+
+    parts = ['SELECT ', (', '.join(self.select))]
+    where_clause = (' WHERE %s' % ' AND '.join(builder.Build() for builder
+                                               in self.where_builders)
+                    if self.where_builders else '')
+    parts += where_clause
+
+    if self.order_by_list:
+      parts.extend([' ORDER BY ',
+                    ', '.join('%s %s' % (order_by.field, order_by.direction)
+                              for order_by in self.order_by_list)])
+    awql = ''.join(parts)
+
+    return ServiceQuery(awql, self.start_index, self.page_size)
+
+  @property
+  def select(self):
+    """Gets the select set of the query."""
+    return self._select
+
+  @select.setter
+  def select(self, select):
+    """Sets the select set of the query to the copy of provided value."""
+    self._select = set(select)
+
+  @property
+  def order_by_list(self):
+    """Gets the order-by list of the query."""
+    return self._order_by_list
+
+  @order_by_list.setter
+  def order_by_list(self, order_by_list):
+    """Sets the order-by list of the query to the copy of provided value."""
+    self._order_by_list = list(order_by_list)
+
+
+class ServiceQuery(object):
+  """A service query storing an AWQL query."""
+
+  def __init__(self, awql, start_index, page_size):
+    """Creates a service query instance storing the provided AWQL query."""
+    self._awql = awql
+    self._start_index = start_index
+    self._page_size = page_size
+    self._total_num_entries = None
+
+  def NextPage(self, page_size=None):
+    """Sets the LIMIT clause of the AWQL to the next page.
+
+    This method is meant to be used with HasNext().
+    The page_size is necessary when using DataService, as its paging mechanism
+    is different from other services. For details, see
+    https://developers.google.com/adwords/api/docs/guides/bid-landscapes#paging_through_results.
+    When the page_size is None, this object's page size is used instead.
+
+    Args:
+      page_size: The optional page size used to increment the index in the LIMIT
+          clause.
+
+    Returns:
+      This service query object.
+
+    Raises:
+      ValueError: If the start index of this object is None, meaning that the
+          LIMIT clause hasn't been set before.
+    """
+    if self._start_index is None:
+      raise ValueError('Cannot page through query with no LIMIT clause.')
+    increment = self._page_size if page_size is None else page_size
+    self._start_index += increment
+    return self
+
+  def HasNext(self, page, page_size=None):
+    """Checks if there is still a page left to query.
+
+    This method is meant to be used with NextPage().
+    The page_size is necessary when using DataService, as its paging mechanism
+    is different from other services. For details, see
+    https://developers.google.com/adwords/api/docs/guides/bid-landscapes#paging_through_results.
+    When the page_size is None, this object's page size is used instead.
+
+    Args:
+      page: A dict containing the 'totalNumEntries' key whose value represents
+          the total number of results from making the query to the AdWords API
+          services.
+      page_size: The optional page size used to increment the index in the LIMIT
+          clause.
+
+    Returns:
+      True if there is still a page left.
+
+    Raises:
+      ValueError: If the start index of this object is None, meaning that the
+          LIMIT clause hasn't been set before.
+    """
+    if self._start_index is None:
+      raise ValueError('Cannot page through query with no LIMIT clause.')
+    if not self._total_num_entries:
+      self._total_num_entries = page['totalNumEntries']
+    increment = self._page_size if page_size is None else page_size
+    return self._start_index + increment < self._total_num_entries
+
+  def Pager(self, service):
+    """A page generator for this service query and the provided service.
+
+    This generates a page as a result from using the provided service's query()
+    method until there are no more results to fetch.
+
+    Args:
+      service: The service object for making a query using this service query.
+
+    Yields:
+      A resulting page from querying the provided service.
+    """
+    has_page = True
+    while has_page:
+      page = service.query(self)
+      yield page
+      has_page = self.HasNext(page)
+      if has_page:
+        self.NextPage()
+
+  def __str__(self):
+    """Returns the stored AWQL query combined with the LIMIT clause."""
+    awql = self._awql + ' LIMIT %s,%s' % (self._start_index, self._page_size)
+    return awql
```

### Comparing `googleads-8.1.0/googleads/util.py` & `googleads-9.0.0/googleads/util.py`

 * *Files identical despite different names*

### Comparing `googleads-8.1.0/googleads/__init__.py` & `googleads-9.0.0/googleads/__init__.py`

 * *Files identical despite different names*

### Comparing `googleads-8.1.0/googleads/oauth2.py` & `googleads-9.0.0/googleads/oauth2.py`

 * *Files identical despite different names*

### Comparing `googleads-8.1.0/googleads/dfp.py` & `googleads-9.0.0/googleads/dfp.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,36 +42,37 @@
 
 _data_downloader_logger = logging.getLogger(
     '%s.%s' % (__name__, 'data_downloader'))
 
 
 # A giant dictionary of DFP versions and the services they support.
 _SERVICE_MAP = {
-    'v201611':
+    'v201702':
         ('ActivityGroupService', 'ActivityService', 'AdExclusionRuleService',
          'AdRuleService', 'AudienceSegmentService', 'BaseRateService',
          'CompanyService', 'ContactService', 'ContentBundleService',
          'ContentMetadataKeyHierarchyService', 'ContentService',
          'CreativeService', 'CreativeSetService', 'CreativeTemplateService',
          'CreativeWrapperService', 'CustomFieldService',
          'CustomTargetingService', 'ExchangeRateService', 'ForecastService',
          'InventoryService', 'LabelService',
          'LineItemCreativeAssociationService', 'LineItemService',
          'LineItemTemplateService', 'LiveStreamEventService',
-         'MobileApplicationService', 'NetworkService', 'OrderService',
-         'PackageService', 'PlacementService', 'PremiumRateService',
-         'ProductService', 'ProductPackageService', 'ProductPackageItemService',
-         'ProductTemplateService', 'ProposalLineItemService', 'ProposalService',
+         'MobileApplicationService', 'NativeStyleService', 'NetworkService',
+         'OrderService', 'PackageService', 'PlacementService',
+         'PremiumRateService', 'ProductService', 'ProductPackageService',
+         'ProductPackageItemService', 'ProductTemplateService',
+         'ProposalLineItemService', 'ProposalService',
          'PublisherQueryLanguageService', 'RateCardService',
          'ReconciliationOrderReportService', 'ReconciliationReportRowService',
          'ReconciliationLineItemReportService',
          'ReconciliationReportService', 'ReportService',
          'SuggestedAdUnitService', 'TeamService', 'UserService',
          'UserTeamAssociationService', 'WorkflowRequestService'),
-    'v201702':
+    'v201705':
         ('ActivityGroupService', 'ActivityService', 'AdExclusionRuleService',
          'AdRuleService', 'AudienceSegmentService', 'BaseRateService',
          'CompanyService', 'ContactService', 'ContentBundleService',
          'ContentMetadataKeyHierarchyService', 'ContentService',
          'CreativeService', 'CreativeSetService', 'CreativeTemplateService',
          'CreativeWrapperService', 'CustomFieldService',
          'CustomTargetingService', 'ExchangeRateService', 'ForecastService',
@@ -85,15 +86,15 @@
          'ProposalLineItemService', 'ProposalService',
          'PublisherQueryLanguageService', 'RateCardService',
          'ReconciliationOrderReportService', 'ReconciliationReportRowService',
          'ReconciliationLineItemReportService',
          'ReconciliationReportService', 'ReportService',
          'SuggestedAdUnitService', 'TeamService', 'UserService',
          'UserTeamAssociationService', 'WorkflowRequestService'),
-    'v201705':
+    'v201708':
         ('ActivityGroupService', 'ActivityService', 'AdExclusionRuleService',
          'AdRuleService', 'AudienceSegmentService', 'BaseRateService',
          'CompanyService', 'ContactService', 'ContentBundleService',
          'ContentMetadataKeyHierarchyService', 'ContentService',
          'CreativeService', 'CreativeSetService', 'CreativeTemplateService',
          'CreativeWrapperService', 'CustomFieldService',
          'CustomTargetingService', 'ExchangeRateService', 'ForecastService',
@@ -107,23 +108,23 @@
          'ProposalLineItemService', 'ProposalService',
          'PublisherQueryLanguageService', 'RateCardService',
          'ReconciliationOrderReportService', 'ReconciliationReportRowService',
          'ReconciliationLineItemReportService',
          'ReconciliationReportService', 'ReportService',
          'SuggestedAdUnitService', 'TeamService', 'UserService',
          'UserTeamAssociationService', 'WorkflowRequestService'),
-    'v201708':
+    'v201711':
         ('ActivityGroupService', 'ActivityService', 'AdExclusionRuleService',
          'AdRuleService', 'AudienceSegmentService', 'BaseRateService',
-         'CompanyService', 'ContactService', 'ContentBundleService',
-         'ContentMetadataKeyHierarchyService', 'ContentService',
-         'CreativeService', 'CreativeSetService', 'CreativeTemplateService',
-         'CreativeWrapperService', 'CustomFieldService',
-         'CustomTargetingService', 'ExchangeRateService', 'ForecastService',
-         'InventoryService', 'LabelService',
+         'CdnConfigurationService', 'CompanyService', 'ContactService',
+         'ContentBundleService', 'ContentMetadataKeyHierarchyService',
+         'ContentService', 'CreativeService', 'CreativeSetService',
+         'CreativeTemplateService', 'CreativeWrapperService',
+         'CustomFieldService', 'CustomTargetingService', 'ExchangeRateService',
+         'ForecastService', 'InventoryService', 'LabelService',
          'LineItemCreativeAssociationService', 'LineItemService',
          'LineItemTemplateService', 'LiveStreamEventService',
          'MobileApplicationService', 'NativeStyleService', 'NetworkService',
          'OrderService', 'PackageService', 'PlacementService',
          'PremiumRateService', 'ProductService', 'ProductPackageService',
          'ProductPackageItemService', 'ProductTemplateService',
          'ProposalLineItemService', 'ProposalService',
@@ -213,16 +214,16 @@
     Args:
       oauth2_client: A googleads.oauth2.GoogleOAuth2Client used to authorize
           your requests.
       application_name: An arbitrary string which will be used to identify your
           application
       [optional]
       network_code: A string identifying the network code of the network you are
-          accessing. All requests other than getAllNetworks and getCurrentUser
-          calls require this header to be set.
+          accessing. All requests other than getAllNetworks require this header
+          to be set.
       cache: A subclass of suds.cache.Cache. If not set, this will default to an
           instance of suds.cache.ObjectCache.
       proxy_config: A googleads.common.ProxyConfig instance or None if a proxy
         isn't being used.
       enable_compression: A boolean indicating if you want to enable compression
         of the SOAP response. If True, the SOAP response will use gzip
         compression, and will be decompressed for you automatically.
@@ -296,15 +297,15 @@
               % (service_name, _SERVICE_MAP[version]))
       else:
         raise googleads.errors.GoogleAdsValueError(
             'Unrecognized version of the DFP API. Version given: %s Supported '
             'versions: %s' % (version, _SERVICE_MAP.keys()))
 
     return googleads.common.SudsServiceProxy(client, self._header_handler,
-                                             _DFPDateTimePacker)
+                                             packer=_DfpPacker)
 
   def GetDataDownloader(self, version=sorted(_SERVICE_MAP.keys())[-1],
                         server=None):
     """Creates a downloader for DFP reports and PQL result sets.
 
     This is a convenience method. It is functionally identical to calling
     DataDownloader(dfp_client, version, server)
@@ -360,14 +361,61 @@
       http_headers['accept-encoding'] = 'gzip'
 
     suds_client.set_options(
         soapheaders=header,
         headers=http_headers)
 
 
+class _DfpPacker(googleads.common.SudsPacker):
+  """A utility applying customized packing logic for DFP."""
+
+  @classmethod
+  def Pack(cls, obj):
+    """Pack the given object using DFP-specific logic.
+
+    Args:
+      obj: an object to be packed for suds using DFP-specific logic, if
+          applicable.
+
+    Returns:
+      The given object packed with DFP-specific logic for suds, if applicable.
+      Otherwise, returns the given object unmodified.
+    """
+    if isinstance(obj, (datetime.datetime, datetime.date)):
+      return cls.DfpDateTimePacker(obj)
+    return obj
+
+  @classmethod
+  def DfpDateTimePacker(cls, value):
+    """Returns dicts formatted for DFP SOAP based on date/datetime.
+
+    Args:
+      value: A date or datetime object to be converted.
+
+    Returns:
+      The value object correctly represented for DFP SOAP.
+    """
+
+    if isinstance(value, datetime.datetime):
+      if value.tzinfo is None:
+        raise googleads.errors.GoogleAdsValueError(
+            'Datetime %s is not timezone aware.' % value
+        )
+
+      return {
+          'date': cls.DfpDateTimePacker(value.date()),
+          'hour': value.hour,
+          'minute': value.minute,
+          'second': value.second,
+          'timeZoneID': value.tzinfo.zone,
+      }
+    elif isinstance(value, datetime.date):
+      return {'year': value.year, 'month': value.month, 'day': value.day}
+
+
 @googleads.common.RegisterUtility('StatementBuilder')
 class StatementBuilder(object):
   """Provides the ability to programmatically construct PQL queries."""
 
   class _OrderByPair(object):
     """Stores and serializes a pair of column/ascending values."""
 
@@ -539,41 +587,14 @@
     # Make this call to throw the exception here if there is a problem
     PQLHelper.GetValueRepresentation(value)
 
     self._values[key] = value
     return self
 
 
-def _DFPDateTimePacker(value):
-  """Returns dicts formatted for DFP SOAP based on date/datetime.
-
-  Args:
-    value: A date or datetime object to be converted.
-
-  Returns:
-    The value object correctly represented for DFP SOAP.
-  """
-
-  if isinstance(value, datetime.datetime):
-    if value.tzinfo is None:
-      raise googleads.errors.GoogleAdsValueError(
-          'Datetime %s is not timezone aware.' % value
-      )
-
-    return {
-        'date': _DFPDateTimePacker(value.date()),
-        'hour': value.hour,
-        'minute': value.minute,
-        'second': value.second,
-        'timeZoneID': value.tzinfo.zone,
-    }
-  elif isinstance(value, datetime.date):
-    return {'year': value.year, 'month': value.month, 'day': value.day}
-
-
 class PQLHelper(object):
   """Utility class for PQL."""
 
   @classmethod
   def GetQueryValuesFromDict(cls, d):
     """Converts a dict of python types into a list of PQL types.
 
@@ -794,15 +815,16 @@
   def DownloadPqlResultToList(self, pql_query, values=None):
     """Downloads the results of a PQL query to a list.
 
     Args:
       pql_query: str a statement filter to apply (the query should not include
                  the limit or the offset)
       [optional]
-      values: list dict of bind values to use with the pql_query.
+      values: A dict of python objects or a list of raw SOAP values to bind
+              to the pql_query.
 
     Returns:
       a list of lists with the first being the header row and each subsequent
       list being a row of results.
     """
     results = []
     self._PageThroughPqlSet(pql_query, results.append, values)
@@ -812,15 +834,16 @@
     """Downloads the results of a PQL query to CSV.
 
     Args:
       pql_query: str a statement filter to apply (the query should not include
                  the limit or the offset)
       file_handle: file the file object to write to.
       [optional]
-      values: list dict of bind values to use with the pql_query.
+      values: A dict of python objects or a list of raw SOAP values to bind
+              to the pql_query.
     """
     pql_writer = csv.writer(file_handle, delimiter=',',
                             quotechar='"', quoting=csv.QUOTE_ALL)
     self._PageThroughPqlSet(pql_query, pql_writer.writerow, values)
 
   def _ConvertValueForCsv(self, pql_value):
     """Sanitizes a field value from a Value object to a CSV suitable format.
@@ -871,16 +894,20 @@
     """Pages through a pql_query and performs an action (output_function).
 
     Args:
       pql_query: str a statement filter to apply (the query should not include
                  the limit or the offset)
       output_function: the function to call to output the results (csv or in
                        memory)
-      values: list dict of bind values to use with the pql_query.
+      values: A dict of python objects or a list of raw SOAP values to bind
+              to the pql_query.
     """
+    if isinstance(values, dict):
+      values = PQLHelper.GetQueryValuesFromDict(values)
+
     pql_service = self._GetPqlService()
     current_offset = 0
 
     while True:
       query_w_limit_offset = '%s LIMIT %d OFFSET %d' % (pql_query,
                                                         SUGGESTED_PAGE_LIMIT,
                                                         current_offset)
```

### Comparing `googleads-8.1.0/googleads/common.py` & `googleads-9.0.0/googleads/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Common client library functions and classes used by all products."""
 
 
-import datetime
 from functools import wraps
 import inspect
 import locale
 import logging
 import logging.config
 import os
 import ssl
@@ -62,15 +61,15 @@
 _PY_VERSION_MICRO = sys.version_info.micro
 _DEPRECATED_VERSION_TEMPLATE = (
     'This library is being run by an unsupported Python version (%s.%s.%s). In '
     'order to benefit from important security improvements and ensure '
     'compatibility with this library, upgrade to Python 2.7.9 or higher.')
 
 
-VERSION = '8.1.0'
+VERSION = '9.0.0'
 _COMMON_LIB_SIG = 'googleads/%s' % VERSION
 _LOGGING_KEY = 'logging'
 _HTTP_PROXY_YAML_KEY = 'http_proxy'
 _HTTPS_PROXY_YAML_KEY = 'https_proxy'
 _PROXY_CONFIG_KEY = 'proxy_config'
 _PYTHON_VERSION = 'Python/%d.%d.%d' % (
     _PY_VERSION_MAJOR, _PY_VERSION_MINOR, _PY_VERSION_MICRO)
@@ -392,38 +391,40 @@
         'Your yaml file is missing some of the required proxy values. Required '
         'values are: %s, actual values are %s' %
         (_PROXY_KEYS, original_proxy_keys))
 
   return proxy
 
 
-def _PackForSuds(obj, factory, datetime_packer=None):
+def _PackForSuds(obj, factory, packer=None):
   """Packs SOAP input into the format we want for suds.
 
   The main goal here is to pack dictionaries with an 'xsi_type' key into
   objects. This allows dictionary syntax to be used even with complex types
   extending other complex types. The contents of dictionaries and lists/tuples
   are recursively packed. Mutable types are copied - we don't mutate the input.
 
   Args:
     obj: A parameter for a SOAP request which will be packed. If this is
         a dictionary or list, the contents will recursively be packed. If this
         is not a dictionary or list, the contents will be recursively searched
         for instances of unpacked dictionaries or lists.
     factory: The suds.client.Factory object which can create instances of the
         classes generated from the WSDL.
-    datetime_packer: A product specific function to unwrap date/datetimes.
+    packer: An optional subclass of googleads.common.SudsPacker that provides
+        customized packing logic.
 
   Returns:
     If the given obj was a dictionary that contained the 'xsi_type' key, this
     will be an instance of a class generated from the WSDL. Otherwise, this will
     be the same data type as the input obj was.
   """
-  if datetime_packer and isinstance(obj, (datetime.datetime, datetime.date)):
-    obj = datetime_packer(obj)
+  if packer:
+    obj = packer.Pack(obj)
+
   if obj in ({}, None):
     # Force suds to serialize empty objects. There are legitimate use cases for
     # this, for example passing in an empty SearchCriteria object to a DFA
     # search method in order to select everything.
     return suds.null()
   elif isinstance(obj, dict):
     if 'xsi_type' in obj:
@@ -446,24 +447,24 @@
         if param.endswith('.Type'):
           setattr(new_obj, param, obj['xsi_type'])
         else:
           setattr(new_obj, param, None)
       for key in obj:
         if key == 'xsi_type': continue
         setattr(new_obj, key, _PackForSuds(obj[key], factory,
-                                           datetime_packer=datetime_packer))
+                                           packer=packer))
     else:
       new_obj = {}
       for key in obj:
         new_obj[key] = _PackForSuds(obj[key], factory,
-                                    datetime_packer=datetime_packer)
+                                    packer=packer)
     return new_obj
   elif isinstance(obj, (list, tuple)):
     return [_PackForSuds(item, factory,
-                         datetime_packer=datetime_packer) for item in obj]
+                         packer=packer) for item in obj]
   else:
     _RecurseOverObject(obj, factory)
     return obj
 
 
 def _RecurseOverObject(obj, factory, parent=None):
   """Recurses over a nested structure to look for changes in Suds objects.
@@ -690,43 +691,56 @@
       # Start with the default set of handlers.
       return_handlers = suds.transport.http.HttpTransport.u2handlers(self)
       return_handlers.extend(self.handlers)
 
       return return_handlers
 
 
+class SudsPacker(object):
+  """A utility class to be passed to _PackForSuds for customized packing.
+
+  A subclass should be used in cases where custom logic is needed to pack a
+  given object in _PackForSuds.
+  """
+
+  @classmethod
+  def Pack(cls, obj):
+    raise NotImplementedError('You must subclass SudsPacker.')
+
+
 class SudsServiceProxy(object):
   """Wraps a suds service object, allowing custom logic to be injected.
 
   This class is responsible for refreshing the HTTP and SOAP headers, so changes
   to the client object will be reflected in future SOAP calls, and for
   transforming SOAP call input parameters, allowing dictionary syntax to be used
   with all SOAP complex types.
 
   Attributes:
     suds_client: The suds.client.Client this service belongs to. If you are
         familiar with suds and want to use autogenerated classes, you can access
         the client and its factory,
   """
 
-  def __init__(self, suds_client, header_handler, datetime_packer=None):
+  def __init__(self, suds_client, header_handler, packer=None):
     """Initializes a suds service proxy.
 
     Args:
       suds_client: The suds.client.Client whose service will be wrapped. Note
         that this is the client itself, not the client's embedded service
         object.
       header_handler: A HeaderHandler responsible for setting the SOAP and HTTP
           headers on the service client.
-      datetime_packer: A product specific function to unwrap date/datetimes.
+      packer: An optional subclass of googleads.common.SudsPacker that provides
+        customized packing logic.
     """
     self.suds_client = suds_client
     self._header_handler = header_handler
     self._method_proxies = {}
-    self._datetime_packer = datetime_packer
+    self._packer = packer
 
   def __getattr__(self, attr):
     if attr in self.suds_client.wsdl.services[0].ports[0].methods:
       if attr not in self._method_proxies:
         self._method_proxies[attr] = self._CreateMethod(attr)
       return self._method_proxies[attr]
     else:
@@ -746,15 +760,15 @@
     def MakeSoapRequest(*args):
       """Perform a SOAP call."""
       self._header_handler.SetHeaders(self.suds_client)
 
       try:
         return soap_service_method(
             *[_PackForSuds(arg, self.suds_client.factory,
-                           self._datetime_packer) for arg in args])
+                           self._packer) for arg in args])
       except suds.WebFault as e:
         if _logger.isEnabledFor(logging.WARNING):
           _logger.warning('Response summary - %s',
                           _ExtractResponseSummaryFields(e.document))
 
         _logger.info('SOAP response:\n%s', e.document.str())
```

### Comparing `googleads-8.1.0/googleads/errors.py` & `googleads-9.0.0/googleads/errors.py`

 * *Files identical despite different names*

### Comparing `googleads-8.1.0/PKG-INFO` & `googleads-9.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: googleads
-Version: 8.1.0
+Version: 9.0.0
 Summary: Google Ads Python Client Library
 Home-page: https://github.com/googleads/googleads-python-lib
 Author: Mark Saniscalchi
 Author-email: api.msaniscalchi@gmail.com
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description:
```

### Comparing `googleads-8.1.0/setup.py` & `googleads-9.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 import os
 import re
 import sys
 from setuptools import setup
 
 PACKAGES = ['googleads']
 
-DEPENDENCIES = ['httplib2>=0.9.2', 'oauth2client>=4.0.0,<5.0.0',
-                'suds-jurko>=0.6', 'pysocks>=1.5.6', 'pytz>=2015.7',
-                'PyYAML>=3.11', 'xmltodict>=0.9.2']
+DEPENDENCIES = ['httplib2>=0.9.2,<1.0.0', 'oauth2client>=4.0.0,<5.0.0',
+                'suds-jurko>=0.6,<0.7', 'pysocks>=1.5.6,<2.0.0', 'pytz>=2015.7',
+                'PyYAML>=3.11,<4.0', 'xmltodict>=0.9.2,<1.0.0']
+
+TEST_DEPENDENCIES = ['mock>=2.0.0,<3.0.0', 'pyfakefs>=3.2,<4.0']
 
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3.4'
 ]
@@ -112,8 +114,10 @@
       license='Apache License 2.0',
       long_description=long_description,
       packages=PACKAGES,
       platforms='any',
       keywords='adwords dfp google',
       classifiers=CLASSIFIERS,
       install_requires=DEPENDENCIES,
+      tests_require=TEST_DEPENDENCIES,
+      test_suite='tests',
       **extra_params)
```

