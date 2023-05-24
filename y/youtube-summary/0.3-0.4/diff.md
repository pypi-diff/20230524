# Comparing `tmp/youtube-summary-0.3.tar.gz` & `tmp/youtube-summary-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-summary-0.3.tar", last modified: Mon May 22 14:41:03 2023, max compression
+gzip compressed data, was "youtube-summary-0.4.tar", last modified: Wed May 24 07:45:08 2023, max compression
```

## Comparing `youtube-summary-0.3.tar` & `youtube-summary-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 14:41:03.449612 youtube-summary-0.3/
--rw-r--r--   0 maorcohen   (501) staff       (20)     1067 2023-05-21 10:58:12.000000 youtube-summary-0.3/LICENSE
--rw-r--r--   0 maorcohen   (501) staff       (20)     1620 2023-05-22 14:41:03.449468 youtube-summary-0.3/PKG-INFO
--rw-r--r--   0 maorcohen   (501) staff       (20)       38 2023-05-22 14:41:03.449656 youtube-summary-0.3/setup.cfg
--rw-r--r--   0 maorcohen   (501) staff       (20)      561 2023-05-22 14:40:50.000000 youtube-summary-0.3/setup.py
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 14:41:03.448252 youtube-summary-0.3/youtube_summary/
--rw-r--r--   0 maorcohen   (501) staff       (20)        0 2023-05-21 18:58:41.000000 youtube-summary-0.3/youtube_summary/__init__.py
--rw-r--r--   0 maorcohen   (501) staff       (20)       29 2023-05-22 10:23:51.000000 youtube-summary-0.3/youtube_summary/__main__.py
--rw-r--r--   0 maorcohen   (501) staff       (20)     6234 2023-05-22 14:23:31.000000 youtube-summary-0.3/youtube_summary/main.py
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 14:41:03.449242 youtube-summary-0.3/youtube_summary.egg-info/
--rw-r--r--   0 maorcohen   (501) staff       (20)     1620 2023-05-22 14:41:03.000000 youtube-summary-0.3/youtube_summary.egg-info/PKG-INFO
--rw-r--r--   0 maorcohen   (501) staff       (20)      332 2023-05-22 14:41:03.000000 youtube-summary-0.3/youtube_summary.egg-info/SOURCES.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)        1 2023-05-22 14:41:03.000000 youtube-summary-0.3/youtube_summary.egg-info/dependency_links.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)       61 2023-05-22 14:41:03.000000 youtube-summary-0.3/youtube_summary.egg-info/entry_points.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)     1050 2023-05-22 14:41:03.000000 youtube-summary-0.3/youtube_summary.egg-info/requires.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)       16 2023-05-22 14:41:03.000000 youtube-summary-0.3/youtube_summary.egg-info/top_level.txt
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-24 07:45:08.506552 youtube-summary-0.4/
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1067 2023-05-21 10:58:12.000000 youtube-summary-0.4/LICENSE
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1621 2023-05-24 07:45:08.506368 youtube-summary-0.4/PKG-INFO
+-rw-r--r--   0 maorcohen   (501) staff       (20)       38 2023-05-24 07:45:08.506596 youtube-summary-0.4/setup.cfg
+-rw-r--r--   0 maorcohen   (501) staff       (20)      561 2023-05-24 07:44:45.000000 youtube-summary-0.4/setup.py
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-24 07:45:08.505402 youtube-summary-0.4/youtube_summary/
+-rw-r--r--   0 maorcohen   (501) staff       (20)        0 2023-05-21 18:58:41.000000 youtube-summary-0.4/youtube_summary/__init__.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)       29 2023-05-22 10:23:51.000000 youtube-summary-0.4/youtube_summary/__main__.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)     7305 2023-05-24 07:43:48.000000 youtube-summary-0.4/youtube_summary/main.py
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-24 07:45:08.506156 youtube-summary-0.4/youtube_summary.egg-info/
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1621 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/PKG-INFO
+-rw-r--r--   0 maorcohen   (501) staff       (20)      332 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)        1 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)       61 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/entry_points.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1050 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/requires.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)       16 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/top_level.txt
```

### Comparing `youtube-summary-0.3/LICENSE` & `youtube-summary-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube-summary-0.3/PKG-INFO` & `youtube-summary-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: youtube-summary
-Version: 0.3
+Version: 0.4
 Home-page: https://github.com/mmaorc/youtube-summary-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # YouTube Summary CLI
 
 A simple CLI tool that summarizes YouTube videos.
 
 ![Screenshot](./docs/screenshot.png)
 
-The timestamp are also clickable, try them 🙂
+The timestamps are also clickable, try them 🙂
 
 ## Installation
 
 ### Install from PyPi
 You can install the application using `pip` or `pipx`:
 ```bash
 pip install --user youtube-summary
```

