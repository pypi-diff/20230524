# Comparing `tmp/provo-1.0.3.tar.gz` & `tmp/provo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provo-1.0.3.tar", last modified: Fri Jan 27 16:28:04 2023, max compression
+gzip compressed data, was "provo-1.0.4.tar", last modified: Wed May 24 12:10:04 2023, max compression
```

## Comparing `provo-1.0.3.tar` & `provo-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 16:28:04.635104 provo-1.0.3/
--rw-rw-rw-   0        0        0    35823 2022-11-18 22:18:22.000000 provo-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3393 2023-01-27 16:28:04.634105 provo-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    26234 2022-11-25 09:26:49.000000 provo-1.0.3/README.md
--rw-rw-rw-   0        0        0     2746 2022-11-24 15:51:36.000000 provo-1.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-27 16:28:04.617105 provo-1.0.3/provo/
--rw-rw-rw-   0        0        0       55 2022-11-19 11:48:56.000000 provo-1.0.3/provo/__init__.py
--rw-rw-rw-   0        0        0     1841 2022-11-20 14:42:08.000000 provo-1.0.3/provo/idvault.py
--rw-rw-rw-   0        0        0    25472 2023-01-26 14:06:59.000000 provo-1.0.3/provo/provontologygraph.py
--rw-rw-rw-   0        0        0    10948 2022-11-24 10:44:43.000000 provo-1.0.3/provo/startingpointclasses.py
--rw-rw-rw-   0        0        0      455 2022-11-24 10:52:04.000000 provo-1.0.3/provo/staticfunctions.py
-drwxrwxrwx   0        0        0        0 2023-01-27 16:28:04.632103 provo-1.0.3/provo/tests/
--rw-rw-rw-   0        0        0        0 2022-11-20 13:47:51.000000 provo-1.0.3/provo/tests/__init__.py
--rw-rw-rw-   0        0        0     1397 2022-11-24 10:26:09.000000 provo-1.0.3/provo/tests/test_provenance_graph.py
--rw-rw-rw-   0        0        0     3423 2022-11-24 10:28:08.000000 provo-1.0.3/provo/tests/test_starting_point_classes.py
--rw-rw-rw-   0        0        0     1526 2022-11-24 10:30:02.000000 provo-1.0.3/provo/tests/test_vault.py
-drwxrwxrwx   0        0        0        0 2023-01-27 16:28:04.625104 provo-1.0.3/provo.egg-info/
--rw-rw-rw-   0        0        0     3393 2023-01-27 16:28:04.000000 provo-1.0.3/provo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-01-27 16:28:04.000000 provo-1.0.3/provo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 16:28:04.000000 provo-1.0.3/provo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-27 16:28:04.000000 provo-1.0.3/provo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-27 16:28:04.635104 provo-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1068 2023-01-24 15:15:56.000000 provo-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:10:04.058351 provo-1.0.4/
+-rw-rw-rw-   0        0        0     1070 2023-05-24 11:53:22.000000 provo-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3367 2023-05-24 12:10:04.057352 provo-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26043 2023-05-24 11:50:51.000000 provo-1.0.4/README.md
+-rw-rw-rw-   0        0        0     2746 2022-11-24 15:51:36.000000 provo-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-24 12:10:04.030352 provo-1.0.4/provo/
+-rw-rw-rw-   0        0        0       55 2022-11-19 11:48:56.000000 provo-1.0.4/provo/__init__.py
+-rw-rw-rw-   0        0        0     1841 2022-11-20 14:42:08.000000 provo-1.0.4/provo/idvault.py
+-rw-rw-rw-   0        0        0    25472 2023-01-26 14:06:59.000000 provo-1.0.4/provo/provontologygraph.py
+-rw-rw-rw-   0        0        0    10948 2022-11-24 10:44:43.000000 provo-1.0.4/provo/startingpointclasses.py
+-rw-rw-rw-   0        0        0      455 2022-11-24 10:52:04.000000 provo-1.0.4/provo/staticfunctions.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:10:04.056352 provo-1.0.4/provo/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-20 13:47:51.000000 provo-1.0.4/provo/tests/__init__.py
+-rw-rw-rw-   0        0        0     1397 2022-11-24 10:26:09.000000 provo-1.0.4/provo/tests/test_provenance_graph.py
+-rw-rw-rw-   0        0        0     3423 2022-11-24 10:28:08.000000 provo-1.0.4/provo/tests/test_starting_point_classes.py
+-rw-rw-rw-   0        0        0     1526 2022-11-24 10:30:02.000000 provo-1.0.4/provo/tests/test_vault.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:10:04.049349 provo-1.0.4/provo.egg-info/
+-rw-rw-rw-   0        0        0     3367 2023-05-24 12:10:03.000000 provo-1.0.4/provo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-05-24 12:10:04.000000 provo-1.0.4/provo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:10:03.000000 provo-1.0.4/provo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-24 12:10:03.000000 provo-1.0.4/provo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 12:10:03.000000 provo-1.0.4/provo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 12:10:04.059355 provo-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1098 2023-05-24 12:01:08.000000 provo-1.0.4/setup.py
```

### Comparing `provo-1.0.3/PKG-INFO` & `provo-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: provo
-Version: 1.0.3
+Version: 1.0.4
 Summary: Construct  PROV-O compliant provenance graphs.
 Home-page: https://github.com/rue-a/provo
 Author: Arne Rümmler
 Author-email: arne.ruemmler@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.11
