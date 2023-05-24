# Comparing `tmp/cellmaps_pipeline-0.1.0a1.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a1.tar", last modified: Mon May 22 23:49:50 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a2.tar", last modified: Wed May 24 17:17:41 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a1.tar` & `cellmaps_pipeline-0.1.0a2.tar`

### file list

```diff
@@ -1,44 +1,51 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 23:49:50.392375 cellmaps_pipeline-0.1.0a1/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a1/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a1/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a1/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a1/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a1/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-22 23:49:50.392514 cellmaps_pipeline-0.1.0a1/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4019 2023-05-22 23:49:10.000000 cellmaps_pipeline-0.1.0a1/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 23:49:50.385210 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      277 2023-05-19 20:47:51.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     7654 2023-05-19 23:52:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    11543 2023-05-22 20:30:15.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 23:49:50.386815 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-22 23:49:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      894 2023-05-22 23:49:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 23:49:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 23:49:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      169 2023-05-22 23:49:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-05-22 23:49:50.000000 cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 23:49:50.391331 cellmaps_pipeline-0.1.0a1/docs/
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/Makefile
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/authors.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-05-22 23:49:50.392999 cellmaps_pipeline-0.1.0a1/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2386 2023-05-19 23:36:32.000000 cellmaps_pipeline-0.1.0a1/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 23:49:50.392192 cellmaps_pipeline-0.1.0a1/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a1/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2554 2023-04-04 23:02:59.000000 cellmaps_pipeline-0.1.0a1/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-19 22:06:11.000000 cellmaps_pipeline-0.1.0a1/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a1/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.609582 cellmaps_pipeline-0.1.0a2/
+-rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a2/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-24 17:17:41.609813 cellmaps_pipeline-0.1.0a2/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4019 2023-05-22 23:49:10.000000 cellmaps_pipeline-0.1.0a2/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.600173 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      277 2023-05-23 23:25:11.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     7654 2023-05-23 16:27:52.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    11405 2023-05-23 23:24:07.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.601735 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1024 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      169 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.606531 cellmaps_pipeline-0.1.0a2/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.595415 cellmaps_pipeline-0.1.0a2/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.595483 cellmaps_pipeline-0.1.0a2/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.607412 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a2/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-05-24 17:17:41.610332 cellmaps_pipeline-0.1.0a2/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2386 2023-05-19 23:36:32.000000 cellmaps_pipeline-0.1.0a2/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.609273 cellmaps_pipeline-0.1.0a2/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     2554 2023-04-04 23:02:59.000000 cellmaps_pipeline-0.1.0a2/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-19 22:06:11.000000 cellmaps_pipeline-0.1.0a2/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a1/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/LICENSE` & `cellmaps_pipeline-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/PKG-INFO` & `cellmaps_pipeline-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Christopher Churas
 Author-email: cchuras@ucsd.edu
 License: MIT license
 Description: ==============
         CM4AI Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a1/README.rst` & `cellmaps_pipeline-0.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         return 0
 
     def _hierarchy(self):
         """
 
         :return:
         """
-        if self._fake is True and os.path.isdir(self._hierarchy_dir):
+        if os.path.isdir(self._hierarchy_dir):
             warnings.warn('Found hierarchy dir, assuming we are good. skipping')
             return 0
 
         ppigen = CosineSimilarityPPIGenerator(embeddingdir=self._coembed_dir)
 
         hiergen = CDAPSHierarchyGenerator()
         return CellmapsGenerateHierarchy(outdir=self._hierarchy_dir,
@@ -141,15 +141,15 @@
                                          input_data_dict=self._input_data_dict).run()
 
     def _coembed(self):
         """
 
         :return:
         """
-        if self._fake is True and os.path.isdir(self._coembed_dir):
+        if os.path.isdir(self._coembed_dir):
             warnings.warn('Found coembedding dir, assuming we are good. skipping')
             return 0
 
         if self._fake:
             gen = FakeCoEmbeddingGenerator(ppi_embeddingdir=self._ppi_embed_dir,
                                            image_embeddingdir=self._image_embed_dir,
                                            image_downloaddir=self._image_dir)
@@ -165,15 +165,15 @@
                                   input_data_dict=self._input_data_dict).run()
 
     def _embed_image(self):
         """
 
         :return:
         """
-        if self._fake is True and os.path.isdir(self._image_embed_dir):
+        if os.path.isdir(self._image_embed_dir):
             warnings.warn('Found image embedding dir, assuming we are good. skipping')
             return 0
 
         if self._fake is True:
             gen = FakeEmbeddingGenerator(self._image_dir)
         else:
             gen = DensenetEmbeddingGenerator(self._image_dir,
@@ -185,15 +185,15 @@
                                      input_data_dict=self._input_data_dict).run()
 
     def _embed_ppi(self):
         """
 
         :return:
         """
-        if self._fake is True and os.path.isdir(self._ppi_embed_dir):
+        if os.path.isdir(self._ppi_embed_dir):
             warnings.warn('Found ppi embedding dir, assuming we are good. skipping')
             return 0
         gen = Node2VecEmbeddingGenerator(
             nx_network=nx.read_edgelist(CellMapsPPIEmbedder.get_apms_edgelist_file(self._ppi_dir),
                                         delimiter='\t'))
 
         return CellMapsPPIEmbedder(outdir=self._ppi_embed_dir,
@@ -202,15 +202,15 @@
                                    input_data_dict=self._input_data_dict).run()
 
     def _download_ppi(self):
         """
 
         :return:
         """
-        if self._fake is True and os.path.isdir(self._ppi_dir):
+        if os.path.isdir(self._ppi_dir):
             warnings.warn('Found ppi dir, assuming we are good. skipping')
             return 0
         apmsgen = APMSGeneNodeAttributeGenerator(
             apms_edgelist=APMSGeneNodeAttributeGenerator.get_apms_edgelist_from_tsvfile(self._edgelist),
             apms_baitlist=APMSGeneNodeAttributeGenerator.get_apms_baitlist_from_tsvfile(self._baitlist))
 
         return CellmapsPPIDownloader(outdir=self._ppi_dir,
@@ -222,15 +222,15 @@
         """
         Downloads Images using
         :py:class:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader`
 
         :return: exit code of :py:meth:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader.run`
         :rtype: int
         """
-        if self._fake is True and os.path.isdir(self._image_dir):
+        if os.path.isdir(self._image_dir):
             warnings.warn('Found image dir, assuming we are good. skipping')
             return 0
         logger.info('Downloading images')
         imagegen = ImageGeneNodeAttributeGenerator(
             unique_list=ImageGeneNodeAttributeGenerator.get_unique_list_from_csvfile(self._unique),
             samples_list=ImageGeneNodeAttributeGenerator.get_samples_from_csvfile(self._samples))
```

