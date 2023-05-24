# Comparing `tmp/midvoxio-0.1.0.tar.gz` & `tmp/midvoxio-0.1.1.tar.gz`

## Comparing `midvoxio-0.1.0.tar` & `midvoxio-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 midvoxio-0.1.0/assets/palette/cat.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.0/assets/palette/pal0.png
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 midvoxio-0.1.0/assets/vox/98/cat.vox
--rw-r--r--   0        0        0    29518 2020-02-02 00:00:00.000000 midvoxio-0.1.0/assets/vox/99/3x3x3.vox
--rw-r--r--   0        0        0    48186 2020-02-02 00:00:00.000000 midvoxio-0.1.0/assets/vox/99/cars.vox
--rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 midvoxio-0.1.0/assets/vox/voxedit/cat.vox
--rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 midvoxio-0.1.0/img/3x3x3.jpg
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/examples.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/config.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/exceptions.py
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/models.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/parser.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/vox.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/voxio.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 midvoxio-0.1.0/src/pyvox/writer.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 midvoxio-0.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 midvoxio-0.1.0/LICENSE
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 midvoxio-0.1.0/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 midvoxio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 midvoxio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 midvoxio-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/palette/cat.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/palette/pal0.png
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/98/cat.vox
+-rw-r--r--   0        0        0    29518 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/99/3x3x3.vox
+-rw-r--r--   0        0        0    48186 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/99/cars.vox
+-rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/voxedit/cat.vox
+-rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 midvoxio-0.1.1/img/3x3x3.jpg
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/examples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/config.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/exceptions.py
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/models.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/parser.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/vox.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/voxio.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/writer.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 midvoxio-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 midvoxio-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 midvoxio-0.1.1/README.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 midvoxio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 midvoxio-0.1.1/PKG-INFO
```

### Comparing `midvoxio-0.1.0/assets/vox/98/cat.vox` & `midvoxio-0.1.1/assets/vox/98/cat.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.0/assets/vox/99/3x3x3.vox` & `midvoxio-0.1.1/assets/vox/99/3x3x3.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.0/assets/vox/99/cars.vox` & `midvoxio-0.1.1/assets/vox/99/cars.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.0/assets/vox/voxedit/cat.vox` & `midvoxio-0.1.1/assets/vox/voxedit/cat.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.0/img/3x3x3.jpg` & `midvoxio-0.1.1/img/3x3x3.jpg`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.0/src/examples.py` & `midvoxio-0.1.1/src/examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from pyvox.models import *
-from pyvox.voxio import  * 
-
-# print(vox_to_arr('assets/vox/99/3x3x3.vox'))
-# viz_vox('assets/vox/98/cat.vox')
-# show_chunks('assets/vox/99/cars.vox')
-# viz_vox('assets/vox/99/cars.vox',1)
-# print(get_rendering_attributes('assets/vox/99/3x3x3.vox'))
-# vox = get_vox('assets/vox/99/cars.vox')
-
-# v=vox_to_arr('assets/vox/98/cat.vox')
-# path='palette/cat.png'
-
-# write_list_to_vox(v,'test.vox',path)
-
-# t=ArrayWriter(v,palette_path=path)
-# t.write('test.vox')
-
-
-# # create new nodes
-# kwargs={
-#     'node_id':1,
-#     'node_attr':{},
-#     'models':[ModelAttr({},0)]
-# }
-
-# shape=nSHP(**kwargs)
-
-# kwargs={
-#     'node_id':2,
-#     'node_attributes':{},
-#     'child_node_id':1,
-#     'reversed_id':-1,
-#     'layer_id':1,
-#     'frames':[
-#             {
-#             '_t': '10 10 10'
-#         }
-#     ]
-# }
-# trans=nTRN(**kwargs)
+from midvoxio.models import *
+from midvoxio.voxio import  * 
+
+# print(vox_to_arr('assets/vox/99/3x3x3.vox'))
+# viz_vox('assets/vox/98/cat.vox')
+# show_chunks('assets/vox/99/cars.vox')
+# viz_vox('assets/vox/99/cars.vox',1)
+# print(get_rendering_attributes('assets/vox/99/3x3x3.vox'))
+# vox = get_vox('assets/vox/99/cars.vox')
+
+# v=vox_to_arr('assets/vox/98/cat.vox')
+# path='palette/cat.png'
+
+# write_list_to_vox(v,'test.vox',path)
+
+# t=ArrayWriter(v,palette_path=path)
+# t.write('test.vox')
+
+
+# # create new nodes
+# kwargs={
+#     'node_id':1,
+#     'node_attr':{},
+#     'models':[ModelAttr({},0)]
+# }
+
+# shape=nSHP(**kwargs)
+
+# kwargs={
+#     'node_id':2,
+#     'node_attributes':{},
+#     'child_node_id':1,
+#     'reversed_id':-1,
+#     'layer_id':1,
+#     'frames':[
+#             {
+#             '_t': '10 10 10'
+#         }
+#     ]
+# }
+# trans=nTRN(**kwargs)
```

