# Comparing `tmp/Operetta_tool-1.3.2.tar.gz` & `tmp/Operetta_tool-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.3.2.tar", last modified: Tue May 16 08:59:42 2023, max compression
+gzip compressed data, was "Operetta_tool-1.3.3.tar", last modified: Wed May 24 10:40:00 2023, max compression
```

## Comparing `Operetta_tool-1.3.2.tar` & `Operetta_tool-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:59:42.812489 Operetta_tool-1.3.2/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.2/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-16 08:59:42.807466 Operetta_tool-1.3.2/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-05-16 08:59:42.811491 Operetta_tool-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 08:59:42.810477 Operetta_tool-1.3.2/operetta/
--rw-rw-rw-   0        0        0      153 2023-05-16 08:58:53.000000 Operetta_tool-1.3.2/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.2/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    48388 2023-05-16 08:50:32.000000 Operetta_tool-1.3.2/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-05-16 08:59:42.812489 Operetta_tool-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-05-16 08:58:51.000000 Operetta_tool-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:40:00.711283 Operetta_tool-1.3.3/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-24 10:40:00.703339 Operetta_tool-1.3.3/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-05-24 10:39:59.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-24 10:40:00.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:39:59.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-05-24 10:40:00.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 10:40:00.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-05-24 10:40:00.711283 Operetta_tool-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 10:40:00.710291 Operetta_tool-1.3.3/operetta/
+-rw-rw-rw-   0        0        0      153 2023-05-24 10:38:15.000000 Operetta_tool-1.3.3/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.3/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    51061 2023-05-24 10:37:03.000000 Operetta_tool-1.3.3/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:40:00.711283 Operetta_tool-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-05-24 10:37:56.000000 Operetta_tool-1.3.3/setup.py
```

### Comparing `Operetta_tool-1.3.2/LICENSE` & `Operetta_tool-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.2/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.3.3/Operetta_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.3.2
+Version: 1.3.3
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.3.2/PKG-INFO` & `Operetta_tool-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.3.2
+Version: 1.3.3
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.3.2/README.md` & `Operetta_tool-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.2/operetta/jbsicon.ico` & `Operetta_tool-1.3.3/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.2/operetta/operetta_annotation.py` & `Operetta_tool-1.3.3/operetta/operetta_annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import math
 import gc
 import warnings
 import tkinter as tk 
 from tkinter import ttk, Text
 from skimage import io, filters
 import pkg_resources
+from PIL import ImageFont, ImageDraw, Image
+
 
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
     
 def split_channels(path_to_images:str, path_to_save:str):
     
     try:
@@ -498,37 +500,19 @@
             
             del thresholded_stack
             
             outlier_indices = list(np.where(mean_intensity > np.mean(mean_intensity) + np.std(mean_intensity))[0]) + list(np.where(mean_intensity < np.mean(mean_intensity) - np.std(mean_intensity))[0]) 
             
             stack = np.delete(stack, outlier_indices, axis=0)
             
-            del mean_intensity, outlier_indices
-            
-            mean_zstack = np.mean(stack, axis=0)
-            std_zstack = np.std(stack, axis=0)
-        
-            # calculate the z-score for each pixel
-            z_score = abs(stack - mean_zstack) / std_zstack
-            
-            del mean_zstack, std_zstack
-        
-            # identify pixels with z-scores above the threshold
-            stack[(z_score > 2.5) | (z_score < -2.5)] = -999
-            
-            del z_score
+           
         
         stack = stack.astype(np.uint64)  
         
-        for n, d in enumerate(stack):   
-            stack[n] = (stack[n] / np.mean(stack[n])) * (((2**16)-1) /  np.log(np.mean(stack[n])))
-            stack[n][stack[n] > ((2**16)-1)] = ((2**16)-1)
-
-        stack[stack > ((2**16)-1)] = ((2**16)-1)
-        stack = stack.astype(np.uint16)   
+    
                 
        
         window = tk.Tk()
         
         window.geometry("500x800")
         window.title("Z-PROJECTION")
     
@@ -641,53 +625,36 @@
         
         def active_changes():
                 
                
                 global img_gamma
                 
                 if projections_type.get() == 'avg':
