# Comparing `tmp/transparent-background-1.2.3.tar.gz` & `tmp/transparent-background-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transparent-background-1.2.3.tar", last modified: Wed Jan 18 05:33:26 2023, max compression
+gzip compressed data, was "transparent-background-1.2.4.tar", last modified: Wed May 24 07:32:05 2023, max compression
```

## Comparing `transparent-background-1.2.3.tar` & `transparent-background-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-01-18 05:33:26.451541 transparent-background-1.2.3/
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     1067 2022-11-30 07:18:12.000000 transparent-background-1.2.3/LICENSE
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     7388 2023-01-18 05:33:26.451541 transparent-background-1.2.3/PKG-INFO
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     6921 2022-12-23 06:55:49.000000 transparent-background-1.2.3/README.md
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       86 2022-11-30 07:18:12.000000 transparent-background-1.2.3/pyproject.toml
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       38 2023-01-18 05:33:26.451541 transparent-background-1.2.3/setup.cfg
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     1064 2023-01-18 05:28:22.000000 transparent-background-1.2.3/setup.py
-drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-01-18 05:33:26.451541 transparent-background-1.2.3/transparent_background/
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     5862 2022-12-05 05:39:31.000000 transparent-background-1.2.3/transparent_background/InSPyReNet.py
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     9281 2023-01-18 05:28:15.000000 transparent-background-1.2.3/transparent_background/Remover.py
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       59 2022-11-30 07:18:12.000000 transparent-background-1.2.3/transparent_background/__init__.py
-drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-01-18 05:33:26.451541 transparent-background-1.2.3/transparent_background/backbones/
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)    25714 2022-11-30 07:18:12.000000 transparent-background-1.2.3/transparent_background/backbones/SwinTransformer.py
-drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-01-18 05:33:26.451541 transparent-background-1.2.3/transparent_background/modules/
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     3977 2022-11-30 07:18:12.000000 transparent-background-1.2.3/transparent_background/modules/attention_module.py
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     2037 2022-11-30 07:18:12.000000 transparent-background-1.2.3/transparent_background/modules/context_module.py
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     1449 2022-11-30 07:18:12.000000 transparent-background-1.2.3/transparent_background/modules/decoder_module.py
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     5608 2022-12-01 02:38:38.000000 transparent-background-1.2.3/transparent_background/modules/layers.py
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     7517 2022-12-23 08:07:20.000000 transparent-background-1.2.3/transparent_background/utils.py
-drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-01-18 05:33:26.451541 transparent-background-1.2.3/transparent_background.egg-info/
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     7388 2023-01-18 05:33:26.000000 transparent-background-1.2.3/transparent_background.egg-info/PKG-INFO
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)      699 2023-01-18 05:33:26.000000 transparent-background-1.2.3/transparent_background.egg-info/SOURCES.txt
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)        1 2023-01-18 05:33:26.000000 transparent-background-1.2.3/transparent_background.egg-info/dependency_links.txt
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       74 2023-01-18 05:33:26.000000 transparent-background-1.2.3/transparent_background.egg-info/entry_points.txt
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)      129 2023-01-18 05:33:26.000000 transparent-background-1.2.3/transparent_background.egg-info/requires.txt
--rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       23 2023-01-18 05:33:26.000000 transparent-background-1.2.3/transparent_background.egg-info/top_level.txt
+drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-05-24 07:32:05.549967 transparent-background-1.2.4/
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     1067 2022-11-30 07:18:12.000000 transparent-background-1.2.4/LICENSE
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     8311 2023-05-24 07:32:05.549967 transparent-background-1.2.4/PKG-INFO
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     7844 2023-05-24 07:30:19.000000 transparent-background-1.2.4/README.md
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       86 2022-11-30 07:18:12.000000 transparent-background-1.2.4/pyproject.toml
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       38 2023-05-24 07:32:05.549967 transparent-background-1.2.4/setup.cfg
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     1064 2023-05-24 07:29:45.000000 transparent-background-1.2.4/setup.py
+drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-05-24 07:32:05.549967 transparent-background-1.2.4/transparent_background/
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     5862 2023-05-24 07:11:24.000000 transparent-background-1.2.4/transparent_background/InSPyReNet.py
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     9744 2023-05-24 07:14:36.000000 transparent-background-1.2.4/transparent_background/Remover.py
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       59 2022-11-30 07:18:12.000000 transparent-background-1.2.4/transparent_background/__init__.py
+drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-05-24 07:32:05.549967 transparent-background-1.2.4/transparent_background/backbones/
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)    25714 2022-11-30 07:18:12.000000 transparent-background-1.2.4/transparent_background/backbones/SwinTransformer.py
+drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-05-24 07:32:05.549967 transparent-background-1.2.4/transparent_background/modules/
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     3977 2022-11-30 07:18:12.000000 transparent-background-1.2.4/transparent_background/modules/attention_module.py
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     2037 2022-11-30 07:18:12.000000 transparent-background-1.2.4/transparent_background/modules/context_module.py
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     1449 2022-11-30 07:18:12.000000 transparent-background-1.2.4/transparent_background/modules/decoder_module.py
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     5608 2022-12-01 02:38:38.000000 transparent-background-1.2.4/transparent_background/modules/layers.py
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     7517 2023-05-24 07:11:24.000000 transparent-background-1.2.4/transparent_background/utils.py
+drwxrwxr-x   0 taehoon1018  (1000) taehoon1018  (1000)        0 2023-05-24 07:32:05.549967 transparent-background-1.2.4/transparent_background.egg-info/
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)     8311 2023-05-24 07:32:05.000000 transparent-background-1.2.4/transparent_background.egg-info/PKG-INFO
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)      699 2023-05-24 07:32:05.000000 transparent-background-1.2.4/transparent_background.egg-info/SOURCES.txt
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)        1 2023-05-24 07:32:05.000000 transparent-background-1.2.4/transparent_background.egg-info/dependency_links.txt
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       74 2023-05-24 07:32:05.000000 transparent-background-1.2.4/transparent_background.egg-info/entry_points.txt
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)      129 2023-05-24 07:32:05.000000 transparent-background-1.2.4/transparent_background.egg-info/requires.txt
+-rw-rw-r--   0 taehoon1018  (1000) taehoon1018  (1000)       23 2023-05-24 07:32:05.000000 transparent-background-1.2.4/transparent_background.egg-info/top_level.txt
```

### Comparing `transparent-background-1.2.3/LICENSE` & `transparent-background-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/PKG-INFO` & `transparent-background-1.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: transparent-background
-Version: 1.2.3
-Summary: Make images with transparent background
-Home-page: https://github.com/plemeri/transparent-background
-Author: Taehun Kim
-Author-email: taehoon1018@postech.ac.kr
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Transparent Background
 
 <p align="center">
     <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/logo.png width=200px>
 </p>
 <p align="center">
     <a href="https://github.com/plemeri/transparent-background/blob/main/LICENSE"><img  src="https://img.shields.io/badge/license-MIT-blue"></a>