### Comparing `cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Christopher Churas
 Author-email: cchuras@ucsd.edu
 License: MIT license
 Description: ==============
         CM4AI Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a1/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 cellmaps_pipeline.egg-info/SOURCES.txt
 cellmaps_pipeline.egg-info/dependency_links.txt
 cellmaps_pipeline.egg-info/not-zip-safe
 cellmaps_pipeline.egg-info/requires.txt
 cellmaps_pipeline.egg-info/top_level.txt
 docs/Makefile
 docs/authors.rst
+docs/cellmaps_pipeline.rst
 docs/conf.py
 docs/contributing.rst
 docs/devbranches.rst
 docs/developer.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/integrationtesting.rst
 docs/make.bat
 docs/modules.rst
 docs/newrelease.rst
 docs/pypircfile.rst
 docs/usage.rst
 docs/versioningscheme.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cellmaps_pipelinecmd.py
 tests/test_cellmapspipeline.py
 tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a1/docs/Makefile` & `cellmaps_pipeline-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/conf.py` & `cellmaps_pipeline-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/index.rst` & `cellmaps_pipeline-0.1.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/installation.rst` & `cellmaps_pipeline-0.1.0a2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/make.bat` & `cellmaps_pipeline-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a2/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a2/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/usage.rst` & `cellmaps_pipeline-0.1.0a2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a2/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/setup.py` & `cellmaps_pipeline-0.1.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/tests/test_cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a2/tests/test_cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a2/tests/test_cellmapspipeline.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a1/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a2/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*

