# Comparing `tmp/havoc_clustering-0.0.4.tar.gz` & `tmp/havoc_clustering-0.0.9.tar.gz`

## Comparing `havoc_clustering-0.0.4.tar` & `havoc_clustering-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/__init__.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/correlation_of_dlfv_groups.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/havoc.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/requirements.txt
--rwxr-xr-x   0        0        0     4849 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/image_creator.py
--rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/print_time.py
--rwxr-xr-x   0        0        0     9335 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/slide.py
--rwxr-xr-x   0        0        0     8331 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/tile_image_utils.py
--rwxr-xr-x   0        0        0     1680 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/unique_colors.py
--rwxr-xr-x   0        0        0     1117 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/ai/model_utils.py
--rwxr-xr-x   0        0        0     7220 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/src/havoc_clustering/general_utility/ai/tileextractor.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/LICENSE
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/README.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 havoc_clustering-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/__init__.py
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/correlation_of_dlfv_groups.py
+-rw-r--r--   0        0        0    11472 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/havoc.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/requirements.txt
+-rwxr-xr-x   0        0        0     4849 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/image_creator.py
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/print_time.py
+-rwxr-xr-x   0        0        0     9335 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/slide.py
+-rwxr-xr-x   0        0        0     8331 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/tile_image_utils.py
+-rwxr-xr-x   0        0        0     1680 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/unique_colors.py
+-rwxr-xr-x   0        0        0     1117 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/ai/model_utils.py
+-rwxr-xr-x   0        0        0     7220 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/src/havoc_clustering/general_utility/ai/tileextractor.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/README.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 havoc_clustering-0.0.9/PKG-INFO
```

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/correlation_of_dlfv_groups.py` & `havoc_clustering-0.0.9/src/havoc_clustering/correlation_of_dlfv_groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,74 +4,80 @@
 import itertools
 from scipy.stats import pearsonr
 import seaborn as sns
 import matplotlib.pyplot as plt
 import glob
 import pathlib
 from collections import OrderedDict
+import json
 
 from havoc_clustering.general_utility import unique_colors
 
 
-# pearson coeffcient clustermap of color groups within the csv (single slide hence there will be 1 colortrack)
-# takes in directory with a dump of all the k<k_val> csv's
-def create_correlation_clustermap_single_slide(dir):
-    for fp in glob.glob(os.path.join(dir, '*k[0-9].csv')):
-        slide_name, kval = pathlib.Path(fp).stem.rsplit('_', 1)
+# Pearson coeffcient clustermap of color groups within the csv for the desired k value.
+# There will be 1 colortrack denoting the cluster colors
+# You may specify the folder containing the cluster_info_df csv's generated by HAVOC
+def create_correlation_clustermap_single_slide(dir, target_k=9):
+    for fp in glob.glob(os.path.join(dir, f'*_cluster_info_df.csv')):
+        slide_name = pathlib.Path(fp).stem.split('_cluster_info_df')[0]
 
-        df = pd.read_csv(os.path.join(dir, f'{slide_name}_{kval}.csv'))
+        df = pd.read_csv(fp)
 
-        colors = list(df['Cluster_color_name'].unique())
+        colors = list(df[f'Cluster_color_name_{target_k}'].unique())
 
         df_corr = pd.DataFrame(np.zeros((len(colors), len(colors))))
         df_corr.columns = colors
         df_corr.index = colors
 
         for (c1, c2) in itertools.combinations(colors, 2):
-            df1 = df[df['Cluster_color_name'] == c1]
-            df2 = df[df['Cluster_color_name'] == c2]
-            dlfv_df1 = df1[[str(x) for x in range(1, 513)]]
-            dlfv_df2 = df2[[str(x) for x in range(1, 513)]]
+            df1 = df[df[f'Cluster_color_name_{target_k}'] == c1]
+            df2 = df[df[f'Cluster_color_name_{target_k}'] == c2]
+            dlfv_df1 = df1[[str(x) for x in range(1, 513)]].values
+            dlfv_df2 = df2[[str(x) for x in range(1, 513)]].values
 
             r_coeff = pearsonr(
-                np.mean(dlfv_df1), np.mean(dlfv_df2)
+                dlfv_df1.mean(axis=0), dlfv_df2.mean(axis=0)
             )
 
             df_corr[c1][c2] = r_coeff[0]
             df_corr[c2][c1] = r_coeff[0]
 
         for c in colors:
             df_corr[c][c] = 1
 
         plt.close('all')
-        sns.clustermap(df_corr, annot=True, cmap="Blues")  # , method='ward')
+        g = sns.clustermap(df_corr, annot=True, cmap="Blues", row_colors=colors, yticklabels=False, xticklabels=False)
         # plt.show()
-        plt.savefig(os.path.join(dir, f'{slide_name}_{kval}_corr_clustermap.jpg'), dpi=300)
+        plt.savefig(os.path.join(dir, f'{slide_name}_k{target_k}_corr_clustermap.jpg'), dpi=300)
 
 
-# pearson coeffcient clustermap of color groups within all the csvs in the folder
-# (multi slide hence there will be 2 colortracks: left will be slide and right will be the cluster)
-# takes in directory with a dump of all the k<k_val> csv's
-def create_correlation_clustermap_multi_slide(dir, kval='*'):
-    # choose color to represent ach slide
+# Pearson coeffcient clustermap of color groups within all the csv's for the desired k value.
+# There will be 2 colortracks denoting the slide & cluster color
+# You may specify the folder containing the cluster_info_df csv's generated by HAVOC
+def create_correlation_clustermap_multi_slide(dir, target_k=9):
+    # choose color for a slide
     color_gen = unique_colors.next_color_generator(scaled=True, mode='rgb')
     group_to_color_rgb = {}
     group_to_color_rgb_name = {}
-    for fp in glob.glob(os.path.join(dir, f'*_k{kval}.csv')):
+    for fp in glob.glob(os.path.join(dir, f'*_cluster_info_df.csv')):
+        slide_name = pathlib.Path(fp).stem.split('_cluster_info_df')[0]
         color_ = next(color_gen)
-        group_to_color_rgb[pathlib.Path(fp).stem] = color_['val']
-        group_to_color_rgb_name[pathlib.Path(fp).stem] = color_['name']
+        group_to_color_rgb[slide_name] = color_['val']
+        group_to_color_rgb_name[slide_name] = color_['name']
+
+    print('Found the following slides: ' + str(list(group_to_color_rgb)))
 
     df_mapping = OrderedDict()
     df_mapping_english_keys = []
-    for fp in glob.glob(os.path.join(dir, f'*_k{kval}.csv')):
+    for fp in glob.glob(os.path.join(dir, f'*_cluster_info_df.csv')):
+        slide_name = pathlib.Path(fp).stem.split('_cluster_info_df')[0]
         df = pd.read_csv(fp)
-        for color, rows in df.groupby('Cluster_color_name'):
+        for color, rows in df.groupby(f'Cluster_color_name_{target_k}'):
             df_mapping[
-                (group_to_color_rgb[pathlib.Path(fp).stem], unique_colors.SCALED_RGB_COLORS[color])
+                (group_to_color_rgb[slide_name], unique_colors.SCALED_RGB_COLORS[color])
             ] = rows[[str(x) for x in range(1, 512 + 1)]].mean().values
             # the above mapping has keys as rgb values to work directly with the colortrack. this is human readable
             # version. ie so we can use in df_corr labels to get extracted ordering
             df_mapping_english_keys.append((pathlib.Path(fp).stem, color))
 
     df_corr = pd.DataFrame(np.zeros((len(df_mapping), len(df_mapping))))
     df_corr.columns = df_mapping.keys()
@@ -92,17 +98,16 @@
     df_corr.columns = df_mapping_english_keys
     df_corr.index = df_mapping_english_keys
 
     # NOTE: REQUIRED! sets up the required format
     colors = pd.DataFrame(df_mapping.keys())
     colors = [colors[i] for i in colors.columns]
 
-    g = sns.clustermap(df_corr.values, cmap="Blues", row_colors=colors)
+    g = sns.clustermap(df_corr.values, cmap="Blues", row_colors=colors, yticklabels=False, xticklabels=False)
 
     # plt.show()
-    plt.savefig(os.path.join(dir, 'multi_slide_corr_clustermap.jpg'), dpi=300)
+    plt.savefig(os.path.join(dir, f'multi_slide_k{target_k}_corr_clustermap.jpg'), dpi=300)
 
-    g.data2d.to_csv(os.path.join(dir, 'r_values_df.csv'), index=False)
+    g.data2d.to_csv(os.path.join(dir, f'multi_slide_k{target_k}_r_values_df.csv'), index=False)
 
-    import json
-    with open(os.path.join(dir, 'colortrack_mapping_SLIDE.json'), 'w') as f:
-        json.dump(group_to_color_rgb_name, f, indent=4)
+    with open(os.path.join(dir, f'multi_slide_k{target_k}_colortrack_mapping_SLIDE.json'), 'w') as f:
+        json.dump(group_to_color_rgb_name, f, indent=4)
```

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/havoc.py` & `havoc_clustering-0.0.9/src/havoc_clustering/havoc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
+import shutil
 import cv2
 import ast
 import pathlib
 import numpy as np
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.manifold import TSNE
 import matplotlib.pyplot as plt
 from tensorflow.keras.backend import clear_session
 import matplotlib as mpl
 from scipy.cluster.hierarchy import dendrogram, linkage
 import pandas as pd