### Comparing `midvoxio-0.1.0/src/pyvox/models.py` & `midvoxio-0.1.1/src/midvoxio/models.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-from ast import Mod
-from collections import namedtuple
-from pprint import pformat
-from struct import unpack_from, calcsize, pack
-
-import numpy as np
-from PIL import Image
-
-from .exceptions import DumpingException
-
-ModelAttr=namedtuple('ModelAttr','attr_dic id')
-default_palette=[
-    0x00000000, 0xffffffff, 0xffccffff, 0xff99ffff, 0xff66ffff, 0xff33ffff, 0xff00ffff, 0xffffccff, 0xffccccff, 0xff99ccff, 0xff66ccff, 0xff33ccff, 0xff00ccff, 0xffff99ff, 0xffcc99ff, 0xff9999ff,
-    0xff6699ff, 0xff3399ff, 0xff0099ff, 0xffff66ff, 0xffcc66ff, 0xff9966ff, 0xff6666ff, 0xff3366ff, 0xff0066ff, 0xffff33ff, 0xffcc33ff, 0xff9933ff, 0xff6633ff, 0xff3333ff, 0xff0033ff, 0xffff00ff,
-    0xffcc00ff, 0xff9900ff, 0xff6600ff, 0xff3300ff, 0xff0000ff, 0xffffffcc, 0xffccffcc, 0xff99ffcc, 0xff66ffcc, 0xff33ffcc, 0xff00ffcc, 0xffffcccc, 0xffcccccc, 0xff99cccc, 0xff66cccc, 0xff33cccc,
-    0xff00cccc, 0xffff99cc, 0xffcc99cc, 0xff9999cc, 0xff6699cc, 0xff3399cc, 0xff0099cc, 0xffff66cc, 0xffcc66cc, 0xff9966cc, 0xff6666cc, 0xff3366cc, 0xff0066cc, 0xffff33cc, 0xffcc33cc, 0xff9933cc,
-    0xff6633cc, 0xff3333cc, 0xff0033cc, 0xffff00cc, 0xffcc00cc, 0xff9900cc, 0xff6600cc, 0xff3300cc, 0xff0000cc, 0xffffff99, 0xffccff99, 0xff99ff99, 0xff66ff99, 0xff33ff99, 0xff00ff99, 0xffffcc99,
-    0xffcccc99, 0xff99cc99, 0xff66cc99, 0xff33cc99, 0xff00cc99, 0xffff9999, 0xffcc9999, 0xff999999, 0xff669999, 0xff339999, 0xff009999, 0xffff6699, 0xffcc6699, 0xff996699, 0xff666699, 0xff336699,
-    0xff006699, 0xffff3399, 0xffcc3399, 0xff993399, 0xff663399, 0xff333399, 0xff003399, 0xffff0099, 0xffcc0099, 0xff990099, 0xff660099, 0xff330099, 0xff000099, 0xffffff66, 0xffccff66, 0xff99ff66,
-    0xff66ff66, 0xff33ff66, 0xff00ff66, 0xffffcc66, 0xffcccc66, 0xff99cc66, 0xff66cc66, 0xff33cc66, 0xff00cc66, 0xffff9966, 0xffcc9966, 0xff999966, 0xff669966, 0xff339966, 0xff009966, 0xffff6666,
-    0xffcc6666, 0xff996666, 0xff666666, 0xff336666, 0xff006666, 0xffff3366, 0xffcc3366, 0xff993366, 0xff663366, 0xff333366, 0xff003366, 0xffff0066, 0xffcc0066, 0xff990066, 0xff660066, 0xff330066,
-    0xff000066, 0xffffff33, 0xffccff33, 0xff99ff33, 0xff66ff33, 0xff33ff33, 0xff00ff33, 0xffffcc33, 0xffcccc33, 0xff99cc33, 0xff66cc33, 0xff33cc33, 0xff00cc33, 0xffff9933, 0xffcc9933, 0xff999933,
-    0xff669933, 0xff339933, 0xff009933, 0xffff6633, 0xffcc6633, 0xff996633, 0xff666633, 0xff336633, 0xff006633, 0xffff3333, 0xffcc3333, 0xff993333, 0xff663333, 0xff333333, 0xff003333, 0xffff0033,
-    0xffcc0033, 0xff990033, 0xff660033, 0xff330033, 0xff000033, 0xffffff00, 0xffccff00, 0xff99ff00, 0xff66ff00, 0xff33ff00, 0xff00ff00, 0xffffcc00, 0xffcccc00, 0xff99cc00, 0xff66cc00, 0xff33cc00,
-    0xff00cc00, 0xffff9900, 0xffcc9900, 0xff999900, 0xff669900, 0xff339900, 0xff009900, 0xffff6600, 0xffcc6600, 0xff996600, 0xff666600, 0xff336600, 0xff006600, 0xffff3300, 0xffcc3300, 0xff993300,
-    0xff663300, 0xff333300, 0xff003300, 0xffff0000, 0xffcc0000, 0xff990000, 0xff660000, 0xff330000, 0xff0000ee, 0xff0000dd, 0xff0000bb, 0xff0000aa, 0xff000088, 0xff000077, 0xff000055, 0xff000044,
-    0xff000022, 0xff000011, 0xff00ee00, 0xff00dd00, 0xff00bb00, 0xff00aa00, 0xff008800, 0xff007700, 0xff005500, 0xff004400, 0xff002200, 0xff001100, 0xffee0000, 0xffdd0000, 0xffbb0000, 0xffaa0000,
-    0xff880000, 0xff770000, 0xff550000, 0xff440000, 0xff220000, 0xff110000, 0xffeeeeee, 0xffdddddd, 0xffbbbbbb, 0xffaaaaaa, 0xff888888, 0xff777777, 0xff555555, 0xff444444, 0xff222222, 0xff111111
-]
-
-
-class XYZI():
-    '''
-    Chunk id 'XYZI' : model voxels, paired with the SIZE chunk
-    -------------------------------------------------------------------------------
-    Bytes  | Type       | Value
-    -------------------------------------------------------------------------------
-    4        | int        | numVoxels (N)
-    4 x N    | int        | (x, y, z, colorIndex) : 1 byte for each component
-    -------------------------------------------------------------------------------
-    '''
-    id=b'XYZI'
-    def __init__(self,xyzi_arr):
-        self.xyzi=xyzi_arr
-        pass
-    
-    def to_b(self):
-        length=len(self.xyzi)
-        bstr=pack('i',length)
-        for i in self.xyzi:
-            bstr+=pack('4B',i[0],i[1],i[2],i[3])
-        return bstr
-
-class SIZE():
-    '''
-     Chunk id 'SIZE' : model size
-    -------------------------------------------------------------------------------
-    Bytes  | Type       | Value
-    -------------------------------------------------------------------------------
-    4        | int        | size x
-    4        | int        | size y
-    4        | int        | size z : gravity direction
-    -------------------------------------------------------------------------------
-    '''
-    id=b'SIZE'
-    def __init__(self,shape):
-        self.size=shape[:-1]
-    def to_b(self):
-        return pack('3i',self.size[0],self.size[1],self.size[2])
-
-class RGBA():
-    '''
-    Chunk id 'RGBA' : palette
-    -------------------------------------------------------------------------------
-    Bytes  | Type       | Value
-    -------------------------------------------------------------------------------
-    4 x 256  | int        | (R, G, B, A) : 1 byte for each component
-                        | * <NOTICE>
-                        | * color [0-254] are mapped to palette index [1-255], e.g : 
-                        | 
-                        | for ( int i = 0; i <= 254; i++ ) {
-                        |     palette[i + 1] = ReadRGBA(); 
-                        | }
-    -------------------------------------------------------------------------------
-    '''
-    id=b'RGBA'
-    def __init__(self,img_path=None,palette_arr=None):
-        if palette_arr:
-            self.palette_arr=palette_arr
-        else:
-            self.palette_arr=self._get_palette_arr_from_img(img_path)
-        pass
-
-    def _get_palette_arr_from_img(self,img_path):
-        img=Image.open(img_path)
-        color=np.array(img)
-        return color[0]
-    
-    def to_b(self):
-        bstr=b''
-        for i in self.palette_arr:
-            bstr+=pack('4B',i[0],i[1],i[2],i[3])
-        return bstr
-
-
-class nTRN():
-    '''
-    Transform Node Chunk : "nTRN"
-
-    int32	: node id
-    DICT	: node attributes
-        (_name : string)
-        (_hidden : 0/1)
-    int32 	: child node id
-    int32 	: reserved id (must be -1)
-    int32	: layer id
-    int32	: num of frames (must be greater than 0)
-
-    // for each frame
-    {
-    DICT	: frame attributes
-        (_r : int8)    ROTATION, see (c)
-        (_t : int32x3) translation
-        (_f : int32)   frame index, start from 0 
-    }xN
-    '''
-    id=b'nTRN'
-    def __init__(self,node_id,node_attributes,
-    child_node_id,reversed_id,layer_id,frames):
-        self.node_id=node_id
-        self.node_attributes=node_attributes
-        self.child_node_id=child_node_id
-        self.reversed_id=reversed_id
-        self.layer_id=layer_id
-        self.frames=frames
-    
-    def to_b(self):
-        byts=pack('i',self.node_id)
-        byts+=Bdict(py_dict=self.node_attributes).bytes
-        byts+=pack('4i',self.child_node_id,
-                        self.reversed_id,
-                        self.layer_id,
-                        len(self.frames))
-        for frame in self.frames:
-            byts+=Bdict(py_dict=frame).bytes
-        return byts
-
-    def __repr__(self):
-        ret=f'''
-====nTRN====
-node_id:{self.node_id}
-frames:{format(self.frames)}
-child_node_id:{self.child_node_id}
-layer_id:{self.layer_id}
-'''
-        return ret
-
-class NGRP():
-    '''
-    Group Node Chunk : "nGRP" 
-    int32	: node id
-    DICT	: node attributes
-    int32 	: num of children nodes
-
-    // for each child
-    {
-    int32	: child node id
-    }xN
-    '''
-    def __init__(self,node_id,dic,num,child_lst):
-        self.node_id=node_id
-        self.node_attr=dic
-        self.children_num=num
-        self.children_ids=child_lst
-        pass
-    def __repr__(self):
-        ret=f'''
-====nGPR====
-node_id:{self.node_id}
-children_ids:{self.children_ids}
-'''
-        return ret
-
-
-class nSHP():
-    '''
-    Shape Node Chunk : "nSHP" 
-
-    int32	: node id
-    DICT	: node attributes
-    int32 	: num of models (must be greater than 0)
-
-    // for each model
-    {
-    int32	: model id
-    DICT	: model attributes : reserved
-        (_f : int32)   frame index, start from 0
-    }xN
-    '''
-    def __init__(self,node_id,models,node_attr={}):
-        self.node_id=node_id
-        self.node_attr=node_attr
-        self.models=models
-    def __repr__(self):
-        ret=f'''
-====nSHP====
-node_id:{self.node_id}
-models:{pformat([i for i in self.models])}
-'''
-        return ret
-    def to_b(self):
-        byts=pack('i',self.node_id)
-        byts+=Bdict(py_dict=self.node_attr).bytes
-        byts+=pack('i',len(self.models))
-        for model in self.models:
-            byts+=pack('i',model.id)
-            byts+=Bdict(py_dict=model.attr_dic)
-        return byts
-
-class Material():
-    '''
-    Material Chunk : "MATL"
-        int32	: material id
-        DICT	: material properties
-            (_type : str) _diffuse, _metal, _glass, _emit
-            (_weight : float) range 0 ~ 1
-            (_rough : float)
-            (_spec : float)
-            (_ior : float)
-            (_att : float)
-            (_flux : float)
-            (_plastic)
-    '''
-    def __init__(self,id,dic):
-        self.id=id
-        self.dic=dic
-        pass
-
-    def __str__(self):
-        return str({'id':self.id,
-                'properties':self.dic
-                })
-
-class Camera():
-    '''
-    Render Camera Chunk : "rCAM"
-        int32	: camera id
-        DICT	: camera attribute
-            (_mode : string)
-            (_focus : vec(3))
-            (_angle : vec(3))
-            (_radius : int)
-            (_frustum : float)
-            (_fov : int)
-    '''
-    def __init__(self,id,dic):
-        self.id=id
-        self.dic=dic
-        pass
-
-    def __str__(self):
-        return str({'id':self.id,
-                'attributes':self.dic
-                })
-
-class Layer():
-    '''
-    Layer Chunk : "LAYR"
-        int32	: layer id
-        DICT	: layer attribute
-            (_name : string)
-            (_hidden : 0/1)
-        int32	: reserved id, must be -1
-    '''
-    def __init__(self,id,dic,rev_id):
-        self.id=id
-        self.dic=dic
-        self.rev_id=rev_id
-
-class Note():
-    '''
-    Palette Note Chunk : "NOTE"
-        int32	: num of color names
-
-        // for each name
-        {
-        STRING	: color name
-        }xN
-    '''
-    def __init__(self,num,color_names):
-        self.num=num
-        self.color_names=color_names
-
-class ROBJ():
-    '''
-    Render Objects Chunk : "rOBJ"
-        DICT	: rendering attributes
-    '''
-    def __init__(self,dic):
-        self.dic=dic
-    
-    def __str__(self):
-        return str(self.dic)
-
-class Bstring():
-    '''
-    STRING type
-        int32   : buffer size (in bytes)
-        int8xN	: buffer (without the ending "\0")
-    '''
-    def __init__(self,bytes=None,offset=0,py_str=None):
-        if bytes:
-            self.string=None
-            self.bytes=bytes
-            self.length=int(unpack_from('i',bytes,offset)[0])
-            self.offset=offset+4
-            self._unpack()
-            self.byte_length=calcsize('i')+self.length*calcsize('s')
-        elif isinstance(py_str,str):
-            self.string=py_str
-            self.bytes=self.to_b()
-        else:
-            raise Exception("no bytes nor str")
-    
-    def _unpack(self):
-        fmt=str(self.length)+'s'
-        self.string=str(unpack_from(fmt,self.bytes,self.offset)[0])[2:-1]
-
-    def to_b(self):
-        byts=pack('i',len(self.string))
-        fmt=str(len(self.string))+'s'
-        byts+=pack(fmt,self.string.encode('utf8'))
-        return byts
-
-class Bdict():
-    '''
-    DICT type
-        int32	: num of key-value pairs
-        // for each key-value pair
-        {
-        STRING	: key
-        STRING	: value
-        }xN
-    '''
-    def __init__(self,bytes=None,offset=0,py_dict=None):
-        if bytes:
-            self.dic={}
-            self.bytes=bytes
-            self.length=int(unpack_from('i', bytes,offset)[0])
-            self.offset=offset+4
-            self._unpack()
-        elif isinstance(py_dict,dict):
-            self.dic=py_dict
-            self.bytes=self.to_b()
-        else:
-            raise Exception("non bytes nor dict")
-        
-    def _unpack(self):
-        for _ in range(self.length):
-            bs1=Bstring(self.bytes,self.offset)
-            key=bs1.string
-            self.offset+=bs1.byte_length
-            bs2=Bstring(self.bytes,self.offset)
-            value=bs2.string
-            self.offset+=bs2.byte_length
-            self.dic[key]=value
-    
-    def to_b(self):
-        byts=pack('i',len(self.dic))
-        for key,value in self.dic.items():
-            byts+=Bstring(py_str=key).bytes
-            byts+=Bstring(py_str=str(value)).bytes
-        return byts
+from ast import Mod
+from collections import namedtuple
+from pprint import pformat
+from struct import unpack_from, calcsize, pack
+
+import numpy as np
+from PIL import Image
+
+from .exceptions import DumpingException
+
+ModelAttr=namedtuple('ModelAttr','attr_dic id')
+default_palette=[
+    0x00000000, 0xffffffff, 0xffccffff, 0xff99ffff, 0xff66ffff, 0xff33ffff, 0xff00ffff, 0xffffccff, 0xffccccff, 0xff99ccff, 0xff66ccff, 0xff33ccff, 0xff00ccff, 0xffff99ff, 0xffcc99ff, 0xff9999ff,
+    0xff6699ff, 0xff3399ff, 0xff0099ff, 0xffff66ff, 0xffcc66ff, 0xff9966ff, 0xff6666ff, 0xff3366ff, 0xff0066ff, 0xffff33ff, 0xffcc33ff, 0xff9933ff, 0xff6633ff, 0xff3333ff, 0xff0033ff, 0xffff00ff,
+    0xffcc00ff, 0xff9900ff, 0xff6600ff, 0xff3300ff, 0xff0000ff, 0xffffffcc, 0xffccffcc, 0xff99ffcc, 0xff66ffcc, 0xff33ffcc, 0xff00ffcc, 0xffffcccc, 0xffcccccc, 0xff99cccc, 0xff66cccc, 0xff33cccc,
+    0xff00cccc, 0xffff99cc, 0xffcc99cc, 0xff9999cc, 0xff6699cc, 0xff3399cc, 0xff0099cc, 0xffff66cc, 0xffcc66cc, 0xff9966cc, 0xff6666cc, 0xff3366cc, 0xff0066cc, 0xffff33cc, 0xffcc33cc, 0xff9933cc,
+    0xff6633cc, 0xff3333cc, 0xff0033cc, 0xffff00cc, 0xffcc00cc, 0xff9900cc, 0xff6600cc, 0xff3300cc, 0xff0000cc, 0xffffff99, 0xffccff99, 0xff99ff99, 0xff66ff99, 0xff33ff99, 0xff00ff99, 0xffffcc99,
+    0xffcccc99, 0xff99cc99, 0xff66cc99, 0xff33cc99, 0xff00cc99, 0xffff9999, 0xffcc9999, 0xff999999, 0xff669999, 0xff339999, 0xff009999, 0xffff6699, 0xffcc6699, 0xff996699, 0xff666699, 0xff336699,
+    0xff006699, 0xffff3399, 0xffcc3399, 0xff993399, 0xff663399, 0xff333399, 0xff003399, 0xffff0099, 0xffcc0099, 0xff990099, 0xff660099, 0xff330099, 0xff000099, 0xffffff66, 0xffccff66, 0xff99ff66,
+    0xff66ff66, 0xff33ff66, 0xff00ff66, 0xffffcc66, 0xffcccc66, 0xff99cc66, 0xff66cc66, 0xff33cc66, 0xff00cc66, 0xffff9966, 0xffcc9966, 0xff999966, 0xff669966, 0xff339966, 0xff009966, 0xffff6666,
+    0xffcc6666, 0xff996666, 0xff666666, 0xff336666, 0xff006666, 0xffff3366, 0xffcc3366, 0xff993366, 0xff663366, 0xff333366, 0xff003366, 0xffff0066, 0xffcc0066, 0xff990066, 0xff660066, 0xff330066,
+    0xff000066, 0xffffff33, 0xffccff33, 0xff99ff33, 0xff66ff33, 0xff33ff33, 0xff00ff33, 0xffffcc33, 0xffcccc33, 0xff99cc33, 0xff66cc33, 0xff33cc33, 0xff00cc33, 0xffff9933, 0xffcc9933, 0xff999933,
+    0xff669933, 0xff339933, 0xff009933, 0xffff6633, 0xffcc6633, 0xff996633, 0xff666633, 0xff336633, 0xff006633, 0xffff3333, 0xffcc3333, 0xff993333, 0xff663333, 0xff333333, 0xff003333, 0xffff0033,
+    0xffcc0033, 0xff990033, 0xff660033, 0xff330033, 0xff000033, 0xffffff00, 0xffccff00, 0xff99ff00, 0xff66ff00, 0xff33ff00, 0xff00ff00, 0xffffcc00, 0xffcccc00, 0xff99cc00, 0xff66cc00, 0xff33cc00,
+    0xff00cc00, 0xffff9900, 0xffcc9900, 0xff999900, 0xff669900, 0xff339900, 0xff009900, 0xffff6600, 0xffcc6600, 0xff996600, 0xff666600, 0xff336600, 0xff006600, 0xffff3300, 0xffcc3300, 0xff993300,
+    0xff663300, 0xff333300, 0xff003300, 0xffff0000, 0xffcc0000, 0xff990000, 0xff660000, 0xff330000, 0xff0000ee, 0xff0000dd, 0xff0000bb, 0xff0000aa, 0xff000088, 0xff000077, 0xff000055, 0xff000044,
+    0xff000022, 0xff000011, 0xff00ee00, 0xff00dd00, 0xff00bb00, 0xff00aa00, 0xff008800, 0xff007700, 0xff005500, 0xff004400, 0xff002200, 0xff001100, 0xffee0000, 0xffdd0000, 0xffbb0000, 0xffaa0000,
+    0xff880000, 0xff770000, 0xff550000, 0xff440000, 0xff220000, 0xff110000, 0xffeeeeee, 0xffdddddd, 0xffbbbbbb, 0xffaaaaaa, 0xff888888, 0xff777777, 0xff555555, 0xff444444, 0xff222222, 0xff111111
+]
+
+
+class XYZI():
+    '''
+    Chunk id 'XYZI' : model voxels, paired with the SIZE chunk
+    -------------------------------------------------------------------------------
+    Bytes  | Type       | Value
+    -------------------------------------------------------------------------------
+    4        | int        | numVoxels (N)
+    4 x N    | int        | (x, y, z, colorIndex) : 1 byte for each component
+    -------------------------------------------------------------------------------
+    '''
+    id=b'XYZI'
+    def __init__(self,xyzi_arr):
+        self.xyzi=xyzi_arr
+        pass
+    
+    def to_b(self):
+        length=len(self.xyzi)
+        bstr=pack('i',length)
+        for i in self.xyzi:
+            bstr+=pack('4B',i[0],i[1],i[2],i[3])
+        return bstr
+
+class SIZE():
+    '''
+     Chunk id 'SIZE' : model size
+    -------------------------------------------------------------------------------
+    Bytes  | Type       | Value
+    -------------------------------------------------------------------------------
+    4        | int        | size x
+    4        | int        | size y
+    4        | int        | size z : gravity direction
+    -------------------------------------------------------------------------------
+    '''
+    id=b'SIZE'
+    def __init__(self,shape):
+        self.size=shape[:-1]
+    def to_b(self):
+        return pack('3i',self.size[0],self.size[1],self.size[2])
+
+class RGBA():
+    '''
+    Chunk id 'RGBA' : palette
+    -------------------------------------------------------------------------------
+    Bytes  | Type       | Value
+    -------------------------------------------------------------------------------
+    4 x 256  | int        | (R, G, B, A) : 1 byte for each component
+                        | * <NOTICE>
+                        | * color [0-254] are mapped to palette index [1-255], e.g : 
+                        | 
+                        | for ( int i = 0; i <= 254; i++ ) {
+                        |     palette[i + 1] = ReadRGBA(); 
+                        | }
+    -------------------------------------------------------------------------------
+    '''
+    id=b'RGBA'
+    def __init__(self,img_path=None,palette_arr=None):
+        if palette_arr:
+            self.palette_arr=palette_arr
+        else:
+            self.palette_arr=self._get_palette_arr_from_img(img_path)
+        pass
+
+    def _get_palette_arr_from_img(self,img_path):
+        img=Image.open(img_path)
+        color=np.array(img)
+        return color[0]
+    
+    def to_b(self):
+        bstr=b''
+        for i in self.palette_arr:
+            bstr+=pack('4B',i[0],i[1],i[2],i[3])
+        return bstr
+
+
+class nTRN():
+    '''
+    Transform Node Chunk : "nTRN"
+
+    int32	: node id
+    DICT	: node attributes
+        (_name : string)
+        (_hidden : 0/1)
+    int32 	: child node id
+    int32 	: reserved id (must be -1)
+    int32	: layer id
+    int32	: num of frames (must be greater than 0)
+
+    // for each frame
+    {
+    DICT	: frame attributes
+        (_r : int8)    ROTATION, see (c)
+        (_t : int32x3) translation
+        (_f : int32)   frame index, start from 0 
+    }xN
+    '''
+    id=b'nTRN'
+    def __init__(self,node_id,node_attributes,
+    child_node_id,reversed_id,layer_id,frames):
+        self.node_id=node_id
+        self.node_attributes=node_attributes
+        self.child_node_id=child_node_id
+        self.reversed_id=reversed_id
+        self.layer_id=layer_id
+        self.frames=frames
+    
+    def to_b(self):
+        byts=pack('i',self.node_id)
+        byts+=Bdict(py_dict=self.node_attributes).bytes
+        byts+=pack('4i',self.child_node_id,
+                        self.reversed_id,
+                        self.layer_id,
+                        len(self.frames))
+        for frame in self.frames:
+            byts+=Bdict(py_dict=frame).bytes
+        return byts
+
+    def __repr__(self):
+        ret=f'''
+====nTRN====
+node_id:{self.node_id}
+frames:{format(self.frames)}
+child_node_id:{self.child_node_id}
+layer_id:{self.layer_id}
+'''
+        return ret
+
+class NGRP():
+    '''
+    Group Node Chunk : "nGRP" 
+    int32	: node id
+    DICT	: node attributes
+    int32 	: num of children nodes
+
+    // for each child
+    {
+    int32	: child node id
+    }xN
+    '''
+    def __init__(self,node_id,dic,num,child_lst):
+        self.node_id=node_id
+        self.node_attr=dic
+        self.children_num=num
+        self.children_ids=child_lst
+        pass
+    def __repr__(self):
+        ret=f'''
+====nGPR====
+node_id:{self.node_id}
+children_ids:{self.children_ids}
+'''
+        return ret
+
+
+class nSHP():
+    '''
+    Shape Node Chunk : "nSHP" 
+
+    int32	: node id
+    DICT	: node attributes
+    int32 	: num of models (must be greater than 0)
+
+    // for each model
+    {
+    int32	: model id
+    DICT	: model attributes : reserved
+        (_f : int32)   frame index, start from 0
+    }xN
+    '''
+    def __init__(self,node_id,models,node_attr={}):
+        self.node_id=node_id
+        self.node_attr=node_attr
+        self.models=models
+    def __repr__(self):
+        ret=f'''
+====nSHP====
+node_id:{self.node_id}
+models:{pformat([i for i in self.models])}
+'''
+        return ret
+    def to_b(self):
+        byts=pack('i',self.node_id)
+        byts+=Bdict(py_dict=self.node_attr).bytes
+        byts+=pack('i',len(self.models))
+        for model in self.models:
+            byts+=pack('i',model.id)
+            byts+=Bdict(py_dict=model.attr_dic)
+        return byts
+
+class Material():
+    '''
+    Material Chunk : "MATL"
+        int32	: material id
+        DICT	: material properties
+            (_type : str) _diffuse, _metal, _glass, _emit
+            (_weight : float) range 0 ~ 1
+            (_rough : float)
+            (_spec : float)
+            (_ior : float)
+            (_att : float)
+            (_flux : float)
+            (_plastic)
+    '''
+    def __init__(self,id,dic):
+        self.id=id
+        self.dic=dic
+        pass
+
+    def __str__(self):
+        return str({'id':self.id,
+                'properties':self.dic
+                })
+
+class Camera():
+    '''
+    Render Camera Chunk : "rCAM"
+        int32	: camera id
+        DICT	: camera attribute
+            (_mode : string)
+            (_focus : vec(3))
+            (_angle : vec(3))
+            (_radius : int)
+            (_frustum : float)
+            (_fov : int)
+    '''
+    def __init__(self,id,dic):
+        self.id=id
+        self.dic=dic
+        pass
+
+    def __str__(self):
+        return str({'id':self.id,
+                'attributes':self.dic
+                })
+
+class Layer():
+    '''
+    Layer Chunk : "LAYR"
+        int32	: layer id
+        DICT	: layer attribute
+            (_name : string)
+            (_hidden : 0/1)
+        int32	: reserved id, must be -1
+    '''
+    def __init__(self,id,dic,rev_id):
+        self.id=id
+        self.dic=dic
+        self.rev_id=rev_id
+
+class Note():
+    '''
+    Palette Note Chunk : "NOTE"
+        int32	: num of color names
+
+        // for each name
+        {
+        STRING	: color name
+        }xN
+    '''
+    def __init__(self,num,color_names):
+        self.num=num
+        self.color_names=color_names
+
+class ROBJ():
+    '''
+    Render Objects Chunk : "rOBJ"
+        DICT	: rendering attributes
+    '''
+    def __init__(self,dic):
+        self.dic=dic
+    
+    def __str__(self):
+        return str(self.dic)
+
+class Bstring():
+    '''
+    STRING type
+        int32   : buffer size (in bytes)
+        int8xN	: buffer (without the ending "\0")
+    '''
+    def __init__(self,bytes=None,offset=0,py_str=None):
+        if bytes:
+            self.string=None
+            self.bytes=bytes
+            self.length=int(unpack_from('i',bytes,offset)[0])
+            self.offset=offset+4
+            self._unpack()
+            self.byte_length=calcsize('i')+self.length*calcsize('s')
+        elif isinstance(py_str,str):
+            self.string=py_str
+            self.bytes=self.to_b()
+        else:
+            raise Exception("no bytes nor str")
+    
+    def _unpack(self):
+        fmt=str(self.length)+'s'
+        self.string=str(unpack_from(fmt,self.bytes,self.offset)[0])[2:-1]
+
+    def to_b(self):
+        byts=pack('i',len(self.string))
+        fmt=str(len(self.string))+'s'
+        byts+=pack(fmt,self.string.encode('utf8'))
+        return byts
+
+class Bdict():
+    '''
+    DICT type
+        int32	: num of key-value pairs
+        // for each key-value pair
+        {
+        STRING	: key
+        STRING	: value
+        }xN
+    '''
+    def __init__(self,bytes=None,offset=0,py_dict=None):
+        if bytes:
+            self.dic={}
+            self.bytes=bytes
+            self.length=int(unpack_from('i', bytes,offset)[0])
+            self.offset=offset+4
+            self._unpack()
+        elif isinstance(py_dict,dict):
+            self.dic=py_dict
+            self.bytes=self.to_b()
+        else:
+            raise Exception("non bytes nor dict")
+        
+    def _unpack(self):
+        for _ in range(self.length):
+            bs1=Bstring(self.bytes,self.offset)
+            key=bs1.string
+            self.offset+=bs1.byte_length
+            bs2=Bstring(self.bytes,self.offset)
+            value=bs2.string
+            self.offset+=bs2.byte_length
+            self.dic[key]=value
+    
+    def to_b(self):
+        byts=pack('i',len(self.dic))
+        for key,value in self.dic.items():
+            byts+=Bstring(py_str=key).bytes
+            byts+=Bstring(py_str=str(value)).bytes
+        return byts
```

### Comparing `midvoxio-0.1.0/src/pyvox/parser.py` & `midvoxio-0.1.1/src/midvoxio/parser.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from struct import unpack_from, calcsize
-import logging
-logging.basicConfig(level=logging.WARNING,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')
-
-
-from .config import *
-from .exceptions import ParsingException
-from .vox import Chunk,Vox
-
-class Parser():
-
-    def __init__(self,fname=None,bcontent=None):
-        with open(fname, 'rb') as f:
-            self.content = f.read()
-        
-        if bcontent:
-            self.content=bcontent
-        self.offset=0
-        pass
-
-    def unpack(self, fmt):
-        r = unpack_from(fmt, self.content, self.offset)
-        self.offset += calcsize(fmt)
-        return r
-    
-    def _parseChunk(self):
-    
-        _id, N, M = self.unpack(CHUNK_FMT)
-
-        content = self.unpack('%ds'%N)[0]
-
-        start = self.offset
-        chunks = [ ]
-        while self.offset<start+M:
-            chunks.append(self._parseChunk())
-
-        return Chunk(_id, content, chunks)
-
-    def parse(self):
-        header, version = self.unpack(VOX_FMT)
-        if header != VOX_HEADER: 
-            raise ParsingException("Not a vox file")
-        if version != VOX_VERSION: 
-            raise ParsingException("Unknown vox version: %s expected %s"%(version,VOX_VERSION))
-        main=self._parseChunk()
-        if main.id != b'MAIN': raise ParsingException("Missing MAIN Chunk")
-        chunks:list[Chunk]=list(main.children)
-            
-        return Vox(chunks)
-
-
+from struct import unpack_from, calcsize
+import logging
+logging.basicConfig(level=logging.WARNING,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')
+
+
+from .config import *
+from .exceptions import ParsingException
+from .vox import Chunk,Vox
+
+class Parser():
+
+    def __init__(self,fname=None,bcontent=None):
+        with open(fname, 'rb') as f:
+            self.content = f.read()
+        
+        if bcontent:
+            self.content=bcontent
+        self.offset=0
+        pass
+
+    def unpack(self, fmt):
+        r = unpack_from(fmt, self.content, self.offset)
+        self.offset += calcsize(fmt)
+        return r
+    
+    def _parseChunk(self):
+    
+        _id, N, M = self.unpack(CHUNK_FMT)
+
+        content = self.unpack('%ds'%N)[0]
+
+        start = self.offset
+        chunks = [ ]
+        while self.offset<start+M:
+            chunks.append(self._parseChunk())
+
+        return Chunk(_id, content, chunks)
+
+    def parse(self):
+        header, version = self.unpack(VOX_FMT)
+        if header != VOX_HEADER: 
+            raise ParsingException("Not a vox file")
+        if version != VOX_VERSION: 
+            raise ParsingException("Unknown vox version: %s expected %s"%(version,VOX_VERSION))
+        main=self._parseChunk()
+        if main.id != b'MAIN': raise ParsingException("Missing MAIN Chunk")
+        chunks:list[Chunk]=list(main.children)
+            
+        return Vox(chunks)
+
+
     pass
```

### Comparing `midvoxio-0.1.0/src/pyvox/vox.py` & `midvoxio-0.1.1/src/midvoxio/vox.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-from struct import unpack_from
-import logging
-logging.basicConfig(level=logging.WARNING,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')
-
-import numpy as np
-
-from .config import *
-from .exceptions import AssigningException, ParsingException
-from .models import *
-
-class Chunk():
-    
-    def __init__(self,id,content=None,children=None):
-        self.id = id
-        self.name = str(id)[2:-1]
-        self.content = content or b''
-        self.children = children or []
-        self.offset=0
-        self._parse()
-    
-    def _parse(self):
-
-        if self.id == b'MAIN':
-            if len(self.content):
-                raise ParsingException('Empty main chunk')
-        
-        elif self.id == b'PACK':
-            logging.debug('Detect Pack chunk which is not supportted in current version, skip now')
-        
-        elif self.id == b'SIZE':
-            self.size=unpack_from(SIZE_FMT,self.content,0)
-
-        elif self.id == b'XYZI':
-            n = int(unpack_from(XYZI_FMT_1,self.content,0)[0])
-            self.voxels = []
-            for i in range(n):
-                self.voxels.append(unpack_from(XYZI_FMT_2, self.content, 4+4*i))
-
-        elif self.id == b'RGBA':
-            self.palette=[]
-            for i in range(255):
-                self.palette.append(unpack_from(RGBA_FMT, self.content, 4*i))
-
-        elif self.id == b'MATL':
-            _id = unpack_from('i', self.content)
-            _dict = Bdict(self.content,4).dic
-            self.material=Material(_id,_dict)
-
-        elif self.id == b'nTRN':
-            _id = int(unpack_from('i', self.content)[0])
-            frames = []
-            bdict = Bdict(self.content,4)
-            (c_id,r_id,l_id,frames_num)=unpack_from('iiii', self.content,bdict.offset)
-            offset=16+bdict.offset
-            for i in range(frames_num):
-                _bdict=Bdict(self.content,offset)
-                frames.append(_bdict.dic)
-                offset=_bdict.offset
-            self.ntrn=nTRN(_id,bdict.dic,c_id,r_id,l_id,frames)
-            
-        elif self.id == b'rOBJ':
-            self.robj = ROBJ(Bdict(self.content).dic)
-            
-        elif self.id == b'nGRP':
-            _node_id = int(unpack_from('i', self.content)[0])
-            bdict=Bdict(self.content,4)
-            _node_attr = bdict.dic
-            children_num = int(unpack_from('i', self.content,bdict.offset)[0])
-            child_ids = []
-            offset=bdict.offset+4
-            for i in range(children_num):
-                child_ids.append(int(unpack_from('i',self.content,offset+4*i)[0]))
-            self.ngrp=NGRP(_node_id,_node_attr,children_num,child_ids)
-
-        elif self.id == b'nSHP':
-            _node_id = int(unpack_from('i', self.content)[0])
-            bdict=Bdict(self.content,4)
-            _node_attr = bdict.dic
-            model_num = int(unpack_from('i', self.content,bdict.offset)[0])
-            models=[]
-            offset=bdict.offset+4
-            for i in range(model_num):
-                _id=int(unpack_from('i',self.content,offset)[0])
-                _bdict=Bdict(self.content,offset+4)
-                _attr_dic=_bdict.dic
-                offset=_bdict.offset
-                mod=ModelAttr(attr_dic=_attr_dic,id=_id)
-                models.append(mod)
-            self.nshp=nSHP(_node_id,models,node_attr=_node_attr)
-
-        elif self.id == b'LAYR':
-            _id = unpack_from('i', self.content)
-            bdic=Bdict(self.content,4)
-            _rev_id = unpack_from('i',self.content,bdic.offset)
-            self.layer=Layer(_id,bdic.dic,_rev_id)
-
-        elif self.id == b'rCAM':
-            _id = unpack_from('i', self.content)
-            _dict = Bdict(self.content,4).dic
-            self.camera=Camera(_id,_dict)
-
-        elif self.id == b'NOTE':
-            num = int(unpack_from('i', self.content)[0])
-            _name_list=[]
-            offset=4
-            for i in range(num):
-                bstr=Bstring(self.content,offset)
-                offset+=bstr.byte_length
-                _name_list.append(bstr.string)
-
-            self.palette_note=Note(num,_name_list)
-
-        elif self.id == b'IMAP':
-            pass
-
-
-        else:
-            raise ParsingException('Unknown chunk type: %s'%self.id)
-
-class Vox():
-
-    def __init__(self,chunks):
-        self.chunks=chunks
-        self.palettes = []
-        self.sizes = []
-        self.voxels = []
-        self.materials = []
-        self.robjs=[]
-        self.layers=[]
-        self.ngrps=[]
-        self.ntrns=[]
-        self.nshps=[]
-        self.cameras=[]
-        self.palette_notes=[]
-        self._parse_chunk()
-        if len(self.palettes)==0:
-            self.palettes.append(default_palette)
-        self._trans(self._get_transform())
-        pass
-
-    def _trans(self,transforms):
-
-        if len(transforms)!=len(self.voxels):
-            print(f'_t in nTRN not match models, transform not applied')
-            return
-        
-        # calcualte the size of the combined moduel
-        tran=[]
-        for i in transforms:
-            tran.append(i[0])
-        tran=np.array(tran).transpose()
-        sizes=np.array(self.sizes).transpose()
-        x=max(sizes[0])+max(tran[0].tolist())-min(tran[0].tolist())
-        y=max(sizes[1])+max(tran[1].tolist())-min(tran[1].tolist())
-        z=max(sizes[2])+max(tran[2].tolist())-min(tran[2].tolist())
-        combined_size=(x,y,z)
-        self.sizes.append(combined_size)
-
-        # combine models
-        combined_voxel=[]
-        for trans,voxel in zip(transforms,self.voxels):
-            for sv in voxel:
-                combined_voxel.append((
-                    sv[0]+trans[0][0]-min(tran[0].tolist()),
-                    sv[1]+trans[0][1]-min(tran[1].tolist()),
-                    sv[2]+trans[0][2]-min(tran[2].tolist()),
-                    sv[3]))
-        self.voxels.append(combined_voxel)
-
-
-    def _get_transform(self,frame_index=0):
-        '''
-        the function returns ([x,y,z],model_id)
-        '''
-        trn:nTRN
-        shp:nSHP
-        trlinks=[]
-        for trn in self.ntrns:
-            for shp in self.nshps:
-                if trn.child_node_id==shp.node_id:
-                    try:
-                        trn.frames[frame_index]['_t']
-                    except KeyError:
-                        trn.frames[frame_index]['_t']='0 0 0'
-                        raise Exception
-                    except:
-                        raise Exception
-                    for model in shp.models:
-                        trlinks.append((
-                            [int(i) for i in trn.frames[frame_index]['_t'].split()],
-                            model.id))
-        return trlinks
-    
-    def _parse_chunk(self):
-        for chunk in self.chunks:
-            chunk:Chunk
-            if chunk.id==b'RGBA':
-                self.palettes.append(chunk.palette)
-            elif chunk.id==b'SIZE':
-                self.sizes.append(chunk.size)
-            elif chunk.id==b'XYZI':
-                self.voxels.append(chunk.voxels)
-            elif chunk.id==b"LAYR":
-                self.layers.append(chunk.layer)
-            elif chunk.id==b'MATL':
-                self.materials.append(chunk.material)
-            elif chunk.id==b'rOBJ':
-                self.robjs.append(chunk.robj)
-            elif chunk.id==b'nTRN':
-                self.ntrns.append(chunk.ntrn)
-            elif chunk.id==b'nGRP':
-                self.ngrps.append(chunk.ngrp)
-            elif chunk.id==b'nSHP':
-                self.nshps.append(chunk.nshp)
-            elif chunk.id==b'rCAM':
-                self.cameras.append(chunk.camera)
-            elif chunk.id==b'NOTE':
-                self.palette_notes.append(chunk.palette_note)
-
-
-    def to_list(self,vox_index=0,palette_index=0):
-        l,w,h=self.sizes[vox_index]
-        arr=np.zeros((l,w,h,4))
-        color=np.array(self.palettes[palette_index])
-        for i in self.voxels[vox_index]:
-            x=i[0]
-            y=i[1]
-            z=i[2]
-            c=i[3]
-            arr[x,y,z]=color[c-1]/255
+from struct import unpack_from
+import logging
+logging.basicConfig(level=logging.WARNING,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')
+
+import numpy as np
+
+from .config import *
+from .exceptions import AssigningException, ParsingException
+from .models import *
+
+class Chunk():
+    
+    def __init__(self,id,content=None,children=None):
+        self.id = id
+        self.name = str(id)[2:-1]
+        self.content = content or b''
+        self.children = children or []
+        self.offset=0
+        self._parse()
+    
+    def _parse(self):
+
+        if self.id == b'MAIN':
+            if len(self.content):
+                raise ParsingException('Empty main chunk')
+        
+        elif self.id == b'PACK':
+            logging.debug('Detect Pack chunk which is not supportted in current version, skip now')
+        
+        elif self.id == b'SIZE':
+            self.size=unpack_from(SIZE_FMT,self.content,0)
+
+        elif self.id == b'XYZI':
+            n = int(unpack_from(XYZI_FMT_1,self.content,0)[0])
+            self.voxels = []
+            for i in range(n):
+                self.voxels.append(unpack_from(XYZI_FMT_2, self.content, 4+4*i))
+
+        elif self.id == b'RGBA':
+            self.palette=[]
+            for i in range(255):
+                self.palette.append(unpack_from(RGBA_FMT, self.content, 4*i))
+
+        elif self.id == b'MATL':
+            _id = unpack_from('i', self.content)
+            _dict = Bdict(self.content,4).dic
+            self.material=Material(_id,_dict)
+
+        elif self.id == b'nTRN':
+            _id = int(unpack_from('i', self.content)[0])
+            frames = []
+            bdict = Bdict(self.content,4)
+            (c_id,r_id,l_id,frames_num)=unpack_from('iiii', self.content,bdict.offset)
+            offset=16+bdict.offset
+            for i in range(frames_num):
+                _bdict=Bdict(self.content,offset)
+                frames.append(_bdict.dic)
+                offset=_bdict.offset
+            self.ntrn=nTRN(_id,bdict.dic,c_id,r_id,l_id,frames)
+            
+        elif self.id == b'rOBJ':
+            self.robj = ROBJ(Bdict(self.content).dic)
+            
+        elif self.id == b'nGRP':
+            _node_id = int(unpack_from('i', self.content)[0])
+            bdict=Bdict(self.content,4)
+            _node_attr = bdict.dic
+            children_num = int(unpack_from('i', self.content,bdict.offset)[0])
+            child_ids = []
+            offset=bdict.offset+4
+            for i in range(children_num):
+                child_ids.append(int(unpack_from('i',self.content,offset+4*i)[0]))
+            self.ngrp=NGRP(_node_id,_node_attr,children_num,child_ids)
+
+        elif self.id == b'nSHP':
+            _node_id = int(unpack_from('i', self.content)[0])
+            bdict=Bdict(self.content,4)
+            _node_attr = bdict.dic
+            model_num = int(unpack_from('i', self.content,bdict.offset)[0])
+            models=[]
+            offset=bdict.offset+4
+            for i in range(model_num):
+                _id=int(unpack_from('i',self.content,offset)[0])
+                _bdict=Bdict(self.content,offset+4)
+                _attr_dic=_bdict.dic
+                offset=_bdict.offset
+                mod=ModelAttr(attr_dic=_attr_dic,id=_id)
+                models.append(mod)
+            self.nshp=nSHP(_node_id,models,node_attr=_node_attr)
+
+        elif self.id == b'LAYR':
+            _id = unpack_from('i', self.content)
+            bdic=Bdict(self.content,4)
+            _rev_id = unpack_from('i',self.content,bdic.offset)
+            self.layer=Layer(_id,bdic.dic,_rev_id)
+
+        elif self.id == b'rCAM':
+            _id = unpack_from('i', self.content)
+            _dict = Bdict(self.content,4).dic
+            self.camera=Camera(_id,_dict)
+
+        elif self.id == b'NOTE':
+            num = int(unpack_from('i', self.content)[0])
+            _name_list=[]
+            offset=4
+            for i in range(num):
+                bstr=Bstring(self.content,offset)
+                offset+=bstr.byte_length
+                _name_list.append(bstr.string)
+
+            self.palette_note=Note(num,_name_list)
+
+        elif self.id == b'IMAP':
+            pass
+
+
+        else:
+            raise ParsingException('Unknown chunk type: %s'%self.id)
+
+class Vox():
+
+    def __init__(self,chunks):
+        self.chunks=chunks
+        self.palettes = []
+        self.sizes = []
+        self.voxels = []
+        self.materials = []
+        self.robjs=[]
+        self.layers=[]
+        self.ngrps=[]
+        self.ntrns=[]
+        self.nshps=[]
+        self.cameras=[]
+        self.palette_notes=[]
+        self._parse_chunk()
+        if len(self.palettes)==0:
+            self.palettes.append(default_palette)
+        self._trans(self._get_transform())
+        pass
+
+    def _trans(self,transforms):
+
+        if len(transforms)!=len(self.voxels):
+            print(f'_t in nTRN not match models, transform not applied')
+            return
+        
+        # calcualte the size of the combined moduel
+        tran=[]
+        for i in transforms:
+            tran.append(i[0])
+        tran=np.array(tran).transpose()
+        sizes=np.array(self.sizes).transpose()
+        x=max(sizes[0])+max(tran[0].tolist())-min(tran[0].tolist())
+        y=max(sizes[1])+max(tran[1].tolist())-min(tran[1].tolist())
+        z=max(sizes[2])+max(tran[2].tolist())-min(tran[2].tolist())
+        combined_size=(x,y,z)
+        self.sizes.append(combined_size)
+
+        # combine models
+        combined_voxel=[]
+        for trans,voxel in zip(transforms,self.voxels):
+            for sv in voxel:
+                combined_voxel.append((
+                    sv[0]+trans[0][0]-min(tran[0].tolist()),
+                    sv[1]+trans[0][1]-min(tran[1].tolist()),
+                    sv[2]+trans[0][2]-min(tran[2].tolist()),
+                    sv[3]))
+        self.voxels.append(combined_voxel)
+
+
+    def _get_transform(self,frame_index=0):
+        '''
+        the function returns ([x,y,z],model_id)
+        '''
+        trn:nTRN
+        shp:nSHP
+        trlinks=[]
+        for trn in self.ntrns:
+            for shp in self.nshps:
+                if trn.child_node_id==shp.node_id:
+                    try:
+                        trn.frames[frame_index]['_t']
+                    except KeyError:
+                        trn.frames[frame_index]['_t']='0 0 0'
+                        raise Exception
+                    except:
+                        raise Exception
+                    for model in shp.models:
+                        trlinks.append((
+                            [int(i) for i in trn.frames[frame_index]['_t'].split()],
+                            model.id))
+        return trlinks
+    
+    def _parse_chunk(self):
+        for chunk in self.chunks:
+            chunk:Chunk
+            if chunk.id==b'RGBA':
+                self.palettes.append(chunk.palette)
+            elif chunk.id==b'SIZE':
+                self.sizes.append(chunk.size)
+            elif chunk.id==b'XYZI':
+                self.voxels.append(chunk.voxels)
+            elif chunk.id==b"LAYR":
+                self.layers.append(chunk.layer)
+            elif chunk.id==b'MATL':
+                self.materials.append(chunk.material)
+            elif chunk.id==b'rOBJ':
+                self.robjs.append(chunk.robj)
+            elif chunk.id==b'nTRN':
+                self.ntrns.append(chunk.ntrn)
+            elif chunk.id==b'nGRP':
+                self.ngrps.append(chunk.ngrp)
+            elif chunk.id==b'nSHP':
+                self.nshps.append(chunk.nshp)
+            elif chunk.id==b'rCAM':
+                self.cameras.append(chunk.camera)
+            elif chunk.id==b'NOTE':
+                self.palette_notes.append(chunk.palette_note)
+
+
+    def to_list(self,vox_index=0,palette_index=0):
+        l,w,h=self.sizes[vox_index]
+        arr=np.zeros((l,w,h,4))
+        color=np.array(self.palettes[palette_index])
+        for i in self.voxels[vox_index]:
+            x=i[0]
+            y=i[1]
+            z=i[2]
+            c=i[3]
+            arr[x,y,z]=color[c-1]/255
         return arr
```

### Comparing `midvoxio-0.1.0/src/pyvox/voxio.py` & `midvoxio-0.1.1/src/midvoxio/voxio.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-'''
-User API
-'''
-import matplotlib.pylab as plt
-import numpy as np
-
-from .exceptions import DumpingException
-
-from .writer import ArrayWriter, ChunkWriter
-from .parser import Parser
-from .vox import Vox
-
-
-def _get_attr(attr_lst):
-    return [str(i) for i in attr_lst]
-
-def vox_to_arr(fname:str,vox_index=0):
-    '''
-    Return an array of the vox file.
-    fname: path to vox file
-    vox_index: which model to show if there is multiple models
-                index -1 means show all the model to gether
-    '''
-    vox=Parser(fname).parse()
-    return vox.to_list(vox_index)
-
-def viz_vox(fname:str,vox_index=0):
-    '''
-    Viz vox file by using matplotlib
-    fname: path to vox file
-    vox_index: which model to show if there is multiple models
-                index -1 means show all the model to gether
-    '''
-    arr=vox_to_arr(fname,vox_index)
-    plot_3d(arr)
-
-def show_chunks(fname:str):
-    '''
-    print chunk names of all chuncks in the vox file
-    '''
-    vox=Parser(fname).parse()
-    print([i.name for i in vox.chunks])
-
-def get_rendering_attributes(fname:str):
-    '''
-    return all redering attributes of a vox file
-    '''
-    vox=Parser(fname).parse()
-    return _get_attr(vox.robjs)
-
-def get_materials(fname:str):
-    '''
-    return all material attributes of a vox file
-    '''
-    vox=Parser(fname).parse()
-    return _get_attr(vox.materials)
-
-def get_cameras(fname:str):
-    '''
-    return all cameras attributes of a vox file
-    '''
-    vox=Parser(fname).parse()
-    return _get_attr(vox.cameras)
-
-def get_vox(fname:str) -> Vox:
-    '''
-    return a Vox class of the vox file
-    '''
-    return Parser(fname).parse()
-
-def write_list_to_vox(arr,vox_fname:str,palette_path=None,palette_arr=None):
-    '''
-    dump and write an arr into vox file
-    arr: python list or numpy array that contains voxel information
-    vox_fname: the name of created vox file
-    palette_path: if you want to use your own palette
-    palette_arr: if you want to use your own palette
-    '''
-    if palette_arr:
-        t=ArrayWriter(arr,palette_arr=palette_arr)
-    elif palette_path:
-        t=ArrayWriter(arr,palette_path=palette_path)
-    else:
-        raise DumpingException("missing the required palette")
-    t.write(vox_fname)
-
-def plot_3d(arr):
-    '''
-    plot vox array
-    '''
-    fig = plt.figure()
-    ax = fig.add_subplot(projection='3d')
-    u = np.moveaxis(arr, (0, 1), (0, 1))
-    m = ax.voxels((u[:, :, :, 3] > 0.1), facecolors=np.clip(u[:, :, :, :4], 0, 1))
-    plt.show()
+'''
+User API
+'''
+import matplotlib.pylab as plt
+import numpy as np
+
+from .exceptions import DumpingException
+
+from .writer import ArrayWriter, ChunkWriter
+from .parser import Parser
+from .vox import Vox
+
+
+def _get_attr(attr_lst):
+    return [str(i) for i in attr_lst]
+
+def vox_to_arr(fname:str,vox_index=0):
+    '''
+    Return an array of the vox file.
+    fname: path to vox file
+    vox_index: which model to show if there is multiple models
+                index -1 means show all the model to gether
+    '''
+    vox=Parser(fname).parse()
+    return vox.to_list(vox_index)
+
+def viz_vox(fname:str,vox_index=0):
+    '''
+    Viz vox file by using matplotlib
+    fname: path to vox file
+    vox_index: which model to show if there is multiple models
+                index -1 means show all the model to gether
+    '''
+    arr=vox_to_arr(fname,vox_index)
+    plot_3d(arr)
+
+def show_chunks(fname:str):
+    '''
+    print chunk names of all chuncks in the vox file
+    '''
+    vox=Parser(fname).parse()
+    print([i.name for i in vox.chunks])
+
+def get_rendering_attributes(fname:str):
+    '''
+    return all redering attributes of a vox file
+    '''
+    vox=Parser(fname).parse()
+    return _get_attr(vox.robjs)
+
+def get_materials(fname:str):
+    '''
+    return all material attributes of a vox file
+    '''
+    vox=Parser(fname).parse()
+    return _get_attr(vox.materials)
+
+def get_cameras(fname:str):
+    '''
+    return all cameras attributes of a vox file
+    '''
+    vox=Parser(fname).parse()
+    return _get_attr(vox.cameras)
+
+def get_vox(fname:str) -> Vox:
+    '''
+    return a Vox class of the vox file
+    '''
+    return Parser(fname).parse()
+
+def write_list_to_vox(arr,vox_fname:str,palette_path=None,palette_arr=None):
+    '''
+    dump and write an arr into vox file
+    arr: python list or numpy array that contains voxel information
+    vox_fname: the name of created vox file
+    palette_path: if you want to use your own palette
+    palette_arr: if you want to use your own palette
+    '''
+    if palette_arr:
+        t=ArrayWriter(arr,palette_arr=palette_arr)
+    elif palette_path:
+        t=ArrayWriter(arr,palette_path=palette_path)
+    else:
+        raise DumpingException("missing the required palette")
+    t.write(vox_fname)
+
+def plot_3d(arr):
+    '''
+    plot vox array
+    '''
+    fig = plt.figure()
+    ax = fig.add_subplot(projection='3d')
+    u = np.moveaxis(arr, (0, 1), (0, 1))
+    m = ax.voxels((u[:, :, :, 3] > 0.1), facecolors=np.clip(u[:, :, :, :4], 0, 1))
+    plt.show()
     plt.close()
```

### Comparing `midvoxio-0.1.0/LICENSE` & `midvoxio-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 midstreeeam
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 midstreeeam
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `midvoxio-0.1.0/README.md` & `midvoxio-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,90 @@
-# PyVox
-The python IO for [magical voxel](https://ephtracy.github.io/)'s [.vox format](https://github.com/ephtracy/voxel-model).
-
-
-## Install
-- clone the repo
-- add the repo to path
-- Install numpy and matplotlib if you haven't
-
-## Usage
-#### vox_to_arr()
-use `vox_to_arr()` to parse .vox file into numpy array.
-```Python
-from voxio import vox_to_arr
-
-print(vox_to_arr('vox/99/3x3x3.vox').shape)
-```
-result:
-```Python
-(3, 3, 3, 4) # the four axis are (x,y,z,color), color is [r,g,b,a] here
-```
-
-
-
-#### viz_vox()
-
-use `viz_vox()` to visualize your .vox file. It uses `matplotlib` to plot the file internally.
-```Python
-from voxio import viz_vox
-
-viz_vox('vox/99/3x3x3.vox')
-```
-then, the python will give you a 3d plot.
-<img src="/img/3x3x3.jpg" width="25%">
-
-
-
-#### get other info
-
-use `get_rendering_attributes()`,`get_cameras()`, and `get_materials()` to get vox info.
-```Python
->>> from voxio import *
->>> print(get_cameras('vox/99/cars.vox')[0])
-{'id': (0,), 'attributes': {'_mode': 'pers', '_focus': '0 0 0', '_angle': '0 0 0', '_radius': '0', '_frustum': '0.414214', '_fov': '45'}}
->>> print(get_rendering_attributes('vox/99/3x3x3.vox')[0])
-{'_type': '_inf', '_i': '0.6', '_k': '255 255 255', '_angle': '50 50', '_area': '0.07'}
->>> print(get_materials('vox/99/3x3x3.vox')[0])
-{'id': (0,), 'properties': {'_type': '_diffuse', '_weight': '1', '_rough': '0.1', '_spec': '0.5', '_ior': '0.3'}}
-```
-
-
-
-#### write_list_to_vox()
-
-use `write_list_to_vox` to generate vox file from exist python list. You can use this function to export the python list as vox file, so you will be able to edit vox file in python.
-
-```Python
-from voxio import write_list_to_vox,plot_3d
-
-arr=[] # define your python list that represent the 3d model here
-
-# define your palette that relate to your model here
-# palette will be able to be automatically generated in the future
-palette=[]
-
-
-# you can use plotio to viz your arr before you save it to vox
-plot_3d(arr) # visualize your arr
-
-write_list_to_vox(arr,'fname.vox',palette_arr=palette) # then, you save the 'fname.vox'
-
-# you can also use png palette
-palette_path='palette.png'
-write_list_tov_vox(arr,'fname.vox',palette_path) # then, you save the 'fname.vox'
-```
-
-
-
-## Others
-
-- This project was originally created for me to use it myself, so the API design is casual and the error message is not complete. Will consider make it more formal if there are really people using it.
-- Gromgull's [py-vox-io](https://github.com/gromgull/py-vox-io) is good to use, but only for MagicalVoxel 0.98 or older version, and he somehow stop updating. This voxio reuse some of Gromgull's code (mostly in parser), but now it fit MagicalVoxel 0.99. Also, there are also new features like `viz_vox()` to visualize the vox array without using magicalvoxel.
-- Lots of functions are still under development.
+# MidVoxIO
+The python IO for [magical voxel](https://ephtracy.github.io/)'s [.vox format](https://github.com/ephtracy/voxel-model).
+
+
+## Install
+
+### pip
+```
+pip install midvoxio
+```
+
+### through repo
+- clone the repo
+- add the repo to path
+- Install numpy and matplotlib if you haven't
+
+## Usage
+#### vox_to_arr()
+use `vox_to_arr()` to parse .vox file into numpy array.
+```Python
+from voxio import vox_to_arr
+
+print(vox_to_arr('vox/99/3x3x3.vox').shape)
+```
+result:
+```Python
+(3, 3, 3, 4) # the four axis are (x,y,z,color), color is [r,g,b,a] here
+```
+
+
+
+#### viz_vox()
+
+use `viz_vox()` to visualize your .vox file. It uses `matplotlib` to plot the file internally.
+```Python
+from voxio import viz_vox
+
+viz_vox('vox/99/3x3x3.vox')
+```
+then, the python will give you a 3d plot.
+<img src="/img/3x3x3.jpg" width="25%">
+
+
+
+#### get other info
+
+use `get_rendering_attributes()`,`get_cameras()`, and `get_materials()` to get vox info.
+```Python
+>>> from voxio import *
+>>> print(get_cameras('vox/99/cars.vox')[0])
+{'id': (0,), 'attributes': {'_mode': 'pers', '_focus': '0 0 0', '_angle': '0 0 0', '_radius': '0', '_frustum': '0.414214', '_fov': '45'}}
+>>> print(get_rendering_attributes('vox/99/3x3x3.vox')[0])
+{'_type': '_inf', '_i': '0.6', '_k': '255 255 255', '_angle': '50 50', '_area': '0.07'}
+>>> print(get_materials('vox/99/3x3x3.vox')[0])
+{'id': (0,), 'properties': {'_type': '_diffuse', '_weight': '1', '_rough': '0.1', '_spec': '0.5', '_ior': '0.3'}}
+```
+
+
+
+#### write_list_to_vox()
+
+use `write_list_to_vox` to generate vox file from exist python list. You can use this function to export the python list as vox file, so you will be able to edit vox file in python.
+
+```Python
+from voxio import write_list_to_vox,plot_3d
+
+arr=[] # define your python list that represent the 3d model here
+
+# define your palette that relate to your model here
+# palette will be able to be automatically generated in the future
+palette=[]
+
+
+# you can use plotio to viz your arr before you save it to vox
+plot_3d(arr) # visualize your arr
+
+write_list_to_vox(arr,'fname.vox',palette_arr=palette) # then, you save the 'fname.vox'
+
+# you can also use png palette
+palette_path='palette.png'
+write_list_tov_vox(arr,'fname.vox',palette_path) # then, you save the 'fname.vox'
+```
+
+
+
+## Others
+
+- This project was originally created for me to use it myself, so the API design is casual and the error message is not complete. Will consider make it more formal if there are really people using it.
+- Gromgull's [py-vox-io](https://github.com/gromgull/py-vox-io) is good to use, but only for MagicalVoxel 0.98 or older version, and he somehow stop updating. This voxio reuse some of Gromgull's code (mostly in parser), but now it fit MagicalVoxel 0.99. Also, there are also new features like `viz_vox()` to visualize the vox array without using magicalvoxel.
+- Lots of functions are still under development.
```

### Comparing `midvoxio-0.1.0/pyproject.toml` & `midvoxio-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "midvoxio"
-version = "0.1.0"
-authors = [
-  { name="Midstream", email="midstream.lou@gmail.com" },
-]
-description = "A python io to load/write/visualize vox files (MagicalVoxel's .vox format)."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-
-[project.urls]
-"Homepage" = "https://github.com/midstreeeam/PyVox"
-"Bug Tracker" = "https://github.com/midstreeeam/PyVox/issues"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "midvoxio"
+version = "0.1.1"
+authors = [
+  { name="Midstream", email="midstream.lou@gmail.com" },
+]
+description = "A python io to load/write/visualize vox files (MagicalVoxel's .vox format)."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+
+[project.urls]
+"Homepage" = "https://github.com/midstreeeam/PyVox"
+"Bug Tracker" = "https://github.com/midstreeeam/PyVox/issues"
```

### Comparing `midvoxio-0.1.0/PKG-INFO` & `midvoxio-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: midvoxio
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python io to load/write/visualize vox files (MagicalVoxel's .vox format).
 Project-URL: Homepage, https://github.com/midstreeeam/PyVox
 Project-URL: Bug Tracker, https://github.com/midstreeeam/PyVox/issues
 Author-email: Midstream <midstream.lou@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# PyVox
+# MidVoxIO
 The python IO for [magical voxel](https://ephtracy.github.io/)'s [.vox format](https://github.com/ephtracy/voxel-model).
 
 
 ## Install
+
+### pip
+```
+pip install midvoxio
+```
+
+### through repo
 - clone the repo
 - add the repo to path
 - Install numpy and matplotlib if you haven't
 
 ## Usage
 #### vox_to_arr()
 use `vox_to_arr()` to parse .vox file into numpy array.
```