-                    mask = stack == -999  
-                    img = np.ma.masked_array(stack, mask=mask)  
-                    img = np.mean(img, axis=0).astype(np.uint16) 
-                    del mask
+                    img = np.mean(stack, axis=0).astype(np.uint64) 
                 elif projections_type.get() == 'max':
-                    mask = stack == -999  
-                    img = np.ma.masked_array(stack, mask=mask)  
-                    img = np.max(img, axis=0).astype(np.uint16)  
-                    del mask
-                elif projections_type.get() == 'min':
-                    mask = stack == -999  
-                    img = np.ma.masked_array(stack, mask=mask)  
-                    img = np.min(img, axis=0).astype(np.uint16)
-                    del mask
+                    img = np.max(stack, axis=0).astype(np.uint64)  
+                elif projections_type.get() == 'min': 
+                    img = np.min(stack, axis=0).astype(np.uint64)
                 elif projections_type.get() == 'std':
-                    mask = stack == -999  
-                    img = np.ma.masked_array(stack, mask=mask)  
-                    img = np.std(img, axis=0).astype(np.uint16) 
-                    del mask
+                    img = np.std(stack, axis=0).astype(np.uint64) 
                 elif projections_type.get() == 'median':
-                    mask = stack == -999  
-                    img = np.ma.masked_array(stack, mask=mask)  
-                    img = np.median(img, axis=0).astype(np.uint16)    
-                    del mask
+                    img = np.median(stack, axis=0).astype(np.uint64)    
+                
                
                 
-                img = img.astype(np.int64)
                 
                 color = combobox.get()
                 
-    
-                img = img - int(threshold_min.get())
                 
                 
-                img[img >  int(threshold_max.get())] = 0
+                img[img >  int(threshold_max.get())] = int(threshold_max.get())
                 
              
 
-                img[img < 0] = 0
+                img[img < int(threshold_min.get())] = 0
                 
                 #brightness
                 img[img > 0] = img[img > 0] + int(brightness.get()*200 - 30000)
                 
                 
                 #contrast
                 img = cv2.multiply(img,  int(contrast.get()/ 10))
@@ -708,14 +675,16 @@
                 
                 img = (img / np.max(img)) * 65535
 
                 img = np.round(img).astype(np.uint16)
             
                 
                 img_gamma = np.zeros((img.shape[0], img.shape[1], 3), dtype=np.uint16)
+                blurred_image = cv2.GaussianBlur(img, (1001, 1001), 0)
+                img = cv2.addWeighted(img, 1.5, blurred_image, -0.25, 0)
                 
                    
                
                 if color == 'green':
                     img_gamma[:,:,1] = img
         
         
@@ -736,15 +705,17 @@
                     img_gamma[:,:,2] = img
                 
                 elif color == 'cyan':
                     img_gamma[:,:,0] = img
                     img_gamma[:,:,1] = img
                  
                 elif color == 'grey':
-                    img_gamma = img
+                    img_gamma[:,:,0] = img
+                    img_gamma[:,:,1] = img
+                    img_gamma[:,:,2] = img
             
             
                 
                 button_finished.set(True)
            
     
         
@@ -770,35 +741,45 @@
            
         
         display_image()
         
         
         def auto_adjust():
             
+            global stack
+            
+            for n, d in enumerate(stack):   
+                stack[n] = (stack[n] / np.mean(stack[n])) * (((2**16)-1) /  np.log(np.mean(stack[n])))
+                stack[n][stack[n] > ((2**16)-1)] = ((2**16)-1)
+      
+        
+            stack[stack > ((2**16)-1)] = ((2**16)-1)
+            stack = stack.astype(np.uint64)   
+            
             projection = np.average(stack, axis=0)
 
-            tmin = int(np.mean(projection))/1.5
+            tmin = int(np.mean(projection))/1.1
             tmax = int(np.max(projection))
 
             
-            gamma.set(20)         
-            slider2.set(20)
+            gamma.set(10)         
+            slider2.set(10)
                      
             threshold_min.set(tmin)
             slider3_min.set(tmin)
             
             threshold_max.set(tmax)
             slider3_max.set(tmax)
             
             
-            brightness.set(170)
-            slider5.set(170)
+            brightness.set(150)
+            slider5.set(150)
       
-            contrast.set(25)
-            slider6.set(25)
+            contrast.set(10)
+            slider6.set(10)
             
             projections_type.current(0)
            
             active_changes()
             
             
         tk.Label(window, text="").pack()