### Comparing `youtube-summary-0.3/setup.py` & `youtube-summary-0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="youtube-summary",
-    version="0.3",
+    version="0.4",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url="https://github.com/mmaorc/youtube-summary-cli",
     install_requires=[line.strip() for line in open("requirements.txt")],
     entry_points={
         "console_scripts": [
```

### Comparing `youtube-summary-0.3/youtube_summary/main.py` & `youtube-summary-0.4/youtube_summary/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 from langchain.callbacks import get_openai_callback
 from langchain.chains.combine_documents.map_reduce import MapReduceDocumentsChain
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from rich.console import Console
-from youtube_transcript_api import NoTranscriptFound, YouTubeTranscriptApi
+from rich.panel import Panel
+from typer.rich_utils import (
+    ALIGN_ERRORS_PANEL,
+    ERRORS_PANEL_TITLE,
+    STYLE_ERRORS_PANEL_BORDER,
+)
+from youtube_transcript_api import (
+    NoTranscriptFound,
+    TranscriptsDisabled,
+    YouTubeTranscriptApi,
+)
 
 # Define named tuple
 SectionSummary = namedtuple("SectionSummary", ["timestamp_seconds", "text"])
 
 VideoInfo = namedtuple("VideoInfo", ["id", "title"])
 
 app = typer.Typer()
@@ -65,15 +75,18 @@
         info_dict = ydl.extract_info(url, download=False)
         title = info_dict.get("title")
         id = info_dict.get("id")
         return VideoInfo(id=id, title=title)
 
 
 def get_transcripts(video_id: str) -> str:
-    transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
+    try:
+        transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
+    except TranscriptsDisabled as e:
+        raise Exception("Transcripts are disabled for this video") from e
 
     try:
         transcript = transcript_list.find_manually_created_transcript(["en"])
     except NoTranscriptFound:
         transcript = transcript_list.find_generated_transcript(["en"])
 
     subtitles = transcript.fetch()
@@ -138,47 +151,72 @@
                 timestamp_seconds=int(float(timestamp_seconds)), text=text
             )
             parsed_lines.append(parsed_line)
 
     return parsed_lines
 
 
+def pretty_timestamp(timestamp_seconds: int) -> str:
+    hours, remainder = divmod(timestamp_seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    return f"{hours}:{minutes}:{seconds}"
+
+
 def get_pretty_section_summary_text(url: str, section_summaries: str) -> str:
     parsed_section_summaries = parse_section_summaries_text(section_summaries)
     pretty_summaries = []
     for section_summary in parsed_section_summaries:
         timestamp_seconds = section_summary.timestamp_seconds
         link = f"{url}&t={timestamp_seconds}"
-        timestamp_pretty = f"{timestamp_seconds // 3600:02d}:{timestamp_seconds // 60:02d}:{timestamp_seconds % 60:02d}"
+        timestamp_pretty = pretty_timestamp(timestamp_seconds)
         summary = f"[link={link}]{timestamp_pretty}[/link]: {section_summary.text}"
         pretty_summaries.append(summary)
     return "\n".join(pretty_summaries)
 
 
+def pretty_print_exception_message(console: Console, e: Exception) -> None:
+    console.print(
+        Panel(
+            f"An error occurred: {e}",
+            border_style=STYLE_ERRORS_PANEL_BORDER,
+            title=ERRORS_PANEL_TITLE,
+            title_align=ALIGN_ERRORS_PANEL,
+            highlight=False,
+        )
+    )
+
+
 @app.command()
-def main(url: str):
+def main(url: str, debug_mode: bool = False):
     console = Console(highlight=False)
+    err_console = Console(stderr=True)
 
-    video_information = extract_video_information(url)
+    try:
+        video_information = extract_video_information(url)
 
-    subtitles = get_transcripts(video_information.id)
+        subtitles = get_transcripts(video_information.id)
 
-    with get_openai_callback() as cb:
-        section_summaries = generate_section_summaries(
-            video_information.title, subtitles
-        )
-        summary = generate_summary(video_information.title, section_summaries)
+        with get_openai_callback() as cb:
+            section_summaries = generate_section_summaries(
+                video_information.title, subtitles
+            )
+            summary = generate_summary(video_information.title, section_summaries)
 
-    console.print()
-    console.print(f"[bold]Video Title:[/bold] {video_information.title}")
+        console.print()
+        console.print(f"[bold]Video Title:[/bold] {video_information.title}")
 
-    console.print()
-    console.print("[bold]Summary:[/bold]")
-    console.print(summary)
-
-    console.print()
-    console.print("[bold]Chapter Summaries:[/bold]")
-    console.print(get_pretty_section_summary_text(url, section_summaries))
-
-    console.print()
-    console.print("[bold]OpenAI Stats:[/bold]")
-    console.print(cb)
+        console.print()
+        console.print("[bold]Summary:[/bold]")
+        console.print(summary)
+
+        console.print()
+        console.print("[bold]Chapter Summaries:[/bold]")
+        console.print(get_pretty_section_summary_text(url, section_summaries))
+
+        console.print()
+        console.print("[bold]OpenAI Stats:[/bold]")
+        console.print(cb)
+    except Exception as e:
+        if debug_mode:
+            raise e
+        pretty_print_exception_message(err_console, e)
+        raise typer.Exit(1)
```

### Comparing `youtube-summary-0.3/youtube_summary.egg-info/PKG-INFO` & `youtube-summary-0.4/youtube_summary.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: youtube-summary
-Version: 0.3
+Version: 0.4
 Home-page: https://github.com/mmaorc/youtube-summary-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # YouTube Summary CLI
 
 A simple CLI tool that summarizes YouTube videos.
 
 ![Screenshot](./docs/screenshot.png)
 
-The timestamp are also clickable, try them 🙂
+The timestamps are also clickable, try them 🙂
 
 ## Installation
 
 ### Install from PyPi
 You can install the application using `pip` or `pipx`:
 ```bash
 pip install --user youtube-summary
```

### Comparing `youtube-summary-0.3/youtube_summary.egg-info/requires.txt` & `youtube-summary-0.4/youtube_summary.egg-info/requires.txt`

 * *Files identical despite different names*