@@ -26,14 +12,18 @@
 
 This is a background removing tool powered by [InSPyReNet (ACCV 2022)](https://github.com/plemeri/InSPyReNet.git). You can easily remove background from the image or video or bunch of other stuffs when you can make the background transparent!
 
 Image | Video | Webcam
 :-:|:-:|:-:
 <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_aeroplane.gif height=200px> | <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_b5.gif height=200px> | <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_webcam.gif height=200px>
 
+## :newspaper: News
+
+Our package is currently not working properly on small images without `--fast` argument. Sorry for the inconvenience and we'll fix this issue with better algorithm coming out shortly.
+
 ## :inbox_tray: Installation
 
 ### Dependencies (python packages)
 
 package | version (>=)
 :-|:-
 `pytorch`       | `1.7.1`
@@ -103,14 +93,16 @@
     * Folder containing videos - `path/to/vid/folder`
     * Integer for webcam address - `0` (e.g., if your webcam is at `/dev/video0`.)
 * `--dest [DEST]` (optional): Specify your destination folder. Default location is current directory.
 * `--type [TYPE]` (optional): Choose between `rgba`, `map` `green`, `blur`, `overlay`, and another image file. Default is `rgba`.
     * `rgba` will generate RGBA output regarding saliency score as an alpha map. Note that this will not work for video and webcam input. 
     * `map` will output saliency map only. 
     * `green` will change the background with green screen. 
+    * `white` will change the background with white color. -> [2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) 
+    * `'[255, 0, 0]'` will change the background with color code [255, 0, 0]. Please use with single quotes. -> [2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) 
     * `blur` will blur the background.
     * `overlay` will cover the salient object with translucent green color, and highlight the edges.
     * Another image file (e.g., `samples/backgroud.png`) will be used as a background, and the object will be overlapped on it.
 * `--ckpt [CKPT]` (optional): Use other checkpoint file. Default is trained with composite dataset and will be automatically downloaded if not available. Please refer to [Model Zoo](https://github.com/plemeri/InSPyReNet/blob/main/docs/model_zoo.md) from [InSPyReNet](https://github.com/plemeri/InSPyReNet) for available pre-trained checkpoints.
 * `--fast` (optional): Fast mode. If specified, it will use low-resolution input and model trained with LR scale. May decrease performance but reduces inference time and gpu memory usage. 
 * `--jit` (optional): Torchscript mode. If specified, it will trace model with pytorch built-in torchscript JIT compiler. May cause delay in initialization, but reduces inference time and gpu memory usage.
     
@@ -129,14 +121,16 @@
 # Usage for image
 img = Image.open('samples/aeroplane.jpg').convert('RGB') # read image
 
 out = remover.process(img) # default setting - transparent background
 out = remover.process(img, type='rgba') # same as above
 out = remover.process(img, type='map') # object map only
 out = remover.process(img, type='green') # image matting - green screen
+out = remover.process(img, type='white') # change backround with white color -> [2023.05.24] Contributed by carpedm20
+out = remover.process(img, type=[255, 0, 0]) # change background with color code [255, 0, 0] -> [2023.05.24] Contributed by carpedm20
 out = remover.process(img, type='blur') # blur background
 out = remover.process(img, type='overlay') # overlay object map onto the image
 out = remover.process(img, type='samples/background.jpg') # use another image as a background
 
 Image.fromarray(out).save('output.png') # save result
 
 # Usage for video
@@ -160,14 +154,18 @@
     out = remover.process(img, type='map') # same as image, except for 'rgba' which is not for video.
     writer.write(cv2.cvtColor(out, cv2.COLOR_BGR2RGB))
 
 cap.release()
 writer.release()
 ```
 
+## :tv: Tutorial
+
+[rsreetech](https://github.com/rsreetech) shared a tutorial using colab. [[Youtube](https://www.youtube.com/watch?v=jKuQEnKmv4A)]
+
 ## :outbox_tray: Uninstall
 
 ```
 pip uninstall transparent-background
 ```
 
 ## :page_facing_up: Licence
```

#### html2text {}

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.1 Name: transparent-background Version: 1.2.3 Summary: Make
-images with transparent background Home-page: https://github.com/plemeri/
-transparent-background Author: Taehun Kim Author-email:
-taehoon1018@postech.ac.kr Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE # Transparent Background
+# Transparent Background
 [https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/
                                    logo.png]
                [https://img.shields.io/badge/license-MIT-blue]
 This is a background removing tool powered by [InSPyReNet (ACCV 2022)](https://
 github.com/plemeri/InSPyReNet.git). You can easily remove background from the
 image or video or bunch of other stuffs when you can make the background
 transparent! Image | Video | Webcam :-:|:-:|:-: [https://
 raw.githubusercontent.com/plemeri/transparent-background/main/figures/
 demo_aeroplane.gif] | [https://raw.githubusercontent.com/plemeri/transparent-
 background/main/figures/demo_b5.gif] | [https://raw.githubusercontent.com/
-plemeri/transparent-background/main/figures/demo_webcam.gif] ## :inbox_tray:
-Installation ### Dependencies (python packages) package | version (>=) :-|:
-- `pytorch` | `1.7.1` `torchvision` | `0.8.2` `opencv-python` | `4.6.0.66`
-`timm` | `0.6.11` `tqdm` | `4.64.1` `kornia` | `0.5.4` `gdown` | `4.5.4`
-`pyvirtualcam` | `0.6.0` Note: If you have any problem with [`pyvirtualcam`]
-(https://pypi.org/project/pyvirtualcam/), please visit their github repository
-or pypi homepage. Due to the backend workflow for Windows and macOS, we only
-support Linux for webcam input. ### Dependencies (webcam input) We basically
-follow the virtual camera settings from [`pyvirtualcam`](https://pypi.org/
-project/pyvirtualcam/). If you do not choose to install virtual camera, it will
-visualize real-time output with `cv2.imshow`. #### A. Linux (v4l2loopback)
-```bash # Install v4l2loopback for webcam relay $ git clone https://github.com/
-umlaeute/v4l2loopback.git && cd v4l2loopback $ make && sudo make install $ sudo
-depmod -a # Create virtual webcam $ sudo modprobe v4l2loopback devices=1 ```
-Note: If you have any problem with installing [`v4l2loopback`](https://
-github.com/umlaeute/v4l2loopback), please visit their github repository. ####
-B. Windows (OBS) Install OBS virtual camera from [install OBS](https://
-obsproject.com/). #### C. macOS (OBS) [not stable] Follow the steps below. *
-[Install OBS](https://obsproject.com/). * Start OBS. * Click "Start Virtual
-Camera" (bottom right), then "Stop Virtual Camera". * Close OBS. ### Install
-`transperent-background` ```bash # via pypi $ pip install transparent-
-background # via github $ pip install git+https://github.com/plemeri/
-transparent-background.git # locally $ pip install . ``` ## :pencil2: Usage ###
-:computer: Command Line ```bash # for apple silicon mps backend, use
-"PYTORCH_ENABLE_MPS_FALLBACK=1" before the command (requires torch >= 1.13) $
-transparent-background --source [SOURCE] --dest [DEST] --type [TYPE] --ckpt
-[CKPT] (--fast) (--jit) ``` * `--source [SOURCE]`: Specify your data in this
-argument. * Single image - `image.png` * Folder containing images - `path/to/
-img/folder` * Single video - `video.mp4` * Folder containing videos - `path/to/
-vid/folder` * Integer for webcam address - `0` (e.g., if your webcam is at `/
-dev/video0`.) * `--dest [DEST]` (optional): Specify your destination folder.
+plemeri/transparent-background/main/figures/demo_webcam.gif] ## :newspaper:
+News Our package is currently not working properly on small images without `--
+fast` argument. Sorry for the inconvenience and we'll fix this issue with
+better algorithm coming out shortly. ## :inbox_tray: Installation ###
+Dependencies (python packages) package | version (>=) :-|:- `pytorch` | `1.7.1`
+`torchvision` | `0.8.2` `opencv-python` | `4.6.0.66` `timm` | `0.6.11` `tqdm` |
+`4.64.1` `kornia` | `0.5.4` `gdown` | `4.5.4` `pyvirtualcam` | `0.6.0` Note: If
+you have any problem with [`pyvirtualcam`](https://pypi.org/project/
+pyvirtualcam/), please visit their github repository or pypi homepage. Due to
+the backend workflow for Windows and macOS, we only support Linux for webcam
+input. ### Dependencies (webcam input) We basically follow the virtual camera
+settings from [`pyvirtualcam`](https://pypi.org/project/pyvirtualcam/). If you
+do not choose to install virtual camera, it will visualize real-time output
+with `cv2.imshow`. #### A. Linux (v4l2loopback) ```bash # Install v4l2loopback
+for webcam relay $ git clone https://github.com/umlaeute/v4l2loopback.git && cd
+v4l2loopback $ make && sudo make install $ sudo depmod -a # Create virtual
+webcam $ sudo modprobe v4l2loopback devices=1 ``` Note: If you have any problem
+with installing [`v4l2loopback`](https://github.com/umlaeute/v4l2loopback),
+please visit their github repository. #### B. Windows (OBS) Install OBS virtual
+camera from [install OBS](https://obsproject.com/). #### C. macOS (OBS) [not
+stable] Follow the steps below. * [Install OBS](https://obsproject.com/). *
+Start OBS. * Click "Start Virtual Camera" (bottom right), then "Stop Virtual
+Camera". * Close OBS. ### Install `transperent-background` ```bash # via pypi $
+pip install transparent-background # via github $ pip install git+https://
+github.com/plemeri/transparent-background.git # locally $ pip install . ``` ##
+:pencil2: Usage ### :computer: Command Line ```bash # for apple silicon mps
+backend, use "PYTORCH_ENABLE_MPS_FALLBACK=1" before the command (requires torch
+>= 1.13) $ transparent-background --source [SOURCE] --dest [DEST] --type [TYPE]
+--ckpt [CKPT] (--fast) (--jit) ``` * `--source [SOURCE]`: Specify your data in
+this argument. * Single image - `image.png` * Folder containing images - `path/
+to/img/folder` * Single video - `video.mp4` * Folder containing videos - `path/
+to/vid/folder` * Integer for webcam address - `0` (e.g., if your webcam is at
+`/dev/video0`.) * `--dest [DEST]` (optional): Specify your destination folder.
 Default location is current directory. * `--type [TYPE]` (optional): Choose
 between `rgba`, `map` `green`, `blur`, `overlay`, and another image file.
 Default is `rgba`. * `rgba` will generate RGBA output regarding saliency score
 as an alpha map. Note that this will not work for video and webcam input. *
 `map` will output saliency map only. * `green` will change the background with
-green screen. * `blur` will blur the background. * `overlay` will cover the
+green screen. * `white` will change the background with white color. ->
+[2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) * `'[255,
+0, 0]'` will change the background with color code [255, 0, 0]. Please use with
+single quotes. -> [2023.05.24] Contributed by [carpedm20](https://github.com/
+carpedm20) * `blur` will blur the background. * `overlay` will cover the
 salient object with translucent green color, and highlight the edges. * Another
 image file (e.g., `samples/backgroud.png`) will be used as a background, and
 the object will be overlapped on it. * `--ckpt [CKPT]` (optional): Use other
 checkpoint file. Default is trained with composite dataset and will be
 automatically downloaded if not available. Please refer to [Model Zoo](https://
 github.com/plemeri/InSPyReNet/blob/main/docs/model_zoo.md) from [InSPyReNet]
 (https://github.com/plemeri/InSPyReNet) for available pre-trained checkpoints.
@@ -68,23 +68,28 @@
 PIL import Image from transparent_background import Remover # Load model
 remover = Remover() # default setting remover = Remover(fast=True, jit=True,
 device='cuda:0', ckpt='~/latest.pth') # custom setting # Usage for image img =
 Image.open('samples/aeroplane.jpg').convert('RGB') # read image out =
 remover.process(img) # default setting - transparent background out =
 remover.process(img, type='rgba') # same as above out = remover.process(img,
 type='map') # object map only out = remover.process(img, type='green') # image
-matting - green screen out = remover.process(img, type='blur') # blur
-background out = remover.process(img, type='overlay') # overlay object map onto
-the image out = remover.process(img, type='samples/background.jpg') # use
-another image as a background Image.fromarray(out).save('output.png') # save
-result # Usage for video cap = cv2.VideoCapture('samples/b5.mp4') # video
-reader for input fps = cap.get(cv2.CAP_PROP_FPS) writer = None while
-cap.isOpened(): ret, frame = cap.read() # read video if ret is False: break
-frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB) img = Image.fromarray
+matting - green screen out = remover.process(img, type='white') # change
+backround with white color -> [2023.05.24] Contributed by carpedm20 out =
+remover.process(img, type=[255, 0, 0]) # change background with color code
+[255, 0, 0] -> [2023.05.24] Contributed by carpedm20 out = remover.process(img,
+type='blur') # blur background out = remover.process(img, type='overlay') #
+overlay object map onto the image out = remover.process(img, type='samples/
+background.jpg') # use another image as a background Image.fromarray(out).save
+('output.png') # save result # Usage for video cap = cv2.VideoCapture('samples/
+b5.mp4') # video reader for input fps = cap.get(cv2.CAP_PROP_FPS) writer = None
+while cap.isOpened(): ret, frame = cap.read() # read video if ret is False:
+break frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB) img = Image.fromarray
 (frame).convert('RGB') if writer is None: writer = cv2.VideoWriter
 ('output.mp4', cv2.VideoWriter_fourcc(*'mp4v'), fps, img.size) # video writer
 for output out = remover.process(img, type='map') # same as image, except for
 'rgba' which is not for video. writer.write(cv2.cvtColor(out,
-cv2.COLOR_BGR2RGB)) cap.release() writer.release() ``` ## :outbox_tray:
+cv2.COLOR_BGR2RGB)) cap.release() writer.release() ``` ## :tv: Tutorial
+[rsreetech](https://github.com/rsreetech) shared a tutorial using colab. [
+[Youtube](https://www.youtube.com/watch?v=jKuQEnKmv4A)] ## :outbox_tray:
 Uninstall ``` pip uninstall transparent-background ``` ## :page_facing_up:
 Licence See [LICENCE](https://github.com/plemeri/transparent-background/blob/
 main/LICENSE) for more details.
```

### Comparing `transparent-background-1.2.3/README.md` & `transparent-background-1.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: transparent-background
+Version: 1.2.4
+Summary: Make images with transparent background
+Home-page: https://github.com/plemeri/transparent-background
+Author: Taehun Kim
+Author-email: taehoon1018@postech.ac.kr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Transparent Background
 
 <p align="center">
     <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/logo.png width=200px>
 </p>
 <p align="center">
     <a href="https://github.com/plemeri/transparent-background/blob/main/LICENSE"><img  src="https://img.shields.io/badge/license-MIT-blue"></a>
@@ -12,14 +26,18 @@
 
 This is a background removing tool powered by [InSPyReNet (ACCV 2022)](https://github.com/plemeri/InSPyReNet.git). You can easily remove background from the image or video or bunch of other stuffs when you can make the background transparent!
 
 Image | Video | Webcam
 :-:|:-:|:-:
 <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_aeroplane.gif height=200px> | <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_b5.gif height=200px> | <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_webcam.gif height=200px>
 
+## :newspaper: News
+
+Our package is currently not working properly on small images without `--fast` argument. Sorry for the inconvenience and we'll fix this issue with better algorithm coming out shortly.
+
 ## :inbox_tray: Installation
 
 ### Dependencies (python packages)
 
 package | version (>=)
 :-|:-
 `pytorch`       | `1.7.1`
@@ -89,14 +107,16 @@
     * Folder containing videos - `path/to/vid/folder`
     * Integer for webcam address - `0` (e.g., if your webcam is at `/dev/video0`.)
 * `--dest [DEST]` (optional): Specify your destination folder. Default location is current directory.
 * `--type [TYPE]` (optional): Choose between `rgba`, `map` `green`, `blur`, `overlay`, and another image file. Default is `rgba`.
     * `rgba` will generate RGBA output regarding saliency score as an alpha map. Note that this will not work for video and webcam input. 
     * `map` will output saliency map only. 
     * `green` will change the background with green screen. 
+    * `white` will change the background with white color. -> [2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) 
+    * `'[255, 0, 0]'` will change the background with color code [255, 0, 0]. Please use with single quotes. -> [2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) 
     * `blur` will blur the background.
     * `overlay` will cover the salient object with translucent green color, and highlight the edges.
     * Another image file (e.g., `samples/backgroud.png`) will be used as a background, and the object will be overlapped on it.
 * `--ckpt [CKPT]` (optional): Use other checkpoint file. Default is trained with composite dataset and will be automatically downloaded if not available. Please refer to [Model Zoo](https://github.com/plemeri/InSPyReNet/blob/main/docs/model_zoo.md) from [InSPyReNet](https://github.com/plemeri/InSPyReNet) for available pre-trained checkpoints.
 * `--fast` (optional): Fast mode. If specified, it will use low-resolution input and model trained with LR scale. May decrease performance but reduces inference time and gpu memory usage. 
 * `--jit` (optional): Torchscript mode. If specified, it will trace model with pytorch built-in torchscript JIT compiler. May cause delay in initialization, but reduces inference time and gpu memory usage.
     
@@ -115,14 +135,16 @@
 # Usage for image
 img = Image.open('samples/aeroplane.jpg').convert('RGB') # read image
 
 out = remover.process(img) # default setting - transparent background
 out = remover.process(img, type='rgba') # same as above
 out = remover.process(img, type='map') # object map only
 out = remover.process(img, type='green') # image matting - green screen
+out = remover.process(img, type='white') # change backround with white color -> [2023.05.24] Contributed by carpedm20
+out = remover.process(img, type=[255, 0, 0]) # change background with color code [255, 0, 0] -> [2023.05.24] Contributed by carpedm20
 out = remover.process(img, type='blur') # blur background
 out = remover.process(img, type='overlay') # overlay object map onto the image
 out = remover.process(img, type='samples/background.jpg') # use another image as a background
 
 Image.fromarray(out).save('output.png') # save result
 
 # Usage for video
@@ -146,14 +168,18 @@
     out = remover.process(img, type='map') # same as image, except for 'rgba' which is not for video.
     writer.write(cv2.cvtColor(out, cv2.COLOR_BGR2RGB))
 
 cap.release()
 writer.release()
 ```
 
+## :tv: Tutorial
+
+[rsreetech](https://github.com/rsreetech) shared a tutorial using colab. [[Youtube](https://www.youtube.com/watch?v=jKuQEnKmv4A)]
+
 ## :outbox_tray: Uninstall
 
 ```
 pip uninstall transparent-background
 ```
 
 ## :page_facing_up: Licence
```

#### html2text {}

```diff
@@ -1,55 +1,67 @@
-# Transparent Background
+Metadata-Version: 2.1 Name: transparent-background Version: 1.2.4 Summary: Make
+images with transparent background Home-page: https://github.com/plemeri/
+transparent-background Author: Taehun Kim Author-email:
+taehoon1018@postech.ac.kr Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE # Transparent Background
 [https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/
                                    logo.png]
                [https://img.shields.io/badge/license-MIT-blue]
 This is a background removing tool powered by [InSPyReNet (ACCV 2022)](https://
 github.com/plemeri/InSPyReNet.git). You can easily remove background from the
 image or video or bunch of other stuffs when you can make the background
 transparent! Image | Video | Webcam :-:|:-:|:-: [https://
 raw.githubusercontent.com/plemeri/transparent-background/main/figures/
 demo_aeroplane.gif] | [https://raw.githubusercontent.com/plemeri/transparent-
 background/main/figures/demo_b5.gif] | [https://raw.githubusercontent.com/
-plemeri/transparent-background/main/figures/demo_webcam.gif] ## :inbox_tray:
-Installation ### Dependencies (python packages) package | version (>=) :-|:
-- `pytorch` | `1.7.1` `torchvision` | `0.8.2` `opencv-python` | `4.6.0.66`
-`timm` | `0.6.11` `tqdm` | `4.64.1` `kornia` | `0.5.4` `gdown` | `4.5.4`
-`pyvirtualcam` | `0.6.0` Note: If you have any problem with [`pyvirtualcam`]
-(https://pypi.org/project/pyvirtualcam/), please visit their github repository
-or pypi homepage. Due to the backend workflow for Windows and macOS, we only
-support Linux for webcam input. ### Dependencies (webcam input) We basically
-follow the virtual camera settings from [`pyvirtualcam`](https://pypi.org/
-project/pyvirtualcam/). If you do not choose to install virtual camera, it will
-visualize real-time output with `cv2.imshow`. #### A. Linux (v4l2loopback)
-```bash # Install v4l2loopback for webcam relay $ git clone https://github.com/
-umlaeute/v4l2loopback.git && cd v4l2loopback $ make && sudo make install $ sudo
-depmod -a # Create virtual webcam $ sudo modprobe v4l2loopback devices=1 ```
-Note: If you have any problem with installing [`v4l2loopback`](https://
-github.com/umlaeute/v4l2loopback), please visit their github repository. ####
-B. Windows (OBS) Install OBS virtual camera from [install OBS](https://
-obsproject.com/). #### C. macOS (OBS) [not stable] Follow the steps below. *
-[Install OBS](https://obsproject.com/). * Start OBS. * Click "Start Virtual
-Camera" (bottom right), then "Stop Virtual Camera". * Close OBS. ### Install
-`transperent-background` ```bash # via pypi $ pip install transparent-
-background # via github $ pip install git+https://github.com/plemeri/
-transparent-background.git # locally $ pip install . ``` ## :pencil2: Usage ###
-:computer: Command Line ```bash # for apple silicon mps backend, use
-"PYTORCH_ENABLE_MPS_FALLBACK=1" before the command (requires torch >= 1.13) $
-transparent-background --source [SOURCE] --dest [DEST] --type [TYPE] --ckpt
-[CKPT] (--fast) (--jit) ``` * `--source [SOURCE]`: Specify your data in this
-argument. * Single image - `image.png` * Folder containing images - `path/to/
-img/folder` * Single video - `video.mp4` * Folder containing videos - `path/to/
-vid/folder` * Integer for webcam address - `0` (e.g., if your webcam is at `/
-dev/video0`.) * `--dest [DEST]` (optional): Specify your destination folder.
+plemeri/transparent-background/main/figures/demo_webcam.gif] ## :newspaper:
+News Our package is currently not working properly on small images without `--
+fast` argument. Sorry for the inconvenience and we'll fix this issue with
+better algorithm coming out shortly. ## :inbox_tray: Installation ###
+Dependencies (python packages) package | version (>=) :-|:- `pytorch` | `1.7.1`
+`torchvision` | `0.8.2` `opencv-python` | `4.6.0.66` `timm` | `0.6.11` `tqdm` |
+`4.64.1` `kornia` | `0.5.4` `gdown` | `4.5.4` `pyvirtualcam` | `0.6.0` Note: If
+you have any problem with [`pyvirtualcam`](https://pypi.org/project/
+pyvirtualcam/), please visit their github repository or pypi homepage. Due to
+the backend workflow for Windows and macOS, we only support Linux for webcam
+input. ### Dependencies (webcam input) We basically follow the virtual camera
+settings from [`pyvirtualcam`](https://pypi.org/project/pyvirtualcam/). If you
+do not choose to install virtual camera, it will visualize real-time output
+with `cv2.imshow`. #### A. Linux (v4l2loopback) ```bash # Install v4l2loopback
+for webcam relay $ git clone https://github.com/umlaeute/v4l2loopback.git && cd
+v4l2loopback $ make && sudo make install $ sudo depmod -a # Create virtual
+webcam $ sudo modprobe v4l2loopback devices=1 ``` Note: If you have any problem
+with installing [`v4l2loopback`](https://github.com/umlaeute/v4l2loopback),
+please visit their github repository. #### B. Windows (OBS) Install OBS virtual
+camera from [install OBS](https://obsproject.com/). #### C. macOS (OBS) [not
+stable] Follow the steps below. * [Install OBS](https://obsproject.com/). *
+Start OBS. * Click "Start Virtual Camera" (bottom right), then "Stop Virtual
+Camera". * Close OBS. ### Install `transperent-background` ```bash # via pypi $
+pip install transparent-background # via github $ pip install git+https://
+github.com/plemeri/transparent-background.git # locally $ pip install . ``` ##
+:pencil2: Usage ### :computer: Command Line ```bash # for apple silicon mps
+backend, use "PYTORCH_ENABLE_MPS_FALLBACK=1" before the command (requires torch
+>= 1.13) $ transparent-background --source [SOURCE] --dest [DEST] --type [TYPE]
+--ckpt [CKPT] (--fast) (--jit) ``` * `--source [SOURCE]`: Specify your data in
+this argument. * Single image - `image.png` * Folder containing images - `path/
+to/img/folder` * Single video - `video.mp4` * Folder containing videos - `path/
+to/vid/folder` * Integer for webcam address - `0` (e.g., if your webcam is at
+`/dev/video0`.) * `--dest [DEST]` (optional): Specify your destination folder.
 Default location is current directory. * `--type [TYPE]` (optional): Choose
 between `rgba`, `map` `green`, `blur`, `overlay`, and another image file.
 Default is `rgba`. * `rgba` will generate RGBA output regarding saliency score
 as an alpha map. Note that this will not work for video and webcam input. *
 `map` will output saliency map only. * `green` will change the background with
-green screen. * `blur` will blur the background. * `overlay` will cover the
+green screen. * `white` will change the background with white color. ->
+[2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) * `'[255,
+0, 0]'` will change the background with color code [255, 0, 0]. Please use with
+single quotes. -> [2023.05.24] Contributed by [carpedm20](https://github.com/
+carpedm20) * `blur` will blur the background. * `overlay` will cover the
 salient object with translucent green color, and highlight the edges. * Another
 image file (e.g., `samples/backgroud.png`) will be used as a background, and
 the object will be overlapped on it. * `--ckpt [CKPT]` (optional): Use other
 checkpoint file. Default is trained with composite dataset and will be
 automatically downloaded if not available. Please refer to [Model Zoo](https://
 github.com/plemeri/InSPyReNet/blob/main/docs/model_zoo.md) from [InSPyReNet]
 (https://github.com/plemeri/InSPyReNet) for available pre-trained checkpoints.
@@ -62,23 +74,28 @@
 PIL import Image from transparent_background import Remover # Load model
 remover = Remover() # default setting remover = Remover(fast=True, jit=True,
 device='cuda:0', ckpt='~/latest.pth') # custom setting # Usage for image img =
 Image.open('samples/aeroplane.jpg').convert('RGB') # read image out =
 remover.process(img) # default setting - transparent background out =
 remover.process(img, type='rgba') # same as above out = remover.process(img,
 type='map') # object map only out = remover.process(img, type='green') # image
-matting - green screen out = remover.process(img, type='blur') # blur
-background out = remover.process(img, type='overlay') # overlay object map onto
-the image out = remover.process(img, type='samples/background.jpg') # use
-another image as a background Image.fromarray(out).save('output.png') # save
-result # Usage for video cap = cv2.VideoCapture('samples/b5.mp4') # video
-reader for input fps = cap.get(cv2.CAP_PROP_FPS) writer = None while
-cap.isOpened(): ret, frame = cap.read() # read video if ret is False: break
-frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB) img = Image.fromarray
+matting - green screen out = remover.process(img, type='white') # change
+backround with white color -> [2023.05.24] Contributed by carpedm20 out =
+remover.process(img, type=[255, 0, 0]) # change background with color code
+[255, 0, 0] -> [2023.05.24] Contributed by carpedm20 out = remover.process(img,
+type='blur') # blur background out = remover.process(img, type='overlay') #
+overlay object map onto the image out = remover.process(img, type='samples/
+background.jpg') # use another image as a background Image.fromarray(out).save
+('output.png') # save result # Usage for video cap = cv2.VideoCapture('samples/
+b5.mp4') # video reader for input fps = cap.get(cv2.CAP_PROP_FPS) writer = None
+while cap.isOpened(): ret, frame = cap.read() # read video if ret is False:
+break frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB) img = Image.fromarray
 (frame).convert('RGB') if writer is None: writer = cv2.VideoWriter
 ('output.mp4', cv2.VideoWriter_fourcc(*'mp4v'), fps, img.size) # video writer
 for output out = remover.process(img, type='map') # same as image, except for
 'rgba' which is not for video. writer.write(cv2.cvtColor(out,
-cv2.COLOR_BGR2RGB)) cap.release() writer.release() ``` ## :outbox_tray:
+cv2.COLOR_BGR2RGB)) cap.release() writer.release() ``` ## :tv: Tutorial
+[rsreetech](https://github.com/rsreetech) shared a tutorial using colab. [
+[Youtube](https://www.youtube.com/watch?v=jKuQEnKmv4A)] ## :outbox_tray:
 Uninstall ``` pip uninstall transparent-background ``` ## :page_facing_up:
 Licence See [LICENCE](https://github.com/plemeri/transparent-background/blob/
 main/LICENSE) for more details.
```

### Comparing `transparent-background-1.2.3/setup.py` & `transparent-background-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="transparent-background",
-    version="1.2.3",
+    version="1.2.4",
     author="Taehun Kim",
     author_email="taehoon1018@postech.ac.kr",
     description="Make images with transparent background",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/plemeri/transparent-background",
     packages=['transparent_background', 'transparent_background.modules', 'transparent_background.backbones'],
```

### Comparing `transparent-background-1.2.3/transparent_background/InSPyReNet.py` & `transparent-background-1.2.4/transparent_background/InSPyReNet.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background/Remover.py` & `transparent-background-1.2.4/transparent_background/Remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,27 +112,38 @@
             pred = self.model(x)
 
         pred = F.interpolate(pred, shape, mode='bilinear', align_corners=True)
         pred = pred.data.cpu()
         pred = pred.numpy().squeeze()   
         
         img = np.array(img)
+
+        if type.startswith('['):
+            type = [int(i) for i in type[1:-1].split(',')]
         
         if type == 'map':
             img = (np.stack([pred] * 3, axis=-1) * 255).astype(np.uint8)
 
         elif type == 'rgba':
             r, g, b = cv2.split(img)
             pred = (pred * 255).astype(np.uint8)
             img = cv2.merge([r, g, b, pred])
 
         elif type == 'green':
             bg = np.stack([np.ones_like(pred)] * 3, axis=-1) * [120, 255, 155]
             img = img * pred[..., np.newaxis] + bg * (1 - pred[..., np.newaxis])
 
+        elif type == "white":
+            bg = np.stack([np.ones_like(pred)] * 3, axis=-1) * [255, 255, 255]
+            img = img * pred[..., np.newaxis] + bg * (1 - pred[..., np.newaxis])
+
+        elif len(type) == 3:
+            bg = np.stack([np.ones_like(pred)] * 3, axis=-1) * type
+            img = img * pred[..., np.newaxis] + bg * (1 - pred[..., np.newaxis])
+
         elif type == 'blur':
             img = img * pred[..., np.newaxis] + cv2.GaussianBlur(img, (0, 0), 15) * (1 - pred[..., np.newaxis])
 
         elif type == 'overlay':
             bg = (np.stack([np.ones_like(pred)] * 3, axis=-1) * [120, 255, 155] + img) // 2
             img = bg * pred[..., np.newaxis] + img * (1 - pred[..., np.newaxis])
             border = cv2.Canny(((pred > .5) * 255).astype(np.uint8), 50, 100)
```

### Comparing `transparent-background-1.2.3/transparent_background/backbones/SwinTransformer.py` & `transparent-background-1.2.4/transparent_background/backbones/SwinTransformer.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background/modules/attention_module.py` & `transparent-background-1.2.4/transparent_background/modules/attention_module.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background/modules/context_module.py` & `transparent-background-1.2.4/transparent_background/modules/context_module.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background/modules/decoder_module.py` & `transparent-background-1.2.4/transparent_background/modules/decoder_module.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background/modules/layers.py` & `transparent-background-1.2.4/transparent_background/modules/layers.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background/utils.py` & `transparent-background-1.2.4/transparent_background/utils.py`

 * *Files identical despite different names*

### Comparing `transparent-background-1.2.3/transparent_background.egg-info/PKG-INFO` & `transparent-background-1.2.4/transparent_background.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transparent-background
-Version: 1.2.3
+Version: 1.2.4
 Summary: Make images with transparent background
 Home-page: https://github.com/plemeri/transparent-background
 Author: Taehun Kim
 Author-email: taehoon1018@postech.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,18 @@
 
 This is a background removing tool powered by [InSPyReNet (ACCV 2022)](https://github.com/plemeri/InSPyReNet.git). You can easily remove background from the image or video or bunch of other stuffs when you can make the background transparent!
 
 Image | Video | Webcam
 :-:|:-:|:-:
 <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_aeroplane.gif height=200px> | <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_b5.gif height=200px> | <img src=https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/demo_webcam.gif height=200px>
 
+## :newspaper: News
+
+Our package is currently not working properly on small images without `--fast` argument. Sorry for the inconvenience and we'll fix this issue with better algorithm coming out shortly.
+
 ## :inbox_tray: Installation
 
 ### Dependencies (python packages)
 
 package | version (>=)
 :-|:-
 `pytorch`       | `1.7.1`
@@ -103,14 +107,16 @@
     * Folder containing videos - `path/to/vid/folder`
     * Integer for webcam address - `0` (e.g., if your webcam is at `/dev/video0`.)
 * `--dest [DEST]` (optional): Specify your destination folder. Default location is current directory.
 * `--type [TYPE]` (optional): Choose between `rgba`, `map` `green`, `blur`, `overlay`, and another image file. Default is `rgba`.
     * `rgba` will generate RGBA output regarding saliency score as an alpha map. Note that this will not work for video and webcam input. 
     * `map` will output saliency map only. 
     * `green` will change the background with green screen. 
+    * `white` will change the background with white color. -> [2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) 
+    * `'[255, 0, 0]'` will change the background with color code [255, 0, 0]. Please use with single quotes. -> [2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) 
     * `blur` will blur the background.
     * `overlay` will cover the salient object with translucent green color, and highlight the edges.
     * Another image file (e.g., `samples/backgroud.png`) will be used as a background, and the object will be overlapped on it.
 * `--ckpt [CKPT]` (optional): Use other checkpoint file. Default is trained with composite dataset and will be automatically downloaded if not available. Please refer to [Model Zoo](https://github.com/plemeri/InSPyReNet/blob/main/docs/model_zoo.md) from [InSPyReNet](https://github.com/plemeri/InSPyReNet) for available pre-trained checkpoints.
 * `--fast` (optional): Fast mode. If specified, it will use low-resolution input and model trained with LR scale. May decrease performance but reduces inference time and gpu memory usage. 
 * `--jit` (optional): Torchscript mode. If specified, it will trace model with pytorch built-in torchscript JIT compiler. May cause delay in initialization, but reduces inference time and gpu memory usage.
     
@@ -129,14 +135,16 @@
 # Usage for image
 img = Image.open('samples/aeroplane.jpg').convert('RGB') # read image
 
 out = remover.process(img) # default setting - transparent background
 out = remover.process(img, type='rgba') # same as above
 out = remover.process(img, type='map') # object map only
 out = remover.process(img, type='green') # image matting - green screen
+out = remover.process(img, type='white') # change backround with white color -> [2023.05.24] Contributed by carpedm20
+out = remover.process(img, type=[255, 0, 0]) # change background with color code [255, 0, 0] -> [2023.05.24] Contributed by carpedm20
 out = remover.process(img, type='blur') # blur background
 out = remover.process(img, type='overlay') # overlay object map onto the image
 out = remover.process(img, type='samples/background.jpg') # use another image as a background
 
 Image.fromarray(out).save('output.png') # save result
 
 # Usage for video
@@ -160,14 +168,18 @@
     out = remover.process(img, type='map') # same as image, except for 'rgba' which is not for video.
     writer.write(cv2.cvtColor(out, cv2.COLOR_BGR2RGB))
 
 cap.release()
 writer.release()
 ```
 
+## :tv: Tutorial
+
+[rsreetech](https://github.com/rsreetech) shared a tutorial using colab. [[Youtube](https://www.youtube.com/watch?v=jKuQEnKmv4A)]
+
 ## :outbox_tray: Uninstall
 
 ```
 pip uninstall transparent-background
 ```
 
 ## :page_facing_up: Licence
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transparent-background Version: 1.2.3 Summary: Make
+Metadata-Version: 2.1 Name: transparent-background Version: 1.2.4 Summary: Make
 images with transparent background Home-page: https://github.com/plemeri/
 transparent-background Author: Taehun Kim Author-email:
 taehoon1018@postech.ac.kr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE # Transparent Background
 [https://raw.githubusercontent.com/plemeri/transparent-background/main/figures/
@@ -11,51 +11,57 @@
 This is a background removing tool powered by [InSPyReNet (ACCV 2022)](https://
 github.com/plemeri/InSPyReNet.git). You can easily remove background from the
 image or video or bunch of other stuffs when you can make the background
 transparent! Image | Video | Webcam :-:|:-:|:-: [https://
 raw.githubusercontent.com/plemeri/transparent-background/main/figures/
 demo_aeroplane.gif] | [https://raw.githubusercontent.com/plemeri/transparent-
 background/main/figures/demo_b5.gif] | [https://raw.githubusercontent.com/
-plemeri/transparent-background/main/figures/demo_webcam.gif] ## :inbox_tray:
-Installation ### Dependencies (python packages) package | version (>=) :-|:
-- `pytorch` | `1.7.1` `torchvision` | `0.8.2` `opencv-python` | `4.6.0.66`
-`timm` | `0.6.11` `tqdm` | `4.64.1` `kornia` | `0.5.4` `gdown` | `4.5.4`
-`pyvirtualcam` | `0.6.0` Note: If you have any problem with [`pyvirtualcam`]
-(https://pypi.org/project/pyvirtualcam/), please visit their github repository
-or pypi homepage. Due to the backend workflow for Windows and macOS, we only
-support Linux for webcam input. ### Dependencies (webcam input) We basically
-follow the virtual camera settings from [`pyvirtualcam`](https://pypi.org/
-project/pyvirtualcam/). If you do not choose to install virtual camera, it will
-visualize real-time output with `cv2.imshow`. #### A. Linux (v4l2loopback)
-```bash # Install v4l2loopback for webcam relay $ git clone https://github.com/
-umlaeute/v4l2loopback.git && cd v4l2loopback $ make && sudo make install $ sudo
-depmod -a # Create virtual webcam $ sudo modprobe v4l2loopback devices=1 ```
-Note: If you have any problem with installing [`v4l2loopback`](https://
-github.com/umlaeute/v4l2loopback), please visit their github repository. ####
-B. Windows (OBS) Install OBS virtual camera from [install OBS](https://
-obsproject.com/). #### C. macOS (OBS) [not stable] Follow the steps below. *
-[Install OBS](https://obsproject.com/). * Start OBS. * Click "Start Virtual
-Camera" (bottom right), then "Stop Virtual Camera". * Close OBS. ### Install
-`transperent-background` ```bash # via pypi $ pip install transparent-
-background # via github $ pip install git+https://github.com/plemeri/
-transparent-background.git # locally $ pip install . ``` ## :pencil2: Usage ###
-:computer: Command Line ```bash # for apple silicon mps backend, use
-"PYTORCH_ENABLE_MPS_FALLBACK=1" before the command (requires torch >= 1.13) $
-transparent-background --source [SOURCE] --dest [DEST] --type [TYPE] --ckpt
-[CKPT] (--fast) (--jit) ``` * `--source [SOURCE]`: Specify your data in this
-argument. * Single image - `image.png` * Folder containing images - `path/to/
-img/folder` * Single video - `video.mp4` * Folder containing videos - `path/to/
-vid/folder` * Integer for webcam address - `0` (e.g., if your webcam is at `/
-dev/video0`.) * `--dest [DEST]` (optional): Specify your destination folder.
+plemeri/transparent-background/main/figures/demo_webcam.gif] ## :newspaper:
+News Our package is currently not working properly on small images without `--
+fast` argument. Sorry for the inconvenience and we'll fix this issue with
+better algorithm coming out shortly. ## :inbox_tray: Installation ###
+Dependencies (python packages) package | version (>=) :-|:- `pytorch` | `1.7.1`
+`torchvision` | `0.8.2` `opencv-python` | `4.6.0.66` `timm` | `0.6.11` `tqdm` |
+`4.64.1` `kornia` | `0.5.4` `gdown` | `4.5.4` `pyvirtualcam` | `0.6.0` Note: If
+you have any problem with [`pyvirtualcam`](https://pypi.org/project/
+pyvirtualcam/), please visit their github repository or pypi homepage. Due to
+the backend workflow for Windows and macOS, we only support Linux for webcam
+input. ### Dependencies (webcam input) We basically follow the virtual camera
+settings from [`pyvirtualcam`](https://pypi.org/project/pyvirtualcam/). If you
+do not choose to install virtual camera, it will visualize real-time output
+with `cv2.imshow`. #### A. Linux (v4l2loopback) ```bash # Install v4l2loopback
+for webcam relay $ git clone https://github.com/umlaeute/v4l2loopback.git && cd
+v4l2loopback $ make && sudo make install $ sudo depmod -a # Create virtual
+webcam $ sudo modprobe v4l2loopback devices=1 ``` Note: If you have any problem
+with installing [`v4l2loopback`](https://github.com/umlaeute/v4l2loopback),
+please visit their github repository. #### B. Windows (OBS) Install OBS virtual
+camera from [install OBS](https://obsproject.com/). #### C. macOS (OBS) [not
+stable] Follow the steps below. * [Install OBS](https://obsproject.com/). *
+Start OBS. * Click "Start Virtual Camera" (bottom right), then "Stop Virtual
+Camera". * Close OBS. ### Install `transperent-background` ```bash # via pypi $
+pip install transparent-background # via github $ pip install git+https://
+github.com/plemeri/transparent-background.git # locally $ pip install . ``` ##
+:pencil2: Usage ### :computer: Command Line ```bash # for apple silicon mps
+backend, use "PYTORCH_ENABLE_MPS_FALLBACK=1" before the command (requires torch
+>= 1.13) $ transparent-background --source [SOURCE] --dest [DEST] --type [TYPE]
+--ckpt [CKPT] (--fast) (--jit) ``` * `--source [SOURCE]`: Specify your data in
+this argument. * Single image - `image.png` * Folder containing images - `path/
+to/img/folder` * Single video - `video.mp4` * Folder containing videos - `path/
+to/vid/folder` * Integer for webcam address - `0` (e.g., if your webcam is at
+`/dev/video0`.) * `--dest [DEST]` (optional): Specify your destination folder.
 Default location is current directory. * `--type [TYPE]` (optional): Choose
 between `rgba`, `map` `green`, `blur`, `overlay`, and another image file.
 Default is `rgba`. * `rgba` will generate RGBA output regarding saliency score
 as an alpha map. Note that this will not work for video and webcam input. *
 `map` will output saliency map only. * `green` will change the background with
-green screen. * `blur` will blur the background. * `overlay` will cover the
+green screen. * `white` will change the background with white color. ->
+[2023.05.24] Contributed by [carpedm20](https://github.com/carpedm20) * `'[255,
+0, 0]'` will change the background with color code [255, 0, 0]. Please use with
+single quotes. -> [2023.05.24] Contributed by [carpedm20](https://github.com/
+carpedm20) * `blur` will blur the background. * `overlay` will cover the
 salient object with translucent green color, and highlight the edges. * Another
 image file (e.g., `samples/backgroud.png`) will be used as a background, and
 the object will be overlapped on it. * `--ckpt [CKPT]` (optional): Use other
 checkpoint file. Default is trained with composite dataset and will be
 automatically downloaded if not available. Please refer to [Model Zoo](https://
 github.com/plemeri/InSPyReNet/blob/main/docs/model_zoo.md) from [InSPyReNet]
 (https://github.com/plemeri/InSPyReNet) for available pre-trained checkpoints.
@@ -68,23 +74,28 @@
 PIL import Image from transparent_background import Remover # Load model
 remover = Remover() # default setting remover = Remover(fast=True, jit=True,
 device='cuda:0', ckpt='~/latest.pth') # custom setting # Usage for image img =
 Image.open('samples/aeroplane.jpg').convert('RGB') # read image out =
 remover.process(img) # default setting - transparent background out =
 remover.process(img, type='rgba') # same as above out = remover.process(img,
 type='map') # object map only out = remover.process(img, type='green') # image
-matting - green screen out = remover.process(img, type='blur') # blur
-background out = remover.process(img, type='overlay') # overlay object map onto
-the image out = remover.process(img, type='samples/background.jpg') # use
-another image as a background Image.fromarray(out).save('output.png') # save
-result # Usage for video cap = cv2.VideoCapture('samples/b5.mp4') # video
-reader for input fps = cap.get(cv2.CAP_PROP_FPS) writer = None while
-cap.isOpened(): ret, frame = cap.read() # read video if ret is False: break
-frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB) img = Image.fromarray
+matting - green screen out = remover.process(img, type='white') # change
+backround with white color -> [2023.05.24] Contributed by carpedm20 out =
+remover.process(img, type=[255, 0, 0]) # change background with color code
+[255, 0, 0] -> [2023.05.24] Contributed by carpedm20 out = remover.process(img,
+type='blur') # blur background out = remover.process(img, type='overlay') #
+overlay object map onto the image out = remover.process(img, type='samples/
+background.jpg') # use another image as a background Image.fromarray(out).save
+('output.png') # save result # Usage for video cap = cv2.VideoCapture('samples/
+b5.mp4') # video reader for input fps = cap.get(cv2.CAP_PROP_FPS) writer = None
+while cap.isOpened(): ret, frame = cap.read() # read video if ret is False:
+break frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB) img = Image.fromarray
 (frame).convert('RGB') if writer is None: writer = cv2.VideoWriter
 ('output.mp4', cv2.VideoWriter_fourcc(*'mp4v'), fps, img.size) # video writer
 for output out = remover.process(img, type='map') # same as image, except for
 'rgba' which is not for video. writer.write(cv2.cvtColor(out,
-cv2.COLOR_BGR2RGB)) cap.release() writer.release() ``` ## :outbox_tray:
+cv2.COLOR_BGR2RGB)) cap.release() writer.release() ``` ## :tv: Tutorial
+[rsreetech](https://github.com/rsreetech) shared a tutorial using colab. [
+[Youtube](https://www.youtube.com/watch?v=jKuQEnKmv4A)] ## :outbox_tray:
 Uninstall ``` pip uninstall transparent-background ``` ## :page_facing_up:
 Licence See [LICENCE](https://github.com/plemeri/transparent-background/blob/
 main/LICENSE) for more details.
```

### Comparing `transparent-background-1.2.3/transparent_background.egg-info/SOURCES.txt` & `transparent-background-1.2.4/transparent_background.egg-info/SOURCES.txt`

 * *Files identical despite different names*