@@ -826,41 +807,42 @@
         return img_gamma
 
 
 
 
 
 
-
 def merge_images(image_list:list):
     
     try:
     
         intensity_factors = []
         for bt in range(len(image_list)):
             intensity_factors.append(1)
             
         def merge1():
             global result
             result = None
             
             for i, image in enumerate(image_list):
                 if result is None:
-                    result = image.astype(float) * intensity_factors[i]
+                    result = image.astype(np.uint64) * intensity_factors[i]
                 else:
-                    result = cv2.addWeighted(result, 1, image.astype(float) * intensity_factors[i], 1, 0)
+                    result = cv2.addWeighted(result, 1, image.astype(np.uint64) * intensity_factors[i], 1, 0)
             
-            result = result.astype('uint16')
+            result[result > ((2**16)-1)] = ((2**16)-1)
+            result = result.astype(np.uint16)
+        
             
     
         
         window = tk.Tk()
         
         window.geometry("500x600")
-        window.title("MERGE channelS")
+        window.title("MERGE CHANNELS")
     
         window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
        
     
        
         tk.Label(window, text="").pack()
         tk.Label(window, text="").pack()
@@ -908,19 +890,20 @@
                 intensity_factors.append((slider_values[str('b' + str(bt))].get()/10))
                 
             global result
             result = None
             
             for i, image in enumerate(image_list):
                 if result is None:
-                    result = image.astype(float) * intensity_factors[i]
+                    result = image.astype(np.uint64) * intensity_factors[i]
                 else:
-                    result = cv2.addWeighted(result, 1, image.astype(float) * intensity_factors[i], 1, 0)
+                    result = cv2.addWeighted(result, 1, image.astype(np.uint64) * intensity_factors[i], 1, 0)
             
-            result = result.astype('uint16')
+            result[result > ((2**16)-1)] = ((2**16)-1)
+            result = result.astype(np.uint16)
         
         button = tk.Button(window, text="Apply", command=merge2)
         
         button.pack()
         
         merge1()
         
@@ -960,15 +943,14 @@
     
     except:
         print("Something went wrong. Check the function input data and try again!")
 
 
 
 
-
 def image_grid(path_to_opera_projection:str, img_length:int, img_width:int):
 
     if not os.path.exists(path_to_opera_projection):
         
         print('\nImage does not exist. Check the correctness of the path to image')
 
     else:
@@ -1209,29 +1191,29 @@
         label2 = tk.Label(window, text="Scale length [um]", anchor="w")
         label2.pack()
         
         length = tk.DoubleVar()
         l = [50, 100, 250, 500, 1000, 1500, 2000, 2500, 3000, 4000, 5000]
     
         length = ttk.Combobox(window, values=l)
-        length.current(3)
+        length.current(4)
         length.pack()
        
         
         tk.Label(window, text="").pack()
         
         label3 = tk.Label(window, text="Scalebar thickness[px]", anchor="w")
         label3.pack()
         
         
         thickness = tk.DoubleVar()
-        items = [10, 15, 25, 30, 35, 50, 75, 100, 125, 150, 200]
+        items = [10, 15, 25, 30, 35, 50, 75, 100]
     
         thickness = ttk.Combobox(window, values=items)
-        thickness.current(2)
+        thickness.current(3)
         thickness.pack()
 
         
 
         tk.Label(window, text="").pack()
         label4 = tk.Label(window, text="Color", anchor="w")
         label4.pack()
@@ -1245,55 +1227,81 @@
         combobox.pack()
         
         
         tk.Label(window, text="").pack()
         label5 = tk.Label(window, text="Font size", anchor="w")
         label5.pack()
         
-        fonts = [0.5,1,1.5,2,2.5,3,3.5,4,4.5,5]
+        fonts = [0.5,1,1.5,2,2.5,3,3.5,4,4.5,5,5.5,6,6.5,7,7.5,8,8.5,9,9.5,10]
     
         font = ttk.Combobox(window, values=fonts)
         
-        font.current(2)
+        font.current(10)
         
         font.pack()
         
         
