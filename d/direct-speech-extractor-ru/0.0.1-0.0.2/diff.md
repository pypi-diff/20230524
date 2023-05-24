# Comparing `tmp/direct_speech_extractor_ru-0.0.1.tar.gz` & `tmp/direct_speech_extractor_ru-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direct_speech_extractor_ru-0.0.1.tar", last modified: Wed May  3 08:58:23 2023, max compression
+gzip compressed data, was "direct_speech_extractor_ru-0.0.2.tar", last modified: Wed May 24 10:56:12 2023, max compression
```

## Comparing `direct_speech_extractor_ru-0.0.1.tar` & `direct_speech_extractor_ru-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-03 08:58:23.720211 direct_speech_extractor_ru-0.0.1/
--rw-r--r--   0 apple      (501) staff       (20)     1079 2023-05-02 22:37:25.000000 direct_speech_extractor_ru-0.0.1/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)       34 2023-05-02 22:37:25.000000 direct_speech_extractor_ru-0.0.1/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)     2965 2023-05-03 08:58:23.719474 direct_speech_extractor_ru-0.0.1/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     2438 2023-05-02 22:37:25.000000 direct_speech_extractor_ru-0.0.1/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-03 08:58:23.712116 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru/
--rw-r--r--   0 apple      (501) staff       (20)       28 2023-05-02 22:37:25.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     8861 2023-05-02 23:22:26.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru/main.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-03 08:58:23.718325 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2965 2023-05-03 08:58:23.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      361 2023-05-03 08:58:23.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-03 08:58:23.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2023-05-03 08:58:23.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       27 2023-05-03 08:58:23.000000 direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-03 08:58:23.720468 direct_speech_extractor_ru-0.0.1/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      852 2023-05-03 08:56:11.000000 direct_speech_extractor_ru-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:56:12.074418 direct_speech_extractor_ru-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-05-24 10:54:49.000000 direct_speech_extractor_ru-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-05-24 10:54:49.000000 direct_speech_extractor_ru-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3021 2023-05-24 10:56:12.072744 direct_speech_extractor_ru-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2478 2023-05-24 10:54:49.000000 direct_speech_extractor_ru-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 10:56:11.985520 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru/
+-rw-rw-rw-   0        0        0       29 2023-05-24 10:54:49.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru/__init__.py
+-rw-rw-rw-   0        0        0    55614 2023-05-24 10:54:49.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:56:12.067648 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/
+-rw-rw-rw-   0        0        0     3021 2023-05-24 10:56:11.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-05-24 10:56:11.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:56:11.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 10:56:11.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-24 10:56:11.000000 direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:56:12.074418 direct_speech_extractor_ru-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-05-24 10:54:49.000000 direct_speech_extractor_ru-0.0.2/setup.py
```

### Comparing `direct_speech_extractor_ru-0.0.1/LICENSE` & `direct_speech_extractor_ru-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Diana Esaian
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2023 Diana Esaian
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `direct_speech_extractor_ru-0.0.1/PKG-INFO` & `direct_speech_extractor_ru-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,40 @@
-Metadata-Version: 2.1
-Name: direct_speech_extractor_ru
-Version: 0.0.1
-Summary: Direct speech extractor for texts in Russian
-Home-page: https://github.com/diana-esaian/direct-speech-extractor-ru
-Author: Diana Esaian
-Author-email: diana.esaian@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: Russian
-Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Direct Speech Extractor
-> Python package for extracting direct speech from texts in Russian
-
-Returned attributes for the list of extracted quotes:
-
--   `text_wordcount` - word count of the whole text 
--   `direct_speech_wordcount` - word count of all the extracted quotes 
--   `ratio` - ratio of the extracted quotes to the whole text (_direct_speech_wordcount to text_wordcount_)
-
-## Installation
-Install the package using pip:
-```sh
-pip install direct-speech-extractor-ru
-```
-
-## Usage
-```python
->>> from direct-speech-extractor-ru import Extractor
->>> text = """Он добр и чувствителен, но вспыльчив. Когда на почте кто-нибудь из посетителей протестует, не соглашается или просто начинает рассуждать, то Михаил Аверьяныч багровеет, трясется всем телом и кричит громовым голосом: «Замолчать!», так что за почтовым отделением давно уже установилась репутация учреждения, в котором страшно бывать. Михаил Аверьяныч уважает и любит Андрея Ефимыча за образованность и благородство души, к прочим же обывателям относится свысока, как к своим подчиненным.
-– А вот и я! – говорит он, входя к Андрею Ефимычу. – Здравствуйте, мой дорогой! Небось я уже надоел вам, а?
-– Напротив, очень рад, – отвечает ему доктор. – Я всегда рад вам."""
-```
-In order to extract all the quotes, use the _direct_spech()_ method:
-```python
->>> extract_direct = Extractor(text)
->>> extracted = extract_direct.direct_speech()
->>> extracted
-[' «Замолчать!»',
- '– А вот и я!',
- '– Здравствуйте, мой дорогой! Небось я уже надоел вам, а?',
- '– Напротив, очень рад,',
- '– Я всегда рад вам.']
-```
-In order to extract information about the word counts and the ratio, use the method _statistics()_:
-```python
->>> extract_direct.statistics(extracted)
-{'text_wordcount': 97,
- 'direct_speech_wordcount': 21,
- 'ratio': 0.21649484536082475}
-```
+# Direct Speech Extractor
+> Python package for extracting direct speech from texts in Russian
+
+Returned attributes for the list of extracted quotes:
+
+-   `text_wordcount` - word count of the whole text 
+-   `direct_speech_wordcount` - word count of all the extracted quotes 
+-   `ratio` - ratio of the extracted quotes to the whole text (_direct_speech_wordcount to text_wordcount_)
+
+## Installation
+Install the package using pip:
+```sh
+pip install direct-speech-extractor-ru
+```
+
+## Usage
+```python
+>>> from direct-speech-extractor-ru import Extractor
+>>> text = """Он добр и чувствителен, но вспыльчив. Когда на почте кто-нибудь из посетителей протестует, не соглашается или просто начинает рассуждать, то Михаил Аверьяныч багровеет, трясется всем телом и кричит громовым голосом: «Замолчать!», так что за почтовым отделением давно уже установилась репутация учреждения, в котором страшно бывать. Михаил Аверьяныч уважает и любит Андрея Ефимыча за образованность и благородство души, к прочим же обывателям относится свысока, как к своим подчиненным.
+– А вот и я! – говорит он, входя к Андрею Ефимычу. – Здравствуйте, мой дорогой! Небось я уже надоел вам, а?
+– Напротив, очень рад, – отвечает ему доктор. – Я всегда рад вам."""
+```
+In order to extract all the quotes, use the _direct_spech()_ method:
+```python
+>>> extract_direct = Extractor(text)
+>>> extracted = extract_direct.direct_speech()
+>>> extracted
+[' «Замолчать!»',
+ '– А вот и я!',
+ '– Здравствуйте, мой дорогой! Небось я уже надоел вам, а?',
+ '– Напротив, очень рад,',
+ '– Я всегда рад вам.']
+```
+In order to extract information about the word counts and the ratio, use the method _statistics()_:
+```python
+>>> extract_direct.statistics(extracted)
+{'text_wordcount': 97,
+ 'direct_speech_wordcount': 21,
+ 'ratio': 0.21649484536082475}
+```
```

