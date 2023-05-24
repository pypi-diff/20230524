# Comparing `tmp/sequana_variant_calling-0.9.5.tar.gz` & `tmp/sequana_variant_calling-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_variant_calling-0.9.5.tar", last modified: Tue Nov 24 10:54:49 2020, max compression
+gzip compressed data, was "dist/sequana_variant_calling-1.0.0.tar", last modified: Wed May 24 07:44:23 2023, max compression
```

## Comparing `sequana_variant_calling-0.9.5.tar` & `sequana_variant_calling-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      128 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6627 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4528 2020-11-24 10:53:40.000000 sequana_variant_calling-0.9.5/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       40 2020-11-24 10:54:08.000000 sequana_variant_calling-0.9.5/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      133 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5662 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    90725 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/dag.png
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/data/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5336 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/logo.png
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     4815 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5163 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/multiqc_config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       73 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14085 2020-11-24 10:51:51.000000 sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/variant_calling.rules
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6627 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      837 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      169 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-08-12 20:02:05.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       40 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/top_level.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      261 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3401 2020-11-24 10:53:06.000000 sequana_variant_calling-0.9.5/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-24 10:54:49.000000 sequana_variant_calling-0.9.5/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2511 2020-06-02 19:53:21.000000 sequana_variant_calling-0.9.5/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6926 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    90725 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5336 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5543 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    19086 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/variant_calling.rules
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/setup.py
```

### Comparing `sequana_variant_calling-0.9.5/PKG-INFO` & `sequana_variant_calling-1.0.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,168 @@
-Metadata-Version: 1.2
-Name: sequana_variant_calling
-Version: 0.9.5
-Summary: A variant calling pipeline to analyse sequencing Illumina data
-Home-page: http://github.com/sequana/
-Author: cokelaer
-Author-email: thomas.cokelaer@pasteur.fr
-Maintainer: cokelaer
-Maintainer-email: thomas.cokelaer@pasteur.fr
-License: new BSD
-Description: This is is the **variant_calling** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-        
-        :Overview: Variant calling from FASTQ files
-        :Input: FASTQ files from Illumina Sequencing instrument
-        :Output: VCF and HTML files
-        :Status: production
-        :Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        You must install Sequana first::
-        
-            pip install sequana
-        
-        Then, just install this package::
-        
-            pip install sequana_variant_calling
-        
-        Usage
-        ~~~~~
-        
-        ::
-        
-            sequana_variant_calling --help
-            sequana_variant_calling --input-directory DATAPATH --reference-file measles.fa
-            sequana_variant_calling --input-directory DATAPATH --reference-file measles.fa
-        
-        This creates a directory **variant_calling**. You just need to execute the pipeline::
-        
-            cd variant_calling
-            sh variant_calling.sh
-        
-        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-        
-            snakemake -s variant_calling.rules -c config.yaml --cores 4 --stats stats.txt
-        
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        This pipelines requires the following executable(s):
-        
-        - bwa
-        - freebayes
-        - picard (picard-tools)
-        - sambamba
-        - samtools
-        - snpEff
-        
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_variant_calling/master/sequana_pipelines/variant_calling/dag.png
-        
-        Details
-        ~~~~~~~~
-        
-        Snakemake variant calling pipeline is based on
-        `tutorial <https://github.com/ekg/alignment-and-variant-calling-tutorial>`_
-        written by Erik Garrison. Input reads (paired or single) are mapped using
-        `bwa <http://bio-bwa.sourceforge.net/>`_ and sorted with
-        `sambamba-sort <http://lomereiter.github.io/sambamba/docs/sambamba-sort.html>`_.
-        PCR duplicates are marked with
-        `sambamba-markdup <http://lomereiter.github.io/sambamba/docs/sambamba-sort.html>`_. 
-        `Freebayes <https://github.com/ekg/freebayes>`_ is used to detect SNPs and short
-        INDELs. The INDEL realignment and base quality recalibration are not necessary
-        with Freebayes. For more information, please refer to a post by Brad Chapman on
-        `minimal BAM preprocessing methods
-        <https://bcbio.wordpress.com/2013/10/21/updated-comparison-of-variant-detection-methods-ensemble-freebayes-and-minimal-bam-preparation-pipelines/>`_.
-        
-        The pipeline provides an analysis of the mapping coverage using
-        `sequana coverage <http://www.biorxiv.org/content/early/2016/12/08/092478>`_.
-        It detects and characterises automatically low and high genome coverage regions.
-        
-        Detected variants are annotated with `SnpEff <http://snpeff.sourceforge.net/>`_ if a
-        GenBank file is provided. The pipeline does the database building automatically.
-        Although most of the species should be handled automatically, some special cases
-        such as particular codon table will required edition of the snpeff configuration file.
-        
-        Finally, joint calling is also available and can be switch on if desired.
-        
-        
-        Changelog
-        ~~~~~~~~~
-        
-        ========= ====================================================================
-        Version   Description
-        ========= ====================================================================
-        0.9.5     * fix typo in the onsuccess and update sequana requirements to use
-                    most up-to-date snakemake rules
-        0.9.4     * fix typo related to the reference-file option new name not changed
-                    everyhere in the pipeline. 
-        0.9.3     * use new framework (faster --help, --from-project option)
-                  * rename --reference into --reference-file and --annotation to
-                    --annotation-file
-                  * add custom summary page
-                  * add multiqc config file
-        0.9.2     * snpeff output files are renamed sample.snpeff (instead of
-                    samplesnpeff)
-                  * add multiqc to show sequana_coverage and snpeff summary sections
-                  * cleanup onsuccess section
-                  * more options sanity checks and options (e.g., 
-                  * genbank_file renamed into annotation_file in the config
-                  * use --legacy in freebayes options
-                  * fix coverage section to use new sequana api
-                  * add the -do-coverage, --do-joint-calling options as well as
-                    --circular and --frebayes--ploidy
-        0.9.1     * Fix input-readtag, which was not populated
-        0.9.0     First release
-        ========= ====================================================================
-        
-        
-Keywords: snakemake,sequana,NGS,freebayes,variant calling
-Platform: Linux
-Platform: Unix
-Platform: MacOsX
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
+
+.. image:: https://badge.fury.io/py/sequana-variant-calling.svg
+     :target: https://pypi.python.org/pypi/sequana_variant_calling
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+    :target: http://joss.theoj.org/papers/10.21105/joss.00352
+    :alt: JOSS (journal of open source software) DOI
+
+.. image:: https://github.com/sequana/variant_calling/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/sequana/variant_calling/actions/workflows
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
+This is the **variant_calling** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+
+:Overview: Variant calling from FASTQ files
+:Input: FASTQ files from Illumina Sequencing instrument
+:Output: VCF and HTML files
+:Status: production
+:Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
+
+
+Installation
+~~~~~~~~~~~~
+
+If you already have all requirements, you can install the packages using pip::
+
+    pip install sequana_variant_calling --upgrade
+
+Otherwise, you can create a *sequana_variant_calling* conda environment executing::
+
+    conda env create -f environment.yml
+
+and later activate the environment::
+
+  conda activate sequana_variant_calling
+
+A third option is to install the pipeline with pip method (see above) and use singularity as explained afterwards.
+
+
+Usage
+~~~~~
+
+::
+
+    sequana_variant_calling --help
+    sequana_variant_calling --input-directory DATAPATH --reference-file measles.fa
+
+This creates a directory **variant_calling**. You just need to execute the pipeline::
+
+    cd variant_calling
+    sh variant_calling.sh
+
+This launch a snakemake pipeline. If you are familiar with snakemake, you can
+retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+
+    snakemake -s variant_calling.rules -c config.yaml --cores 4 --stats stats.txt
+
+Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+
+Usage with singularity::
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+With singularity, initiate the working directory as follows::
+
+    sequana_variant_calling --use-singularity
+
+Images are downloaded in the working directory but you can store then in a directory globally (e.g.)::
+
+    sequana_variant_calling --use-singularity --singularity-prefix ~/.sequana/apptainers
+
+and then::
+
+    cd variant_calling
+    sh variant_calling.sh
+
+if you decide to use snakemake manually, do not forget to add singularity options::
+
+    snakemake -s variant_calling.rules -c config.yaml --cores 4 --stats stats.txt --use-singularity --singularity-prefix ~/.sequana/apptainers --singularity-args "-B /home:/home"
+
+    
+
+Requirements
+~~~~~~~~~~~~
+
+This pipelines requires the following executable(s):
+
+- bwa
+- freebayes
+- picard (picard-tools)
+- sambamba
+- samtools
+- snpEff you will need 5.0 or 5.1d (note the d); 5.1 does not work.
+
+.. image:: https://raw.githubusercontent.com/sequana/sequana_variant_calling/main/sequana_pipelines/variant_calling/dag.png
+
+Details
+~~~~~~~~
+
+Snakemake variant calling pipeline is based on
+`tutorial <https://github.com/ekg/alignment-and-variant-calling-tutorial>`_
+written by Erik Garrison. Input reads (paired or single) are mapped using
+`bwa <http://bio-bwa.sourceforge.net/>`_ and sorted with
+`sambamba-sort <http://lomereiter.github.io/sambamba/docs/sambamba-sort.html>`_.
+PCR duplicates are marked with
+`sambamba-markdup <http://lomereiter.github.io/sambamba/docs/sambamba-sort.html>`_. 
+`Freebayes <https://github.com/ekg/freebayes>`_ is used to detect SNPs and short
+INDELs. The INDEL realignment and base quality recalibration are not necessary
+with Freebayes. For more information, please refer to a post by Brad Chapman on
+`minimal BAM preprocessing methods
+<https://bcbio.wordpress.com/2013/10/21/updated-comparison-of-variant-detection-methods-ensemble-freebayes-and-minimal-bam-preparation-pipelines/>`_.
+
+The pipeline provides an analysis of the mapping coverage using
+`sequana coverage <http://www.biorxiv.org/content/early/2016/12/08/092478>`_.
+It detects and characterises automatically low and high genome coverage regions.
+
+Detected variants are annotated with `SnpEff <http://snpeff.sourceforge.net/>`_ if a
+GenBank file is provided. The pipeline does the database building automatically.
+Although most of the species should be handled automatically, some special cases
+such as particular codon table will required edition of the snpeff configuration file.
+
+Finally, joint calling is also available and can be switch on if desired.
+
+
+Changelog
+~~~~~~~~~
+
+========= ======================================================================
+Version   Description
+========= ======================================================================
+1.0.0     * use last warppers and graphviz apptainer
+0.12.0    * set all apptainers containers and add vcf to bcf conversions
+          * Update rule sambamba to use latest wrappers
+0.11.0    * Add singularity containers
+0.10.0    * fully integrated sequana wrappers and simplification of HTML reports
+0.9.10    * Uses new sequana_pipetools and wrappers
+0.9.5     * fix typo in the onsuccess and update sequana requirements to use
+            most up-to-date snakemake rules
+0.9.4     * fix typo related to the reference-file option new name not changed
+            everyhere in the pipeline. 
+0.9.3     * use new framework (faster --help, --from-project option)
+          * rename --reference into --reference-file and --annotation to
+            --annotation-file
+          * add custom summary page
+          * add multiqc config file
+0.9.2     * snpeff output files are renamed sample.snpeff (instead of
+            samplesnpeff)
+          * add multiqc to show sequana_coverage and snpeff summary sections
+          * cleanup onsuccess section
+          * more options sanity checks and options (e.g., 
+          * genbank_file renamed into annotation_file in the config
+          * use --legacy in freebayes options
+          * fix coverage section to use new sequana api
+          * add the -do-coverage, --do-joint-calling options as well as
+            --circular and --frebayes--ploidy
+0.9.1     * Fix input-readtag, which was not populated
+0.9.0     First release
+========= ======================================================================
+
+Contribute & Code of Conduct
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To contribute to this project, please take a look at the 
+`Contributing Guidelines <https://github.com/sequana/sequana/blob/maib/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
+`Code of Conduct <https://github.com/sequana/sequana/blob/main/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
+
```

### Comparing `sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/config.yaml` & `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -5,50 +5,49 @@
 #
 # One of input_directory, input_pattern and input_samples must be provided
 # If input_directory provided, use it otherwise if input_pattern provided,
 # use it, otherwise use input_samples.
 # ============================================================================
 #
 # Mandatory fields
-input_directory: "%(input_directory)s"
-input_readtag: "%(input_readtag)s"
-input_pattern: "%(input_pattern)s"
+input_directory: 
+input_readtag: _R[12]_
+input_pattern: '*fastq.gz'
 annotation_file:
 reference_file:
 
+apptainers:
+    sequana_tools: "https://zenodo.org/record/7963917/files/sequana_tools_0.15.1.img"
+    graphviz: "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
 
-#################################################################
-# sequencing information. These informations will be inserted as
-# read group in BAM files
-#
-# :Parameters:
+
+# you may add ID, PF, SM, PU, LB read tags
 #
-# - platform: Name of the sequencing platform
-# - instrument: name ot the instrument type
-# - flowcell: flowcell ID
-sequencing:
-    platform: Illumina
-    instrument: unknown
-    flowcell: unknown
+add_read_group:
+    #PU: Illumina
+    options: ''
+
+
+
 ##############################################################################
 # BWA - Mapping
 #
 # :Parameters:
 #
 # - reference_file: the name of the reference file.
 # - index_algorithm: the BWA index algorithm (is or bwtsw).
 # - options: any options recognised by BWA MEM tool.
 # - threads: number of threads to be used.
 # - tmp_directory: temporary directory
 #
-bwa_mem_ref:
-    index_algorithm: 'is'
-    options: '-T 30'
-    threads: 2
-    tmp_directory: './tmp/'
+bwa_mem:
+    index_algorithm: is
+    options: -T 30
+    threads: 4
+    tmp_directory: ./tmp/
 
 ##############################################################################
 # SnpEff - Annotate variants detected
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
@@ -61,16 +60,17 @@
 #	    -no-downstream: Do not show DOWNSTREAM changes
 #	    -no-intergenic: Do not show INTERGENIC changes
 #	    -no-intron: Do not show INTRON changes
 #	    -no-upstream: Do not show UPSTREAM changes
 #	    -no-utr: Do not show 5_PRIME_UTR or 3_PRIME_UTR changes
 #
 snpeff:
-    do: no
-    options: "-no-downstream -no-upstream"
+    do: true
+    build_options: # -noCheckCds -noCheckProtein
+    options: -no-downstream -no-upstream 
 
 ##############################################################################
 # Freebayes - Variant caller
 #
 # :Parameters:
 #
 # - ploidy: set the ploidy of your samples.
@@ -82,44 +82,46 @@
 
 ##############################################################################
 # Joint Freebayes - Variant caller
 #
 # :Parameters:
 #
 # - options: any options recognised by freebayes.
-#
+# - Note that ploidy is the one from the 'freebayes' section
 joint_freebayes:
     do: false
-    options:
+    options: ''
 
 ##############################################################################
 # Sambamba - Marks or removes duplicates
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
-# - remove: boolean if you want remove or not duplicated reads.
+# - remove_duplicates: boolean if you want remove or not duplicated reads.
 # - tmp_directory: set the temporary directory.
 #
 sambamba_markdup:
-    do: yes
-    remove: no
-    tmp_directory: "./tmp/"
+    do: true
+    remove_duplicates: false
+    tmp_directory: ./tmp/
+    options:
 
 ##############################################################################
 # Filter reads with a mapping score lower than an integer 
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
 # - threshold: mapping score threshold (between 0 and 60).
 #
 sambamba_filter:
-    do: yes
+    do: true
     threshold: 30
+    options:
 
 ##############################################################################
 # Sequana coverage - Analyse the coverage of the mapping 
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
@@ -127,25 +129,24 @@
 # - circular: if your genome is circular.
 # - window_size: window size to compute the running median.
 # - low_threshold: threshold to detect low coverage regions.
 # - high_threshold: threshold to detect high coverage regions.
 # - gc_window_size: window size to compute GC content.
 #
 sequana_coverage:
-    do: false
+    do: true
     circular: true
     window_size: 3001
     chunksize: 5000000
     double_threshold: 0.5
     gc_window_size: 201
-    genbank_file: ''
     high_threshold: 4.0
     low_threshold: -4.0
     mixture_models: 2
-    reference_file:
+    genbank_file: # filled automatically at setup but deprecated
 
 ##############################################################################
 # Filter VCF
 #
 # :Parameters:
 #
 # - freebayes_score: threshold for minimum freebayes quality score.
@@ -153,15 +154,15 @@
 # - min_depth: threshold for minimum coverage depth.
 # - forward_depth: threshold for minimum coverage depth of forward strand.
 # - reverse_depth: threshold for minimum coverage depth of reverse strand.
 # - strand_ratio: threshold for minimum strand ratio between 0 and 0.5.
 #
 freebayes_vcf_filter:
     freebayes_score: 20
-    frequency: 0.7
+    frequency: 0.1
     min_depth: 10
     forward_depth: 3
     reverse_depth: 3
     strand_ratio: 0.2
 
 ##############################################################################
 # Filter Joint VCF
@@ -185,9 +186,12 @@
 # :Parameters:
 #
 # - options: any options recognised by multiqc
 # - output-directory: Create report in the specified output directory
 # - config_file: by default, we use sequana RNA-seq multiqc_config file. 
 #       If you want your own multiqc, fill this entry
 multiqc:
-    options: "-p -f -m snpeff -m sequana_coverage"
+    options: -p -f
+    modules: snpeff sequana_coverage
+    input_directory: .
+    config_file: multiqc_config.yaml
```

### Comparing `sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/dag.png` & `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/logo.png` & `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/logo.png`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/main.py` & `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,43 @@
+#
+#  This file is part of Sequana software
+#
+#  Copyright (c) 2016-2021 - Sequana Development Team
+#
+#  Distributed under the terms of the 3-clause BSD license.
+#  The full license is in the LICENSE file, distributed with this software.
+#
+#  website: https://github.com/sequana/sequana
+#  documentation: http://sequana.readthedocs.io
+#
+##############################################################################
 import sys
 import os
 import argparse
+import subprocess
 
 from sequana_pipetools.options import *
+from sequana_pipetools.options import before_pipeline
 from sequana_pipetools.misc import Colors
 from sequana_pipetools.info import sequana_epilog, sequana_prolog
+from sequana_pipetools import SequanaManager
 
 col = Colors()
 
 NAME = "variant_calling"
 
 
 class Options(argparse.ArgumentParser):
     def __init__(self, prog=NAME, epilog=None):
         usage = col.purple(sequana_prolog.format(**{"name": NAME}))
         super(Options, self).__init__(usage=usage, prog=prog, description="",
             epilog=epilog,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter
         )
+
         # add a new group of options to the parser
         so = SlurmOptions()
         so.add_options(self)
 
         # add a snakemake group of options to the parser
         so = SnakemakeOptions(working_directory=NAME)
         so.add_options(self)
@@ -56,14 +72,17 @@
 
         pipeline_group.add_argument("-o", "--circular", action="store_true")
         pipeline_group.add_argument("--freebayes-ploidy", type=int, default=1)
 
         pipeline_group.add_argument("--create-bigwig", action="store_true",
             help="create the bigwig files from the BAM files" )
 
+        self.add_argument("--run", default=False, action="store_true",
+            help="execute the pipeline directly")
+
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
             if len(args_list)>2:
                 msg = "WARNING [sequana]: With --from-project option, " + \
                         "pipeline and data-related options will be ignored."
                 print(col.error(msg))
@@ -76,23 +95,19 @@
 
 def main(args=None):
 
     if args is None:
         args = sys.argv
 
     # whatever needs to be called by all pipeline before the options parsing
-    from sequana_pipetools.options import before_pipeline
     before_pipeline(NAME)
 
     # option parsing including common epilog
     options = Options(NAME, epilog=sequana_epilog).parse_args(args[1:])
 
-
-    from sequana.pipelines_common import SequanaManager
-
     # the real stuff is here
     manager = SequanaManager(options, NAME)
 
     # create the beginning of the command and the working directory
     manager.setup()
 
     # fill the config file with input parameters
@@ -109,31 +124,32 @@
             #print("." in cfg.annotation_file,  cfg.annotation_file.split(".")[-1])
             if "." not in cfg.annotation_file or \
                 cfg.annotation_file.split(".")[-1] not in ['gbk', 'gff', 'gff3']:
     
                 logger.error("The annotation file must end with .gbk or .gff or .gff3. You provided {}".format(cfg.annotation_file))
                 sys.exit(1)
             cfg['sequana_coverage']['genbank_file'] = cfg.annotation_file
+        else:
+            cfg.snpeff.do = False
+            cfg['sequana_coverage']['genbank_file'] = ""
 
         cfg['sequana_coverage']['do'] = options.do_coverage
         cfg['sequana_coverage']["circular"] = options.circular
-
-
         cfg['joint_freebayes']['do'] = options.do_joint_calling
-    
-
-        cfg['bwa_mem_ref']['threads'] = options.threads
+        cfg['bwa_mem']['threads'] = options.threads
         cfg['freebayes']['ploidy'] = options.freebayes_ploidy
 
         cfg.reference_file = os.path.abspath(options.reference)
         manager.exists(cfg.reference_file)
 
         # coverage
 
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
+    if options.run:
+        subprocess.Popen(["sh", '{}.sh'.format(NAME)], cwd=options.workdir)
 
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_variant_calling-0.9.5/sequana_pipelines/variant_calling/multiqc_config.yaml` & `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/PKG-INFO` & `sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,114 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sequana-variant-calling
-Version: 0.9.5
+Version: 1.0.0
 Summary: A variant calling pipeline to analyse sequencing Illumina data
 Home-page: http://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
-Description: This is is the **variant_calling** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+Description: 
+        .. image:: https://badge.fury.io/py/sequana-variant-calling.svg
+             :target: https://pypi.python.org/pypi/sequana_variant_calling
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/variant_calling/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/variant_calling/actions/workflows
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        This is the **variant_calling** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
         
         :Overview: Variant calling from FASTQ files
         :Input: FASTQ files from Illumina Sequencing instrument
         :Output: VCF and HTML files
         :Status: production
         :Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
         
         
         Installation
         ~~~~~~~~~~~~
         
-        You must install Sequana first::
+        If you already have all requirements, you can install the packages using pip::
+        
+            pip install sequana_variant_calling --upgrade
+        
+        Otherwise, you can create a *sequana_variant_calling* conda environment executing::
+        
+            conda env create -f environment.yml
+        
+        and later activate the environment::
         
-            pip install sequana
+          conda activate sequana_variant_calling
         
-        Then, just install this package::
+        A third option is to install the pipeline with pip method (see above) and use singularity as explained afterwards.
         
-            pip install sequana_variant_calling
         
         Usage
         ~~~~~
         
         ::
         
             sequana_variant_calling --help
             sequana_variant_calling --input-directory DATAPATH --reference-file measles.fa
-            sequana_variant_calling --input-directory DATAPATH --reference-file measles.fa
         
         This creates a directory **variant_calling**. You just need to execute the pipeline::
         
             cd variant_calling
             sh variant_calling.sh
         
-        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can
         retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
         
             snakemake -s variant_calling.rules -c config.yaml --cores 4 --stats stats.txt
         
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+        
+        Usage with singularity::
+        ~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        With singularity, initiate the working directory as follows::
+        
+            sequana_variant_calling --use-singularity
+        
+        Images are downloaded in the working directory but you can store then in a directory globally (e.g.)::
+        
+            sequana_variant_calling --use-singularity --singularity-prefix ~/.sequana/apptainers
+        
+        and then::
+        
+            cd variant_calling
+            sh variant_calling.sh
+        
+        if you decide to use snakemake manually, do not forget to add singularity options::
+        
+            snakemake -s variant_calling.rules -c config.yaml --cores 4 --stats stats.txt --use-singularity --singularity-prefix ~/.sequana/apptainers --singularity-args "-B /home:/home"
+        
+            
         
         Requirements
         ~~~~~~~~~~~~
         
         This pipelines requires the following executable(s):
         
         - bwa
         - freebayes
         - picard (picard-tools)
         - sambamba
         - samtools
-        - snpEff
+        - snpEff you will need 5.0 or 5.1d (note the d); 5.1 does not work.
         
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_variant_calling/master/sequana_pipelines/variant_calling/dag.png
+        .. image:: https://raw.githubusercontent.com/sequana/sequana_variant_calling/main/sequana_pipelines/variant_calling/dag.png
         
         Details
         ~~~~~~~~
         
         Snakemake variant calling pipeline is based on
         `tutorial <https://github.com/ekg/alignment-and-variant-calling-tutorial>`_
         written by Erik Garrison. Input reads (paired or single) are mapped using
@@ -90,17 +133,23 @@
         
         Finally, joint calling is also available and can be switch on if desired.
         
         
         Changelog
         ~~~~~~~~~
         
-        ========= ====================================================================
+        ========= ======================================================================
         Version   Description
-        ========= ====================================================================
+        ========= ======================================================================
+        1.0.0     * use last warppers and graphviz apptainer
+        0.12.0    * set all apptainers containers and add vcf to bcf conversions
+                  * Update rule sambamba to use latest wrappers
+        0.11.0    * Add singularity containers
+        0.10.0    * fully integrated sequana wrappers and simplification of HTML reports
+        0.9.10    * Uses new sequana_pipetools and wrappers
         0.9.5     * fix typo in the onsuccess and update sequana requirements to use
                     most up-to-date snakemake rules
         0.9.4     * fix typo related to the reference-file option new name not changed
                     everyhere in the pipeline. 
         0.9.3     * use new framework (faster --help, --from-project option)
                   * rename --reference into --reference-file and --annotation to
                     --annotation-file
@@ -114,29 +163,39 @@
                   * genbank_file renamed into annotation_file in the config
                   * use --legacy in freebayes options
                   * fix coverage section to use new sequana api
                   * add the -do-coverage, --do-joint-calling options as well as
                     --circular and --frebayes--ploidy
         0.9.1     * Fix input-readtag, which was not populated
         0.9.0     First release
-        ========= ====================================================================
+        ========= ======================================================================
+        
+        Contribute & Code of Conduct
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        To contribute to this project, please take a look at the 
+        `Contributing Guidelines <https://github.com/sequana/sequana/blob/maib/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
+        `Code of Conduct <https://github.com/sequana/sequana/blob/main/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
         
         
 Keywords: snakemake,sequana,NGS,freebayes,variant calling
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
```

### Comparing `sequana_variant_calling-0.9.5/sequana_variant_calling.egg-info/SOURCES.txt` & `sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 sequana_pipelines/variant_calling/__init__.py
 sequana_pipelines/variant_calling/config.yaml
 sequana_pipelines/variant_calling/dag.png
 sequana_pipelines/variant_calling/logo.png
 sequana_pipelines/variant_calling/main.py
 sequana_pipelines/variant_calling/multiqc_config.yaml
 sequana_pipelines/variant_calling/requirements.txt
+sequana_pipelines/variant_calling/schema.yaml
 sequana_pipelines/variant_calling/variant_calling.rules
-sequana_pipelines/variant_calling/data/__init__.py
 sequana_variant_calling.egg-info/PKG-INFO
 sequana_variant_calling.egg-info/SOURCES.txt
 sequana_variant_calling.egg-info/dependency_links.txt
 sequana_variant_calling.egg-info/entry_points.txt
 sequana_variant_calling.egg-info/not-zip-safe
 sequana_variant_calling.egg-info/requires.txt
-sequana_variant_calling.egg-info/top_level.txt
-test/test_main.py
+sequana_variant_calling.egg-info/top_level.txt
```

### Comparing `sequana_variant_calling-0.9.5/setup.py` & `sequana_variant_calling-1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,87 @@
-# -*- coding: utf-8 -*-
 # License: 3-clause BSD
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
-_MAJOR               = 0
-_MINOR               = 9
-_MICRO               = 5
+_MAJOR               = 1
+_MINOR               = 0
+_MICRO               = 0
 
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
     'url' : "http://github.com/sequana/",
     'description': "A variant calling pipeline to analyse sequencing Illumina data" ,
     'platforms' : ['Linux', 'Unix', 'MacOsX', 'Windows'],
     'keywords' : ['snakemake', "sequana", "NGS", "freebayes", "variant calling"],
     'classifiers' : [
-          'Development Status :: 4 - Beta',
-          #'Development Status :: 5 - Production/Stable',
+          'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
 
 NAME = "variant_calling"
 
-class Install(install):
-    def run(self):
-        cmd = "sequana_completion --name {} --force ".format(NAME)
-        try: subprocess.run(cmd.split())
-        except:pass
-        install.run(self)
-
-class Develop(develop):
-    def run(self):
-        cmd = "sequana_completion --name {} --force ".format(NAME)
-        try:subprocess.run(cmd.split())
-        except:pass
-        develop.run(self)
 
 setup(
     name             = "sequana_{}".format(NAME),
     version          = version,
     maintainer       = metainfo['authors']['main'][0],
     maintainer_email = metainfo['authors']['main'][1],
     author           = metainfo['authors']['main'][0],
     author_email     = metainfo['authors']['main'][1],
     long_description = open("README.rst").read(),
     keywords         = metainfo['keywords'],
     description      = metainfo['description'],
     license          = metainfo['license'],
+    long_description_content_type = "text/x-rst",
     platforms        = metainfo['platforms'],
     url              = metainfo['url'],
     classifiers      = metainfo['classifiers'],
 
     # package installation
-    packages = ["sequana_pipelines.variant_calling", 
-        "sequana_pipelines.variant_calling.data"],
+    packages = ["sequana_pipelines.variant_calling"],
 
     install_requires = open("requirements.txt").read(),
-
+    extras_require={
+        "testing": [
+            "pytest",
+            "pytest-cov",
+            "pytest-xdist",
+            "pytest-mock",
+            "pytest-timeout",
+            "pytest-runner",
+            "coveralls",
+        ],
+    },
     # This is recursive include of data files
     exclude_package_data = {"": ["__pycache__"]},
     package_data = {
         '': ['*.yaml', "*.rules", "*json", "requirements.txt", "*png"],
         'sequana_pipelines.variant_calling.fastqc.data' : ['*.*'], 
         },
 
     zip_safe=False,
 
     entry_points = {'console_scripts':[
-        'sequana_pipelines_variant_calling=sequana_pipelines.variant_calling.main:main',
         'sequana_variant_calling=sequana_pipelines.variant_calling.main:main']
     }
 
 )
```

