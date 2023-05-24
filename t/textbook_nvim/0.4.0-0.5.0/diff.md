# Comparing `tmp/textbook_nvim-0.4.0.tar.gz` & `tmp/textbook_nvim-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbook_nvim-0.4.0.tar", last modified: Tue May  9 22:46:57 2023, max compression
+gzip compressed data, was "textbook_nvim-0.5.0.tar", last modified: Wed May 24 15:51:19 2023, max compression
```

## Comparing `textbook_nvim-0.4.0.tar` & `textbook_nvim-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      122 2023-05-02 15:35:59.171660 textbook_nvim-0.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2023-05-02 15:35:59.171660 textbook_nvim-0.4.0/LICENSE
--rw-r--r--   0        0        0     3734 2023-05-05 05:44:28.162521 textbook_nvim-0.4.0/README.md
--rw-r--r--   0        0        0      538 2023-05-09 21:03:37.158779 textbook_nvim-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7011 2023-05-09 22:46:46.999279 textbook_nvim-0.4.0/rplugin/python3/textbook.py
--rw-r--r--   0        0        0        0 2023-05-02 15:35:59.171660 textbook_nvim-0.4.0/src/textbook_nvim/__init__.py
--rw-r--r--   0        0        0     1222 2023-05-09 21:04:06.559013 textbook_nvim-0.4.0/src/textbook_nvim/cli.py
--rw-r--r--   0        0        0     1717 2023-05-09 21:04:13.735737 textbook_nvim-0.4.0/src/textbook_nvim/parser.py
--rw-r--r--   0        0        0     6796 2023-05-09 21:04:17.389099 textbook_nvim-0.4.0/src/textbook_nvim/render.py
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 textbook_nvim-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      122 2023-05-02 15:35:59.171660 textbook_nvim-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2023-05-02 15:35:59.171660 textbook_nvim-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4067 2023-05-09 23:09:50.640499 textbook_nvim-0.5.0/README.md
+-rw-r--r--   0        0        0      551 2023-05-24 15:50:26.609734 textbook_nvim-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7011 2023-05-09 23:09:50.640499 textbook_nvim-0.5.0/rplugin/python3/textbook.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:35:59.171660 textbook_nvim-0.5.0/src/textbook_nvim/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-09 23:09:50.640499 textbook_nvim-0.5.0/src/textbook_nvim/cli.py
+-rw-r--r--   0        0        0     1717 2023-05-09 23:09:50.640499 textbook_nvim-0.5.0/src/textbook_nvim/parser.py
+-rw-r--r--   0        0        0     7926 2023-05-24 15:50:03.066141 textbook_nvim-0.5.0/src/textbook_nvim/render.py
+-rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 textbook_nvim-0.5.0/PKG-INFO
```

### Comparing `textbook_nvim-0.4.0/LICENSE` & `textbook_nvim-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.4.0/README.md` & `textbook_nvim-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,234 +1,255 @@
 00000000: 2320 7465 7874 626f 6f6b 2e6e 7669 6d0a  # textbook.nvim.