+from tensorflow.keras.models import load_model
 
 from havoc_clustering.general_utility.ai.tileextractor import TileExtractor
 from havoc_clustering.general_utility.image_creator import ImageCreator
-from havoc_clustering.general_utility import unique_colors
 from havoc_clustering import correlation_of_dlfv_groups
-
-from tensorflow.keras.models import load_model
 from havoc_clustering.general_utility.ai.model_utils import ModelUtils
+from havoc_clustering.general_utility import unique_colors
+
 
 
 class HAVOC:
 
     def __init__(self, slide, feature_extractor_path, out_dir, tile_size=512, hd_backdrop=False):
 
         self.feature_extractor_path = feature_extractor_path
@@ -52,62 +53,86 @@
             thumbnail = cv2.cvtColor(np.array(thumbnail), cv2.COLOR_RGB2BGR)
             thumbnail = thumbnail[:(te.trimmed_height // thumbnail_factor), :(te.trimmed_width // thumbnail_factor),
                         ...]
             image_creator.image = cv2.resize(thumbnail, image_creator.image.shape[:2][::-1])
 
         self.image_creator = image_creator
 
-    def run(self, k_vals=[9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', save_tiles=False):
-        self.process_dlfvs(min_non_blank_amt, layer_name)
-        self.make_colortile(save_tiles, k_vals)
-        correlation_of_dlfv_groups.create_correlation_clustermap_single_slide(self.out_dir)
+    def run(self, k_vals=[9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', **kwargs):
+
+        save_tiles_k_vals = kwargs['save_tiles_k_vals'] if 'save_tiles_k_vals' in kwargs else ()
+        make_tsne = 'make_tsne' in kwargs
+        make_dendrogram = 'make_dendrogram' in kwargs
+        make_corr_map = 'make_corr_map' in kwargs
+
+        # we save all the tiles to a tmp folder and then copy the tiles into color folders when we do colortiling
+        if not set(save_tiles_k_vals).issubset(k_vals):
+            raise Exception('save_tiles_k_vals must be a subset of k_vals')
+
+        df = self.process_dlfvs(min_non_blank_amt, layer_name, len(save_tiles_k_vals))
+        df['Coor'] = df['Coor'].apply(ast.literal_eval)
 
-    def process_dlfvs(self, min_non_blank_amt, layer_name):
+        for k in k_vals:
+            cluster_info_df = self.create_cluster_info_df(
+                df[[str(x) for x in range(1, 512 + 1)]], k, linkage_method='ward')
+            df = pd.concat([cluster_info_df, df], axis=1)
+
+        df.to_csv(os.path.join(self.out_dir, f'{self.slide.name}_cluster_info_df.csv'), index=None)
+
+        for k in k_vals:
+            if make_dendrogram:
+                self.make_dendrogram(df, target_k=k)
+            if make_tsne:
+                self.make_tsne(df, target_k=k)
+            if make_corr_map:
+                correlation_of_dlfv_groups.create_correlation_clustermap_single_slide(self.out_dir, target_k=k)
+
+            self.create_colortiled_slide(df, target_k=k, save_tiles=k in save_tiles_k_vals)
+
+        if len(save_tiles_k_vals):
+            # done copying to k color folders
+            shutil.rmtree(os.path.join(self.out_dir, 'tiles', 'tmp'))
+
+    def process_dlfvs(self, min_non_blank_amt, layer_name, save_tiles):
         te = TileExtractor(self.slide, self.tile_size)
         gen = te.iterate_tiles2(min_non_blank_amt=min_non_blank_amt, batch_size=4)
 
+        if save_tiles:
+            # we save all the tiles to a tmp folder and then copy the tiles into color folders when we do colortiling
+            pathlib.Path(os.path.join(self.out_dir, 'tiles', 'tmp')).mkdir(parents=True, exist_ok=True)
+
         coors = []
         dlfvs = []
         feat_extractor_model = load_model(self.feature_extractor_path)
         for res in gen:
             tiles, currcoors = res['tiles'], res['coordinates']
             batch = ModelUtils.prepare_images(tiles)
             currdlfvs = np.concatenate(
                 ModelUtils.get_layer_datas(feat_extractor_model, batch, layers=[layer_name]))
             coors.append(currcoors)
             dlfvs.append(currdlfvs)
 
-        self.coors = np.concatenate(coors)
-        self.dlfvs = np.concatenate(dlfvs)
+            if save_tiles:
+                # each iteration contains a batch of tiles
+                for pos in range(len(tiles)):
+                    curr_sp = os.path.join(self.out_dir, 'tiles', 'tmp', str(tuple(currcoors[pos])) + '.jpg')
+                    cv2.imwrite(curr_sp, tiles[pos])
+
+        dlfvs = np.concatenate(dlfvs)
+        coors = np.concatenate(coors)
+
+        scaled_dlfvs = MinMaxScaler(copy=False).fit_transform(dlfvs)
+
+        df = pd.DataFrame(scaled_dlfvs, columns=[str(x) for x in range(1, 512 + 1)])
+        df['Slide'] = [self.slide.name] * len(df)
+        df['Coor'] = [str(x) for x in coors.tolist()]
 
         clear_session()
 
-    def make_colortile(self, save_tiles, k_vals):
-        scaled_convolved_data = MinMaxScaler(copy=False).fit_transform(self.dlfvs)
-
-        # iterating over cluster values
-        for k in k_vals:
-
-            if k > len(self.dlfvs): break
-
-            cluster_info_df = self.create_cluster_info_df(
-                X=scaled_convolved_data,
-                data_labels=[str(x) for x in self.coors.tolist()],
-                k=k,
-                linkage_method='ward'
-            )
-            cluster_info_df['Coor'] = cluster_info_df['DL'].apply(lambda x: ast.literal_eval(x))
-
-            self.make_dendrogram(cluster_info_df)
-            self.make_tsne(cluster_info_df)
-
-            # NOTE: saving the entire file can be large...only do when needed
-            cluster_info_df.to_csv(os.path.join(self.out_dir, '{}_k{}.csv'.format(self.slide.name, k)), index=False)
-
-            self.create_colortiled_slide(cluster_info_df, save_tiles=save_tiles)
+        return df
 
     '''
     Use this when we want to make "good copies". Initialize using thumbnail instead during development/testing 
     '''
 
     def _initialize(self):
         '''
@@ -122,116 +147,126 @@
         for res in te.iterate_tiles2(batch_size=1):
             tile, coor = res['tiles'][0], res['coordinates'][0]
             self.image_creator.add_tile(tile, coor)
 
         print('DONE')
 
     # cluster the data into k groups and assign each a color
-    def create_cluster_info_df(self, X, data_labels, k=7, linkage_method='complete'):
+    def create_cluster_info_df(self, X, k, linkage_method='complete'):
 
         cluster = AgglomerativeClustering(n_clusters=k, linkage=linkage_method)
         cluster_labels = cluster.fit_predict(X)
 
-        temp_df = pd.DataFrame({'Cluster': cluster_labels, 'DL': data_labels})
+        temp_df = pd.DataFrame({f'Cluster_{k}': cluster_labels})
 
         color_gen = unique_colors.next_color_generator(scaled=False, mode='rgb', shuffle=False)
         cluster_to_color = {c: next(color_gen) for c in sorted(np.unique(cluster_labels))}
-        temp_df['Cluster_color_name'] = temp_df['Cluster'].apply(lambda x: cluster_to_color[x]['name'])
-        temp_df['Cluster_color_rgb'] = temp_df['Cluster'].apply(lambda x: cluster_to_color[x]['val'])
-        temp_df[list(range(1, 512 + 1))] = X
-        # sort by color
-        temp_df = temp_df.sort_values('Cluster_color_name')
+        temp_df[f'Cluster_color_name_{k}'] = temp_df[f'Cluster_{k}'].apply(lambda x: cluster_to_color[x]['name'])
+        temp_df[f'Cluster_color_rgb_{k}'] = temp_df[f'Cluster_{k}'].apply(lambda x: cluster_to_color[x]['val'])
 
         return temp_df
 
-    def create_colortiled_slide(self, cluster_info_df, save_tiles=False, copy=False):
+    def create_colortiled_slide(self, cluster_info_df, target_k, save_tiles=False, copy=False):
 
         # make the color folders for saving the actual tiles
         if save_tiles:
-            for c in cluster_info_df['Cluster_color_name'].unique():
-                pathlib.Path(os.path.join(self.out_dir, c)).mkdir(parents=True, exist_ok=True)
-
-            for res in TileExtractor(self.slide, self.tile_size).iterate_tiles2(batch_size=1):
-                tile, coor = res['tiles'][0], res['coordinates'][0]
+            for c in cluster_info_df[f'Cluster_color_name_{target_k}'].unique():
+                pathlib.Path(os.path.join(self.out_dir, 'tiles', str(target_k), c)).mkdir(parents=True, exist_ok=True)
 
-                # save in color folder
-                # NOTE: this if statement is only for the case where we basically not using all tiles (ie blank)
-                res = cluster_info_df[cluster_info_df['Coor'].apply(lambda x: all(x == coor))]
-                if len(res):
-                    # get the cluster this coordinate belongs to and then the color that cluster belongs to
-                    curr_color = res['Cluster_color_name'].values[0]
-                    curr_sp = os.path.join(self.out_dir, curr_color, str(tuple(coor)) + '.jpg')
-                    cv2.imwrite(curr_sp, tile)
+                coords = cluster_info_df['Coor'][cluster_info_df[f'Cluster_color_name_{target_k}'] == c]
+                for _, coord in coords.items():
+                    fname = str(tuple(coord)) + '.jpg'
+                    try:
+                        shutil.copy2(os.path.join(self.out_dir, 'tiles', 'tmp', fname),
+                                     os.path.join(self.out_dir, 'tiles', str(target_k), c, fname))
+                    except FileNotFoundError:
+                        print(f'Tile for coordinate {coord} not found')
 
         # this allows us to re-use the initialized image with various desired borders
         if copy:
             img_copy = self.image_creator.image.copy()
 
         # group on cluster color and get all the associated coordinates
-        for color, coors in cluster_info_df.groupby('Cluster_color_rgb')['Coor'].apply(list).to_dict().items():
+        for color, coors in cluster_info_df.groupby(f'Cluster_color_rgb_{target_k}')['Coor'].apply(
+                list).to_dict().items():
             # change rgb to bgr
             self.image_creator.add_borders(coors, color=color[::-1], add_big_text=False)
 
         cv2.imwrite(
-            os.path.join(self.out_dir, '{}_k{}_colortiled.jpg'.format(self.slide.name,
-                                                                      cluster_info_df['Cluster_color_name'].nunique())),
+            os.path.join(self.out_dir, '{}_k{}_colortiled.jpg'.format(self.slide.name, target_k)),
             self.image_creator.image
         )
 
         if copy:
             self.image_creator.image = img_copy
 
-    def make_tsne(self, cluster_info_df):
-        import matplotlib as mpl
+    def make_tsne(self, cluster_info_df, target_k):
         print('Generating TSNE')
 
-        scaled_fv_data = MinMaxScaler(copy=False).fit_transform(cluster_info_df[list(range(1, 512 + 1))])
-        res = TSNE(2).fit_transform(scaled_fv_data)
+        res = TSNE(2).fit_transform(cluster_info_df[[str(x) for x in range(1, 512 + 1)]])
 
-        cluster_info_df['TSNE_X'] = res[:, 0]
-        cluster_info_df['TSNE_Y'] = res[:, 1]
+        tsne_df = pd.DataFrame({'TSNE_X': res[:, 0], 'TSNE_Y': res[:, 1]})
 
-        cluster_info_df['Cluster_color_hex'] = cluster_info_df['Cluster_color_rgb'].apply(
+        tsne_df['Cluster_color_hex'] = cluster_info_df[f'Cluster_color_rgb_{target_k}'].apply(
             lambda rgb_tuple: mpl.colors.rgb2hex([x / 255. for x in rgb_tuple]))
 
         # go through each cluster and get the data belonging to it. plot it with its corresponding color
         plt.close('all')
-        for hex, rows in cluster_info_df.groupby('Cluster_color_hex'):
+        for hex, rows in tsne_df.groupby('Cluster_color_hex'):
             plt.scatter(
                 rows['TSNE_X'],
                 rows['TSNE_Y'],
                 s=20,
                 c=[hex] * len(rows)
             )
 
-        sp = os.path.join(self.out_dir,
-                          '{}_k{}_tsne.jpg'.format(self.slide.name, cluster_info_df['Cluster'].nunique()))
+        sp = os.path.join(self.out_dir, '{}_k{}_tsne.jpg'.format(self.slide.name, target_k))
         plt.savefig(sp, dpi=200, bbox_inches='tight')
 
-    def make_dendrogram(self, cluster_info_df):
-        cluster_info_df = cluster_info_df.reset_index(drop=True)
+    def make_dendrogram(self, cluster_info_df, target_k):
 
-        cluster_info_df['Cluster_color_hex'] = cluster_info_df['Cluster_color_rgb'].apply(
+        cluster_color_hex = cluster_info_df[f'Cluster_color_rgb_{target_k}'].apply(
             lambda rgb_tuple: mpl.colors.rgb2hex([x / 255. for x in rgb_tuple]))
-        Z = linkage(cluster_info_df[list(range(1, 512 + 1))], 'ward')
+        Z = linkage(cluster_info_df[[str(x) for x in range(1, 512 + 1)]], 'ward')
 
         # NOTE: THIS IS FOR MAKING DENDROGRAM COLORS MATCH THE COLORTILE SLIDE
         link_cols = {}
         for i, i12 in enumerate(Z[:, :2].astype(int)):
-            c1, c2 = (link_cols[x] if x > len(Z) else cluster_info_df.loc[x]['Cluster_color_hex']
+            c1, c2 = (link_cols[x] if x > len(Z) else cluster_color_hex.loc[x]
                       for x in i12)
             link_cols[i + 1 + len(Z)] = c1 if c1 == c2 else '#0000FF'
 
         plt.close('all')
         plt.title('Hierarchical Clustering Dendrogram')
         plt.ylabel('distance')
 
         dendrogram(
             Z,
             no_labels=True,
             color_threshold=None,
             link_color_func=lambda x: link_cols[x]
         )
 
-        sp = os.path.join(self.out_dir,
-                          '{}_k{}_dendrogram.jpg'.format(self.slide.name, cluster_info_df['Cluster'].nunique()))
-        plt.savefig(sp, dpi=200, bbox_inches='tight')
+        sp = os.path.join(self.out_dir, '{}_k{}_dendrogram.jpg'.format(self.slide.name, target_k))
+        plt.savefig(sp, dpi=500, bbox_inches='tight')
+
+if __name__ == '__main__':
+    from havoc_clustering.general_utility.slide import Slide
+
+    s = Slide('/media/pdiamandis/32TB/TEMP STUFF/can delete/colab test/10P-1A.svs')
+    feat = '/media/pdiamandis/32TB/TEMP STUFF/can delete/colab test/model'
+    out = '/media/pdiamandis/32TB/TEMP STUFF/can delete/colab test/out'
+    h = HAVOC(s, feat, out)
+
+    kwargs = {
+        # make a dendrogram of the clustering used to make the colortile maps (generated for each k value)
+        'make_dendrogram': True,
+        # make a tsne of each color cluster (generated for each k value)
+        'make_tsne': True,
+        # make a Pearson coeffcient clustermap of each color cluster (generated for each k value)
+        'make_corr_map': True,
+        # save the tiles belonging to each color cluster within the colortile map for a given k
+        # ie [4,9] would save the colored tiles belonging to k=4 and k=9
+        # NOTE: this should be a subset of k_vals
+        'save_tiles_k_vals': [4]
+    }
+    h.run(k_vals=[4,9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', **kwargs)
```

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/image_creator.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/image_creator.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/print_time.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/print_time.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/slide.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/slide.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/tile_image_utils.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/tile_image_utils.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/unique_colors.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/unique_colors.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/ai/model_utils.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/ai/model_utils.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/src/havoc_clustering/general_utility/ai/tileextractor.py` & `havoc_clustering-0.0.9/src/havoc_clustering/general_utility/ai/tileextractor.py`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/.gitignore` & `havoc_clustering-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/LICENSE` & `havoc_clustering-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `havoc_clustering-0.0.4/README.md` & `havoc_clustering-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -42,36 +42,51 @@
 havoc = HAVOC(s, feature_extractor_path, save_dir, tile_size=512, hd_backdrop=False)
 
 # to run, requires the following:
 # 1. the k values to use for clustering
 # 2. the blank filter cutoff. 0.5 means that there must be less than (100-50=50)% blank within a tile to decide to use it.
     # ie tiles that are >50% blank would be skipped; a non-conservative number to only cluster tiles with plentiful tissue
 # 3. the layer name within the feature extractor model that is responsible for generating the features
-# 4. whether you want to save the tiles belonging to each color cluster within the colortile map
-havoc.run(k_vals=[9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', save_tiles=False)
+# 4. Additional kwargs; OPTIONAL
+kwargs = {
+    # make a dendrogram of the clustering used to make the colortile maps (generated for each k value)
+    'make_dendrogram': True,
+    # make a tsne of each color cluster (generated for each k value)
+    'make_tsne': True,
+    # make a Pearson coeffcient clustermap of each color cluster (generated for each k value)
+    'make_corr_map': True,
+    # save the tiles belonging to each color cluster within the colortile map for a given k
+    # ie [4,9] would save the colored tiles belonging to k=4 and k=9
+    # NOTE: this should be a subset of k_vals
+    'save_tiles_k_vals': []
+}
+havoc.run(k_vals=[9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', **kwargs)
 ```
 
 ## Result output
 - Colortiled maps
-- CSV files of cluster info + DLFVs (for each desired k value)
-- TSNEs
-- Dendrograms
-- Correlation clustermap
+- CSV file of cluster info + DLFVs (cluster_info_df.csv)
+- Optionally:
+    - TSNEs
+    - Dendrograms
+    - Correlation clustermap
 
 ## Multi-slide correlation map
 
 By running HAVOC on multiple slides, you may want to combine all the generated correlation clustermaps into a mega clustermap.
 
-1. Create a folder with all the k<k_clusters>.csv files
+1. Create a folder containing each slide's cluster_info_df.csv file
 2. 
 ```python
 from havoc_clustering.correlation_of_dlfv_groups import create_correlation_clustermap_multi_slide
 
-create_correlation_clustermap_multi_slide(folder_of_csvs, kval='*')
+create_correlation_clustermap_multi_slide(folder_of_csvs, target_k=9)
 ```
 
+NOTE: the target_k should be a k-value you ran HAVOC with 
+
 ## Citation
 
 Please refer to the paper "HAVOC: Small-scale histomic mapping of biodiversity across entire tumor specimens using deep neural networks"
 
 ## License
 [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.txt)
```

### Comparing `havoc_clustering-0.0.4/pyproject.toml` & `havoc_clustering-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "opencv-python", "scikit-learn", "matplotlib", "pandas", "openslide-python", "seaborn"]
 build-backend = "hatchling.build"
 
 [project]
 name = "havoc-clustering"
-version = "0.0.4"
+version = "0.0.9"
 authors = [
   { name="Kevin Faust", email="kevin.faust@mail.utoronto.ca" },
 ]
 description = "Histomic Atlases of Variation Of Cancers (HAVOC) is a versatile tool that helps map histomic heterogeneity across H&E-stained digital slide images to help guide regional deployment of molecular resources to the most relevant/biodiverse tumor niches"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `havoc_clustering-0.0.4/PKG-INFO` & `havoc_clustering-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: havoc-clustering
-Version: 0.0.4
+Version: 0.0.9
 Summary: Histomic Atlases of Variation Of Cancers (HAVOC) is a versatile tool that helps map histomic heterogeneity across H&E-stained digital slide images to help guide regional deployment of molecular resources to the most relevant/biodiverse tumor niches
 Project-URL: Homepage, https://bitbucket.org/diamandislabii/havoc
 Author-email: Kevin Faust <kevin.faust@mail.utoronto.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -55,36 +55,51 @@
 havoc = HAVOC(s, feature_extractor_path, save_dir, tile_size=512, hd_backdrop=False)
 
 # to run, requires the following:
 # 1. the k values to use for clustering
 # 2. the blank filter cutoff. 0.5 means that there must be less than (100-50=50)% blank within a tile to decide to use it.
     # ie tiles that are >50% blank would be skipped; a non-conservative number to only cluster tiles with plentiful tissue
 # 3. the layer name within the feature extractor model that is responsible for generating the features
-# 4. whether you want to save the tiles belonging to each color cluster within the colortile map
-havoc.run(k_vals=[9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', save_tiles=False)
+# 4. Additional kwargs; OPTIONAL
+kwargs = {
+    # make a dendrogram of the clustering used to make the colortile maps (generated for each k value)
+    'make_dendrogram': True,
+    # make a tsne of each color cluster (generated for each k value)
+    'make_tsne': True,
+    # make a Pearson coeffcient clustermap of each color cluster (generated for each k value)
+    'make_corr_map': True,
+    # save the tiles belonging to each color cluster within the colortile map for a given k
+    # ie [4,9] would save the colored tiles belonging to k=4 and k=9
+    # NOTE: this should be a subset of k_vals
+    'save_tiles_k_vals': []
+}
+havoc.run(k_vals=[9], min_non_blank_amt=0.5, layer_name='global_average_pooling2d_1', **kwargs)
 ```
 
 ## Result output
 - Colortiled maps
-- CSV files of cluster info + DLFVs (for each desired k value)
-- TSNEs
-- Dendrograms
-- Correlation clustermap
+- CSV file of cluster info + DLFVs (cluster_info_df.csv)
+- Optionally:
+    - TSNEs
+    - Dendrograms
+    - Correlation clustermap
 
 ## Multi-slide correlation map
 
 By running HAVOC on multiple slides, you may want to combine all the generated correlation clustermaps into a mega clustermap.
 
-1. Create a folder with all the k<k_clusters>.csv files
+1. Create a folder containing each slide's cluster_info_df.csv file
 2. 
 ```python
 from havoc_clustering.correlation_of_dlfv_groups import create_correlation_clustermap_multi_slide
 
-create_correlation_clustermap_multi_slide(folder_of_csvs, kval='*')
+create_correlation_clustermap_multi_slide(folder_of_csvs, target_k=9)
 ```
 
+NOTE: the target_k should be a k-value you ran HAVOC with 
+
 ## Citation
 
 Please refer to the paper "HAVOC: Small-scale histomic mapping of biodiversity across entire tumor specimens using deep neural networks"
 
 ## License
 [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.txt)
```