### Comparing `direct_speech_extractor_ru-0.0.1/direct_speech_extractor_ru.egg-info/PKG-INFO` & `direct_speech_extractor_ru-0.0.2/direct_speech_extractor_ru.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: direct-speech-extractor-ru
-Version: 0.0.1
-Summary: Direct speech extractor for texts in Russian
-Home-page: https://github.com/diana-esaian/direct-speech-extractor-ru
-Author: Diana Esaian
-Author-email: diana.esaian@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: Russian
-Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Direct Speech Extractor
-> Python package for extracting direct speech from texts in Russian
-
-Returned attributes for the list of extracted quotes:
-
--   `text_wordcount` - word count of the whole text 
--   `direct_speech_wordcount` - word count of all the extracted quotes 
--   `ratio` - ratio of the extracted quotes to the whole text (_direct_speech_wordcount to text_wordcount_)
-
-## Installation
-Install the package using pip:
-```sh
-pip install direct-speech-extractor-ru
-```
-
-## Usage
-```python
->>> from direct-speech-extractor-ru import Extractor
->>> text = """Он добр и чувствителен, но вспыльчив. Когда на почте кто-нибудь из посетителей протестует, не соглашается или просто начинает рассуждать, то Михаил Аверьяныч багровеет, трясется всем телом и кричит громовым голосом: «Замолчать!», так что за почтовым отделением давно уже установилась репутация учреждения, в котором страшно бывать. Михаил Аверьяныч уважает и любит Андрея Ефимыча за образованность и благородство души, к прочим же обывателям относится свысока, как к своим подчиненным.
-– А вот и я! – говорит он, входя к Андрею Ефимычу. – Здравствуйте, мой дорогой! Небось я уже надоел вам, а?
-– Напротив, очень рад, – отвечает ему доктор. – Я всегда рад вам."""
-```
-In order to extract all the quotes, use the _direct_spech()_ method:
-```python
->>> extract_direct = Extractor(text)
->>> extracted = extract_direct.direct_speech()
->>> extracted
-[' «Замолчать!»',
- '– А вот и я!',
- '– Здравствуйте, мой дорогой! Небось я уже надоел вам, а?',
- '– Напротив, очень рад,',
- '– Я всегда рад вам.']
-```
-In order to extract information about the word counts and the ratio, use the method _statistics()_:
-```python
->>> extract_direct.statistics(extracted)
-{'text_wordcount': 97,
- 'direct_speech_wordcount': 21,
- 'ratio': 0.21649484536082475}
-```
+Metadata-Version: 2.1
+Name: direct-speech-extractor-ru
+Version: 0.0.2
+Summary: Direct speech extractor for texts in Russian
+Home-page: https://github.com/diana-esaian/direct-speech-extractor-ru
+Author: Diana Esaian
+Author-email: diana.esaian@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Natural Language :: Russian
+Classifier: Topic :: Text Processing
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Direct Speech Extractor
+> Python package for extracting direct speech from texts in Russian
+
+Returned attributes for the list of extracted quotes:
+
+-   `text_wordcount` - word count of the whole text 
+-   `direct_speech_wordcount` - word count of all the extracted quotes 
+-   `ratio` - ratio of the extracted quotes to the whole text (_direct_speech_wordcount to text_wordcount_)
+
+## Installation
+Install the package using pip:
+```sh
+pip install direct-speech-extractor-ru
+```
+
+## Usage
+```python
+>>> from direct-speech-extractor-ru import Extractor
+>>> text = """Он добр и чувствителен, но вспыльчив. Когда на почте кто-нибудь из посетителей протестует, не соглашается или просто начинает рассуждать, то Михаил Аверьяныч багровеет, трясется всем телом и кричит громовым голосом: «Замолчать!», так что за почтовым отделением давно уже установилась репутация учреждения, в котором страшно бывать. Михаил Аверьяныч уважает и любит Андрея Ефимыча за образованность и благородство души, к прочим же обывателям относится свысока, как к своим подчиненным.
+– А вот и я! – говорит он, входя к Андрею Ефимычу. – Здравствуйте, мой дорогой! Небось я уже надоел вам, а?
+– Напротив, очень рад, – отвечает ему доктор. – Я всегда рад вам."""
+```
+In order to extract all the quotes, use the _direct_spech()_ method:
+```python
+>>> extract_direct = Extractor(text)
+>>> extracted = extract_direct.direct_speech()
+>>> extracted
+[' «Замолчать!»',
+ '– А вот и я!',
+ '– Здравствуйте, мой дорогой! Небось я уже надоел вам, а?',
+ '– Напротив, очень рад,',
+ '– Я всегда рад вам.']
+```
+In order to extract information about the word counts and the ratio, use the method _statistics()_:
+```python
+>>> extract_direct.statistics(extracted)
+{'text_wordcount': 97,
+ 'direct_speech_wordcount': 21,
+ 'ratio': 0.21649484536082475}
+```
```