+        
         tk.Label(window, text="").pack()
         
         label6 = tk.Label(window, text="Position", anchor="w")
         label6.pack()
         
         position_bar = ["right_bottom", "right_top", "left_top", "left_bottom"]
     
         position_type = ttk.Combobox(window, values=position_bar)
         
         position_type.current(0)
         
         position_type.pack()
         
+        tk.Label(window, text="").pack()
+        label7 = tk.Label(window, text="Horizontal position", anchor="w")
+        label7.pack()
+        
+        horizontal = [-10,-9,-8,-7,-6,-5,-4,-3,-2,-1,0,1,2,3,4,5,6,7,8,9,10]
+    
+        hor = ttk.Combobox(window, values=horizontal)
+        
+        hor.current(10)
+        
+        hor.pack()
+        
+        tk.Label(window, text="").pack()
+        label7 = tk.Label(window, text="Vertical position", anchor="w")
+        label7.pack()
+        
+        vertical = [-10,-9,-8,-7,-6,-5,-4,-3,-2,-1,0,1,2,3,4,5,6,7,8,9,10]
+    
+        ver = ttk.Combobox(window, values=vertical)
+        
+        ver.current(10)
+        
+        ver.pack()
+        
        
         button_finished = tk.BooleanVar(value=False)
         
         def active_changes():
             
 
                 scale_color = (65535, 65535, 65535)
                
                 global image3
                 
                 image3 = image2.copy()
                 
-                # Determine the desired size of the scale bar and convert it to pixels
-                scale_length_um = int(length.get())  # Length of the scale bar in millimeters
-                pixels_per_um = met['X_resolution[m]'][0]*1000000   # Number of pixels equivalent to 1 millimeter
+               
+                scale_length_um = int(length.get())  
+                pixels_per_um = met['X_resolution[m]'][0]*1000000   
                 scale_length_px = int(scale_length_um * pixels_per_um)
  
                 # Calculate the position of the scale bar
-                image_height, image_width, _ = image3.shape
+                image_height = image3.shape[0]
+                image_width = image3.shape[1]
                 
                 scale_position = (int(image_width*0.96) - scale_length_px, int(image_height*0.96))  # Adjust the position as needed
 
  
                 # Draw the scale bar on the image
                 if str(combobox.get()) == 'grey':
                     scale_color = (32768, 32768, 32768)
@@ -1309,42 +1317,68 @@
                     scale_color = (0, 65535, 65535)
                 elif str(combobox.get()) == 'cyan':
                     scale_color = (65535, 65535, 0)
                 elif str(combobox.get()) == 'black':
                     scale_color = (0, 0, 0)
                 elif str(combobox.get()) == 'white':
                     scale_color = (65535, 65535, 65535)
-                    
-                
+                  
+
+
+                font_typ = ImageFont.truetype('arialbd.ttf', int(np.log2(image_height)* float(font.get())))
+
                 scale_thickness = int(thickness.get())  
                 
                 if str(position_type.get()) == 'left_top':
-                    scale_position = (int(image_width*0.04) + scale_length_px, int(image_height*0.04)) 
-                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
-                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
-     
-
+                    scale_position = (int(image_width*0.04) + scale_length_px + int(hor.get())*int(np.log10(image_width)*10), int(image_height*0.04) + int(ver.get())*int(np.log10(image_height)*10)) 
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] ), scale_color, scale_thickness)
+                    overlay = np.zeros((image3.shape[0], image3.shape[1]), dtype = np.uint16)
+                    overlay_rgb = np.repeat(overlay[:, :, np.newaxis], 3, axis=2).astype(np.uint16)
+                    img_pil = Image.fromarray(overlay_rgb, mode='RGB')
+                    draw = ImageDraw.Draw(img_pil)
+                    draw.text((scale_position[0] + 10, scale_position[1] + int(np.log10(image_height)*15)), f'{scale_length_um} \u03BCm', fill = str(combobox.get()), font = font_typ)
+                    img_pil = cv2.cvtColor(np.array(img_pil), cv2.COLOR_RGB2BGR).astype(np.uint16)
+                    img_pil = cv2.normalize(img_pil, None, 0, 65535, cv2.NORM_MINMAX)
+                    image3 = cv2.add(image3, img_pil) 
+                    
                 elif str(position_type.get()) == 'left_bottom':
