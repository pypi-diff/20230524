# Comparing `tmp/lumina-1.0.1.tar.gz` & `tmp/lumina-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumina-1.0.1.tar", last modified: Sun May 21 10:49:09 2023, max compression
+gzip compressed data, was "lumina-1.0.4.tar", last modified: Wed May 24 16:03:42 2023, max compression
```

## Comparing `lumina-1.0.1.tar` & `lumina-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 10:49:09.423286 lumina-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-21 10:49:09.401284 lumina-1.0.1/Lumina/
--rw-rw-rw-   0        0        0        0 2023-05-19 16:55:29.000000 lumina-1.0.1/Lumina/__init__.py
--rw-rw-rw-   0        0        0      146 2023-05-19 16:53:55.000000 lumina-1.0.1/Lumina/colors.py
--rw-rw-rw-   0        0        0    16857 2023-05-20 20:11:24.000000 lumina-1.0.1/Lumina/lumina.py
--rw-rw-rw-   0        0        0     2628 2023-05-21 10:49:09.422284 lumina-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1987 2023-05-21 10:40:57.000000 lumina-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 10:49:09.420282 lumina-1.0.1/lumina.egg-info/
--rw-rw-rw-   0        0        0     2628 2023-05-21 10:49:09.000000 lumina-1.0.1/lumina.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-21 10:49:09.000000 lumina-1.0.1/lumina.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 10:49:09.000000 lumina-1.0.1/lumina.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-21 10:49:09.000000 lumina-1.0.1/lumina.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 10:49:09.000000 lumina-1.0.1/lumina.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 10:49:09.424287 lumina-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-05-21 10:05:56.000000 lumina-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:03:42.310601 lumina-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:03:42.306601 lumina-1.0.4/Lumina/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:03:32.000000 lumina-1.0.4/Lumina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 16:03:32.000000 lumina-1.0.4/Lumina/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-05-24 16:03:32.000000 lumina-1.0.4/Lumina/lumina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-24 16:03:42.310601 lumina-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-24 16:03:32.000000 lumina-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:03:42.306601 lumina-1.0.4/lumina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-24 16:03:42.000000 lumina-1.0.4/lumina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-24 16:03:42.000000 lumina-1.0.4/lumina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:03:42.000000 lumina-1.0.4/lumina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 16:03:42.000000 lumina-1.0.4/lumina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 16:03:42.000000 lumina-1.0.4/lumina.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:03:42.310601 lumina-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-24 16:03:32.000000 lumina-1.0.4/setup.py
```

### Comparing `lumina-1.0.1/Lumina/lumina.py` & `lumina-1.0.4/Lumina/lumina.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,349 +1,354 @@
-import cv2
-import numpy as np
-from typing import List , Tuple , Union
-
-
-class Lumina():
-    def __init__(self,verbose=True) -> None:
-        self.verbose = verbose
-        if self.verbose:
-            print('[+] Lumina module loaded....')
-        
-    def cornerRect(self,image:np.array,bbox:List,colors:Tuple=(0,0,255),thickness:int=2,line_len:int=10,draw_rectangle:bool=False,rect_color:Tuple=(0,255,0),rect_thickness:int=2) -> np.array:
-        """
-        THIS FUNCTION WILL CREATE A CORNER RECTANGLE
-        
-        : param image : cv2.imread() image
-        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
-        : prarm colors : expects a tuple (0,255,0)
-        : param thickness : it will change line's thickness
-        : param line_len : line len will change line distance from starting point, if line len is higher number then it will be a big straight line
-        : param draw rectangle : will draw rectangle
-        : param rect color : will change rectangle color
-        : param rect thickness : it will change rectangle's thickness
-        
-        : return : customized image
-        
-        """
-        if thickness >= 1:
-            if draw_rectangle:
-                cv2.rectangle(image,(bbox[0],bbox[1]),(bbox[2],bbox[3]),color=rect_color,thickness=rect_thickness,lineType=cv2.LINE_AA)
-            
-            #top left
-            cv2.line(image,(bbox[0],bbox[1]),(bbox[0]+line_len,bbox[1]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            cv2.line(image,(bbox[0],bbox[1]),(bbox[0],bbox[1]+line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            #top right
-            cv2.line(image,(bbox[2],bbox[1]),(bbox[2]-line_len,bbox[1]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            cv2.line(image,(bbox[2],bbox[1]),(bbox[2],bbox[1]+line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            #bottom right
-            cv2.line(image,(bbox[2],bbox[3]),(bbox[2]-line_len,bbox[3]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            cv2.line(image,(bbox[2],bbox[3]),(bbox[2],bbox[3]-line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            #bottom left
-            cv2.line(image,(bbox[0],bbox[3]),(bbox[0]+line_len,bbox[3]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-            cv2.line(image,(bbox[0],bbox[3]),(bbox[0],bbox[3]-line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        
-        else:
-            print('Thickness should be >= 1 ,  returning image without corner rectangle..')
-        
-        return image
-    
-    def rectangle(self,image:np.array,bbox:List,colors:Tuple=(0,0,255),thickness:int=2) -> np.array:
-        """
-        THIS FUNCTION WILL CREATE A  RECTANGLE
-        
-        : param image : cv2.imread() image
-        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
-        : prarm colors : expects a tuple (0,255,0)
-        : param thickness : it will change rectangle's thickness
-        
-        : return : customized image
-        
-        """
-        
-        cv2.rectangle(image,(bbox[0],bbox[1]),(bbox[2],bbox[3]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        return image
-    
-    def rect_transparent(self,image:np.array,bbox:List,colors:Tuple=(0,255,255),transparency:float=0.5,cornerRect:bool=True,thickness:int=2,line_len:int=10) -> np.array:
-        
-        """
-        THIS FUNCTION WILL CREATE A TRANSPARENT RECTANGLE WITH CORNER RECTANGLE IF PASSED TRUE
-        
-        : param image : cv2.imread() image
-        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
-        : prarm colors : expects a tuple (0,255,0)
-        : param transparency : how transparent your rectangle will be , lower float means high transparent
-        : param corner_rect : it will enable corner rect function
-        : param thickness : it will change corner rect's thickness
-        : param line_len : line len will change line distance from starting point, if line len is higher number then it will be a big straight line
-        
-        : return : customized image
-        
-        """
-        
-        overlay = image.copy()
-        
-        cv2.rectangle(overlay,(bbox[0],bbox[1]),(bbox[2],bbox[3]), colors, -1)
-        image = cv2.addWeighted(overlay, transparency, image, 1 - transparency, 0)
-        if cornerRect:
-            self.cornerRect(image,bbox,colors,thickness,line_len)
-
-        return image
-   
-    
-    def circle(self,image:np.array,center:Tuple=(20,50),radius:int=2,colors:Tuple=(0,255,0),thickness:int=2) -> np.array:
-        
-        """
-        THIS FUNCTION WILL CREATE A CIRCLE
-        
-        : param image : cv2.imread() image
-        : param center : expects a tuple for drawing the circle
-        : param radius : circle's radius
-        : prarm colors : expects a tuple (0,255,0)
-        : param thickness : it will change circle's thickness
-
-        : return : customized image
-        
-        """
-        cv2.circle(image,center=center,radius=radius,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        
-        return image
-    
-    
-    def putText(self,image:np.array,texts:str,bbox:Union[List,Tuple],font:cv2.FONT_HERSHEY_PLAIN=cv2.FONT_HERSHEY_PLAIN,colors:Tuple=(0,0,255),scale:int=2,thickness:int=2,border:bool=True,rect_color:Tuple=(0,255,0),border_size:int=2) -> np.array:
-        
-        """
-        THIS FUNCTION WILL PUT TEXT IN THE IMAGE
-        
-        : param image : cv2.imread() image
-        : param texts : expects a text
-        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
-        : param font : expects cv2.FONT_
-        : prarm colors : expects a tuple (0,255,0)
-        : param scale : text scale number , expects int val
-        : param thickness : it will change texts thickness , expects int
-        : param border : if True , it will create a border around text
-        : param rect color : will change border's rectangle color
-        : param border size : it will change border rectangle's side
- 
-        
-        : return : customized image
-        
-        """
-        
-        if border:
-            (w, h), _ = cv2.getTextSize(str(texts),font, scale, thickness)
-            cv2.rectangle(image,(bbox[0],bbox[1]),(bbox[0]+w+border_size,bbox[1]-h-border_size),rect_color,-1,cv2.LINE_AA)
-            cv2.putText(image,text=str(texts),org=(bbox[0],bbox[1]),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        else:
-            cv2.putText(image,text=str(texts),org=(bbox[0],bbox[1]),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        return image
-    
-    def putText_center(self,image:np.array,texts:str,bbox:List,font:cv2.FONT_HERSHEY_PLAIN=cv2.FONT_HERSHEY_PLAIN,colors:Tuple=(0,0,255),scale:int=2,thickness:int=2,border:bool=True,rect_color:Tuple=(0,255,0),border_size:int=2) -> np.array:
-        
-        """
-        THIS FUNCTION WILL PUT TEXT IN THE CENTER OF THE OBEJCT.
-        
-        : param image : cv2.imread() image
-        : param texts : expects a text
-        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
-        : param font : expects cv2.FONT_
-        : prarm colors : expects a tuple (0,255,0)
-        : param scale : text scale number , expects int val
-        : param thickness : it will change texts thickness , expects int
-        : param border : if True , it will create a border around text
-        : param rect color : will change border's rectangle color
-        : param border size : it will change border rectangle's side
- 
-        
-        : return : customized image
-        
-        """
-        
-        center_x , center_y = int((bbox[0] + bbox[2])/2) , int((bbox[1] + bbox[3])/2)
-        if border:
-            (w, h), _ = cv2.getTextSize(str(texts),font, scale, thickness)
-            cv2.rectangle(image,(center_x-10,center_y),(center_x+w+border_size,center_y-h-border_size),rect_color,-1,cv2.LINE_AA)
-            cv2.putText(image,text=str(texts),org=(center_x-10,center_y),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        else:
-            cv2.putText(image,text=str(texts),org=(center_x-10,center_y),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        return image
-    
-    def putText_centerStyle(self,image:np.array,texts:str,bbox:List=[10,20,30,40],font=cv2.FONT_HERSHEY_PLAIN,colors:Tuple=(0,0,255),circleRadius:int=5,Fontscale:int=2,thickness:int=1,border:bool=True,text_color:Tuple=(0,255,0),border_size:int=2) -> np.array:
-        
-        """
-        THIS FUNCTION WILL PUT TEXT IN THE CENTER OF THE OBEJCT AND CREATE A GOOD VISUALIZATION
-        
-        : param image : cv2.imread() image
-        : param texts : expects a text
-        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
-        : param font : expects cv2.FONT_
-        : prarm colors : expects a tuple (0,255,0)
-        : param circleRadius : expects a int value for the circle radius
-        : param Fontscale : text scale number , expects int val
-        : param thickness : it will change texts thickness , expects int
-        : param border : if True , it will create a border around text
-        : param text color : will change text's color
-        : param border size : it will change border size of text
- 
-        
-        : return : customized image
-        
-        """
-        
-        center_x , center_y = int((bbox[0] + bbox[2])/2) , int((bbox[1] + bbox[3])/2)
-        (w, h), _ = cv2.getTextSize(str(texts),font, Fontscale, thickness)
-       
-        if border:
-            cv2.rectangle(image,(center_x+60,center_y-30+10),(center_x+60+w+border_size,center_y-h-border_size-30+10),colors,-1,cv2.LINE_AA)
-    
-        cv2.circle(image,center=(center_x,center_y),radius=circleRadius,color=colors,thickness=-1,lineType=cv2.LINE_AA)
-        cv2.circle(image,center=(center_x,center_y),radius=circleRadius*2,color=colors,thickness=1,lineType=cv2.LINE_AA)
-        cv2.line(image,(center_x,center_y),(center_x+30,center_y-30),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        cv2.line(image,(center_x+30,center_y-30),(center_x+60,center_y-30),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
-        cv2.putText(image,text=str(texts),org=(center_x+60,center_y-30+10),fontFace=font,fontScale=Fontscale,color=text_color,thickness=thickness,lineType=cv2.LINE_AA)
-       
-        return image
-
-    def line_create(self,image:np.array,start_point:Tuple=(10,20),end_point:Tuple=(50,50),colors:Tuple=(0,255,0,10),lineThickness:int=55,transparency:float=.6) -> np.array:
-        
-        """
-        THIS FUCNTION WILL CREATE A LINE
-        
-        : param image : cv2.imread() image
-        : param start point : expects a tuple for line start point
-        : param end point : expects a tuple for line end point
-        : prarm colors : expects a tuple (0,255,0)
-        : param lineThickness : it will change line's thickness , expects int
-        : param transparency : how transparent your line will be
- 
-        : return : customized image
-        
-        """
-        
-        overlay = image.copy()
-        cv2.line(image,start_point,end_point,color=colors,thickness=lineThickness,lineType=cv2.LINE_AA)
-        image = cv2.addWeighted(overlay, transparency, image, 1 - transparency, 0)
-        
-        return image
-    
-    def polygon_create(self,image:np.array,poly_points:List[List]=[[10,20],[20,30],[30,40]],colors:Tuple=(0,255,0),isClosed:True=True,thickness:int=2) -> np.array: 
-        
-        """
-        THIS FUNCTION WILL CREATE A POLYGON
-        
-        : param image : cv2.imread() image
-        : param poly_points:  expects a list of list coordinate to draw polygon
-        : prarm colors : expects a tuple (0,255,0)
-        : param isClosed : expects a bool 
-        : param lineThickness : it will change line's thickness , expects int
-   
- 
-        : return : customized image
-        
-        """
-        cv2.polylines(image, [np.array(poly_points,dtype=np.int32)], isClosed=isClosed, color=colors, thickness=thickness,lineType=cv2.LINE_AA)
-        return image
-    
-    
-    def fillPolygon_create(self,image:np.array,poly_points:List[List]=[[10,20],[20,30],[30,40]],colors:Tuple=(0,255,0),transparency:float=.8) -> np.array:
-        """
-        THIS FUNCTION CREATE A FILL POLYGON WILL COLOR
-        
-        : param image : cv2.imread() image
-        : param poly_points:  expects a list of list coordinate to draw polygon
-        : prarm colors : expects a tuple (0,255,0)
-        : param lineThickness : it will change line's thickness , expects int
-   
- 
-        : return : customized image
-        
-        """
-        overlay = image.copy()
-        cv2.fillPoly(image, [np.array(poly_points,dtype=np.int32)], colors,lineType=cv2.LINE_AA)
-        image = cv2.addWeighted(overlay, transparency, image, 1 - transparency, 0)
-        return image
-    
-    def line_in_out_counter(self,image:np.array,line_start_pos:Tuple=(10,20),line_end_pos:Tuple=(30,40),detection_pos:Tuple=(50,50),line_color:Tuple=(0,255,0),lineThickness:int=2,lineTransparecy:float=0.5) -> Tuple[np.array,bool]:
-        
-        """
-        THIS FUNCTION WILL DETECT IF ANY OBJECT IS INSIDE ITS LINE BY GIVEN OBJECT DETECTION POINTS , IF IT IS THEN IT WILL COUNT THE OBJECT , IT IS USED FOR OBJECT TRACKING
-        
-        : param image : cv2.imread() image
-        : param start point : expects a tuple for line start point
-        : param end point : expects a tuple for line end point
-        : param detection pos : your detection points coordinates , expects tuple
-        : prarm Linecolors : expects a tuple (0,255,0)
-        : param lineThickness : it will change line's thickness , expects int
-        : param transparency : how transparent your line will be
- 
-        : return : customized image , bool ( if detction pos is inside the line or not)
-        
-        """
-        
-        line_created = self.line_create(image,start_point=line_start_pos,end_point=line_end_pos,colors=line_color,lineThickness=lineThickness,transparency=lineTransparecy)
-        distance = cv2.pointPolygonTest(np.array([(line_start_pos[0],line_start_pos[1]), (line_end_pos[0],line_end_pos[1])]), detection_pos, False)
-        
-        if distance > 0:
-            detect = True
-        else:
-            detect = False
-        
-        return (line_created , detect)
-    
-    
-    def polygon_in_out_counter(self,image:np.array,poly_points:List[List]=[[10,20],[30,40],[55,60]],detectionPoints:Tuple=(10,30),colors:Tuple=(0,255,0),transparency:float=0.2) -> Tuple[np.array,bool]:
-        """
-        THIS FUNCTION WILL DETECT IF ANY OBJECT IS INSIDE ITS POLYGON AREA BY GIVEN OBJECT DETECTION POINTS , IF IT IS THEN IT WILL COUNT THE OBJECT , IT IS USED FOR OBJECT TRACKING
-        
-        : param image : cv2.imread() image
-        : param poly_points:  expects a list of list coordinate to draw polygon
-        : param detection pos : your detection points coordinates , expects tuple
-        : prarm colors : expects a tuple (0,255,0)
-        : param lineThickness : it will change line's thickness , expects int
-   
- 
-        : return : customized image , bool ( if detction pos is inside the line or not)
-        
-        """
-        
-        poly_fill = self.fillPolygon_create(image, [np.array(poly_points,dtype=np.int32)], colors,transparency=transparency)
-        distance = cv2.pointPolygonTest(np.array(poly_points), detectionPoints, measureDist=False)
-        if distance > 0:
-            detect = True
-        else:
-            detect = False
-        
-        return (poly_fill , detect)
-    
-    def create_mask(self,image,points:List[List]=[[10,20],[30,40],[55,60]]) -> np.array:
-        
-        """
-        THIS FUNCTION WILL CREATE IMAGE MASK
-        
-        : param image : cv2.imread() image
-        : param points:  expects a list of list coordinate to create mask
-        
-        : return : image mask
-        
-        """
-        
-        image_height, image_width,_ = image.shape
-        mask = np.zeros((image_height, image_width), dtype=np.uint8)
-        cv2.fillPoly(mask, [np.array(points,dtype=np.int32)], 255,cv2.LINE_AA)
-        mask = cv2.bitwise_and(image,image,mask=mask)
-        return mask
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+import cv2
+import numpy as np
+from typing import List , Tuple , Union
+
+
+class Lumina():
+    def __init__(self,verbose=True) -> None:
+        self.verbose = verbose
+        if self.verbose:
+            print('[+] Lumina module loaded....')
+        
+    def cornerRect(self,image:np.array,bbox:List,colors:Tuple=(0,0,255),thickness:int=2,line_len:int=10,draw_rectangle:bool=False,rect_color:Tuple=(0,255,0),rect_thickness:int=2) -> np.array:
+        """
+        THIS FUNCTION WILL CREATE A CORNER RECTANGLE
+        
+        : param image : cv2.imread() image
+        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
+        : prarm colors : expects a tuple (0,255,0)
+        : param thickness : it will change line's thickness
+        : param line_len : line len will change line distance from starting point, if line len is higher number then it will be a big straight line
+        : param draw rectangle : will draw rectangle
+        : param rect color : will change rectangle color
+        : param rect thickness : it will change rectangle's thickness
+        
+        : return : customized image
+        
+        """
+        if thickness >= 1:
+            if draw_rectangle:
+                cv2.rectangle(image,(bbox[0],bbox[1]),(bbox[2],bbox[3]),color=rect_color,thickness=rect_thickness,lineType=cv2.LINE_AA)
+            
+            #top left
+            cv2.line(image,(bbox[0],bbox[1]),(bbox[0]+line_len,bbox[1]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            cv2.line(image,(bbox[0],bbox[1]),(bbox[0],bbox[1]+line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            #top right
+            cv2.line(image,(bbox[2],bbox[1]),(bbox[2]-line_len,bbox[1]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            cv2.line(image,(bbox[2],bbox[1]),(bbox[2],bbox[1]+line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            #bottom right
+            cv2.line(image,(bbox[2],bbox[3]),(bbox[2]-line_len,bbox[3]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            cv2.line(image,(bbox[2],bbox[3]),(bbox[2],bbox[3]-line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            #bottom left
+            cv2.line(image,(bbox[0],bbox[3]),(bbox[0]+line_len,bbox[3]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+            cv2.line(image,(bbox[0],bbox[3]),(bbox[0],bbox[3]-line_len),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        
+        else:
+            print('Thickness should be >= 1 ,  returning image without corner rectangle..')
+        
+        return image
+    
+    def rectangle(self,image:np.array,bbox:List,colors:Tuple=(0,0,255),thickness:int=2) -> np.array:
+        """
+        THIS FUNCTION WILL CREATE A  RECTANGLE
+        
+        : param image : cv2.imread() image
+        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
+        : prarm colors : expects a tuple (0,255,0)
+        : param thickness : it will change rectangle's thickness
+        
+        : return : customized image
+        
+        """
+        
+        cv2.rectangle(image,(bbox[0],bbox[1]),(bbox[2],bbox[3]),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        return image
+    
+    def rect_transparent(self,image:np.array,bbox:List,colors:Tuple=(0,255,255),transparency:float=0.5,cornerRect:bool=True,thickness:int=2,line_len:int=10) -> np.array:
+        
+        """
+        THIS FUNCTION WILL CREATE A TRANSPARENT RECTANGLE WITH CORNER RECTANGLE IF PASSED TRUE
+        
+        : param image : cv2.imread() image
+        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
+        : prarm colors : expects a tuple (0,255,0)
+        : param transparency : how transparent your rectangle will be , lower float means high transparent
+        : param corner_rect : it will enable corner rect function
+        : param thickness : it will change corner rect's thickness
+        : param line_len : line len will change line distance from starting point, if line len is higher number then it will be a big straight line
+        
+        : return : customized image
+        
+        """
+        
+        overlay = image.copy()
+        
+        cv2.rectangle(overlay,(bbox[0],bbox[1]),(bbox[2],bbox[3]), colors, -1)
+        image = cv2.addWeighted(overlay, transparency, image, 1 - transparency, 0)
+        if cornerRect:
+            self.cornerRect(image,bbox,colors,thickness,line_len)
+
+        return image
+   
+    
+    def circle(self,image:np.array,center:Tuple=(20,50),radius:int=2,colors:Tuple=(0,255,0),thickness:int=2) -> np.array:
+        
+        """
+        THIS FUNCTION WILL CREATE A CIRCLE
+        
+        : param image : cv2.imread() image
+        : param center : expects a tuple for drawing the circle
+        : param radius : circle's radius
+        : prarm colors : expects a tuple (0,255,0)
+        : param thickness : it will change circle's thickness
+
+        : return : customized image
+        
+        """
+        cv2.circle(image,center=center,radius=radius,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        
+        return image
+    
+    
+    def putText(self,image:np.array,texts:str,bbox:Union[List,Tuple],font:cv2.FONT_HERSHEY_PLAIN=cv2.FONT_HERSHEY_PLAIN,colors:Tuple=(0,0,255),scale:int=2,thickness:int=2,border:bool=True,rect_color:Tuple=(0,255,0),border_size:int=2) -> np.array:
+        
+        """
+        THIS FUNCTION WILL PUT TEXT IN THE IMAGE
+        
+        : param image : cv2.imread() image
+        : param texts : expects a text
+        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
+        : param font : expects cv2.FONT_
+        : prarm colors : expects a tuple (0,255,0)
+        : param scale : text scale number , expects int val
+        : param thickness : it will change texts thickness , expects int
+        : param border : if True , it will create a border around text
+        : param rect color : will change border's rectangle color
+        : param border size : it will change border rectangle's side
+ 
+        
+        : return : customized image
+        
+        """
+        
+        if border:
+            (w, h), _ = cv2.getTextSize(str(texts),font, scale, thickness)
+            cv2.rectangle(image,(bbox[0],bbox[1]),(bbox[0]+w+border_size,bbox[1]-h-border_size),rect_color,-1,cv2.LINE_AA)
+            cv2.putText(image,text=str(texts),org=(bbox[0],bbox[1]),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        else:
+            cv2.putText(image,text=str(texts),org=(bbox[0],bbox[1]),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        return image
+    
+    def putText_center(self,image:np.array,texts:str,bbox:List,font:cv2.FONT_HERSHEY_PLAIN=cv2.FONT_HERSHEY_PLAIN,colors:Tuple=(0,0,255),scale:int=2,thickness:int=2,border:bool=True,rect_color:Tuple=(0,255,0),border_size:int=2) -> np.array:
+        
+        """
+        THIS FUNCTION WILL PUT TEXT IN THE CENTER OF THE OBEJCT.
+        
+        : param image : cv2.imread() image
+        : param texts : expects a text
+        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
+        : param font : expects cv2.FONT_
+        : prarm colors : expects a tuple (0,255,0)
+        : param scale : text scale number , expects int val
+        : param thickness : it will change texts thickness , expects int
+        : param border : if True , it will create a border around text
+        : param rect color : will change border's rectangle color
+        : param border size : it will change border rectangle's side
+ 
+        
+        : return : customized image
+        
+        """
+        
+        center_x , center_y = int((bbox[0] + bbox[2])/2) , int((bbox[1] + bbox[3])/2)
+        if border:
+            (w, h), _ = cv2.getTextSize(str(texts),font, scale, thickness)
+            cv2.rectangle(image,(center_x-10,center_y),(center_x+w+border_size,center_y-h-border_size),rect_color,-1,cv2.LINE_AA)
+            cv2.putText(image,text=str(texts),org=(center_x-10,center_y),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        else:
+            cv2.putText(image,text=str(texts),org=(center_x-10,center_y),fontFace=font,fontScale=scale,color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        return image
+    
+    def putText_centerStyle(self,image:np.array,texts:str,bbox:List=[10,20,30,40],font=cv2.FONT_HERSHEY_PLAIN,colors:Tuple=(0,0,255),circleRadius:int=5,Fontscale:int=2,thickness:int=1,border:bool=True,text_color:Tuple=(0,255,0),border_size:int=2) -> np.array:
+        
+        """
+        THIS FUNCTION WILL PUT TEXT IN THE CENTER OF THE OBEJCT AND CREATE A GOOD VISUALIZATION
+        
+        : param image : cv2.imread() image
+        : param texts : expects a text
+        : param bbox  : A list containing rect top left x , y and bottom right x , y --> [x1,y1,x2,y2]
+        : param font : expects cv2.FONT_
+        : prarm colors : expects a tuple (0,255,0)
+        : param circleRadius : expects a int value for the circle radius
+        : param Fontscale : text scale number , expects int val
+        : param thickness : it will change texts thickness , expects int
+        : param border : if True , it will create a border around text
+        : param text color : will change text's color
+        : param border size : it will change border size of text
+ 
+        
+        : return : customized image
+        
+        """
+        
+        center_x , center_y = int((bbox[0] + bbox[2])/2) , int((bbox[1] + bbox[3])/2)
+        (w, h), _ = cv2.getTextSize(str(texts),font, Fontscale, thickness)
+       
+        if border:
+            cv2.rectangle(image,(center_x+60,center_y-30+10),(center_x+60+w+border_size,center_y-h-border_size-30+10),colors,-1,cv2.LINE_AA)
+    
+        cv2.circle(image,center=(center_x,center_y),radius=circleRadius,color=colors,thickness=-1,lineType=cv2.LINE_AA)
+        cv2.circle(image,center=(center_x,center_y),radius=circleRadius*2,color=colors,thickness=1,lineType=cv2.LINE_AA)
+        cv2.line(image,(center_x,center_y),(center_x+30,center_y-30),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        cv2.line(image,(center_x+30,center_y-30),(center_x+60,center_y-30),color=colors,thickness=thickness,lineType=cv2.LINE_AA)
+        cv2.putText(image,text=str(texts),org=(center_x+60,center_y-30+10),fontFace=font,fontScale=Fontscale,color=text_color,thickness=thickness,lineType=cv2.LINE_AA)
+       
+        return image
+
+    def line_create(self,image:np.array,start_point:Tuple=(10,20),end_point:Tuple=(50,50),colors:Tuple=(0,255,0,10),lineThickness:int=55,transparency:float=.6) -> np.array:
+        
+        """
+        THIS FUCNTION WILL CREATE A LINE
+        
+        : param image : cv2.imread() image
+        : param start point : expects a tuple for line start point
+        : param end point : expects a tuple for line end point
+        : prarm colors : expects a tuple (0,255,0)
+        : param lineThickness : it will change line's thickness , expects int
+        : param transparency : how transparent your line will be
+ 
+        : return : customized image
+        
+        """
+        
+        overlay = image.copy()
+        cv2.line(image,start_point,end_point,color=colors,thickness=lineThickness,lineType=cv2.LINE_AA)
+        image = cv2.addWeighted(overlay, transparency, image, 1 - transparency, 0)
+        
+        return image
+    
+    def polygon_create(self,image:np.array,poly_points:List[List]=[[10,20],[20,30],[30,40]],colors:Tuple=(0,255,0),isClosed:True=True,thickness:int=2) -> np.array: 
+        
+        """
+        THIS FUNCTION WILL CREATE A POLYGON
+        
+        : param image : cv2.imread() image
+        : param poly_points:  expects a list of list coordinate to draw polygon
+        : prarm colors : expects a tuple (0,255,0)
+        : param isClosed : expects a bool 
+        : param lineThickness : it will change line's thickness , expects int
+   
+ 
+        : return : customized image
+        
+        """
+        cv2.polylines(image, [np.array(poly_points,dtype=np.int32)], isClosed=isClosed, color=colors, thickness=thickness,lineType=cv2.LINE_AA)
+        return image
+    
+    
+    def fillPolygon_create(self,image:np.array,poly_points:List[List]=[[10,20],[20,30],[30,40]],colors:Tuple=(0,255,0),transparency:float=.8) -> np.array:
+        """
+        THIS FUNCTION CREATE A FILL POLYGON WILL COLOR
+        
+        : param image : cv2.imread() image
+        : param poly_points:  expects a list of list coordinate to draw polygon
+        : prarm colors : expects a tuple (0,255,0)
+        : param lineThickness : it will change line's thickness , expects int
+   
+ 
+        : return : customized image
+        
+        """
+        overlay = image.copy()
+        cv2.fillPoly(image, [np.array(poly_points,dtype=np.int32)], colors,lineType=cv2.LINE_AA)
+        image = cv2.addWeighted(overlay, transparency, image, 1 - transparency, 0)
+        return image
+    
+    def line_in_out_counter(self,image:np.array,line_start_pos:Tuple=(10,20),line_end_pos:Tuple=(30,40),detection_pos:Tuple=(50,50),line_color:Tuple=(0,255,0),lineThickness:int=2,lineTransparecy:float=0.5) -> Tuple[np.array,bool]:
+        
+        """
+        THIS FUNCTION WILL DETECT IF ANY OBJECT IS INSIDE ITS LINE BY GIVEN OBJECT DETECTION POINTS , IF IT IS THEN IT WILL COUNT THE OBJECT , IT IS USED FOR OBJECT TRACKING
+        
+        : param image : cv2.imread() image
+        : param start point : expects a tuple for line start point
+        : param end point : expects a tuple for line end point
+        : param detection pos : your detection points coordinates , expects tuple
+        : prarm Linecolors : expects a tuple (0,255,0)
+        : param lineThickness : it will change line's thickness , expects int
+        : param transparency : how transparent your line will be
+ 
+        : return : customized image , bool ( if detction pos is inside the line or not)
+        
+        """
+        
+        line_created = self.line_create(image,start_point=line_start_pos,end_point=line_end_pos,colors=line_color,lineThickness=lineThickness,transparency=lineTransparecy)
+        distance = cv2.pointPolygonTest(np.array([(line_start_pos[0],line_start_pos[1]), (line_end_pos[0],line_end_pos[1])]), detection_pos, False)
+        
+        if distance > 0:
+            detect = True
+        else:
+            detect = False
+        
+        return (line_created , detect)
+    
+    
+    def polygon_in_out_counter(self,image:np.array,poly_points:List[List]=[[10,20],[30,40],[55,60]],detectionPoints:Tuple=(10,30),colors:Tuple=(0,255,0),transparency:float=0.2) -> Tuple[np.array,bool]:
+        """
+        THIS FUNCTION WILL DETECT IF ANY OBJECT IS INSIDE ITS POLYGON AREA BY GIVEN OBJECT DETECTION POINTS , IF IT IS THEN IT WILL COUNT THE OBJECT , IT IS USED FOR OBJECT TRACKING
+        
+        : param image : cv2.imread() image
+        : param poly_points:  expects a list of list coordinate to draw polygon
+        : param detection pos : your detection points coordinates , expects tuple
+        : prarm colors : expects a tuple (0,255,0)
+        : param lineThickness : it will change line's thickness , expects int
+   
+ 
+        : return : customized image , bool ( if detction pos is inside the line or not)
+        
+        """
+        
+        poly_fill = self.fillPolygon_create(image, [np.array(poly_points,dtype=np.int32)], colors,transparency=transparency)
+        distance = cv2.pointPolygonTest(np.array(poly_points), detectionPoints, measureDist=False)
+        if distance > 0:
+            detect = True
+        else:
+            detect = False
+        
+        return (poly_fill , detect)
+    
+    def create_mask(self,image,points:List[List]=[[10,20],[30,40],[55,60]]) -> np.array:
+        
+        """
+        THIS FUNCTION WILL CREATE IMAGE MASK
+        
+        : param image : cv2.imread() image
+        : param points:  expects a list of list coordinate to create mask
+        
+        : return : image mask
+        
+        """
+        
+        image_height, image_width,_ = image.shape
+        mask = np.zeros((image_height, image_width), dtype=np.uint8)
+        cv2.fillPoly(mask, [np.array(points,dtype=np.int32)], 255,cv2.LINE_AA)
+        mask = cv2.bitwise_and(image,image,mask=mask)
+        return mask
+    
+    
+        
+    
+        
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `lumina-1.0.1/PKG-INFO` & `lumina-1.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1
-Name: lumina
-Version: 1.0.1
-Summary: Customize your object detection bounding boxes and filter the tracking zones with Lumina
-Author: Souvik Saha
-Author-email: ssouvik.191@gmail.com
-Keywords: machine_learning,development,data_augmentations
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-
-# Lumina 🚀
-#### With Lumina, you can customize object bounding boxes for better visualization and create zones for more efficient tracking.
-
-<img src='images\logo1.png'>
-
-## Output from Lumina 
-
-<img src='images\output_video5_AdobeExpress.gif'>
-
-##  How to use Lumina❓
-#### Install the module first using pip 🚀
-
-```python
-pip install lumina
-
-```
-#### For Github clone 🚀
-Github clone link : [Lumina](https://github.com/Souviksaha1998/Lumina) repo 🖥️
-
-## After Installation, Import the Lumina class  🚀
-
-```python
-# create a .py file
-# import modules
-from Lumina.lumina import Lumina
-from Lumina.colors import color_palette
-# create a object of lumina 
-lumina = Lumina()
-#if you want color palette then do this, it will return random colors
-color = color_palette() 
-```
-## Usage (Functions of lumina)🎯
-#### you can use this functions by - (lumina.<function_name>)
-<img src='images\ex1.png'>
-<img src='images\ex2.png'>
-<img src='images\ex3.png'>
-<img src='images\ex4.png'>
-
-***
-## 1.1 Polygon zone creation for detection or tracking
-### This function will create a polygon zone.
-<img src='images\ex5.png'>
-
-## 1.2 polygon_in_out_counter function will create polygon region and return image and bool = True , if anything is inside in the poly region. -- this function is helpful for region based tracking. Alternatively You can use line_in_out_counter
-
-<img src='images\ex6.png'>
-
-## 1.3 This function will create a mask, based on points. If you don't want to capture the whole frame then you can use this function. This will reduce computational cost.
-
-<img src='images\ex7.png'>
-
-
-### It is my goal to constantly improve Lumina, and these are some of the initial features. I will be adding more features to better customize Lumina in the future. Thanks in advance. :)
-
-***
-
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
-
-
+Metadata-Version: 2.1
+Name: lumina
+Version: 1.0.4
+Summary: Customize your object detection bounding boxes and filter the tracking zones with Lumina
+Author: Souvik Saha
+Author-email: ssouvik.191@gmail.com
+Keywords: machine_learning,development,data_augmentations
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+
+# Lumina 🚀
+#### With Lumina, you can customize object bounding boxes for better visualization and create zones for more efficient tracking.
+
+<img src='images\logo1.png'>
+
+## Output from Lumina 
+
+<img src='images\output_video5_AdobeExpress.gif'>
+
+##  How to use Lumina❓
+#### Install the module first using pip 🚀
+
+```python
+pip install lumina
+
+```
+#### For Github clone 🚀
+Github clone link : [Lumina](https://github.com/Souviksaha1998/Lumina) repo 🖥️
+
+## After Installation, Import the Lumina class  🚀
+
+```python
+# create a .py file
+# import modules
+from Lumina.lumina import Lumina
+from Lumina.colors import color_palette
+# create a object of lumina 
+lumina = Lumina()
+#if you want color palette then do this, it will return random colors
+color = color_palette() 
+```
+## Usage (Functions of lumina)🎯
+#### you can use this functions by - (lumina.<function_name>)
+<img src='images\ex1.png'>
+<img src='images\ex2.png'>
+<img src='images\ex3.png'>
+<img src='images\ex4.png'>
+
+***
+## 1.1 Polygon zone creation for detection or tracking
+### This function will create a polygon zone.
+<img src='images\ex5.png'>
+
+## 1.2 polygon_in_out_counter function will create polygon region and return image and bool = True , if anything is inside in the poly region. -- this function is helpful for region based tracking. Alternatively You can use line_in_out_counter
+
+<img src='images\ex6.png'>
+
+## 1.3 This function will create a mask, based on points. If you don't want to capture the whole frame then you can use this function. This will reduce computational cost.
+
+<img src='images\ex7.png'>
+
+
+### It is my goal to constantly improve Lumina, and these are some of the initial features. I will be adding more features to better customize Lumina in the future. Thanks in advance. :)
+
+***
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
+
+
```

### Comparing `lumina-1.0.1/README.md` & `lumina-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lumina-1.0.1/lumina.egg-info/PKG-INFO` & `lumina-1.0.4/lumina.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1
-Name: lumina
-Version: 1.0.1
-Summary: Customize your object detection bounding boxes and filter the tracking zones with Lumina
-Author: Souvik Saha
-Author-email: ssouvik.191@gmail.com
-Keywords: machine_learning,development,data_augmentations
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-
-# Lumina 🚀
-#### With Lumina, you can customize object bounding boxes for better visualization and create zones for more efficient tracking.
-
-<img src='images\logo1.png'>
-
-## Output from Lumina 
-
-<img src='images\output_video5_AdobeExpress.gif'>
-
-##  How to use Lumina❓
-#### Install the module first using pip 🚀
-
-```python
-pip install lumina
-
-```
-#### For Github clone 🚀
-Github clone link : [Lumina](https://github.com/Souviksaha1998/Lumina) repo 🖥️
-
-## After Installation, Import the Lumina class  🚀
-
-```python
-# create a .py file
-# import modules
-from Lumina.lumina import Lumina
-from Lumina.colors import color_palette
-# create a object of lumina 
-lumina = Lumina()
-#if you want color palette then do this, it will return random colors
-color = color_palette() 
-```
-## Usage (Functions of lumina)🎯
-#### you can use this functions by - (lumina.<function_name>)
-<img src='images\ex1.png'>
-<img src='images\ex2.png'>
-<img src='images\ex3.png'>
-<img src='images\ex4.png'>
-
-***
-## 1.1 Polygon zone creation for detection or tracking
-### This function will create a polygon zone.
-<img src='images\ex5.png'>
-
-## 1.2 polygon_in_out_counter function will create polygon region and return image and bool = True , if anything is inside in the poly region. -- this function is helpful for region based tracking. Alternatively You can use line_in_out_counter
-
-<img src='images\ex6.png'>
-
-## 1.3 This function will create a mask, based on points. If you don't want to capture the whole frame then you can use this function. This will reduce computational cost.
-
-<img src='images\ex7.png'>
-
-
-### It is my goal to constantly improve Lumina, and these are some of the initial features. I will be adding more features to better customize Lumina in the future. Thanks in advance. :)
-
-***
-
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
-
-
+Metadata-Version: 2.1
+Name: lumina
+Version: 1.0.4
+Summary: Customize your object detection bounding boxes and filter the tracking zones with Lumina
+Author: Souvik Saha
+Author-email: ssouvik.191@gmail.com
+Keywords: machine_learning,development,data_augmentations
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+
+# Lumina 🚀
+#### With Lumina, you can customize object bounding boxes for better visualization and create zones for more efficient tracking.
+
+<img src='images\logo1.png'>
+
+## Output from Lumina 
+
+<img src='images\output_video5_AdobeExpress.gif'>
+
+##  How to use Lumina❓
+#### Install the module first using pip 🚀
+
+```python
+pip install lumina
+
+```
+#### For Github clone 🚀
+Github clone link : [Lumina](https://github.com/Souviksaha1998/Lumina) repo 🖥️
+
+## After Installation, Import the Lumina class  🚀
+
+```python
+# create a .py file
+# import modules
+from Lumina.lumina import Lumina
+from Lumina.colors import color_palette
+# create a object of lumina 
+lumina = Lumina()
+#if you want color palette then do this, it will return random colors
+color = color_palette() 
+```
+## Usage (Functions of lumina)🎯
+#### you can use this functions by - (lumina.<function_name>)
+<img src='images\ex1.png'>
+<img src='images\ex2.png'>
+<img src='images\ex3.png'>
+<img src='images\ex4.png'>
+
+***
+## 1.1 Polygon zone creation for detection or tracking
+### This function will create a polygon zone.
+<img src='images\ex5.png'>
+
+## 1.2 polygon_in_out_counter function will create polygon region and return image and bool = True , if anything is inside in the poly region. -- this function is helpful for region based tracking. Alternatively You can use line_in_out_counter
+
+<img src='images\ex6.png'>
+
+## 1.3 This function will create a mask, based on points. If you don't want to capture the whole frame then you can use this function. This will reduce computational cost.
+
+<img src='images\ex7.png'>
+
+
+### It is my goal to constantly improve Lumina, and these are some of the initial features. I will be adding more features to better customize Lumina in the future. Thanks in advance. :)
+
+***
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
+
+
```

### Comparing `lumina-1.0.1/setup.py` & `lumina-1.0.4/setup.py`

 * *Files identical despite different names*