+Requires-Python: >=3.08
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 README
 ======
 
 The package supports the creation of
```

### Comparing `provo-1.0.3/README.md` & `provo-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 # README
 
-The package supports the creation of [PROV-O](https://www.w3.org/TR/prov-o/) compliant provenance graphs. 
+The package supports the creation of [PROV-O](https://www.w3.org/TR/prov-o/) compliant provenance graphs.
 
 The package requires __Python 3.11__.
 
 ## Installation
 
 You can install the package from the Python Package Index (PyPI):
 
 `pip install provo`
 
-Or by downloading this repo:
+Or by downloading this repository:
 
-1. Download and unzip the package
-2. Open Shell and _cd_ to unzipped package
+1. Download and unzip the repository
+2. Open Shell and _cd_ to unzipped repository
 3. Run `pip install -e .` (in the folder that contains ```setup.py```)
 
 ## Contents
 
-The package implements the [PROV-O starting point classes](https://www.w3.org/TR/prov-o/#starting-points-figure) __Entity__, __Activity__ and __Agent__ as Python classes with methods to establish starting point properties between instances of these classes.
+The package is a Python API to PROV-O. It implements the [PROV-O starting point classes](https://www.w3.org/TR/prov-o/#starting-points-figure) __Entity__, __Activity__ and __Agent__ as Python classes with methods to establish the _PROV-O starting point properties_ between instances of these classes.
 
 ## Features
 
-The package's objective is it to support the programmatical creation of provenance graphs that are compliant with the W3C Recommendation PROV-O: The PROV Ontology. Users of the package shall be enabled to tightly couple the generation of data with the generation of their provenance. As the package implements PROV-O, the created graph is exportable as an RDF document. Finally, the graph can be exported as a mermaid flowchart with some configuration options to adjust the style of the resulting chart.
+The package's objective is to support the programmatical creation of provenance graphs that are compliant with the W3C Recommendation PROV-O: The PROV Ontology. Users of the package shall be enabled to tightly couple the generation of data with the generation of their provenance. As the package implements PROV-O, the created graph is exportable as an RDF document. Finally, the graph can be exported as a mermaid flowchart with some configuration options to adjust the style of the resulting chart.
 
 ### Compliance
 
 - The PROV-O classes __Entity__, __Activity__, and __Agent__ are implemented as Python classes.
 - The PROV-O properties _wasGeneratedBy_, _wasDerivedFrom_, _wasAttributedTo_, _startedAtTime_, _used_, _wasInformedBy_, _endedAtTime_, _wasAssociatedWith_, and _actedOnBehalfOf_ are implemented as instance methods of their according classes.
 - Attributes that are passed to these methods are type-checked to enforce compliance with PROV-O.
 - Node Ids are checked for validity.
-- (Accidental) use of the same ID for different objects throws an error.
+- Use of the same ID for different objects throws an error.
 
 ### Ease of Use
 
 - The package implements full type hint support, thus enabling rich support from the IDE.
 - The classes `Provence_Ontology_Graph`, `Entity`, `Activity`, and `Agent` can be printed to terminal in a user-friendly, readable way with the default `print()` command.
-- For some quick testing, objects of the classes `Entity`, `Activity`, and `Agent` can be instantiated with auto-generated Ids (although it's not recommended using this for production).
+- Objects of the classes `Entity`, `Activity`, and `Agent` can be instantiated with auto-generated Ids (although it's not recommended using this for production).
 - Export as [mermaid flowchart](https://mermaid-js.github.io/mermaid/#/flowchart) to review the graph visually.
 
 ### Interface to RDF via the [rdflib](https://rdflib.readthedocs.io/en/stable/) package
 
 - The graph's contents can be converted to an `rdflib.Graph` object.
 - The graph can be exported in various RDF serializations.
 
 ## Manual
 
-The package is centered around the class ProvenanceOntologyGraph. Entities, Activities, and Agents are added to this graph by using the according add-methods. Relations between the starting point classes are constructed by using the respective methods of the classes. 
-
+The package is centered around the class `ProvenanceOntologyGraph`. Entities, Activities, and Agents are added to this graph using the according class methods. Relations between the PROV-O class objects are constructed using their respective class methods.
 
 ### Create a Provenance Ontology Graph
 
 The graph can be initialized with default or user defined attributes. The graph can be printed to the terminal with `print(graph)`.
 
 ```python
 # ex1 - create a provenance graph
@@ -69,36 +68,36 @@
     lang="en"
 )
 ```
 
 `namespace=`
 
 - Default is `"https://provo-example.org/"`.
-- Has to be valid url, validation is currently performed with the [validators]() package.
+- Has to be valid url, validation is currently performed with the [validators](https://pypi.org/project/validators/) package.
 - Has to end with `/` or `#`.
 
 `namespace_abbreviation=`
 
 - Default is `""`.
 - Used when converting to other models, such as RDF (-> prefixes)
 - Only characters from the Latin alphabet are allowed.
 - RDF core prefixes (*owl*, *rdf*, *rdfs*, *xsd* and *xml*) are prohibited from use.
 
 >**Note** 
-> Although not prohibited, the following prefixes are commonly uses and thus recommended to be avoided: *brick*, *csvw*, *dc*, *dcat*, *dcmitype*, *cdterms*, *dcam*, *doap*, *foaf*, *geo*, *odrl*, *org*, *prof*, *prov*, *qb*, *sdo*, *sh*, *skos*, *sosa*, *ssn*, *time*, *vann* and *void*.
+> Although not prohibited, the following prefixes are commonly used and thus recommended being avoided: *brick*, *csvw*, *dc*, *dcat*, *dcmitype*, *cdterms*, *dcam*, *doap*, *foaf*, *geo*, *odrl*, *org*, *prof*, *prov*, *qb*, *sdo*, *sh*, *skos*, *sosa*, *ssn*, *time*, *vann* and *void*.
 
 `lang=`
 
 - Default is `"en"`.
 - Used when converting to other models that support a *lang* tag.
 - Has to be compliant with [RFC 5646](https://www.rfc-editor.org/info/rfc5646) (Phillips, A., Ed., and M. Davis, Ed., "Tags for Identifying Languages", BCP 47, RFC 5646, September 2009). Compliance is not validated!
 
-### Create Entities, Activities and Agents and define relation between them
+### Create Entities, Activities and Agents and define relations between them
 
-The creation for the three starting term classes follows the same pattern. The classes only differ in their methods. PROV-O Classes are instantiated by using the add methods of the provenance graph class. Below you find an extensively commented version of the `add_entity()` method. 
+The creation for classes follows the same pattern. The classes only differ in their methods. PROV-O Classes are instantiated by using the add methods of the provenance graph class. Below you find the `add_entity()` method of `ProvenanceOntologyGraph` for reference.
 
 ```python
 # definition of add_entity() in ProvOntologyGraph()
 def add_entity(self, 
     id_string: str = "", 
     label: str = "", 
     description: str = "", 
@@ -153,15 +152,15 @@
 # label: Anonymous activity
 # description: An arbitrary activity.
 # ---
 ```
 
 ### RDF interface
 
-The graph can be directly serialized as RDF document or be converted to an rdflib Graph, for further manipulation.
+The graph can be directly serialized as RDF document or be converted to an `rdflib` Graph, for further manipulation.
 
 ```python
 # ex3 - serialize provenance graph as RDF document
 prov_ontology_graph.serialize_as_rdf("manual_examples.ttl")
 ```
 
 ```
@@ -602,20 +601,11 @@
 http://example.org#government[/Government\]:::agent
 http://example.org#civil_action_group[/Civil Action Group\]:::agent
 http://example.org#national_newspaper_inc[/National Newspaper Inc.\]:::agent
 http://example.org#derek[/Derek\]:::agent
 http://example.org#national_newspaper_inc-. instructed .->http://example.org#derek
 ```
 
-## Used Packages
-
-- rdflib: https://rdflib.readthedocs.io/en/stable/, BSD License
-- validators: https://github.com/python-validators/validators, MIT License
-
-
-## License
-
-GNU General Public License v3.0
 
 ## Contact
 
 Arne Rümmler ([arne.ruemmler@gmail.com](mailto:arne.ruemmler@gmail.com))
```

### Comparing `provo-1.0.3/README.rst` & `provo-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo/idvault.py` & `provo-1.0.4/provo/idvault.py`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo/provontologygraph.py` & `provo-1.0.4/provo/provontologygraph.py`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo/startingpointclasses.py` & `provo-1.0.4/provo/startingpointclasses.py`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo/tests/test_provenance_graph.py` & `provo-1.0.4/provo/tests/test_provenance_graph.py`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo/tests/test_starting_point_classes.py` & `provo-1.0.4/provo/tests/test_starting_point_classes.py`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo/tests/test_vault.py` & `provo-1.0.4/provo/tests/test_vault.py`

 * *Files identical despite different names*

### Comparing `provo-1.0.3/provo.egg-info/PKG-INFO` & `provo-1.0.4/provo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: provo
-Version: 1.0.3
+Version: 1.0.4
 Summary: Construct  PROV-O compliant provenance graphs.
 Home-page: https://github.com/rue-a/provo
 Author: Arne Rümmler
 Author-email: arne.ruemmler@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.11
+Requires-Python: >=3.08
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 README
 ======
 
 The package supports the creation of
```

### Comparing `provo-1.0.3/setup.py` & `provo-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="provo",
     author="Arne Rümmler",
     author_email="arne.ruemmler@gmail.com",
-    version="1.0.3",
+    version="1.0.4",
     description="Construct  PROV-O compliant provenance graphs.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rue-a/provo",
     packages=find_packages(".", exclude=["tests", "tests.*"]),
+    install_requires=["rdflib", "validators", "uuid"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: OSI Approved :: MIT License",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires=">=3.11",
+    python_requires=">=3.08",
 )
```