-                    scale_position = (int(image_width*0.04) + scale_length_px, int(image_height*0.96))  
-                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
-                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
-     
-
+                    scale_position = (int(image_width*0.04) + scale_length_px + int(hor.get())*int(np.log10(image_width)*10), int(image_height*0.96) - int(ver.get())*int(np.log10(image_height)*10))  
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] ), scale_color, scale_thickness)
+                    overlay = np.zeros((image3.shape[0], image3.shape[1]), dtype = np.uint16)
+                    overlay_rgb = np.repeat(overlay[:, :, np.newaxis], 3, axis=2).astype(np.uint16)
+                    img_pil = Image.fromarray(overlay_rgb, mode='RGB')
+                    draw = ImageDraw.Draw(img_pil)
+                    draw.text((scale_position[0] + 10, scale_position[1] + int(np.log10(image_height)*15)), f'{scale_length_um} \u03BCm', fill = str(combobox.get()), font = font_typ)
+                    img_pil = cv2.cvtColor(np.array(img_pil), cv2.COLOR_RGB2BGR).astype(np.uint16)
+                    img_pil = cv2.normalize(img_pil, None, 0, 65535, cv2.NORM_MINMAX)
+                    image3 = cv2.add(image3, img_pil) 
+                    
                 elif str(position_type.get()) == 'right_top':
-                    scale_position = (int(image_width*0.96) - scale_length_px, int(image_height*0.04))  
-                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
-                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
-     
+                    scale_position = (int(image_width*0.96) - scale_length_px + int(hor.get())*int(np.log10(image_width)*10), int(image_height*0.04) + int(ver.get())*int(np.log10(image_height)*10))  
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] ), scale_color, scale_thickness)
+                    overlay = np.zeros((image3.shape[0], image3.shape[1]), dtype = np.uint16)
+                    overlay_rgb = np.repeat(overlay[:, :, np.newaxis], 3, axis=2).astype(np.uint16)
+                    img_pil = Image.fromarray(overlay_rgb, mode='RGB')
+                    draw = ImageDraw.Draw(img_pil)
+                    draw.text((scale_position[0] + 10, scale_position[1] + int(np.log10(image_height)*15)), f'{scale_length_um} \u03BCm', fill = str(combobox.get()), font = font_typ)
+                    img_pil = cv2.cvtColor(np.array(img_pil), cv2.COLOR_RGB2BGR).astype(np.uint16)
+                    img_pil = cv2.normalize(img_pil, None, 0, 65535, cv2.NORM_MINMAX)
+                    image3 = cv2.add(image3, img_pil) 
+                    
                 elif str(position_type.get()) == 'right_bottom':
-                    scale_position = (int(image_width*0.96) - scale_length_px, int(image_height*0.96))  
-                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
-                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
-     
-
-            
+                    scale_position = (int(image_width*0.96) - scale_length_px + int(hor.get())*int(np.log10(image_width)*10), int(image_height*0.96) - int(ver.get())*int(np.log10(image_height)*10))  
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] ), scale_color, scale_thickness)
+                    overlay = np.zeros((image3.shape[0], image3.shape[1]), dtype = np.uint16)
+                    overlay_rgb = np.repeat(overlay[:, :, np.newaxis], 3, axis=2).astype(np.uint16)
+                    img_pil = Image.fromarray(overlay_rgb, mode='RGB')
+                    draw = ImageDraw.Draw(img_pil)
+                    draw.text((scale_position[0] + 10, scale_position[1] + int(np.log10(image_height)*15)), f'{scale_length_um} \u03BCm', fill = str(combobox.get()), font = font_typ)
+                    img_pil = cv2.cvtColor(np.array(img_pil), cv2.COLOR_RGB2BGR).astype(np.uint16)
+                    img_pil = cv2.normalize(img_pil, None, 0, 65535, cv2.NORM_MINMAX)
+                    image3 = cv2.add(image3, img_pil) 
 
                 
                 button_finished.set(True)
            
     
         
         tk.Label(window, text="").pack()
@@ -1389,10 +1423,8 @@
     
         cv2.destroyAllWindows()
     
         
         return image3
 
     except:
-        print("Something went wrong. Check the function input data and try again!")
-        
-        
+        print("Something went wrong. Check the function input data and try again!")
```

### Comparing `Operetta_tool-1.3.2/setup.py` & `Operetta_tool-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.2' 
+VERSION = '1.3.3' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