-00000010: 0a54 6869 7320 706c 7567 696e 2061 6c6c  .This plugin all
-00000020: 6f77 7320 6d61 6e61 6765 6d65 6e74 2061  ows management a
-00000030: 6e64 2072 656e 6465 7269 6e67 206f 6620  nd rendering of 
-00000040: 606a 7570 7974 6572 6020 6e6f 7465 626f  `jupyter` notebo
-00000050: 6f6b 7320 696e 7369 6465 206f 6620 606e  oks inside of `n
-00000060: 656f 7669 6d60 2074 6872 6f75 6768 2074  eovim` through t
-00000070: 6865 2060 6a75 7079 7465 7874 6020 666f  he `jupytext` fo
-00000080: 726d 6174 2061 6e64 2060 7269 6368 6020  rmat and `rich` 
-00000090: 636f 6d70 6f6e 656e 7473 2e0a 0a43 6c69  components...Cli
-000000a0: 636b 206f 6e20 7468 6520 666f 6c6c 6f77  ck on the follow
-000000b0: 696e 6720 696d 6167 6520 746f 2073 6565  ing image to see
-000000c0: 2061 2064 656d 6f3a 0a0a 5b21 5b41 6c74   a demo:..[![Alt
-000000d0: 2074 6578 745d 2868 7474 7073 3a2f 2f69   text](https://i
-000000e0: 6d67 2e79 6f75 7475 6265 2e63 6f6d 2f76  mg.youtube.com/v
-000000f0: 692f 6d43 386b 5a61 3933 7568 672f 302e  i/mC8kZa93uhg/0.
-00000100: 6a70 6729 5d28 6874 7470 733a 2f2f 7777  jpg)](https://ww
-00000110: 772e 796f 7574 7562 652e 636f 6d2f 7761  w.youtube.com/wa
-00000120: 7463 683f 763d 6d43 386b 5a61 3933 7568  tch?v=mC8kZa93uh
-00000130: 6729 0a0a 2323 2049 6e73 7461 6c6c 6174  g)..## Installat
-00000140: 696f 6e0a 0a59 6f75 276c 6c20 6e65 6564  ion..You'll need
-00000150: 2074 6f20 696e 7374 616c 6c20 736f 6d65   to install some
-00000160: 2075 7469 6c69 7469 6573 2061 6e64 2064   utilities and d
-00000170: 6570 656e 6465 6e63 6965 7320 7468 726f  ependencies thro
-00000180: 7567 6820 6070 6970 603a 0a0a 6060 6073  ugh `pip`:..```s
-00000190: 680a 7069 7020 696e 7374 616c 6c20 7465  h.pip install te
-000001a0: 7874 626f 6f6b 5f6e 7669 6d0a 6060 600a  xtbook_nvim.```.
-000001b0: 0a41 6674 6572 2074 6861 742c 2079 6f75  .After that, you
-000001c0: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
-000001d0: 2070 6c75 6769 6e20 7573 696e 6720 6070   plugin using `p
-000001e0: 6163 6b65 7260 2c20 666f 7220 696e 7374  acker`, for inst
-000001f0: 616e 6365 3a0a 0a60 6060 6c75 610a 7573  ance:..```lua.us
-00000200: 6520 7b22 6a75 7365 6c61 7261 312f 7465  e {"juselara1/te
-00000210: 7874 626f 6f6b 2e6e 7669 6d22 2c20 7275  xtbook.nvim", ru
-00000220: 6e20 3d20 223a 5570 6461 7465 5265 6d6f  n = ":UpdateRemo
-00000230: 7465 506c 7567 696e 7322 7d0a 6060 600a  tePlugins"}.```.
-00000240: 0a23 2320 5573 6167 650a 0a54 6865 2069  .## Usage..The i
-00000250: 6465 6120 6265 6869 6e64 2060 7465 7874  dea behind `text
-00000260: 626f 6f6b 6020 6973 2074 6f20 6f66 6665  book` is to offe
-00000270: 7220 6120 6e6f 6e2d 696e 7472 7573 6976  r a non-intrusiv
-00000280: 6520 7761 7920 746f 2065 6469 7420 6e6f  e way to edit no
-00000290: 7465 626f 6f6b 2066 696c 6573 2064 6566  tebook files def
-000002a0: 696e 6564 2061 7320 706c 6169 6e20 7465  ined as plain te
-000002b0: 7874 2e20 4279 2064 6566 6175 6c74 2c20  xt. By default, 
-000002c0: 6974 2075 7365 7320 7468 6520 7065 7263  it uses the perc
-000002d0: 656e 7420 666f 726d 6174 2061 7320 6120  ent format as a 
-000002e0: 6365 6c6c 2073 6570 6172 6174 6f72 2c20  cell separator, 
-000002f0: 6275 7420 796f 7520 6361 6e20 6465 6669  but you can defi
-00000300: 6e65 2061 2072 6567 6578 2074 6f20 7061  ne a regex to pa
-00000310: 7273 6520 616e 7920 6b69 6e64 206f 6620  rse any kind of 
-00000320: 666f 726d 6174 2e0a 0a46 6f72 2069 6e73  format...For ins
-00000330: 7461 6e63 652c 2074 6865 2066 6f6c 6c6f  tance, the follo
-00000340: 7769 6e67 2074 6578 7420 6465 6669 6e65  wing text define
-00000350: 7320 6120 5079 7468 6f6e 206e 6f74 6562  s a Python noteb
-00000360: 6f6f 6b3a 0a0a 6060 6070 7974 686f 6e0a  ook:..```python.
-00000370: 2320 2525 205b 6d61 726b 646f 776e 5d0a  # %% [markdown].
-00000380: 2320 4d61 726b 646f 776e 2063 6f64 652e  # Markdown code.
-00000390: 2e2e 0a0a 2320 2525 205b 7261 775d 0a70  ....# %% [raw].p
-000003a0: 7269 6e74 2822 4865 6c6c 6f2c 2077 6f72  rint("Hello, wor
-000003b0: 6c64 2122 290a 6060 600a 0a54 6f20 7265  ld!").```..To re
-000003c0: 6e64 6572 2074 6869 7320 6669 6c65 2c20  nder this file, 
-000003d0: 796f 7520 7368 6f75 6c64 2072 756e 2074  you should run t
-000003e0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-000003f0: 6d61 6e64 2074 6f20 7370 6563 6966 7920  mand to specify 
-00000400: 7468 6520 6375 7272 656e 7420 6275 6666  the current buff
-00000410: 6572 2061 7320 7468 6520 736f 7572 6365  er as the source
-00000420: 3a0a 0a60 6060 7669 6d0a 3a54 6578 7442  :..```vim.:TextB
-00000430: 6f6f 6b42 7566 6665 720a 6060 600a 0a54  ookBuffer.```..T
-00000440: 6865 6e2c 2079 6f75 2073 686f 756c 6420  hen, you should 
-00000450: 6f70 656e 2074 6865 2072 656e 6465 7220  open the render 
-00000460: 7669 6577 3a0a 0a60 6060 7669 6d0a 3a54  view:..```vim.:T
-00000470: 6578 7442 6f6f 6b4f 7065 6e0a 6060 600a  extBookOpen.```.
-00000480: 0a54 6869 7320 7769 6c6c 2073 7061 776e  .This will spawn
-00000490: 2061 206e 6577 2062 7566 6665 7220 7769   a new buffer wi
-000004a0: 7468 2074 6865 2072 656e 6465 7265 6420  th the rendered 
-000004b0: 7465 7874 2e20 5468 6572 652c 2079 6f75  text. There, you
-000004c0: 2077 696c 6c20 6861 7665 2074 6865 2066   will have the f
-000004d0: 6f6c 6c6f 7769 6e67 206f 7074 696f 6e73  ollowing options
-000004e0: 3a0a 0a2d 2060 3a54 6578 7442 6f6f 6b53  :..- `:TextBookS
-000004f0: 796e 6360 3a20 7379 6e63 7320 7468 6520  ync`: syncs the 
-00000500: 6375 7273 6f72 2070 6f73 6974 696f 6e20  cursor position 
-00000510: 696e 2074 6865 2073 616d 6520 6365 6c6c  in the same cell
-00000520: 2061 7320 7468 6520 706c 6169 6e20 7465   as the plain te
-00000530: 7874 2066 696c 652e 0a2d 2060 3a54 6578  xt file..- `:Tex
-00000540: 7442 6f6f 6b53 656c 6563 7443 656c 6c20  tBookSelectCell 
-00000550: 5b63 656c 6c5f 6964 5d60 3a20 7768 656e  [cell_id]`: when
-00000560: 206e 6f20 6172 6775 6d65 6e74 7320 6172   no arguments ar
-00000570: 6520 7061 7373 6564 2c20 7365 6c65 6374  e passed, select
-00000580: 7320 7468 6520 6365 6c6c 2075 6e64 6572  s the cell under
-00000590: 2074 6865 2063 7572 736f 722e 204f 7468   the cursor. Oth
-000005a0: 6572 7769 7365 2c20 7365 6c65 6374 7320  erwise, selects 
-000005b0: 7468 6520 6365 6c6c 206f 6620 7468 6520  the cell of the 
-000005c0: 6063 656c 6c5f 6964 602e 0a2d 2060 3a54  `cell_id`..- `:T
-000005d0: 6578 7442 6f6f 6b4e 6578 7443 656c 6c60  extBookNextCell`
-000005e0: 3a20 7365 6c65 6374 7320 7468 6520 6e65  : selects the ne
-000005f0: 7874 2063 656c 6c2e 0a2d 2060 3a54 6578  xt cell..- `:Tex
-00000600: 7442 6f6f 6b50 7265 7643 656c 6c60 3a20  tBookPrevCell`: 
-00000610: 7365 6c65 6374 7320 7468 6520 7072 6576  selects the prev
-00000620: 696f 7573 2063 656c 6c2e 0a2d 2060 3a54  ious cell..- `:T
-00000630: 6578 7442 6f6f 6b41 6464 4365 6c6c 2063  extBookAddCell c
-00000640: 656c 6c5f 7479 7065 2061 6674 6572 603a  ell_type after`:
-00000650: 2063 7265 6174 6573 2061 2063 656c 6c20   creates a cell 
-00000660: 6f66 2074 7970 6520 6063 656c 6c5f 7479  of type `cell_ty
-00000670: 7065 6020 2860 7261 7760 206f 7220 606d  pe` (`raw` or `m
-00000680: 6172 6b64 6f77 6e60 2920 616e 6420 6361  arkdown`) and ca
-00000690: 6e20 6265 2062 6566 6f72 6520 2860 3060  n be before (`0`
-000006a0: 2920 6f72 2061 6674 6572 2028 6031 6029  ) or after (`1`)
-000006b0: 2074 6865 2063 656c 6c20 756e 6465 7220   the cell under 
-000006c0: 7468 6520 6375 7273 6f72 2e0a 2d20 603a  the cursor..- `:
-000006d0: 5465 7874 426f 6f6b 436f 6e66 6967 603a  TextBookConfig`:
-000006e0: 2072 656c 6f61 6473 2074 6865 2063 6f6e   reloads the con
-000006f0: 6669 6775 7261 7469 6f6e 2e0a 2d20 603a  figuration..- `:
-00000700: 5465 7874 426f 6f6b 436c 6f73 6560 3a20  TextBookClose`: 
-00000710: 636c 6f73 6573 2074 6865 2072 656e 6465  closes the rende
-00000720: 7265 6420 7669 6577 2061 6e64 2070 6c61  red view and pla
-00000730: 6365 7320 7468 6520 6375 7273 6f72 2069  ces the cursor i
-00000740: 6e20 7468 6520 7361 6d65 2063 656c 6c20  n the same cell 
-00000750: 6173 2074 6865 2072 656e 6465 7265 6420  as the rendered 
-00000760: 7669 6577 2e0a 0a23 2320 436f 6e66 6967  view...## Config
-00000770: 7572 6174 696f 6e0a 0a59 6f75 2063 616e  uration..You can
-00000780: 2061 6464 2074 6865 2066 6f6c 6c6f 7769   add the followi
-00000790: 6e67 206c 696e 6573 2074 6f20 796f 7572  ng lines to your
-000007a0: 2060 696e 6974 2e6c 7561 6020 636f 6e66   `init.lua` conf
-000007b0: 6967 7572 6174 696f 6e3a 0a0a 6060 606c  iguration:..```l
-000007c0: 7561 0a76 696d 2e67 2e54 6578 7442 6f6f  ua.vim.g.TextBoo
-000007d0: 6b54 6d70 5061 7468 203d 2022 2f74 6d70  kTmpPath = "/tmp
-000007e0: 2220 2d2d 2063 6f6e 6669 6720 7061 7468  " -- config path
-000007f0: 2e0a 7669 6d2e 672e 5465 7874 426f 6f6b  ..vim.g.TextBook
-00000800: 4365 6c6c 496e 6469 6361 746f 7220 3d20  CellIndicator = 
-00000810: 223e 2220 2d2d 2069 6e64 6963 6174 6f72  ">" -- indicator
-00000820: 2066 6f72 2063 656c 6c20 7365 6c65 6374   for cell select
-00000830: 696f 6e2e 0a76 696d 2e67 2e54 6578 7442  ion..vim.g.TextB
-00000840: 6f6f 6b43 656c 6c50 6174 7465 726e 203d  ookCellPattern =
-00000850: 2022 5e23 2025 2520 5b28 3f50 3c63 656c   "^# %% [(?P<cel
-00000860: 6c5f 7479 7065 3e5c 5c77 2b29 5d22 202d  l_type>\\w+)]" -
-00000870: 2d20 7265 6765 7820 746f 2070 6172 7365  - regex to parse
-00000880: 2074 6865 2063 656c 6c20 7365 7061 7261   the cell separa
-00000890: 746f 722e 0a76 696d 2e67 2e54 6578 7442  tor..vim.g.TextB
-000008a0: 6f6f 6b43 656c 6c53 6570 6172 6174 6f72  ookCellSeparator
-000008b0: 203d 2022 2320 2525 207b 7d22 202d 2d20   = "# %% {}" -- 
-000008c0: 6465 6669 6e65 7320 7468 6520 6365 6c6c  defines the cell
-000008d0: 2073 6570 6172 6174 6f72 2e0a 7669 6d2e   separator..vim.
-000008e0: 672e 5465 7874 426f 6f6b 4365 6c6c 5465  g.TextBookCellTe
-000008f0: 7874 203d 2022 2043 656c 6c3a 207b 7d22  xt = " Cell: {}"
-00000900: 202d 2d20 7465 7874 2074 6f20 6469 7370   -- text to disp
-00000910: 6c61 7920 7468 6520 6365 6c6c 732e 0a76  lay the cells..v
-00000920: 696d 2e67 2e54 6578 7442 6f6f 6b43 656c  im.g.TextBookCel
-00000930: 6c43 6f6c 6f72 203d 2022 5c5c 2335 3138  lColor = "\\#518
-00000940: 3045 3622 202d 2d20 6365 6c6c 2074 6f20  0E6" -- cell to 
-00000950: 6469 7370 6c61 7920 7468 6520 6365 6c6c  display the cell
-00000960: 2069 642e 0a76 696d 2e67 2e54 6578 7442   id..vim.g.TextB
-00000970: 6f6f 6b54 6865 6d65 203d 2022 7669 6d22  ookTheme = "vim"
-00000980: 202d 2d20 636f 6c6f 7220 6869 6768 6c69   -- color highli
-00000990: 6774 6869 6e67 2074 6865 6d65 2e0a 7669  gthing theme..vi
-000009a0: 6d2e 672e 5465 7874 426f 6f6b 436f 6d6d  m.g.TextBookComm
-000009b0: 656e 7450 6174 7465 726e 203d 2022 5e5c  entPattern = "^\
-000009c0: 5c23 2220 2d2d 2064 6566 696e 6573 2074  \#" -- defines t
-000009d0: 6865 206d 6172 6b64 6f77 6e20 636f 6d6d  he markdown comm
-000009e0: 656e 7420 7061 7474 6572 6e2e 0a0a 6c6f  ent pattern...lo
-000009f0: 6361 6c20 6d6f 6465 203d 2027 6e27 0a6c  cal mode = 'n'.l
-00000a00: 6f63 616c 206f 7074 696f 6e73 203d 207b  ocal options = {
-00000a10: 6e6f 7265 6d61 703d 7472 7565 2c20 7369  noremap=true, si
-00000a20: 6c65 6e74 3d74 7275 657d 0a0a 6c6f 6361  lent=true}..loca
-00000a30: 6c20 6269 6e64 7320 3d20 7b0a 2020 2020  l binds = {.    
-00000a40: 7b62 696e 643d 223c 4c65 6164 6572 3e74  {bind="<Leader>t
-00000a50: 6f22 2c20 636f 6d6d 616e 643d 223a 5465  o", command=":Te
-00000a60: 7874 426f 6f6b 4f70 656e 3c43 523e 227d  xtBookOpen<CR>"}
-00000a70: 2c0a 2020 2020 7b62 696e 643d 223c 4c65  ,.    {bind="<Le
-00000a80: 6164 6572 3e74 7222 2c20 636f 6d6d 616e  ader>tr", comman
-00000a90: 643d 223a 5465 7874 426f 6f6b 5379 6e63  d=":TextBookSync
-00000aa0: 3c43 523e 227d 2c0a 2020 2020 7b62 696e  <CR>"},.    {bin
-00000ab0: 643d 223c 4c65 6164 6572 3e74 6922 2c20  d="<Leader>ti", 
-00000ac0: 636f 6d6d 616e 643d 223a 5465 7874 426f  command=":TextBo
-00000ad0: 6f6b 4275 6666 6572 3c43 523e 227d 2c0a  okBuffer<CR>"},.
-00000ae0: 2020 2020 7b62 696e 643d 223c 4c65 6164      {bind="<Lead
-00000af0: 6572 3e74 7322 2c20 636f 6d6d 616e 643d  er>ts", command=
-00000b00: 223a 5465 7874 426f 6f6b 5365 6c65 6374  ":TextBookSelect
-00000b10: 4365 6c6c 3c43 523e 227d 2c0a 2020 2020  Cell<CR>"},.    
-00000b20: 7b62 696e 643d 223c 4c65 6164 6572 3e74  {bind="<Leader>t
-00000b30: 6722 2c20 636f 6d6d 616e 643d 223a 5465  g", command=":Te
-00000b40: 7874 426f 6f6b 5365 6c65 6374 4365 6c6c  xtBookSelectCell
-00000b50: 227d 2c0a 2020 2020 7b62 696e 643d 223c  "},.    {bind="<
-00000b60: 4c65 6164 6572 3e74 6a22 2c20 636f 6d6d  Leader>tj", comm
-00000b70: 616e 643d 223a 5465 7874 426f 6f6b 5365  and=":TextBookSe
-00000b80: 6c65 6374 4e65 7874 4365 6c6c 3c43 523e  lectNextCell<CR>
-00000b90: 227d 2c0a 2020 2020 7b62 696e 643d 223c  "},.    {bind="<
-00000ba0: 4c65 6164 6572 3e74 6b22 2c20 636f 6d6d  Leader>tk", comm
-00000bb0: 616e 643d 223a 5465 7874 426f 6f6b 5365  and=":TextBookSe
-00000bc0: 6c65 6374 5072 6576 4365 6c6c 3c43 523e  lectPrevCell<CR>
-00000bd0: 227d 2c0a 2020 2020 7b62 696e 643d 223c  "},.    {bind="<
-00000be0: 4c65 6164 6572 3e74 7122 2c20 636f 6d6d  Leader>tq", comm
-00000bf0: 616e 643d 223a 5465 7874 426f 6f6b 436c  and=":TextBookCl
-00000c00: 6f73 653c 4352 3e22 7d2c 0a20 2020 207b  ose<CR>"},.    {
-00000c10: 6269 6e64 3d22 3c4c 6561 6465 723e 746d  bind="<Leader>tm
-00000c20: 6122 2c20 636f 6d6d 616e 643d 223a 5465  a", command=":Te
-00000c30: 7874 426f 6f6b 4164 6443 656c 6c20 6d61  xtBookAddCell ma
-00000c40: 726b 646f 776e 2031 3c43 523e 227d 2c0a  rkdown 1<CR>"},.
-00000c50: 2020 2020 7b62 696e 643d 223c 4c65 6164      {bind="<Lead
-00000c60: 6572 3e74 6d62 222c 2063 6f6d 6d61 6e64  er>tmb", command
-00000c70: 3d22 3a54 6578 7442 6f6f 6b41 6464 4365  =":TextBookAddCe
-00000c80: 6c6c 206d 6172 6b64 6f77 6e20 303c 4352  ll markdown 0<CR
-00000c90: 3e22 7d2c 0a20 2020 207b 6269 6e64 3d22  >"},.    {bind="
-00000ca0: 3c4c 6561 6465 723e 7472 6122 2c20 636f  <Leader>tra", co
-00000cb0: 6d6d 616e 643d 223a 5465 7874 426f 6f6b  mmand=":TextBook
-00000cc0: 4164 6443 656c 6c20 7261 7720 313c 4352  AddCell raw 1<CR
-00000cd0: 3e22 7d2c 0a20 2020 207b 6269 6e64 3d22  >"},.    {bind="
-00000ce0: 3c4c 6561 6465 723e 7472 6222 2c20 636f  <Leader>trb", co
-00000cf0: 6d6d 616e 643d 223a 5465 7874 426f 6f6b  mmand=":TextBook
-00000d00: 4164 6443 656c 6c20 7261 7720 303c 4352  AddCell raw 0<CR
-00000d10: 3e22 7d2c 0a7d 0a0a 666f 7220 5f2c 2076  >"},.}..for _, v
-00000d20: 616c 7565 2069 6e20 6970 6169 7273 2862  alue in ipairs(b
-00000d30: 696e 6473 2920 646f 0a20 2020 2076 696d  inds) do.    vim
-00000d40: 2e61 7069 2e6e 7669 6d5f 7365 745f 6b65  .api.nvim_set_ke
-00000d50: 796d 6170 280a 2020 2020 2020 2020 2020  ymap(.          
-00000d60: 2020 6d6f 6465 2c20 7661 6c75 652e 6269    mode, value.bi
-00000d70: 6e64 2c20 7661 6c75 652e 636f 6d6d 616e  nd, value.comman
-00000d80: 642c 206f 7074 696f 6e73 0a20 2020 2020  d, options.     
-00000d90: 2020 2029 0a65 6e64 0a60 6060 0a0a 3e20     ).end.```..> 
-00000da0: 2a2a 4e6f 7465 2a2a 3a20 616c 6c20 7061  **Note**: all pa
-00000db0: 7474 6572 6e73 206d 7573 7420 6265 2069  tterns must be i
-00000dc0: 6d70 6c65 6d65 6e74 6564 2061 7320 5079  mplemented as Py
-00000dd0: 7468 6f6e 2072 6567 6578 2e0a 0a3e 202a  thon regex...> *
-00000de0: 2a4e 6f74 652a 2a3a 2074 6865 2063 656c  *Note**: the cel
-00000df0: 6c20 7365 7061 7261 746f 7220 6d75 7374  l separator must
-00000e00: 2068 6176 6520 7468 6520 6e61 6d65 6420   have the named 
-00000e10: 6772 6f75 7020 6063 656c 6c5f 7479 7065  group `cell_type
-00000e20: 602c 2074 6869 7320 6973 2075 7365 6420  `, this is used 
-00000e30: 666f 7220 7061 7273 696e 672e 0a0a 3e20  for parsing...> 
-00000e40: 2a2a 4e6f 7465 2a2a 3a20 6074 6578 7462  **Note**: `textb
-00000e50: 6f6f 6b2e 6e76 696d 6020 7573 6573 2074  ook.nvim` uses t
-00000e60: 6865 2060 7079 676d 656e 7473 6020 5b73  he `pygments` [s
-00000e70: 7479 6c65 735d 2868 7474 7073 3a2f 2f70  tyles](https://p
-00000e80: 7967 6d65 6e74 732e 6f72 672f 7374 796c  ygments.org/styl
-00000e90: 6573 2f29 2e0a                           es/)..
+00000010: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000020: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000030: 672f 7079 7069 2f74 6578 7462 6f6f 6b5f  g/pypi/textbook_
+00000040: 6e76 696d 223e 3c69 6d67 2073 7263 3d22  nvim"><img src="
+00000050: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000060: 6c64 732e 696f 2f70 7970 692f 762f 7465  lds.io/pypi/v/te
+00000070: 7874 626f 6f6b 5f6e 7669 6d2e 7376 6722  xtbook_nvim.svg"
+00000080: 2f3e 3c2f 613e 0a3c 6120 6872 6566 3d22  /></a>.<a href="
+00000090: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000a0: 6f6d 2f70 7366 2f62 6c61 636b 223e 3c69  om/psf/black"><i
+000000b0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000000c0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000000d0: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
+000000e0: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
+000000f0: 7667 222f 3e3c 2f61 3e0a 0a54 6869 7320  vg"/></a>..This 
+00000100: 706c 7567 696e 2061 6c6c 6f77 7320 6d61  plugin allows ma
+00000110: 6e61 6765 6d65 6e74 2061 6e64 2072 656e  nagement and ren
+00000120: 6465 7269 6e67 206f 6620 606a 7570 7974  dering of `jupyt
+00000130: 6572 6020 6e6f 7465 626f 6f6b 7320 696e  er` notebooks in
+00000140: 7369 6465 206f 6620 606e 656f 7669 6d60  side of `neovim`
+00000150: 2074 6872 6f75 6768 2074 6865 2060 6a75   through the `ju
+00000160: 7079 7465 7874 6020 666f 726d 6174 2061  pytext` format a
+00000170: 6e64 2060 7269 6368 6020 636f 6d70 6f6e  nd `rich` compon
+00000180: 656e 7473 2e0a 0a43 6c69 636b 206f 6e20  ents...Click on 
+00000190: 7468 6520 666f 6c6c 6f77 696e 6720 696d  the following im
+000001a0: 6167 6520 746f 2073 6565 2061 2064 656d  age to see a dem
+000001b0: 6f3a 0a0a 5b21 5b41 6c74 2074 6578 745d  o:..[![Alt text]
+000001c0: 2868 7474 7073 3a2f 2f69 6d67 2e79 6f75  (https://img.you
+000001d0: 7475 6265 2e63 6f6d 2f76 692f 6d43 386b  tube.com/vi/mC8k
+000001e0: 5a61 3933 7568 672f 302e 6a70 6729 5d28  Za93uhg/0.jpg)](
+000001f0: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+00000200: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00000210: 6d43 386b 5a61 3933 7568 6729 0a0a 2323  mC8kZa93uhg)..##
+00000220: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a59   Installation..Y
+00000230: 6f75 276c 6c20 6e65 6564 2074 6f20 696e  ou'll need to in
+00000240: 7374 616c 6c20 736f 6d65 2075 7469 6c69  stall some utili
+00000250: 7469 6573 2061 6e64 2064 6570 656e 6465  ties and depende
+00000260: 6e63 6965 7320 7468 726f 7567 6820 6070  ncies through `p
+00000270: 6970 603a 0a0a 6060 6073 680a 7069 7020  ip`:..```sh.pip 
+00000280: 696e 7374 616c 6c20 7465 7874 626f 6f6b  install textbook
+00000290: 5f6e 7669 6d0a 6060 600a 0a41 6674 6572  _nvim.```..After
+000002a0: 2074 6861 742c 2079 6f75 2063 616e 2069   that, you can i
+000002b0: 6e73 7461 6c6c 2074 6865 2070 6c75 6769  nstall the plugi
+000002c0: 6e20 7573 696e 6720 6070 6163 6b65 7260  n using `packer`
+000002d0: 2c20 666f 7220 696e 7374 616e 6365 3a0a  , for instance:.
+000002e0: 0a60 6060 6c75 610a 7573 6520 7b22 6a75  .```lua.use {"ju
+000002f0: 7365 6c61 7261 312f 7465 7874 626f 6f6b  selara1/textbook
+00000300: 2e6e 7669 6d22 2c20 7275 6e20 3d20 223a  .nvim", run = ":
+00000310: 5570 6461 7465 5265 6d6f 7465 506c 7567  UpdateRemotePlug
+00000320: 696e 7322 7d0a 6060 600a 0a23 2320 5573  ins"}.```..## Us
+00000330: 6167 650a 0a54 6865 2069 6465 6120 6265  age..The idea be
+00000340: 6869 6e64 2060 7465 7874 626f 6f6b 6020  hind `textbook` 
+00000350: 6973 2074 6f20 6f66 6665 7220 6120 6e6f  is to offer a no
+00000360: 6e2d 696e 7472 7573 6976 6520 7761 7920  n-intrusive way 
+00000370: 746f 2065 6469 7420 6e6f 7465 626f 6f6b  to edit notebook
+00000380: 2066 696c 6573 2064 6566 696e 6564 2061   files defined a
+00000390: 7320 706c 6169 6e20 7465 7874 2e20 4279  s plain text. By
+000003a0: 2064 6566 6175 6c74 2c20 6974 2075 7365   default, it use
+000003b0: 7320 7468 6520 7065 7263 656e 7420 666f  s the percent fo
+000003c0: 726d 6174 2061 7320 6120 6365 6c6c 2073  rmat as a cell s
+000003d0: 6570 6172 6174 6f72 2c20 6275 7420 796f  eparator, but yo
+000003e0: 7520 6361 6e20 6465 6669 6e65 2061 2072  u can define a r
+000003f0: 6567 6578 2074 6f20 7061 7273 6520 616e  egex to parse an
+00000400: 7920 6b69 6e64 206f 6620 666f 726d 6174  y kind of format
+00000410: 2e0a 0a46 6f72 2069 6e73 7461 6e63 652c  ...For instance,
+00000420: 2074 6865 2066 6f6c 6c6f 7769 6e67 2074   the following t
+00000430: 6578 7420 6465 6669 6e65 7320 6120 5079  ext defines a Py
+00000440: 7468 6f6e 206e 6f74 6562 6f6f 6b3a 0a0a  thon notebook:..
+00000450: 6060 6070 7974 686f 6e0a 2320 2525 205b  ```python.# %% [
+00000460: 6d61 726b 646f 776e 5d0a 2320 4d61 726b  markdown].# Mark
+00000470: 646f 776e 2063 6f64 652e 2e2e 0a0a 2320  down code.....# 
+00000480: 2525 205b 636f 6465 5d0a 7072 696e 7428  %% [code].print(
+00000490: 2248 656c 6c6f 2c20 776f 726c 6421 2229  "Hello, world!")
+000004a0: 0a60 6060 0a0a 546f 2072 656e 6465 7220  .```..To render 
+000004b0: 7468 6973 2066 696c 652c 2079 6f75 2073  this file, you s
+000004c0: 686f 756c 6420 7275 6e20 7468 6520 666f  hould run the fo
+000004d0: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+000004e0: 746f 2073 7065 6369 6679 2074 6865 2063  to specify the c
+000004f0: 7572 7265 6e74 2062 7566 6665 7220 6173  urrent buffer as
+00000500: 2074 6865 2073 6f75 7263 653a 0a0a 6060   the source:..``
+00000510: 6076 696d 0a3a 5465 7874 426f 6f6b 4275  `vim.:TextBookBu
+00000520: 6666 6572 0a60 6060 0a0a 5468 656e 2c20  ffer.```..Then, 
+00000530: 796f 7520 7368 6f75 6c64 206f 7065 6e20  you should open 
+00000540: 7468 6520 7265 6e64 6572 2076 6965 773a  the render view:
+00000550: 0a0a 6060 6076 696d 0a3a 5465 7874 426f  ..```vim.:TextBo
+00000560: 6f6b 4f70 656e 0a60 6060 0a0a 5468 6973  okOpen.```..This
+00000570: 2077 696c 6c20 7370 6177 6e20 6120 6e65   will spawn a ne
+00000580: 7720 6275 6666 6572 2077 6974 6820 7468  w buffer with th
+00000590: 6520 7265 6e64 6572 6564 2074 6578 742e  e rendered text.
+000005a0: 2054 6865 7265 2c20 796f 7520 7769 6c6c   There, you will
+000005b0: 2068 6176 6520 7468 6520 666f 6c6c 6f77   have the follow
+000005c0: 696e 6720 6f70 7469 6f6e 733a 0a0a 2d20  ing options:..- 
+000005d0: 603a 5465 7874 426f 6f6b 5379 6e63 603a  `:TextBookSync`:
+000005e0: 2073 796e 6373 2074 6865 2063 7572 736f   syncs the curso
+000005f0: 7220 706f 7369 7469 6f6e 2069 6e20 7468  r position in th
+00000600: 6520 7361 6d65 2063 656c 6c20 6173 2074  e same cell as t
+00000610: 6865 2070 6c61 696e 2074 6578 7420 6669  he plain text fi
+00000620: 6c65 2e0a 2d20 603a 5465 7874 426f 6f6b  le..- `:TextBook
+00000630: 5365 6c65 6374 4365 6c6c 205b 6365 6c6c  SelectCell [cell
+00000640: 5f69 645d 603a 2077 6865 6e20 6e6f 2061  _id]`: when no a
+00000650: 7267 756d 656e 7473 2061 7265 2070 6173  rguments are pas
+00000660: 7365 642c 2073 656c 6563 7473 2074 6865  sed, selects the
+00000670: 2063 656c 6c20 756e 6465 7220 7468 6520   cell under the 
+00000680: 6375 7273 6f72 2e20 4f74 6865 7277 6973  cursor. Otherwis
+00000690: 652c 2073 656c 6563 7473 2074 6865 2063  e, selects the c
+000006a0: 656c 6c20 6f66 2074 6865 2060 6365 6c6c  ell of the `cell
+000006b0: 5f69 6460 2e0a 2d20 603a 5465 7874 426f  _id`..- `:TextBo
+000006c0: 6f6b 4e65 7874 4365 6c6c 603a 2073 656c  okNextCell`: sel
+000006d0: 6563 7473 2074 6865 206e 6578 7420 6365  ects the next ce
+000006e0: 6c6c 2e0a 2d20 603a 5465 7874 426f 6f6b  ll..- `:TextBook
+000006f0: 5072 6576 4365 6c6c 603a 2073 656c 6563  PrevCell`: selec
+00000700: 7473 2074 6865 2070 7265 7669 6f75 7320  ts the previous 
+00000710: 6365 6c6c 2e0a 2d20 603a 5465 7874 426f  cell..- `:TextBo
+00000720: 6f6b 4164 6443 656c 6c20 6365 6c6c 5f74  okAddCell cell_t
+00000730: 7970 6520 6166 7465 7260 3a20 6372 6561  ype after`: crea
+00000740: 7465 7320 6120 6365 6c6c 206f 6620 7479  tes a cell of ty
+00000750: 7065 2060 6365 6c6c 5f74 7970 6560 2028  pe `cell_type` (
+00000760: 6063 6f64 6560 206f 7220 606d 6172 6b64  `code` or `markd
+00000770: 6f77 6e60 2920 616e 6420 6361 6e20 6265  own`) and can be
+00000780: 2062 6566 6f72 6520 2860 3060 2920 6f72   before (`0`) or
+00000790: 2061 6674 6572 2028 6031 6029 2074 6865   after (`1`) the
+000007a0: 2063 656c 6c20 756e 6465 7220 7468 6520   cell under the 
+000007b0: 6375 7273 6f72 2e0a 2d20 603a 5465 7874  cursor..- `:Text
+000007c0: 426f 6f6b 436f 6e66 6967 603a 2072 656c  BookConfig`: rel
+000007d0: 6f61 6473 2074 6865 2063 6f6e 6669 6775  oads the configu
+000007e0: 7261 7469 6f6e 2e0a 2d20 603a 5465 7874  ration..- `:Text
+000007f0: 426f 6f6b 5265 6e64 6572 603a 2073 796e  BookRender`: syn
+00000800: 6373 2074 6865 2063 7572 7265 6e74 2062  cs the current b
+00000810: 7566 6665 7220 7769 7468 2069 7473 2070  uffer with its p
+00000820: 6169 7265 6420 6069 7079 6e62 6020 6669  aired `ipynb` fi
+00000830: 6c65 2074 6872 6f75 6768 2060 6a75 7079  le through `jupy
+00000840: 7465 7874 602e 0a2d 2060 3a54 6578 7442  text`..- `:TextB
+00000850: 6f6f 6b43 6c6f 7365 603a 2063 6c6f 7365  ookClose`: close
+00000860: 7320 7468 6520 7265 6e64 6572 6564 2076  s the rendered v
+00000870: 6965 7720 616e 6420 706c 6163 6573 2074  iew and places t
+00000880: 6865 2063 7572 736f 7220 696e 2074 6865  he cursor in the
+00000890: 2073 616d 6520 6365 6c6c 2061 7320 7468   same cell as th
+000008a0: 6520 7265 6e64 6572 6564 2076 6965 772e  e rendered view.
+000008b0: 0a0a 2323 2043 6f6e 6669 6775 7261 7469  ..## Configurati
+000008c0: 6f6e 0a0a 596f 7520 6361 6e20 6164 6420  on..You can add 
+000008d0: 7468 6520 666f 6c6c 6f77 696e 6720 6c69  the following li
+000008e0: 6e65 7320 746f 2079 6f75 7220 6069 6e69  nes to your `ini
+000008f0: 742e 6c75 6160 2063 6f6e 6669 6775 7261  t.lua` configura
+00000900: 7469 6f6e 3a0a 0a60 6060 6c75 610a 7669  tion:..```lua.vi
+00000910: 6d2e 672e 5465 7874 426f 6f6b 546d 7050  m.g.TextBookTmpP
+00000920: 6174 6820 3d20 222f 746d 7022 202d 2d20  ath = "/tmp" -- 
+00000930: 636f 6e66 6967 2070 6174 682e 0a76 696d  config path..vim
+00000940: 2e67 2e54 6578 7442 6f6f 6b43 656c 6c49  .g.TextBookCellI
+00000950: 6e64 6963 6174 6f72 203d 2022 3e22 202d  ndicator = ">" -
+00000960: 2d20 696e 6469 6361 746f 7220 666f 7220  - indicator for 
+00000970: 6365 6c6c 2073 656c 6563 7469 6f6e 2e0a  cell selection..
+00000980: 7669 6d2e 672e 5465 7874 426f 6f6b 4365  vim.g.TextBookCe
+00000990: 6c6c 5061 7474 6572 6e20 3d20 225e 2320  llPattern = "^# 
+000009a0: 2525 205b 283f 503c 6365 6c6c 5f74 7970  %% [(?P<cell_typ
+000009b0: 653e 5c5c 772b 295d 2220 2d2d 2072 6567  e>\\w+)]" -- reg
+000009c0: 6578 2074 6f20 7061 7273 6520 7468 6520  ex to parse the 
+000009d0: 6365 6c6c 2073 6570 6172 6174 6f72 2e0a  cell separator..
+000009e0: 7669 6d2e 672e 5465 7874 426f 6f6b 4365  vim.g.TextBookCe
+000009f0: 6c6c 5365 7061 7261 746f 7220 3d20 2223  llSeparator = "#
+00000a00: 2025 2520 7b7d 2220 2d2d 2064 6566 696e   %% {}" -- defin
+00000a10: 6573 2074 6865 2063 656c 6c20 7365 7061  es the cell sepa
+00000a20: 7261 746f 722e 0a76 696d 2e67 2e54 6578  rator..vim.g.Tex
+00000a30: 7442 6f6f 6b43 656c 6c54 6578 7420 3d20  tBookCellText = 
+00000a40: 2220 4365 6c6c 3a20 7b7d 2220 2d2d 2074  " Cell: {}" -- t
+00000a50: 6578 7420 746f 2064 6973 706c 6179 2074  ext to display t
+00000a60: 6865 2063 656c 6c73 2e0a 7669 6d2e 672e  he cells..vim.g.
+00000a70: 5465 7874 426f 6f6b 4365 6c6c 436f 6c6f  TextBookCellColo
+00000a80: 7220 3d20 225c 5c23 3531 3830 4536 2220  r = "\\#5180E6" 
+00000a90: 2d2d 2063 656c 6c20 746f 2064 6973 706c  -- cell to displ
+00000aa0: 6179 2074 6865 2063 656c 6c20 6964 2e0a  ay the cell id..
+00000ab0: 7669 6d2e 672e 5465 7874 426f 6f6b 5468  vim.g.TextBookTh
+00000ac0: 656d 6520 3d20 2276 696d 2220 2d2d 2063  eme = "vim" -- c
+00000ad0: 6f6c 6f72 2068 6967 686c 6967 7468 696e  olor highligthin
+00000ae0: 6720 7468 656d 652e 0a76 696d 2e67 2e54  g theme..vim.g.T
+00000af0: 6578 7442 6f6f 6b43 6f6d 6d65 6e74 5061  extBookCommentPa
+00000b00: 7474 6572 6e20 3d20 225e 5c5c 2322 202d  ttern = "^\\#" -
+00000b10: 2d20 6465 6669 6e65 7320 7468 6520 6d61  - defines the ma
+00000b20: 726b 646f 776e 2063 6f6d 6d65 6e74 2070  rkdown comment p
+00000b30: 6174 7465 726e 2e0a 0a6c 6f63 616c 206d  attern...local m
+00000b40: 6f64 6520 3d20 276e 270a 6c6f 6361 6c20  ode = 'n'.local 
+00000b50: 6f70 7469 6f6e 7320 3d20 7b6e 6f72 656d  options = {norem
+00000b60: 6170 3d74 7275 652c 2073 696c 656e 743d  ap=true, silent=
+00000b70: 7472 7565 7d0a 0a6c 6f63 616c 2062 696e  true}..local bin
+00000b80: 6473 203d 207b 0a20 2020 207b 6269 6e64  ds = {.    {bind
+00000b90: 3d22 3c4c 6561 6465 723e 746f 222c 2063  ="<Leader>to", c
+00000ba0: 6f6d 6d61 6e64 3d22 3a54 6578 7442 6f6f  ommand=":TextBoo
+00000bb0: 6b4f 7065 6e3c 4352 3e22 7d2c 0a20 2020  kOpen<CR>"},.   
+00000bc0: 207b 6269 6e64 3d22 3c4c 6561 6465 723e   {bind="<Leader>
+00000bd0: 7472 222c 2063 6f6d 6d61 6e64 3d22 3a54  tr", command=":T
+00000be0: 6578 7442 6f6f 6b53 796e 633c 4352 3e22  extBookSync<CR>"
+00000bf0: 7d2c 0a20 2020 207b 6269 6e64 3d22 3c4c  },.    {bind="<L
+00000c00: 6561 6465 723e 7469 222c 2063 6f6d 6d61  eader>ti", comma
+00000c10: 6e64 3d22 3a54 6578 7442 6f6f 6b42 7566  nd=":TextBookBuf
+00000c20: 6665 723c 4352 3e22 7d2c 0a20 2020 207b  fer<CR>"},.    {
+00000c30: 6269 6e64 3d22 3c4c 6561 6465 723e 7473  bind="<Leader>ts
+00000c40: 222c 2063 6f6d 6d61 6e64 3d22 3a54 6578  ", command=":Tex
+00000c50: 7442 6f6f 6b53 656c 6563 7443 656c 6c3c  tBookSelectCell<
+00000c60: 4352 3e22 7d2c 0a20 2020 207b 6269 6e64  CR>"},.    {bind
+00000c70: 3d22 3c4c 6561 6465 723e 7467 222c 2063  ="<Leader>tg", c
+00000c80: 6f6d 6d61 6e64 3d22 3a54 6578 7442 6f6f  ommand=":TextBoo
+00000c90: 6b53 656c 6563 7443 656c 6c22 7d2c 0a20  kSelectCell"},. 
+00000ca0: 2020 207b 6269 6e64 3d22 3c4c 6561 6465     {bind="<Leade
+00000cb0: 723e 746a 222c 2063 6f6d 6d61 6e64 3d22  r>tj", command="
+00000cc0: 3a54 6578 7442 6f6f 6b53 656c 6563 744e  :TextBookSelectN
+00000cd0: 6578 7443 656c 6c3c 4352 3e22 7d2c 0a20  extCell<CR>"},. 
+00000ce0: 2020 207b 6269 6e64 3d22 3c4c 6561 6465     {bind="<Leade
+00000cf0: 723e 746b 222c 2063 6f6d 6d61 6e64 3d22  r>tk", command="
+00000d00: 3a54 6578 7442 6f6f 6b53 656c 6563 7450  :TextBookSelectP
+00000d10: 7265 7643 656c 6c3c 4352 3e22 7d2c 0a20  revCell<CR>"},. 
+00000d20: 2020 207b 6269 6e64 3d22 3c4c 6561 6465     {bind="<Leade
+00000d30: 723e 7471 222c 2063 6f6d 6d61 6e64 3d22  r>tq", command="
+00000d40: 3a54 6578 7442 6f6f 6b43 6c6f 7365 3c43  :TextBookClose<C
+00000d50: 523e 227d 2c0a 2020 2020 7b62 696e 643d  R>"},.    {bind=
+00000d60: 223c 4c65 6164 6572 3e74 6d61 222c 2063  "<Leader>tma", c
+00000d70: 6f6d 6d61 6e64 3d22 3a54 6578 7442 6f6f  ommand=":TextBoo
+00000d80: 6b41 6464 4365 6c6c 206d 6172 6b64 6f77  kAddCell markdow
+00000d90: 6e20 313c 4352 3e22 7d2c 0a20 2020 207b  n 1<CR>"},.    {
+00000da0: 6269 6e64 3d22 3c4c 6561 6465 723e 746d  bind="<Leader>tm
+00000db0: 6222 2c20 636f 6d6d 616e 643d 223a 5465  b", command=":Te
+00000dc0: 7874 426f 6f6b 4164 6443 656c 6c20 6d61  xtBookAddCell ma
+00000dd0: 726b 646f 776e 2030 3c43 523e 227d 2c0a  rkdown 0<CR>"},.
+00000de0: 2020 2020 7b62 696e 643d 223c 4c65 6164      {bind="<Lead
+00000df0: 6572 3e74 7261 222c 2063 6f6d 6d61 6e64  er>tra", command
+00000e00: 3d22 3a54 6578 7442 6f6f 6b41 6464 4365  =":TextBookAddCe
+00000e10: 6c6c 2063 6f64 6520 313c 4352 3e22 7d2c  ll code 1<CR>"},
+00000e20: 0a20 2020 207b 6269 6e64 3d22 3c4c 6561  .    {bind="<Lea
+00000e30: 6465 723e 7472 6222 2c20 636f 6d6d 616e  der>trb", comman
+00000e40: 643d 223a 5465 7874 426f 6f6b 4164 6443  d=":TextBookAddC
+00000e50: 656c 6c20 636f 6465 2030 3c43 523e 227d  ell code 0<CR>"}
+00000e60: 2c0a 7d0a 0a66 6f72 205f 2c20 7661 6c75  ,.}..for _, valu
+00000e70: 6520 696e 2069 7061 6972 7328 6269 6e64  e in ipairs(bind
+00000e80: 7329 2064 6f0a 2020 2020 7669 6d2e 6170  s) do.    vim.ap
+00000e90: 692e 6e76 696d 5f73 6574 5f6b 6579 6d61  i.nvim_set_keyma
+00000ea0: 7028 0a20 2020 2020 2020 2020 2020 206d  p(.            m
+00000eb0: 6f64 652c 2076 616c 7565 2e62 696e 642c  ode, value.bind,
+00000ec0: 2076 616c 7565 2e63 6f6d 6d61 6e64 2c20   value.command, 
+00000ed0: 6f70 7469 6f6e 730a 2020 2020 2020 2020  options.        
+00000ee0: 290a 656e 640a 6060 600a 0a3e 202a 2a4e  ).end.```..> **N
+00000ef0: 6f74 652a 2a3a 2061 6c6c 2070 6174 7465  ote**: all patte
+00000f00: 726e 7320 6d75 7374 2062 6520 696d 706c  rns must be impl
+00000f10: 656d 656e 7465 6420 6173 2050 7974 686f  emented as Pytho
+00000f20: 6e20 7265 6765 782e 0a0a 3e20 2a2a 4e6f  n regex...> **No
+00000f30: 7465 2a2a 3a20 7468 6520 6365 6c6c 2073  te**: the cell s
+00000f40: 6570 6172 6174 6f72 206d 7573 7420 6861  eparator must ha
+00000f50: 7665 2074 6865 206e 616d 6564 2067 726f  ve the named gro
+00000f60: 7570 2060 6365 6c6c 5f74 7970 6560 2c20  up `cell_type`, 
+00000f70: 7468 6973 2069 7320 7573 6564 2066 6f72  this is used for
+00000f80: 2070 6172 7369 6e67 2e0a 0a3e 202a 2a4e   parsing...> **N
+00000f90: 6f74 652a 2a3a 2060 7465 7874 626f 6f6b  ote**: `textbook
+00000fa0: 2e6e 7669 6d60 2075 7365 7320 7468 6520  .nvim` uses the 
+00000fb0: 6070 7967 6d65 6e74 7360 205b 7374 796c  `pygments` [styl
+00000fc0: 6573 5d28 6874 7470 733a 2f2f 7079 676d  es](https://pygm
+00000fd0: 656e 7473 2e6f 7267 2f73 7479 6c65 732f  ents.org/styles/
+00000fe0: 292e 0a                                  )..
```

### Comparing `textbook_nvim-0.4.0/pyproject.toml` & `textbook_nvim-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textbook_nvim"
-version = "0.4.0"
+version = "0.5.0"
 authors = [{name = "Juan Lara", email = "julara@unal.edu.co"}]
 description = "Main python package for the textbook.nvim plugin."
 requires-python = ">3.8"
 dependencies = [
-    "pydantic", "pynvim", "rich", "click", "jupytext"
+    "pydantic", "pynvim", "rich", "click", "jupytext", "flatlatex"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 
 [project.optional-dependencies]
 dev = ["flit", "black"]
```

### Comparing `textbook_nvim-0.4.0/rplugin/python3/textbook.py` & `textbook_nvim-0.5.0/rplugin/python3/textbook.py`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.4.0/src/textbook_nvim/cli.py` & `textbook_nvim-0.5.0/src/textbook_nvim/cli.py`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.4.0/src/textbook_nvim/parser.py` & `textbook_nvim-0.5.0/src/textbook_nvim/parser.py`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.4.0/src/textbook_nvim/render.py` & `textbook_nvim-0.5.0/src/textbook_nvim/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from enum import Enum
 import re
 from abc import ABC, abstractmethod
+from flatlatex.latexfuntypes import LatexSyntaxError
 from pydantic import BaseModel
 from textbook_nvim.parser import ParsedCell, ParsedText
 from typing import Dict, List, Tuple, Type, Union
 from rich.console import Console, Group
 from rich.syntax import Syntax
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from pathlib import Path
+from flatlatex import converter as Converter
 
 
 class RenderedCell(BaseModel):
     text: str
     cell_range: Tuple[int, int]
 
 
@@ -82,14 +84,17 @@
     text: str
     idx: int
     md_type: MarkdownEnum
 
 
 class MarkdownRender(AbstractRender):
     table_pattern = re.compile(r"\|.+\|")
+    eq_pattern = re.compile(r"\$(?P<equation>[^\n]+)\$")
+    eq_block_pattern = re.compile(r"\$\$\n(?P<equation>[^\$]+)\$\$")
+    eq_converter = Converter()
     sep_validator = re.compile(r"[\-\s]+")
 
     def render_table(self, group: List[MarkdownRow]) -> Union[Markdown, Table]:
         if re.search(self.sep_validator, "".join(group[1].text.split("|"))) is None:
             return Markdown("\n".join(line.text for line in group))
         table = Table()
         headers = group[0].text.strip().split("|")
@@ -98,14 +103,38 @@
         for row in group[2:]:
             cells = row.text.strip().split("|")
             if len(cells) != n_cols:
                 return Markdown("\n".join(line.text for line in group))
             table.add_row(*cells)
         return table
 
+    def render_equations(self, lines: List[str]) -> List[str]:
+        text = "\n".join(lines)
+
+        def parse_line_eq(match: re.Match):
+            text = match.group("equation")
+            try:
+                render = f" `{self.eq_converter.convert(text)}` "
+            except LatexSyntaxError:
+                render = f" ${text}$ "
+            return render
+
+        line_eq = re.sub(self.eq_pattern, parse_line_eq, text)
+
+        def parse_block_eq(match: re.Match):
+            text = match.group("equation")
+            try:
+                render = f"\n`{self.eq_converter.convert(text)}`\n"
+            except LatexSyntaxError:
+                render = f"$$\n{text}$$\n"
+            return render
+
+        block_eq = re.sub(self.eq_block_pattern, parse_block_eq, line_eq)
+        return block_eq.split("\n")
+
     def generate_components(
         self, groups: List[List[MarkdownRow]]
     ) -> List[Union[Markdown, Table]]:
         components = []
         for group in groups:
             if group[0].md_type == MarkdownEnum.TEXT or len(group) < 3:
                 components.append(Markdown("\n".join(line.text for line in group)))
@@ -135,15 +164,16 @@
         return Group(*components)
 
     def render(self) -> RenderedCell:
         lines = self.parsed_cell.text.split("\n")[1:]
         (*clean_lines,) = map(
             lambda line: re.sub(self.comment_pattern, "", line), lines
         )
-        md = Panel(self.render_lines(clean_lines), title="markdown")
+        eq_lines = self.render_equations(clean_lines)
+        md = Panel(self.render_lines(eq_lines), title="markdown")
         text = Text(self.cell_text.format(self.cell_id))
         text.stylize(self.cell_color)
         with self.console.capture() as capture:
             self.console.print(text)
             self.console.print(md)
         rendered_lines = capture.get().split("\n")
         self.console.print(text)
```

