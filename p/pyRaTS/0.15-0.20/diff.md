# Comparing `tmp/pyRaTS-0.15.tar.gz` & `tmp/pyRaTS-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRaTS-0.15.tar", last modified: Mon Dec 19 14:45:50 2022, max compression
+gzip compressed data, was "pyRaTS-0.20.tar", last modified: Wed May 24 11:12:36 2023, max compression
```

## Comparing `pyRaTS-0.15.tar` & `pyRaTS-0.20.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 14:45:50.634770 pyRaTS-0.15/
--rw-rw-rw-   0        0        0     3360 2022-12-19 14:45:50.633772 pyRaTS-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-19 14:45:50.609837 pyRaTS-0.15/pyRaTS/
-drwxrwxrwx   0        0        0        0 2022-12-19 14:45:50.629782 pyRaTS-0.15/pyRaTS/src/
-drwxrwxrwx   0        0        0        0 2022-12-19 14:45:50.627796 pyRaTS-0.15/pyRaTS/src/pyRaTS.egg-info/
--rw-rw-rw-   0        0        0     3360 2022-12-19 14:45:50.000000 pyRaTS-0.15/pyRaTS/src/pyRaTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2022-12-19 14:45:50.000000 pyRaTS-0.15/pyRaTS/src/pyRaTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 14:45:50.000000 pyRaTS-0.15/pyRaTS/src/pyRaTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-12-19 14:45:50.000000 pyRaTS-0.15/pyRaTS/src/pyRaTS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    78294 2022-12-19 14:07:20.000000 pyRaTS-0.15/pyRaTS/src/pyRaTS.py
--rw-rw-rw-   0        0        0       42 2022-12-19 14:45:50.634770 pyRaTS-0.15/setup.cfg
--rw-rw-rw-   0        0        0     1113 2022-12-19 14:45:18.000000 pyRaTS-0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:12:36.265825 pyRaTS-0.20/
+-rw-rw-rw-   0        0        0     3446 2023-05-24 11:12:36.264829 pyRaTS-0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 11:12:36.235924 pyRaTS-0.20/pyRaTS/
+drwxrwxrwx   0        0        0        0 2023-05-24 11:12:36.262834 pyRaTS-0.20/pyRaTS/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 11:12:36.260841 pyRaTS-0.20/pyRaTS/src/pyRaTS.egg-info/
+-rw-rw-rw-   0        0        0     3446 2023-05-24 11:12:36.000000 pyRaTS-0.20/pyRaTS/src/pyRaTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-24 11:12:36.000000 pyRaTS-0.20/pyRaTS/src/pyRaTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:12:36.000000 pyRaTS-0.20/pyRaTS/src/pyRaTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 11:12:36.000000 pyRaTS-0.20/pyRaTS/src/pyRaTS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    98664 2023-05-21 22:10:41.000000 pyRaTS-0.20/pyRaTS/src/pyRaTS.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 11:12:36.265825 pyRaTS-0.20/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-05-22 09:27:43.000000 pyRaTS-0.20/setup.py
```

### Comparing `pyRaTS-0.15/PKG-INFO` & `pyRaTS-0.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRaTS
-Version: 0.15
+Version: 0.20
 Summary: processing of (RAndom) TimeSeries for vibration fatigue
 Home-page: https://github.com/ArvidTrapp/pyRaTS
 Author: Arvid Trapp
 Author-email: arvid.trapp@hm.edu
 Maintainer: Arvid Trapp, Peter Wolfsteiner
 Maintainer-email: arvid.trapp@hm.edu
 Keywords: vibration fatigue, non-stationarity matrix, structural dynamics,Fatigue Damage Spectrum
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 pyRaTS - processing of (RAndom) TimeSeries for vibration fatigue
 ---------------------------------------------
 
-Providing an object-oriented framework to analyze and process time series with the focus on random vibration fatigue. 
+Providing an object-oriented framework to analyze and process time series with the focus on random vibration fatigue. PyRaTS  is capable of handling single- and multi-channel, as well as single- and multi-process time series configurations. 
 Implementation of the non-stationarity matrix, the Fatigue Damage Spectrum and quasi-stationary signal definitions to deal with the challenges of non-stationary loading. 
 
 Installing this package
 -----------------------
 
 Use `pip` to install it by:
 
@@ -40,26 +40,24 @@
     import pyRaTS as ts
     import numpy as np
 
     # Defining the series by pseudo-random generator...
     T  = 10
     fs = 1024
     N  = T*fs
-    dt = 1/fs
-    t  = np.arange(N)/fs
     x  = np.random.randn(N)
 
     # Initialize series and some basic plots...
-    sig = ts.timeseries(x,t,name = 'sample timeseries')
+    sig = ts.timeseries(x,name = 'sample timeseries', fs = fs)
     sig.plot()
     sig.plot_prob()
     sig.plot_psd()
 
     # derive response series and some further basic plots...
-    respsig, _ = sig.der_sdofResponse(fD = 50)
+    respsig = sig.der_sdofResponse(fD = 50)
     respsig.plot_psd()
     respsig.plot_ls()
 	
 Some methods for a statistical analysis of random time series / estimation of statistical descriptors
 -----------------------------------------
 
 	* spectral moments (est_specMoms)
```

### Comparing `pyRaTS-0.15/pyRaTS/src/pyRaTS.egg-info/PKG-INFO` & `pyRaTS-0.20/pyRaTS/src/pyRaTS.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRaTS
-Version: 0.15
+Version: 0.20
 Summary: processing of (RAndom) TimeSeries for vibration fatigue
 Home-page: https://github.com/ArvidTrapp/pyRaTS
 Author: Arvid Trapp
 Author-email: arvid.trapp@hm.edu
 Maintainer: Arvid Trapp, Peter Wolfsteiner
 Maintainer-email: arvid.trapp@hm.edu
 Keywords: vibration fatigue, non-stationarity matrix, structural dynamics,Fatigue Damage Spectrum
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 pyRaTS - processing of (RAndom) TimeSeries for vibration fatigue
 ---------------------------------------------
 
-Providing an object-oriented framework to analyze and process time series with the focus on random vibration fatigue. 
+Providing an object-oriented framework to analyze and process time series with the focus on random vibration fatigue. PyRaTS  is capable of handling single- and multi-channel, as well as single- and multi-process time series configurations. 
 Implementation of the non-stationarity matrix, the Fatigue Damage Spectrum and quasi-stationary signal definitions to deal with the challenges of non-stationary loading. 
 
 Installing this package
 -----------------------
 
 Use `pip` to install it by:
 
@@ -40,26 +40,24 @@
     import pyRaTS as ts
     import numpy as np
 
     # Defining the series by pseudo-random generator...
     T  = 10
     fs = 1024
     N  = T*fs
-    dt = 1/fs
-    t  = np.arange(N)/fs
     x  = np.random.randn(N)
 
     # Initialize series and some basic plots...
-    sig = ts.timeseries(x,t,name = 'sample timeseries')
+    sig = ts.timeseries(x,name = 'sample timeseries', fs = fs)
     sig.plot()
     sig.plot_prob()
     sig.plot_psd()
 
     # derive response series and some further basic plots...
-    respsig, _ = sig.der_sdofResponse(fD = 50)
+    respsig = sig.der_sdofResponse(fD = 50)
     respsig.plot_psd()
     respsig.plot_ls()
 	
 Some methods for a statistical analysis of random time series / estimation of statistical descriptors
 -----------------------------------------
 
 	* spectral moments (est_specMoms)
```

### Comparing `pyRaTS-0.15/pyRaTS/src/pyRaTS.py` & `pyRaTS-0.20/pyRaTS/src/pyRaTS.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
+
 """
 PYthon module for the processing of RAndom vibration TimeSeries - pyRaTS
+Version: 0.2
 @author: Arvid Trapp, Munich University of Applied Sciences
 arvid.trapp@hm.edu
 """
 
 from cmath import log
 from subprocess import call
 import numpy as np
@@ -26,15 +28,14 @@
 
 - get_tfSDOF:               obtain basic SDOF-system's transfer function
 - get_twoSidedFourierCoeff: mirror one-sided Fourier coefficients
 - get_tf:                   prepare linear transfer function
 - get_nonstat:              postprocess calculation of non-stationarity matrix
 - get_GaussianSeries:       generate stationary Gaussian time series
 - get_weightFunc:           get weighting function (optimization)
-- get_weightFunc_WOI:       get weighting function (optimization)
 - get_lsQsDirlik:           get load spectra for quasi-stationary loading using Dirlik
 
 - soe_lsEquivalent:         SOE for load spectral equivalence
 - soe_FDSEquivalent:        SOE for FDS equivalence
 
 - plot_fds:                 plot FDS of (multiple) signals
 - plot_nonstat:             plot non-stationarity matrix
@@ -110,14 +111,16 @@
     SOURCES:
         P. Wolfsteiner, A. Trapp, Fatigue life due to non-Gaussian excitation – An analysis of the fatigue damage spectrum using higher order spectra, International Journal of Fatigue 127 (2019) 203–216
     '''      
     Omega   = 2*np.pi*fvec
     omega_0 = fD*2*np.pi/np.sqrt(1-D**2)
     if func == 'acc2dis':
         H = 1/(-Omega**2+2*D*omega_0*1j*Omega+omega_0**2)
+    elif func == 'acc2dis4mm':
+        H = 1000/(-Omega**2+2*D*omega_0*1j*Omega+omega_0**2)
     elif func == 'acc2vel':
         H = 1j*Omega/(-Omega**2+2*D*omega_0*1j*Omega+omega_0**2)
     elif func == 'acc2acc':    
         H = -Omega**2/(-Omega**2+2*D*omega_0*1j*Omega+omega_0**2)
     return H  
 
 def get_analyticalSignal(Xts,ffper,fl,fu):
@@ -250,15 +253,15 @@
 
     nonstat['Axx']      = nonstat['Rxx']/nonstat['Rxx_stat']
     nonstat['Axx_sym']  = nonstat['Rxx_sym']/nonstat['Rxx_stat']
     nonstat['Axx_stat'] = nonstat['Rxx_stat']/nonstat['Rxx_stat']
     nonstat['Mxx']      = 3*nonstat['Rxx']
     nonstat['Mxx_sym']  = 3*nonstat['Rxx_sym']
     nonstat['Mxx_stat'] = 3*nonstat['Rxx_stat']
-    nonstat['kurtosis'] = np.sum(nonstat['Mxx'])/np.sum(nonstat['Rxx_stat'])-3
+    nonstat['kurtosis'] = np.sum(nonstat['Mxx'])/np.sum(nonstat['Rxx_stat'])
     nonstat['Kxx']      = nonstat['Rxx']-nonstat['Rxx_stat']
     nonstat['Kxx_sym']  = nonstat['Rxx_sym']-nonstat['Rxx_stat']
     nonstat['Kxx_stat'] = nonstat['Rxx_stat']-nonstat['Rxx_stat'] # np.zeros([Nf, Nf])
     nonstat['Cxx']      = 3*(nonstat['Rxx']-nonstat['Rxx_stat'])
     nonstat['Cxx_sym']  = 3*(nonstat['Rxx_sym']-nonstat['Rxx_stat'])
     nonstat['Cxx_stat'] = 3*(nonstat['Rxx_stat']-nonstat['Rxx_stat']) # np.zeros([Nf, Nf])
     diag_m4             = np.sqrt(np.diag(real_mue4))
@@ -318,34 +321,16 @@
     '''
     p = x[:inp['R']]
     wfunc = x[inp['R']:].reshape((inp['R'], inp['res']*inp['Nf']))
     wfunc_it = np.zeros((inp['R'],len(inp['fpsd'])))
     fAxis = np.linspace(0,inp['fend'],inp['res']*inp['Nf'])
     fAxis = np.append(fAxis,[fAxis[-1] + np.mean(np.diff(fAxis)),inp['fpsd'][-1]])
     for rr in range(inp['R']):
-        # wfunc_it[rr] = np.interp(inp['fpsd'],np.linspace(0,inp['fpsd'][-1],inp['res']*inp['Nf']),wfunc[rr])
-        # interpfunc   = sp.interpolate.interp1d(fAxis,wfunc[rr],kind = 'cubic')
         interpfunc   = sp.interpolate.interp1d(fAxis,np.append(wfunc[rr],[1,1]))
         wfunc_it[rr] = interpfunc(inp['fpsd'])
-        # wfunc_it[rr] = glsInterp(np.linspace(0,inp['fpsd'][-1],inp['res']*inp['Nf']),wfunc[rr],inp['fpsd'])
-    return wfunc_it
-
-def get_weightFunc_WOI(x,inp):
-    ''' get weighting function (optimization)
-    >>> for internal use <<<  
-    SOURCES:
-        Wolfsteiner, P., Trapp, A., and Fertl, L., 'Random vibration fatigue with non-stationary loads using an extended fatigue damage spectrum with load spectra', ISMA 2022 Conference
-    '''
-    p = x[:inp['R']]
-    wfunc = x[inp['R']:].reshape((inp['R'], inp['res']*inp['Nf']))
-    wfunc_it = np.zeros((inp['R'],len(inp['fpsd'])))
-    fAxis = np.linspace(0,inp['fpsd'][-1],inp['res']*inp['Nf'])
-    for rr in range(inp['R']):
-        interpfunc   = sp.interpolate.interp1d(fAxis,wfunc[rr])
-        wfunc_it[rr] = interpfunc(inp['fpsd'])
     return wfunc_it
 
 def get_lsQsDirlik(psd,fpsd,si_X,weights): 
     ''' get load spectra for quasi-stationary loading using Dirlik 
     >>> for internal use >>>
     '''
     dfpsd = fpsd[1]-fpsd[0]
@@ -362,17 +347,17 @@
     R  = (out['alpha2']-Xm-D1**2)/(1-out['alpha2']-D1+D1**2)
     D2 = (1-out['alpha2']-D1+D1**2)/(1-R)
     D3 = 1-D1-D2
     Q  = 1.25*(out['alpha2']-D3-D2*R)/D1
     
     Z  = si_X/np.sqrt(out['specm0'])[:,None] 
 
-    out['DK_lk']   = D1[:,None]*np.exp(-Z/Q[:,None]) + D2[:,None]*np.exp(-Z**2/(2*R[:,None]**2)) + D3[:,None]*np.exp(-Z**2/2)
-    out['DK_lk_ps']   = out['DK_lk']*out['ny_p'][:,None]
-    return np.matmul(weights,out['DK_lk_ps'])
+    out['DK_ls']   = D1[:,None]*np.exp(-Z/Q[:,None]) + D2[:,None]*np.exp(-Z**2/(2*R[:,None]**2)) + D3[:,None]*np.exp(-Z**2/2)
+    out['DK_ls_ps']   = out['DK_ls']*out['ny_p'][:,None]
+    return np.matmul(weights,out['DK_ls_ps'])
 
 def soe_lsEquivalent(x,inp):
     ''' system of equations (SOE) for load spectral equivalence
     >>> for internal use <<< 
     SOURCES:
         Wolfsteiner, P., Trapp, A., and Fertl, L., 'Random vibration fatigue with non-stationary loads using an extended fatigue damage spectrum with load spectra', ISMA 2022 Conference 
     '''    
@@ -430,15 +415,15 @@
             plt.legend()
             plt.grid(True)
         plt.show()
     except:
         print('Input:',inp)
         warnings.warn('function "plot_fds()" cannot be carried out')
 
-def plot_nonstat(inp,func = 'Mxx'):
+def plot_nonstat(inp,func = 'Mxx',lim = None):
     '''
     plot non-stationarity matrix
     INPUTS:
         :param inp:    dictionary
             non-stationary matrix dictionary
         :param func:   string
             function(s) to be plotted
@@ -542,29 +527,35 @@
             def_title = 'non-stationarity synchronicity matrix (symmetric)'
             def_clabl1 = '$\\rho_{{'+2*inp['var']+'}}$ ($\mu_4$-coverage: {p:.2f}%) [-]'.format(p = inp['m4rep'])
             def_clabl2 = '$A_{'+2*inp['var']+',stat}$ [-]'   
         elif func == 'rhoxx':
             quant = [inp['rhoxx_sym']]
             def_title = 'non-stationarity synchronicity matrix (symmetric)'
             def_clabl1 = '$\\rho_{{'+2*inp['var']+'}}$ ($\mu_4$-coverage: {p:.2f}%) [-]'.format(p = inp['m4rep'])
-        cnt = 0    
-        for qq in quant:
+        cnt = 0 
+        figs = []   
+        for cc,nonstat in enumerate(quant):
             cnt = cnt +1 
             fig = plt.figure()
-            pos = plt.imshow(qq, extent=[0, inp['f_end'], inp['f_end'], 0])   
+            if lim is not None:
+                pos = plt.imshow(nonstat, extent=[inp['f_start'], inp['f_end'], inp['f_end'], inp['f_start']],vmin=lim[0], vmax=lim[1])   
+            else:
+                pos = plt.imshow(nonstat, extent=[inp['f_start'], inp['f_end'], inp['f_end'], inp['f_start']])   
             plt.xlabel("$f_1$ [Hz]")
             plt.ylabel("$f_2$ [Hz]")
             plt.grid(True)
             if cnt == 1:
                 plt.title(def_title)
-                fig.colorbar(pos,label = def_clabl1)
+                cb = fig.colorbar(pos,label = def_clabl1)
             else: 
                 plt.title(def_title[4:])
-                fig.colorbar(pos,label = def_clabl2)
-            plt.show()      
+                cb = fig.colorbar(pos,label = def_clabl2)
+            plt.show()
+            figs.append(fig)     
+        return figs
 
 def plot_lsEquivalent(x,inp=None):
     ''' plot function for SOE: load spectral equivalence 
     >>> for internal use >>>
     '''
     global optiparam
 
@@ -621,277 +612,647 @@
         si_it = np.interp(optiparam['ni_eval'],np.flip(ls_it),np.flip(si_X))
         res[ff] = np.sum((optiparam['si_eval'][ff]-si_it)**2)
     print(np.sum(res))  
     
     print('Iteration: ',optiparam['it'])
     optiparam['it'] += 1 
 
+
+class timeseries: 
+    ''' outer class definition
+    outer object for arranging time series components (arr) and channel definition (chan)
+    '''
+    '''
+        Attributes
+        ----------
+        arr:        array of tsarr-objects for managing multi-channel multi-process data
+        chan:       array of tsarr-objects for managing multi-channel data
+        ----------
+        nc:         numper of channels
+        np:         number of processes 
+        scsp:       Is single-channel, single-process?
+        psdmx:      PSD Matrix
+        fpsdmx:     frequency vector for PSD Matrix
+        dfpsdmx:    resolution of PSD Matrix
+        qsls:       quasi-stationary load spectra
+        
+        ...various attributes from tsarr        
+        ----------
+        Methods
+        ---------- 
+        genChan():      internal: generate channel attribute to simplify multi-process configurations
+        whos():         generate console output for configuration output
+        callPlots():    internal: callPlots
+        callProps():    internal: callProps
+        callMethods():  internal: callMethods
+        est_qsls():     estimate quasi-stationary load spectrum
+        est_stats():    init call: estimate key statistical values
+        est_psdmx():    estimate PSDs and CPSDs (timeseries class)
+        plot_psdmx():   plot PSD Matrix  
+        ...various methods from tsarr 
+    '''
+            
+    def __init__(self, srs,var = 'x', **kwargs):
+        # prepare timeseries array (microstructure)
+        self.arr = []
+        if isinstance(srs,(np.ndarray,dict,tsarr)):
+            srs = [[srs]]
+        elif isinstance(srs[0],(np.ndarray,dict,tsarr)):
+            srs = [srs]
+            
+        # generate timeseries array (microstructure)
+        for ii,chan in enumerate(srs):
+            self.arr.append([])
+            for proc in chan:
+                if type(proc) == dict:
+                    if 'psd' in proc.keys(): # Dictionary with PSD Input -> random time series
+                        kwargs['x'],_ = get_GaussianSeries(proc)
+                    # else: Dictionary with time series input
+                    kwargs.update(proc)
+                    self.arr[ii].append(tsarr(**kwargs))
+                elif type(proc) == tsarr:    # tsarr input
+                    self.arr[ii].append(proc)
+                else:                        # list with time series input
+                    self.arr[ii].append(tsarr(proc, **kwargs))
+        self.var = var
+        
+        # provide a channel array (easy access, option: replacing it with a property function)
+        if self.np > 1:
+            self.genChan()
+        
+        # basic statistical properties
+        self.est_stats()
+        
+        # determine if single channel single process     
+        if self.nc == 1 and self.np == 1: 
+            self.scsp = True
+        else:
+            self.scsp = False
+            # auto-naming of subelements if nothing was passed
+            if np.all([item == 'x' for sublist in self.vars for item in sublist]):
+                    for cc,chan in enumerate(self.arr):
+                        for pp,proc in enumerate(chan):
+                            if self.np == 1:
+                                proc.var = self.var + '_{c=' + str(cc+1) + '}'
+                            elif self.nc == 1:
+                                proc.var = self.var + '_{p=' + str(pp+1) + '}'
+                            else:
+                                proc.var = self.var + '_{c=' + str(cc+1) + ',p=' + str(pp+1) + '}'
     
-###############################################################################
-class series: 
+    def genChan(self):   
+        '''generate channel attribute to simplify multi-process configurations'''
+        self.chans = []                
+        if self.nc == 1:
+            self.chans.append(tsarr(np.concatenate(self.xs)[0],np.mean(self.fss),var = self.var,unit = self.arr[0][0].unit)) 
+        else:       
+            for cc,chan in enumerate(self.arr):
+                self.chans.append(tsarr(self.x[cc],fs = self.fs[cc],var = self.var + '_{c=' + str(cc+1) + '}',unit = self.arr[0][0].unit))                
+                
+    
+    # timeseries properties                     
+    @property
+    def nc(self): # number of channels
+        return len(self.arr)
+    @property
+    def np(self): # number of processes
+        return len(self.arr[0])  
+    
+    # properties that return channel perspective
+    @property
+    def x(self): # data
+        if self.nc == 1:
+            return self.chan[0].x
+        else:
+            return [np.concatenate(chan) for chan in self.xs]
+    @property
+    def t(self): # time vector
+        if self.nc == 1:
+            return self.chan[0].t
+        else:
+            if np.all([chanT == self.T[0] for chanT in self.T]):
+                return self.chan[0].t
+            else:
+                return [np.concatenate(chan) for chan in self.ts]
+    @property
+    def T(self): # duration
+        if self.nc == 1:
+            return self.chan[0].T
+        else:
+            return [np.sum(chan) for chan in self.Ts]
+    @property
+    def Tsig(self): # duration if all T the same
+        if np.all([chanT == self.T[0] for chanT in self.T]):
+            return self.T[0]
+        else:
+            return None
+    @property
+    def N(self): # number of samples
+        if self.nc == 1:
+            return self.chan[0].N
+        else:
+            return [np.sum(chan) for chan in self.Ns]
+    @property
+    def Nsig(self):  # number of samples if all N the same
+        if np.all([chanN == self.N[0] for chanN in self.N]):
+            return self.N[0]
+        else:
+            return None
+    @property
+    def fs(self):  # sampling rate
+        if self.nc == 1:
+            return self.chan[0].fs
+        else:
+            return [np.mean(chan) for chan in self.fss]
+    @property
+    def fssig(self):  # sampling rate if all fs the same
+        if np.all([chanfs == self.fs[0] for chanfs in self.fs]):
+            return self.fs[0]
+        else:
+            return None    
+    # properties that return tsarr perspective (multi-process)            
+    @property
+    def xs(self):  # multi-process return of x
+        return self.callProps('x')    
+    @property
+    def ts(self): # multi-process return of t
+        return self.callProps('t')   
+    @property
+    def vars(self): # multi-process return of var
+        return self.callProps('var')  
+    @property
+    def Ts(self): # multi-process return of T
+        return self.callProps('T')    
+    @property
+    def Ns(self): # multi-process return of N
+        return self.callProps('N')     
+    @property
+    def fss(self): # multi-process return of fs
+        return self.callProps('fs')   
+    @property
+    def units(self): # multi-process return of units
+        return self.callProps('unit')  
+    @property
+    def chan(self): # multi-channel array (np = 1)
+        if self.np == 1:
+            return [chan[0] for chan in self.arr]
+        else:
+            return self.chans
+          
+    def whos(self):
+        ''' generate console output for configuration output  '''
+        if self.nc == 1:
+            str1 = 'single-channel'
+        else:
+            str1 = 'multi-channel (nc = {})'.format(self.nc)
+        if self.np == 1:
+            str2 = 'single-process'
+        else:
+            str2 = 'multi-process (np = {})'.format(self.np)
+        print(str1,str2)
+         
+    def callPlots(self,passmethod,*args,access='chan',**kwargs):
+        ''' manage plot functions for timeseries class
+        >>> for internal use >>>
+        '''
+        if access == 'chan':
+            fig, axs = plt.subplots(self.nc, 1)
+        elif access == 'proc':
+            fig, axs = plt.subplots(self.nc, self.np)
+        elif access == 'comp':
+            fig, axs = plt.subplots(1, 1)
+            cls = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf']
+        else:
+            warnings.warn('internal calling error')
+        axs = np.atleast_2d(axs)
+        
+        if access == 'chan':
+            for cc,chan in enumerate(self.chan):
+                    callmethd = getattr(chan,passmethod)
+                    callmethd(*args,ax=axs[0,cc],**kwargs) 
+        elif access == 'proc':
+            for cc,chan in enumerate(self.arr):
+                for pp,proc in enumerate(chan):
+                    callmethd = getattr(proc,passmethod)
+                    callmethd(*args,ax=axs[cc,pp],**kwargs) 
+        elif access == 'comp':
+            for cc,chan in enumerate(self.chan):
+                    callmethd = getattr(chan,passmethod)
+                    callmethd(*args,ax=axs[0,0],**kwargs) 
+            for nn,line in enumerate(axs[0,0].lines):
+                line.set_color(cls[nn % 10])       
+            axs[0,0].legend()
+        else:
+            warnings.warn('internal calling error')        
+        plt.show()
+        return axs
+                        
+    def callProps(self,passprop):
+        ''' manage calling of properties for timeseries class
+        >>> for internal use >>>
+        '''
+        retvalues = []
+        for cc,chan in enumerate(self.arr):
+            retvalues.append([])
+            for pp,proc in enumerate(chan):
+                getprop = getattr(proc,passprop)
+                retvalues[cc].append(getprop) 
+        return retvalues    
+        
+    def callMethods(self,passmethod,*args,access='chan',**kwargs):
+        ''' manage calling of methods for timeseries class
+        >>> for internal use >>>
+        '''
+        retvalues = []
+        if access == 'chan':
+            for cc,chan in enumerate(self.chan):
+                retvalues.append([])
+                callmethd = getattr(chan,passmethod)
+                retvalues[cc].append(callmethd(*args,**kwargs))
+        elif access == 'proc':
+            for cc,chan in enumerate(self.arr):
+                retvalues.append([])
+                for proc in chan:
+                    callmethd = getattr(proc,passmethod)
+                    retvalues[cc].append(callmethd(*args,**kwargs)) 
+        else:
+            warnings.warn('internal calling error')        
+        return retvalues  
+            
+    def est_qsls(self,si_X = None):
+        ''' estimate quasi-stationary load spectrum
+        INPUTS:
+        :param  si_X: vector
+            evaluate spectral load spectra estimators for given amplitude vector     
+        SOURCES:
+            A. Trapp, P. Wolfsteiner, Fatigue assessment of non-stationary random loading in the frequency domain by a quasi-stationary Gaussian approximation, International Journal of Fatigue 148 (2021) 106214     
+        ''' 
+        if self.scsp:
+            self.qsls = self.arr[0,0].ls
+            return
+        self.qsls = []
+        for chan in self.arr:
+            maxvals = [proc.stat['maxvalue'] for proc in chan]
+            overallmax = np.max(maxvals)
+            ls = ({'si_X': np.linspace(0,overallmax*1.1,1000)})
+            ls['ni_X'] = np.zeros(ls['si_X'].shape)
+            for proc in chan:
+                proc.est_ls(si_X = ls['si_X'])
+                ls['ni_X'] = ls['ni_X'] + proc.ls['ni_X'] 
+            self.qsls.append(ls) 
+            
+    def est_stats(self): 
+        ''' estimate key statistical values (timeseries class)
+        -> called by __init__
+        '''        
+        self.stat = {'mean': [np.mean(chan.x) for chan in self.chan]}
+        self.stat['std'] = [np.std(chan.x) for chan in self.chan]
+        self.stat['var'] = [np.var(chan.x) for chan in self.chan]
+        self.stat['skewness'] = [sp.stats.skew(chan.x) for chan in self.chan]
+        self.stat['kurtosis'] = [sp.stats.kurtosis(chan.x)+3 for chan in self.chan]
+        xMV  = [chan.x for chan in self.chan]
+        self.stat['cov'] = np.cov(xMV)
+        self.stat['corrcoef'] = np.corrcoef(xMV)
+        self.stat['largestvalues']  = [np.max(chan.x) for chan in self.chan]
+        self.stat['smallestvalues'] = [np.min(chan.x) for chan in self.chan]
+        self.stat['maxvalues']      = np.max(np.abs([self.stat['smallestvalues'],self.stat['largestvalues'] ]),axis = 0)
+        self.stat['max']            = self.stat['maxvalues'] 
+        self.stat['largestvalue']   = np.max(self.stat['largestvalues'])
+        self.stat['smallestvalue']  = np.min(self.stat['smallestvalues'])
+        self.stat['maxvalue']       = np.max(self.stat['maxvalues'])
+        self.stat['max']            = self.stat['maxvalue']  
+    
+    def est_psdmx(self,df = 1):  
+        ''' estimate PSDs and CPSDs (timeseries class)
+        INPUTS:
+        :param df:    scalar
+            frequency resolution of PSDmx
+        '''   
+        self.psdmx = np.empty((self.nc, self.nc), dtype=object)
+        for ii,chan1 in enumerate(self.chan):
+            for jj,chan2 in enumerate(self.chan):
+                self.fpsdmx,self.psdmx[ii,jj] = sp.signal.csd(chan1.x,chan2.x,chan1.fs,nperseg=round(chan1.fs/df))
+        self.dfpsdmx = np.mean(np.diff(self.fpsdmx)) 
+    
+    def plot_psdmx(self):
+        ''' plot PSD Matrix'''
+        if not hasattr(self, 'fpsdmx'):
+            self.est_psdmx()
+        fig,ax = plt.subplots(self.nc,self.nc)
+        ax = np.atleast_2d(ax)
+        
+        for ii in np.arange(self.nc):
+            for jj in np.arange(self.nc):
+                lbl = "$G_{" + self.chan[ii].var + self.chan[jj].var + "}" + ': \sigma^2$ = {:.3f}'.format(self.stat['cov'][ii,jj]) + ' [(' + self.chan[ii].unit + ')$^2$]'
+                if ii>jj: # Real/Imag
+                    ax[ii,jj].plot(self.fpsdmx,np.real(self.psdmx[ii,jj]),'k',label = 'Real, Cov = {:.3f}'.format(self.stat['cov'][ii,jj]) + ' [(' + self.chan[ii].unit + ')$^2$]') 
+                    ax2 = ax[ii,jj].twinx()
+                    ax2.plot(self.fpsdmx,np.imag(self.psdmx[ii,jj]),'r',label = 'Imag')
+                    ax2.legend()    
+                elif ii<jj:
+                    ax[ii,jj].plot(self.fpsdmx,np.abs(self.psdmx[ii,jj]),'k',label = 'Abs') 
+                    ax2 = ax[ii,jj].twinx()
+                    ax2.plot(self.fpsdmx,np.real(self.psdmx[ii,jj])/(np.sqrt(self.psdmx[ii,ii])*np.sqrt(self.psdmx[jj,jj])),'r',label = 'Coh')    
+                    ax2.set_ylim((-1,1)) 
+                    ax2.set_ylabel('Coherence [-]')  
+                    ax2.legend()                  
+                elif ii==jj:
+                    ax[ii,jj].plot(self.fpsdmx,self.psdmx[ii,jj],'k',label = lbl)         
+                ax[ii,jj].set_xlabel("f [Hz]")
+                ax[ii,jj].set_ylabel("$G_{" + self.chan[ii].var + self.chan[jj].var + "}$ [(" + self.chan[ii].unit  + ")$^2$/Hz]")
+                ax[ii,jj].legend()   
+                ax[ii,jj].grid(True) 
+                       
+    def plot(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot',*args,access = access, **kwargs)                           
+    def plot_psd(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot_psd',*args,access = access, **kwargs)                  
+    def plot_X(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot_X',*args,access = access, **kwargs)                    
+    def plot_prob(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot_prob',*args,access = access, **kwargs)          
+    def plot_ls(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot_ls',*args,access = access, **kwargs)   
+    def plot_pseudoDam(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot_pseudoDam',*args,access = access, **kwargs)    
+    def plot_tf(self,*args,access = 'chan',**kwargs):
+        return self.callPlots('plot_tf',*args,access = access, **kwargs)       
+                 
+    def est_psd(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('est_psd',*args,access = access, **kwargs)             
+    def est_ls(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('est_ls',*args,access = access, **kwargs)            
+    def est_dirlik(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('est_dirlik',*args,access = access, **kwargs)              
+    def est_fds(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('est_fds',*args,access = access, **kwargs)              
+    def est_nonstat(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('est_nonstat',*args,access = access, **kwargs)           
+    def der_statResponse(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('der_statResponse',*args,access = access, **kwargs)        
+    def der_sdofResponse(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_sdofResponse',*args,access = access, **kwargs))           
+    def der_sdofTransfer(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_sdofTransfer',*args,access = access, **kwargs))        
+    def der_response(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_response',*args,access = access, **kwargs))         
+    def der_highpass(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_highpass',*args,access = access, **kwargs)) 
+    def der_lowpass(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_lowpass',*args,access = access, **kwargs))     
+    def der_bandpass(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_bandpass',*args,access = access, **kwargs))
+    def der_deriviative(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_deriviative',*args,access = access, **kwargs))
+    def der_scale2max(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_scale2max',*args,access = access, **kwargs))
+    def der_lsEquivalent(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('der_lsEquivalent',*args,access = access, **kwargs) # TODO klappt das ueberhaupt bei Mehrkanaligkeit? Wie bei Mehrprozessinput?
+    def der_iFDS(self,*args,access = 'chan',**kwargs):
+        return self.callMethods('der_iFDS',*args,access = access, **kwargs)         # TODO klappt das ueberhaupt bei Mehrkanaligkeit?                                           
+    def der_qsSTFT(self,*args,access = 'chan',**kwargs):
+        return timeseries(self.callMethods('der_qsSTFT',*args,access = access, **kwargs))
+                          
+class tsarr:
     '''
         Attributes
         ----------
         x:         (load/response)-series
+        t:         time vector
+        dt:        time step
+        fs:        sampling frequency
+        T:         duration of timeseries
         N:         number of samples
         var:       variable name
         unit:      unit to be displayed in plots
         prob:      estimate of probability density function (PDF)
         grid:      grid for estimate of PDF
         pgauss:    Gaussian PDF of same variance
-        stat:      Dictionary of statistical indicators
+        stat:      dictionary of statistical indicators
         psd:       power spectral density (PSD)
         fpsd:      normalized frequency vector for PSD
         dfpsd:     increment of frequency vector for PSD
         Xos:       one-sided Fourier coefficients
         Xts:       two-sided Fourier coefficients
+                
         ----------
         Methods
         ---------- 
-        plot():         plot of series
-        est_prob():     estimate probability density function (PDF)
-        est_bstats():   estimate key statistical values 
-        est_psd_woFS(): estimate PSD via Welch, without temporal information
-        plot_psd():     plot power spectral density (PSD)
-        plot_prob():    plot probability density function (PDF)
+        plot():             plot time series
+        plot_psd():         plot PSD that was lastly estimated via est_psd()
+        plot_X():           plot abs of Fourier coefficients 
+        plot_tf():          plot transfer function (interpretation: object is transfer function) 
+        plot_ls(method):    plot load spectrum
+        plot_fds(idx):      plot FDSs of signal given bei calculation indices
+        plot_nonstat():     plot non-stationarity matrix
+
+        est_psd(df):                        estimate power spectral density (PSD) 
+        est_stats():                        estimate key statistical values
+        est_ls():                           derive/estimate load spectrum via RFC/DK
+        est_dirlik(m):                      estimate Dirlik load spectrum and damage 
+        est_fds(m,D,method,Nf,func):        estimate Fatigue Damage Spectrum
+        est_nonstat(Nf,fl,fu,olap,wfunc):   estimate non-stationary matrix
+
+        der_statResponse(f,H):          derive statistical response (PSD & Non-stat.-Matrix)
+        der_sdofResponse(fD, D, func):  derive response timeseries of single-degree-of-freedom system 
+        der_sdofTransfer(fD, D, func):  derive single-degree-of-freedom system's transfer functions
+        der_response(f,H):              derive timeseries of structural response for given transfer function
+        der_highpass(f):                derive timeseries of ideal high pass filtered signal
+        der_lowpass(f):                 derive timeseries of ideal low pass filtered signal
+        der_bandpass(f):                derive timeseries of ideal band pass filtered signal
+        der_scale2max(self,value):      derive timeseries scaled to reference value
+        der_deriviative(opt):           derive deriviative timeseries 
+        der_lsEquivalent():             derive quasi-stationary load definition on the basis of the load spectra of the Fatigue Damage Spectrum
+        der_iFDS():                     derive load definition on the basis of the inverse Fatigue Damage Spectrum
+        
+        get_analyticalSignal(fl,fu):                    get analytical signal
+        get_posTaperedAnalyticalSignal(fl,fu,wfunc):    get positive(!) tapered analytical signal
+        get_corrFactors(fbands,olap,wfunc):             get correction factors
         ----------   
     '''
-    def __init__(self, srs,var="x", unit="m/s$^2$", name = ''):
-        self.x   = srs               # inputseries
-        self.N   = self.x.size       # number of samples
+        
+    def __init__(self, x, fs=1, var="x", unit="m/s$^2$", name = '', **kwargs):
+        ''' Initialize underlying signal components that are managed by timeseries class '''
+        self.x    = x
+        self.N    = len(self.x)
         self.var  = var              # variable name
+        if self.var.count('_') > 1:  # clean up underscores
+            first_underscore = self.var.find('_')
+            cleantext = self.var[first_underscore+1:].replace('_', ',').replace('{', '').replace('}', '')
+            self.var = self.var[:first_underscore+1] + '{' + cleantext + '}'
         self.unit = unit             # unit of series
-        self.name = name
-        if name:
-            self.name = '(' + name + ')'
-        '''  basic methods (to be carried out when initialized)  '''
-        self.est_bstats()
-        self.est_psd_woFS()
-
-    @property # for storage efficiency
-    def Xts(self):                                      # two-sided Fourier coefficients
-        Xts_woShift = np.fft.fft(self.x)
-        return np.fft.fftshift(Xts_woShift)
-    @property # for storage efficiency
-    def Xos(self):                                      # one-sided Fourier coefficients
-        Xts_woShift = np.fft.fft(self.x)
-        Nos         = np.ceil((self.N+1)/2)             # number of one-sided Fourier coefficients
-        return Xts_woShift[0:int(Nos)] 
-
-    def plot(self):
-        ''' plot of series '''  
-        plt.figure()
-        plt.plot(self.x,'k')
-        plt.xlabel("index [-]")
-        plt.ylabel("$" + self.var + "$ [" + self.unit + "]")
-        plt.show()
-        plt.title('realization ' + self.name)
-
-    def est_bstats(self):
-        ''' estimate key statistical values 
-        -> called by __init__
-        '''        
-        self.stat = {'mean': np.mean(self.x)}
-        self.stat['std'] = np.std(self.x)
-        self.stat['var'] = np.var(self.x)
-        self.stat['skewness'] = sp.stats.skew(self.x)
-        self.stat['kurtosis'] = sp.stats.kurtosis(self.x)
-        
-        # probability density function
-        self.est_prob()
-        
-        # higher-order moments
-        maxorder = 7
-        moms  = np.zeros(maxorder)
-        hmoms = np.zeros(maxorder)
-
-        for ii in range(1,maxorder):
-            moms[ii] = sp.stats.moment(self.x,ii)
-            if ii > 2 :
-                hmoms[ii] = moms[ii]/(sp.stats.moment(self.x,moment=2)**(ii/2))
-        self.stat['moms'] = moms
-        self.stat['hmoms'] = hmoms
-        
-        # Extreme values and Peak factors
-        self.stat['largestvalue']   = np.max(self.x)
-        self.stat['smallestvalue']  = np.min(self.x)
-        self.stat['maxvalue']       = np.max(np.abs([self.stat['smallestvalue'],self.stat['largestvalue'] ]))
-        self.stat['max']            = self.stat['maxvalue']   
-
-    def est_prob(self,bins='auto'):
-        ''' calculate probability density function (PDF) 
-        -> called by est_bstats (thus indirect call by __init__)
-        INPUTS:
-        :param bins:    scalar or array-like
-            number of bins / vector of bin-edges
-        '''
-        self.prob, bin_edges = np.histogram(self.x, bins, density=True)
-        self.grid = (bin_edges[1:]+bin_edges[0:-1])/2
-        self.pgauss = 1/ np.sqrt(self.stat['var']*2*np.pi) * np.exp(-(self.grid- self.stat['mean'])**2 / (2 * self.stat['var']))
-
-    def est_psd_woFS(self):
-        ''' estimate power spectral density (PSD) via Welch, without any temporal information
-        -> called by __init__
-        '''
-        self.fpsd,self.psd = sp.signal.welch(self.x)
-        self.dfpsd          = np.mean(np.diff(self.fpsd)) 
-
-    def plot_psd(self):
-        ''' plot power spectral density (PSD) '''
-        plt.figure()
-        plt.plot(self.fpsd,self.psd,'k')
-        plt.xlabel("normalized frequency [x\pi rad/sample]")
-        plt.ylabel("$G_{" + self.var + self.var + "}$ [(" + self.unit + ")$^2$/Hz]")
-        plt.legend([r'$\sigma^2 =  ${:.3f}'.format(np.sum(self.psd*self.dfpsd)) + ' [(' + self.unit + ')$^2$]'])   
-        plt.grid(True)
-        plt.title('power spectral density ' + self.name)
-        plt.show()    
-
-    def plot_prob(self):
-        ''' plot probability density function (PDF) '''
-        plt.figure()
-        plt.plot(self.grid,self.prob,'k',label = "$p(" + self.var + ")$")
-        plt.plot(self.grid,self.pgauss,'g--',label = "$p_g(" + self.var + ")$")
-        plt.xlabel("$" + self.var + "$ [" + self.unit + "]")
-        plt.ylabel("$p(" + self.var + ")$ [-]")
-        plt.legend()
-        plt.grid(True)
-        plt.title('probability density function ' + self.name)
-        plt.show()
-
-###############################################################################
-# Inheritance of series for timeseries (including time stamp) 
-class timeseries(series):  
-    def __init__(self, srs, tvec=None,**kwargs):
-        '''
-            Attributes
-            ----------
-            t:         time vector
-            dt:        time step
-            fs:        sampling frequency
-            T:         duration of timeseries
-            ----------
-            Methods
-            ---------- 
-            plot():             plot time series
-            plot_psd():         plot PSD that was lastly estimated via est_psd()
-            plot_X():           plot abs of Fourier coefficients 
-            plot_tf():          plot transfer function (interpretation: object is transfer function) 
-            plot_ls(method):    plot load spectrum
-            plot_FDS(idx):      plot FDSs of signal given bei calculation indices
-            plot_nonstat():     plot non-stationarity matrix
-
-            est_psd():                          estimate power spectral density (PSD) 
-            est_stats():                        estimate key statistical values
-            est_ls():                           derive/estimate load spectrum via RFC/DK
-            est_dirlik(m):                      estimate Dirlik load spectrum and damage 
-            est_fds(m,D,method,Nf,func):        estimate Fatigue Damage Spectrum
-            est_nonstat(Nf,fl,fu,olap,wfunc):   estimate non-stationary matrix
-
-            der_statResponse(f,H):          derive statistical response (PSD & Non-stat.-Matrix)
-            der_sdofResponse(fD, D, func):  derive response timeseries of single-degree-of-freedom system 
-            der_sdofTransfer(fD, D, func):  derive single-degree-of-freedom system's transfer functions
-            der_response(f,H):              derive timeseries of structural response for given transfer function
-            der_highpass(f):                derive timeseries of ideal high pass filtered signal
-            der_lowpass(f):                 derive timeseries of ideal low pass filtered signal
-            der_bandpass(f):                derive timeseries of ideal band pass filtered signal
-            der_lsEquivalent():             derive quasi-stationary load definition on the basis of the load spectra of the Fatigue Damage Spectrum
-            der_iFDS():                     derive load definition on the basis of the inverse Fatigue Damage Spectrum
-            
-            get_analyticalSignal(fl,fu):                    get analytical signal
-            get_posTaperedAnalyticalSignal(fl,fu,wfunc):    get positive(!) tapered analytical signal
-            get_corrFactors(fbands,olap,wfunc):             get correction factors
-            ----------   
-        '''
-        if type(srs) is dict:
-            if 'var' in srs.keys():
-                kwargs.update({'var': srs['var']})
-            if 'unit' in srs.keys():
-                kwargs.update({'unit': srs['unit']})
-            srs,tvec = get_GaussianSeries(srs)  
-        if tvec is None:
-            tvec = np.linspace(0,1,len(srs))
-        super().__init__(srs,**kwargs)        
-        self.dt  = np.mean(np.diff(tvec)) 
-        self.fs  = 1/self.dt
+        self.name = name             # name of series
+        self.fs  = fs
+        self.dt  = 1/self.fs
         self.fNy = self.fs/2
         self.T   = self.N/self.fs
         self.df  = 1/self.T
         self.est_psd()
+        
+        if name:
+            self.name = '(' + name + ')'
+        
         self.est_stats()
         self.est_ls()
         self.FDScalcs = []
-
+        
     @property # for storage efficiency
     def t(self):                                        # time-vector
         return np.arange(0,self.N)/self.fs
+    
     @property # for storage efficiency
     def Xts(self):                                      # two-sided Fourier coefficients
         Xts_woShift = self.dt*np.fft.fft(self.x)
         return np.fft.fftshift(Xts_woShift)
+    
     @property # for storage efficiency
     def Xos(self):                                      # one-sided Fourier coefficients
         Xts_woShift = self.dt*np.fft.fft(self.x)
         Nos         = np.ceil((self.N+1)/2)             # number of one-sided Fourier coefficients
-        return Xts_woShift[0:int(Nos)]        
+        return Xts_woShift[0:int(Nos)]       
+     
     @property # for storage efficiency
     def fper(self):                                     # one-sided frequency vector
         frq_woShift = np.fft.fftfreq(self.N, self.dt)
         Nos         = np.ceil((self.N+1)/2)             # number of one-sided Fourier coefficients
         return np.abs(frq_woShift[0:int(Nos)])
+    
     @property # for storage efficiency
     def ffper(self):                                    # two-sided frequency vector
         frq_woShift = np.fft.fftfreq(self.N, self.dt)
         return np.fft.fftshift(frq_woShift) 
-
-    def est_psd(self,df = 1):
-        ''' estimate power spectral density (PSD) 
-        -> called by __init__
-        '''
-        self.fpsd,self.psd = sp.signal.welch(self.x,self.fs,nperseg=round(self.fs/df))
-        self.dfpsd = np.mean(np.diff(self.fpsd))
-        
-    def plot(self):
+                
+    def plot(self,ax = None):
         ''' plot timeseries
+        INPUTS:
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
         '''
-        legd = "$" + self.var + '$: $\sigma^2$ = {sigq: .2f} [({unit})$^2$]; $ \\beta $ = {beta: .2f} [-]'.format(sigq = self.stat['var'], unit = self.unit,beta = self.stat['kurtosis']) 
-        plt.figure()
-        plt.plot(self.t,self.x,'k',label = legd)    
-        plt.xlabel("t [s]")
-        plt.ylabel("$" + self.var + "$ [" + self.unit + "]")
-        plt.grid(True)
-        plt.legend()
-        plt.title('time series ' + self.name)
-        plt.show()
+        if ax is None:
+            fig, ax = plt.subplots()
+            
+        legd = "$" + self.var + '$: $\sigma^2$ = {sigq: .3f} [({unit})$^2$]; $ \\beta $ = {beta: .3f} [-]'.format(sigq = self.stat['var'], unit = self.unit,beta = self.stat['kurtosis']) 
+        ax.plot(self.t,self.x,'k',label = legd)    
+        ax.set_xlabel("t [s]")
+        ax.set_ylabel("$" + self.var + "$ [" + self.unit + "]")
+        ax.grid(True)
+        ax.legend()
+        ax.set_title('time series ' + self.name)
 
-    def plot_psd(self):
+    def plot_psd(self,ax = None):
         ''' plot PSD that was lastly estimated via est_psd()
+        INPUTS:
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
         '''
-        plt.figure()
-        plt.plot(self.fpsd,self.psd,'k')
-        plt.xlabel("f [Hz]")
-        plt.ylabel("$G_{" + self.var + self.var + "}$ [(" + self.unit + ")$^2$/Hz]")
-        plt.legend([r'$\sigma^2$ = {:.3f}'.format(np.sum(self.psd*self.dfpsd)) + ' [(' + self.unit + ')$^2$]'])   
-        plt.grid(True)
-        plt.title('power spectral density ' + self.name)
-        plt.show()
+        if ax is None:
+            fig, ax = plt.subplots()
+        varvgl = np.sum(self.psd*self.dfpsd)
+        lbl = "$G_{" + self.var + self.var + "}" + ': \sigma^2$ = {:.3f}'.format(self.stat['var']) + ' [(' + self.unit + ')$^2$]'
+        ax.plot(self.fpsd,self.psd,'k',label=lbl)
+        ax.set_xlabel("f [Hz]")
+        ax.set_ylabel("$G_{" + self.var + self.var + "}$ [(" + self.unit + ")$^2$/Hz]")
+        ax.legend()   
+        ax.grid(True)
+        ax.set_title('power spectral density ' + self.name)
                 
-    def plot_X(self):
+    def plot_X(self,ax = None):
         ''' plot abs of Fourier coefficients 
+        INPUTS:
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
         '''
-        plt.figure()
-        plt.plot(self.ffper,abs(self.Xts),'k')   
-        plt.xlabel("f [Hz]")
-        plt.ylabel("|$" + self.var.upper() + "$| [" + self.unit + "/Hz]")
-        plt.grid(True)
-        plt.title('(absolute) Fourier coefficients ' + self.name)
-        plt.show()      
-
-    def plot_tf(self,plot ='bode'):
+        if ax is None:
+            fig, ax = plt.subplots()
+        lbl = self.var[0].upper() + self.var[1:]
+        ax.plot(self.ffper,abs(self.Xts),'k',label = lbl)   
+        ax.set_xlabel("f [Hz]")
+        ax.set_ylabel("|$" + self.var[0].upper() + self.var[1:] + "$| [" + self.unit + "/Hz]")
+        ax.grid(True)
+        ax.set_title('(absolute) Fourier coefficients ' + self.name)   
+    
+    def plot_prob(self,ax = None):
+        ''' plot probability density function (PDF) 
+        INPUTS:
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
+        '''
+        if ax is None:
+            fig, ax = plt.subplots()    
+        ax.plot(self.grid,self.prob,'k',label = "$p(" + self.var + ")$")
+        ax.plot(self.grid,self.pgauss,'g--',label = "$p_g(" + self.var + ")$")
+        ax.set_xlabel("$" + self.var + "$ [" + self.unit + "]")
+        ax.set_ylabel("$p(" + self.var + ")$ [-]")
+        ax.legend()
+        ax.grid(True)
+        ax.set_title('probability density function ' + self.name)
+    
+    def plot_ls(self,method = None,ax = None):
+        ''' plot load spectrum
+        INPUTS:
+        :param method:    (list of) function handle(s)
+            function for load spectrum estimation
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
+        SOURCES:
+            - FLife - Vibration Fatigue by Spectral Methods: https://github.com/ladisk/FLife
+            - J. Slavič, M. Boltežar, M. Mršnik, M. Cesnik, J. Javh, Vibration fatigue by spectral methods: From structural dynamics to fatigue, Elsevier, 2020
+        '''
+        if ax is None:
+            fig, ax = plt.subplots()    
+        ax.semilogx(self.ls['ni_x'],self.ls['si_x'],'r',label='RFC[$'+self.var+'$]')
+        ax.semilogx(self.ls['ni_X'],self.ls['si_X'],'k',label='DK[$'+self.var+'$]')
+        ax.set_xlabel("cumulated cycles")
+        ax.set_ylabel("amplitudes [" + self.unit + "]")
+        ax.grid(True) 
+        ax.set_title('load spectrum ' + self.name)
+        ax.set_xlim(0.5, 1.2*max(self.ls['ni_x']))
+        if method != None:
+            sd   = FLife.SpectralData(input=(self.psd,self.fpsd))
+            if type(method) == type:
+                method = [method] # make method iterable
+            for pdfesti in method:
+                method_name = str(pdfesti)[::-1]
+                method_name = method_name[2:method_name.find(".")][::-1]
+                spdf = pdfesti(sd).get_PDF(self.ls['si_X'])
+                spdf = spdf/np.sum(spdf)
+                loadspectrum = np.cumsum(spdf)*self.T*self.stat['ny_p']
+                ax.semilogx(loadspectrum,self.ls['si_X'],label = method_name+'[$'+self.var+'$]')   
+        ax.legend()
+        
+    def plot_pseudoDam(self,m = np.linspace(3,8,61),ax = None):
+        ''' plot pseudo-damage
+        INPUTS:
+        :param m:    list
+            SN-curve exponents for evaluation
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
+        SOURCES:
+            ...
+        '''
+        if ax is None:
+            fig, ax = plt.subplots()   
+        
+        counts = np.hstack((self.ls['ni_x'][0],np.diff(self.ls['ni_x']))) 
+        sig_eq = []
+        for mm in m:    
+            dam_eq = np.sum(counts*self.ls['si_x']**mm)
+            sig_eq.append(dam_eq**(1/mm))     
+                    
+        ax.plot(m,sig_eq,'k',label='s_{eq}[$'+self.var+'$]')
+        ax.set_xlabel("SN curve exponents")
+        ax.set_ylabel("pseudo-damage [" + self.unit + "]")
+        ax.grid(True) 
+        ax.set_title('pseudo-damage ' + self.name) 
+        ax.legend()
+                                   
+    def plot_tf(self,plot ='bode',ax=None):
         ''' plot transfer function
+        INPUTS:
+        :param ax:    pyplot axis-object
+            for including plot in outer subplot call
         '''
         if plot.lower() == 'aphase':
             func1 = np.abs
             func2 = lambda x: np.unwrap(np.angle(x))
             tit1  = 'Fourier coefficients (absolute)'
             ylbl1 = "|$" + self.var.upper() + "$| [" + self.unit + "/Hz]"
             tit2  = 'Fourier coefficients (phase)'
@@ -906,67 +1267,115 @@
         else:
             func1 = np.real
             func2 = np.imag
             tit1  = 'Fourier coefficients (real)'
             ylbl1 = "Real[$" + self.var.upper() + "$] [" + self.unit + "/Hz]"
             tit2  = 'Fourier coefficients (imaginary)'
             ylbl2 = "Imag[$" + self.var.upper() + "$] [" + self.unit + "/Hz]"
-        fig, axs = plt.subplots(2)
-        axs[0].plot(self.fper,func1(self.Xos),'k')   
-        axs[0].set_xlabel("f [Hz]")
-        axs[0].set_ylabel(ylbl1)
-        axs[0].grid(True)
-        axs[0].set_title(tit1)
-        axs[1].plot(self.fper,func2(self.Xos),'k')   
-        axs[1].set_xlabel("f [Hz]")
-        axs[1].set_ylabel(ylbl2)
-        axs[1].grid(True)
-        axs[1].set_title(tit2)
-        fig.show() 
-
+        if ax is None:
+            fig, ax = plt.subplots(2)    
+        if type(ax) is not np.ndarray:
+            ax = np.array([ax,ax.twinx()]) 
+        ax[0].plot(self.fper,func1(self.Xos),'k')   
+        ax[0].set_xlabel("f [Hz]")
+        ax[0].set_ylabel(ylbl1)
+        ax[0].grid(True)
+        ax[0].set_title(tit1)
+        ax[1].plot(self.fper,func2(self.Xos),'r')   
+        ax[1].set_xlabel("f [Hz]")
+        ax[1].set_ylabel(ylbl2)
+        ax[1].grid(True)
+        ax[1].set_title(tit2)
+        
+    def est_prob(self,bins='auto'):
+        ''' calculate probability density function (PDF) 
+        -> called by est_stats (thus indirect call by __init__)
+        INPUTS:
+        :param bins:    scalar or array-like
+            number of bins / vector of bin-edges
+        '''
+        try:
+            self.prob, bin_edges = np.histogram(self.x, bins, density=True)
+            self.grid = (bin_edges[1:]+bin_edges[0:-1])/2
+            self.pgauss = 1/ np.sqrt(self.stat['var']*2*np.pi) * np.exp(-(self.grid- self.stat['mean'])**2 / (2 * self.stat['var']))
+        except:
+            print("PDF estimation went wrong (can appear for tf objects)")
+    
+    def est_psd(self,df = 1):
+        ''' estimate power spectral density (PSD) 
+        -> called by __init__
+        '''
+        self.fpsd,self.psd = sp.signal.welch(self.x,self.fs,nperseg=round(self.fs/df))
+        self.dfpsd = np.mean(np.diff(self.fpsd))    
+            
     def est_stats(self):
         ''' estimate key statistical values 
-        -> called by __init__
+        -> called by __init__     
         SOURCES:
             A.G. Davenport, Note on the distribution of the largest value of a random function with application to gust loading, Proceedings of the Institution of Civil Engineers 28 (2) (1964) 187–196
         '''    
+        self.stat = {'mean': np.mean(self.x)}
+        self.stat['std'] = np.std(self.x)
+        self.stat['var'] = np.var(self.x)
+        self.stat['skewness'] = sp.stats.skew(self.x)
+        self.stat['kurtosis'] = sp.stats.kurtosis(self.x)+3
+        
+        # probability density function
+        self.est_prob()
+        
+        # higher-order moments
+        maxorder = 7
+        moms  = np.zeros(maxorder)
+        hmoms = np.zeros(maxorder)
+
+        for ii in range(1,maxorder):
+            moms[ii] = sp.stats.moment(self.x,ii)
+            if ii > 2 :
+                hmoms[ii] = moms[ii]/(sp.stats.moment(self.x,moment=2)**(ii/2))
+        self.stat['moms'] = moms
+        self.stat['hmoms'] = hmoms
+        
+        # Extreme values and Peak factors
+        self.stat['largestvalue']   = np.max(self.x)
+        self.stat['smallestvalue']  = np.min(self.x)
+        self.stat['maxvalue']       = np.max(np.abs([self.stat['smallestvalue'],self.stat['largestvalue'] ]))
+        self.stat['max']            = self.stat['maxvalue']  
+        
         # spectral moments
         self.stat = {**self.stat, **est_specMoms(self.psd,self.fpsd)}
         # peak factors
         termPF                      = np.sqrt(2*np.log(self.stat['ny_0'] *self.T))
         self.stat['peakfactor']     = termPF + 0.57721566490153286061/termPF 
         self.stat['peakfactor_std'] = np.pi/ np.sqrt(6) / termPF
         self.stat['expectedpeak']   = self.stat['peakfactor'] *self.stat['std']
-        self.stat['expectedpeakscatter']   = self.stat['peakfactor_std'] *self.stat['std']  
-
+        self.stat['expectedpeakscatter']   = self.stat['peakfactor_std'] *self.stat['std'] 
+         
     def est_ls(self,si_X = None):
         ''' derive/estimate load spectrum via RFC/DK
         -> called by __init__
         '''
         cycles = np.array(list(rf.extract_cycles(self.x)))
         cycles = cycles[np.argsort(cycles[:,0])]
         cycles = np.flipud(cycles)
         ampls  = cycles[:,0]/2
         counts = cycles[:,2]   
-        self.lk = {'si_x': ampls, 'ni_x': np.cumsum(counts),'mues_x': cycles[:,1]}
-        self.lk['npeaks']    = len(ampls)
-        self.lk['npeaks_ps'] = self.lk['npeaks']/self.T
+        self.ls = {'si_x': ampls, 'ni_x': np.cumsum(counts),'mues_x': cycles[:,1]}
+        self.ls['npeaks']    = len(ampls)
+        self.ls['npeaks_ps'] = self.ls['npeaks']/self.T
         zero_crossings = np.where(np.diff(np.sign(self.x)))[0]
-        self.lk['nzerocrossings'] = round(len(zero_crossings)/2)
-        self.lk['nzerocrossings_ps'] = self.lk['nzerocrossings']/self.T
+        self.ls['nzerocrossings'] = round(len(zero_crossings)/2)
+        self.ls['nzerocrossings_ps'] = self.ls['nzerocrossings']/self.T
         if np.any(si_X) == None: # no specification
-            self.lk['si_X'] = np.linspace(1.2*self.lk['si_x'][0],0,1000)
+            self.ls['si_X'] = np.linspace(1.2*self.ls['si_x'][0],0,1000)
         elif np.isscalar(si_X): # given limit
-            self.lk['si_X'] = np.linspace(si_X,0,1000)   
+            self.ls['si_X'] = np.linspace(si_X,0,1000)   
         else: # given vector
-            self.lk['si_X'] = si_X
+            self.ls['si_X'] = si_X
         self.est_dirlik()
-        if isinstance(self,qstimeseries):
-            self.est_qsLS()
-
+            
     def est_dirlik(self,m = 1):
         ''' estimate Dirlik load spectrum and damage 
         INPUTS:
         :param m:    scalar
             S-N-curve exponent
         SOURCES:
             - T. Dirlik, Application of computers in fatigue analysis. PhD Thesis, University of Warwick, 1985
@@ -974,55 +1383,37 @@
         '''
         Xm = self.stat['specm1']/self.stat['specm0']*np.sqrt(self.stat['specm2']/self.stat['specm4'])
         D1 = 2*(Xm-self.stat['alpha2']**2)/(1+self.stat['alpha2']**2)
         R  = (self.stat['alpha2']-Xm-D1**2)/(1-self.stat['alpha2']-D1+D1**2)
         D2 = (1-self.stat['alpha2']-D1+D1**2)/(1-R)
         D3 = 1-D1-D2
         Q  = 1.25*(self.stat['alpha2']-D3-D2*R)/D1
-        Z  = self.lk['si_X']/(np.sqrt(self.stat['specm0']))    
+        Z  = self.ls['si_X']/(np.sqrt(self.stat['specm0']))    
 
-        self.lk['DK_pk']   = (D1/Q*np.exp(-Z/Q) + D2*Z/R**2*np.exp(-Z**2/(2*R**2)) + D3*Z*np.exp(-Z**2/2) ) / (np.sqrt(self.stat['specm0']))
-        self.lk['DK_lk']   = D1*np.exp(-Z/Q) + D2*np.exp(-Z**2/(2*R**2)) + D3*np.exp(-Z**2/2)
-        self.lk['DK_lkps'] = self.lk['DK_lk']*self.stat['ny_p']
-        self.lk['ni_X']    = self.lk['DK_lkps']*self.T 
-        self.lk['DK_D']    = self.stat['ny_p']*np.sqrt(self.stat['specm0'])**m*(D1*Q**m*sp.special.gamma(1+m)+np.sqrt(2)**m*sp.special.gamma(1+m/2)*(D2*abs(R)**m+D3))              
-
-    def plot_ls(self,method = None):
-        ''' plot load spectrum
-        INPUTS:
-        :param method:    (list of) function handle(s)
-            function for load spectrum estimation
-        SOURCES:
-            - FLife - Vibration Fatigue by Spectral Methods: https://github.com/ladisk/FLife
-            - J. Slavič, M. Boltežar, M. Mršnik, M. Cesnik, J. Javh, Vibration fatigue by spectral methods: From structural dynamics to fatigue, Elsevier, 2020
+        self.ls['DK_pk']   = (D1/Q*np.exp(-Z/Q) + D2*Z/R**2*np.exp(-Z**2/(2*R**2)) + D3*Z*np.exp(-Z**2/2) ) / (np.sqrt(self.stat['specm0']))
+        self.ls['DK_ls']   = D1*np.exp(-Z/Q) + D2*np.exp(-Z**2/(2*R**2)) + D3*np.exp(-Z**2/2)
+        self.ls['DK_lsps'] = self.ls['DK_ls']*self.stat['ny_p']
+        self.ls['ni_X']    = self.ls['DK_lsps']*self.T 
+        self.ls['DK_D']    = self.stat['ny_p']*np.sqrt(self.stat['specm0'])**m*(D1*Q**m*sp.special.gamma(1+m)+np.sqrt(2)**m*sp.special.gamma(1+m/2)*(D2*abs(R)**m+D3))              
+
+    def der_qsSTFT(self,N = None,alpha=0.99):
+        if N == None:
+            N = self.fs
+        '''
+        |X(f,t)|
+        np.random.rand() [0,1] -> 
+        Xn(f,t) = complex(|X(f,t)|*cos(),|X(f,t)|*sin())
+        |Xn(f,t)| = |X(f,t)|
+        {ifft(Xn(f,t=1)), ifft(Xn(f,t=2)), ifft(Xn(f,t=…))}
+        {wt(ifft(Xn(f,t=1))), ifft(Xn(f,t=2)), ifft(Xn(f,t=…))}
+        scipy.signal.windows.tukey
         '''
-        plt.figure()
-        plt.semilogx(self.lk['ni_x'],self.lk['si_x'],'r',label='RFC[$'+self.var+'$]')
-        plt.semilogx(self.lk['ni_X'],self.lk['si_X'],'k',label='DK[$'+self.var+'$]')
-        if isinstance(self,qstimeseries):
-            plt.semilogx(self.qs['ni_X'],self.qs['si_X'],'b',label='QS[DK[$'+self.var+'$]]')
-        plt.xlabel("cumulated cycles")
-        plt.ylabel("amplitudes [" + self.unit + "]")
-        plt.grid(True) 
-        plt.title('load spectrum ' + self.name)
-        plt.xlim(0.5, 1.2*max(self.lk['ni_x']))
-        if method != None:
-            sd   = FLife.SpectralData(input=(self.psd,self.fpsd))
-            if type(method) == type:
-                method = [method] # make method iterable
-            for pdfesti in method:
-                method_name = str(pdfesti)[::-1]
-                method_name = method_name[2:method_name.find(".")][::-1]
-                spdf = pdfesti(sd).get_PDF(self.lk['si_X'])
-                spdf = spdf/np.sum(spdf)
-                loadspectrum = np.cumsum(spdf)*self.T*self.stat['ny_p']
-                plt.semilogx(loadspectrum,self.lk['si_X'],label = method_name+'[$'+self.var+'$]')   
-        plt.legend()
-        plt.show()
-
+        xneu = 0    
+        out = tsarr(xneu)
+    
     def der_lsEquivalent(self,R = 5, Nf = 10, res = 2, D = 0.03, func='acc2dis',optix = None,plot = False,maxit = 100):
         ''' derive quasi-stationary load definition on the basis of the load spectra of the Fatigue Damage Spectrum
         INPUTS:
             :param R:       scalar
                 number of stationary processes
             :param Nf:      scalar
                 number of resonant-frequency samples  
@@ -1035,15 +1426,15 @@
             :param optix:   array-like
                 (use) input values
             :param plot:    boolean
                 use plot function in optimization
             :param maxit:   scalar
                 restrict number of iterations  
         OUTPUT:
-            :(qs)timeseries object    
+            :timeseries object    
         SOURCES:
             Wolfsteiner, P., Trapp, A., and Fertl, L., 'Random vibration fatigue with non-stationary loads using an extended fatigue damage spectrum with load spectra', ISMA 2022 Conference
         '''
         print('LS-FDS Approximation')
 
         '''get load spectra'''
         ls,lsinterp = self.get_ls(Nf = Nf, D = D, func=func,plot=False)
@@ -1092,19 +1483,20 @@
         else:
             optix = sp.optimize.minimize(soe_lsEquivalent,x0,args = inp,method = 'SLSQP',bounds = bnds,constraints=LC,callback=txt_lsEquivalent,tol=1e-8,options={'disp': True,'ftol':1e-7,'maxiter':maxit})
         print(optix) # print results    
         
         '''generate PSD'''
         psd_it = optiparam['psd'] * get_weightFunc(optix['x'],optiparam)
 
-        '''generate qs-timeseries object (time-domain realization)'''
+        '''generate qs-timeseries object (time-domain realization)''' # TODO
         sigs = []
         for rr in range(R):
-            sigs.append({'psd': np.abs(psd_it[rr,:]),'fpsd':inp['fpsd'],'T':optix['x'][rr]*self.T})
-        out = qstimeseries(sigs,var = 'iRLS[' + self.var + ']')
+            sigs.append({'psd': np.abs(psd_it[rr,:]),'fpsd':inp['fpsd'],'T':optix['x'][rr]*self.T,'var': 'iRLS,proc = ' + str(rr) + '[' + self.var + ']'})
+        out = timeseries(sigs) # TODO Wie Namen weitergabe?
+        # out = timeseries(sigs,var = 'iRLS[' + self.var + ']') # TODO Wie Namen weitergabe?
 
         '''save optimization results'''
         now = datetime.now()
         current_time = now.strftime("%H_%M_%S")
         np.save('res_LSOpti_' + current_time + '.npy', optix['x'])
 
         '''return object'''
@@ -1184,16 +1576,16 @@
         print(optix) # print results
 
         '''generate PSD'''
         interpfunc   = sp.interpolate.interp1d(inp['fAxis'],np.append(optix['x'],[1,1]))
         psd_it = self.psd*interpfunc(inp['fpsd'])
 
         '''generate timeseries object (time-domain realization)'''
-        siginp = {'psd': np.abs(psd_it),'fpsd':inp['fpsd'],'T':self.T}
-        out = timeseries(siginp,var = 'iFDS[' + self.var + ']')
+        siginp = {'psd': np.abs(psd_it),'fpsd':inp['fpsd'],'T':self.T,'var': 'iFDS[' + self.var + ']'}
+        out    = timeseries(siginp)
 
         '''save optimization results'''
         now = datetime.now()
         current_time = now.strftime("%H_%M_%S")
         np.save('res_FDSOpti_m' + str(m) + '_' + current_time + '.npy', optix['x'])
 
         '''return object'''
@@ -1237,15 +1629,15 @@
                     return pastCalc 
         f_0    = out['fD']/np.sqrt(1-out['D']**2)
         sig_eq = np.zeros((Nf,len(m)))
         print('calculate FDS via: '+str(method))
         for ff in tqdm(np.arange(Nf)):
             if method == 'RFC': 
                 method_name = method
-                resp, _ = self.der_sdofResponse(fD = f_0[ff], D = D, func = func)
+                resp = self.der_sdofResponse(fD = f_0[ff], D = D, func = func)
                 cycles = np.array(list(rf.extract_cycles(resp.x)))
                 ampls  = cycles[:,0]/2
                 counts = cycles[:,2]
                 for mm in np.arange(len(m)):
                     dam_eq =  np.sum(counts*ampls**m[mm])
                     sig_eq[ff,mm] = dam_eq**(1/m[mm]) 
             elif method == 'DK':
@@ -1279,14 +1671,15 @@
             plot_fds(self.FDScalcs)
         else:
             fsd2Bplotted = [self.FDScalcs[ii] for ii in indx]
             plot_fds(fsd2Bplotted)
 
     def plot_nonstat(self,**kwargs):
         ''' plot non-stationarity matrix 
+        -> pass to static method
         INPUTS:
             ---
         '''
         plot_nonstat(self.nonstat,**kwargs)
 
     def est_nonstat(self,Nf = 20, fl = 0, fu = None,olap = 1,wfunc = sp.signal.windows.triang):
         ''' estimate non-stationary matrix
@@ -1350,24 +1743,26 @@
         ''' saving results '''  
         self.nonstat = get_nonstat(mue2,mue4,mue4sym) 
 
         fbands[fbands < fl] = fl
         fbands[fbands > fu] = fu
         self.nonstat['f_delta'] = dfband
         self.nonstat['f_mid']   = (fbands[:-olap]+fbands[olap:])/2
+        self.nonstat['f_start'] = fl
         self.nonstat['f_end']   = fu
         self.nonstat['var']     = self.var
         self.nonstat['unit']    = self.unit
         self.nonstat['moms']    = self.stat['moms']     
         if fl != 0 and fu!=self.fNy:
             refsig = self.der_bandpass([fl, fu])
             self.nonstat['m4ref'] = refsig.stat['moms'][4]
         else:
             self.nonstat['m4ref'] = self.stat['moms'][4]
-        self.nonstat['m4rep'] = 100*np.sum(self.nonstat['Mxx'])/self.nonstat['m4ref']          
+        self.nonstat['m4rep'] = 100*np.sum(self.nonstat['Mxx'])/self.nonstat['m4ref']
+        return self.nonstat          
        
     def der_statResponse(self,f,H,**kwargs):  
         ''' derive statistical response (PSD & Non-stat.-Matrix) 
             via frequency response function
         INPUTS:
             :param f:    array_like
                 frequency vector
@@ -1393,14 +1788,15 @@
         mue2 = self.nonstat['Gxx']*np.abs(Hnonstat)**2
         mue4 = self.nonstat['Rxx']/4*np.outer(np.abs(Hnonstat**2),np.abs(Hnonstat**2))
         mue4sym = self.nonstat['Rxx_sym']/4*np.outer(np.abs(Hnonstat**2),np.abs(Hnonstat**2))
         nonstat = get_nonstat(mue2,mue4,mue4sym)
         nonstat['f_delta'] = self.nonstat['f_delta']
         nonstat['f_mid']   = self.nonstat['f_mid']
         nonstat['f_end']   = self.nonstat['f_end']
+        nonstat['f_start'] = self.nonstat['f_start']
         nonstat['var']  = kwargs.get('var',self.var.replace('x','y'))
         nonstat['unit'] = kwargs.get('unit',self.unit)
         nonstat['moms'] = [np.nan,np.nan,np.nan,np.nan,np.nan,np.nan]
         nonstat['m4ref'],nonstat['m4rep'] = np.nan,np.nan
         return [self.fpsd,Gyy],nonstat
                          
     def get_analyticalSignal(self,fl,fu):
@@ -1462,57 +1858,82 @@
         OUTPUTS:  
             outobj: timeseries object
                 output timeseries (response) 
         '''
         H = get_tfSDOF(self.fper,fD = fD, D = D, func = func)
         if func == 'acc2dis':
             newunit = self.unit + '*s^2'
+        elif func == 'acc2dis4mm':
+            if (self.unit == 'm/s$^2$') | (self.unit == 'm/s^2'):
+                newunit = 'mm'
+            else:
+                newunit = 'm' + self.unit + '*s^2'
         elif func == 'acc2vel':
             newunit = self.unit + '*s'
         elif func == 'acc2acc':
             newunit = self.unit       
         y      = np.fft.irfft(self.Xos*H*self.N*self.df,n=self.N)
         if 'var' not in kwargs.keys():
             kwargs = dict(kwargs,var = self.var.replace('x','y'))
         if 'unit' not in kwargs.keys():
             kwargs = dict(kwargs,unit = newunit) 
         if 'name' not in kwargs.keys():
             kwargs = dict(kwargs,name = func + ' SDOF response for ' + self.name.replace('(','').replace(')',''))                               
-        outobj = timeseries(y,self.t,**kwargs)
-        return  outobj, H
+        outobj = tsarr(y,fs=self.fs,**kwargs)
+        return  outobj
 
     def der_sdofTransfer(self,fD = 50, D = 0.03,func = 'acc2dis',**kwargs):
         ''' derive single-degree-of-freedom system's transfer functions
         INPUTS:
         :param fD:   scalar
             resonant frequency
         :param D:    scalar
             damping coefficient            
         :param func: string
             type of transfer function 'acc2dis','acc2vel','acc2acc'
         OUTPUTS:  
             outobj: timeseries object
-                output timeseries (response) 
+                output timeseries (transfer function) 
         '''
         H = get_tfSDOF(self.fper,fD = fD, D = D, func = func)
         # H = get_tfSDOF(self.fpsd,fD = fD, D = D, func = func)
         if func == 'acc2dis':
             newunit = self.unit + '$*s^2$'
+        elif func == 'acc2dis4mm':
+            newunit = 'm' + self.unit + '*s^2'
         elif func == 'acc2vel':
             newunit = self.unit + '*s'
         elif func == 'acc2acc':
             newunit = self.unit       
         y      = np.fft.irfft(H*self.N*self.df,n=self.N)
         # y      = np.fft.irfft(H*self.N*self.df,n=2*len(H))
         if 'var' not in kwargs.keys():
             kwargs = dict(kwargs,var = self.var.replace('x','y'))
         if 'unit' not in kwargs.keys():
             kwargs = dict(kwargs,unit = newunit)                   
-        outobj = timeseries(y,self.t,**kwargs)
-        return  outobj   
+        outobj = tsarr(y,fs=self.fs,**kwargs)
+        return  outobj  
+    
+    def der_tfObj(self,f,H,**kwargs):  
+        ''' derive timeseries of structural response for given transfer function
+        INPUTS:
+            :param f:    array_like
+                frequency vector
+            :param H:    array_like
+                frequency response function
+        OUTPUTS:  
+            outobj: timeseries object
+                output timeseries (transfer function)    
+        SOURCES:
+            J. Slavič, M. Boltežar, M. Mršnik, M. Cesnik, J. Javh, Vibration fatigue by spectral methods: From structural dynamics to fatigue, Elsevier, 2020          
+        '''
+        H = get_tf(f,H,self.fper)            
+        y = np.fft.irfft(H*self.N*self.df,n=self.N)                    
+        outobj = tsarr(y,fs=self.fs,**kwargs)
+        return  outobj    
 
     def der_highpass(self,f,**kwargs):
         ''' derive timeseries of ideal high pass filtered signal
         INPUTS:
             :param f:    scaler
                 cuttingfrequency
         '''
@@ -1521,15 +1942,16 @@
         Xfilt[fmask] = self.Xos[fmask]
         if 'var' not in kwargs.keys():
             kwargs = dict(kwargs,var = self.var + '_{hp}')
         if 'unit' not in kwargs.keys():
             kwargs = dict(kwargs,unit = self.unit) 
         if 'name' not in kwargs.keys():
             kwargs = dict(kwargs,name = 'highpass filtered ts of ' + self.name.replace('(','').replace(')',''))   
-        return timeseries(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),self.t,**kwargs)
+        # return timeseries(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),self.t,**kwargs)
+        return tsarr(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),fs=self.fs,**kwargs)
     
     def der_lowpass(self,f,**kwargs):
         ''' derive timeseries of ideal low pass filtered signal
         INPUTS:
             :param f:    scaler
                 cuttingfrequency
         '''
@@ -1538,32 +1960,51 @@
         Xfilt[fmask] = self.Xos[fmask]
         if 'var' not in kwargs.keys():
             kwargs = dict(kwargs,var = self.var + '_{lp}')
         if 'unit' not in kwargs.keys():
             kwargs = dict(kwargs,unit = self.unit) 
         if 'name' not in kwargs.keys():
             kwargs = dict(kwargs,name = 'lowpass filtered ts of ' + self.name.replace('(','').replace(')',''))  
-        return timeseries(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),self.t,**kwargs)
+        # return timeseries(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),self.t,**kwargs)
+        return tsarr(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),fs=self.fs,**kwargs)
     
     def der_bandpass(self,f,**kwargs):
         ''' derive timeseries of ideal band pass filtered signal
         INPUTS:
-            :param f:    scaler
+            :param f:    scalar
                 cuttingfrequency
         '''
         Xfilt  = np.zeros(len(self.Xos),dtype='cdouble')
         fmask  = (self.fper >= f[0]) & (self.fper <= f[1])
         Xfilt[fmask] = self.Xos[fmask]
         if 'var' not in kwargs.keys():
             kwargs = dict(kwargs,var = self.var + '_{bp}')
         if 'unit' not in kwargs.keys():
             kwargs = dict(kwargs,unit = self.unit) 
         if 'name' not in kwargs.keys():
-            kwargs = dict(kwargs,name = 'bandpass filtered ts of ' + self.name.replace('(','').replace(')',''))  
-        return timeseries(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),self.t,**kwargs)    
+            kwargs = dict(kwargs,name = 'bandpass filtered ts of ' + self.name.replace('(','').replace(')',''))    
+        return tsarr(np.fft.irfft(Xfilt*self.N*self.df,n=self.N),fs=self.fs,**kwargs)
+    
+    def der_deriviative(self,opt='dt',**kwargs):
+        ''' derive deriviative timeseries 
+        INPUTS:
+            :param opt:    string
+                deriviative option
+        '''
+        if opt == 'dt':
+            H = 1j*2*np.pi*self.fper
+        elif opt == 'dtdt':
+            H = (1j*2*np.pi*self.fper)**2
+        elif opt == 'intint':
+            H = 1/(1j*2*np.pi*self.fper)
+        elif opt ==  'int':
+            H = 1/(1j*2*np.pi*self.fper)**2
+        y = np.fft.irfft(self.Xos*H*self.N*self.df,n=self.N)
+        return tsarr(y,fs=self.fs,**kwargs)
+            
     
     def der_response(self,f,H,**kwargs):  
         ''' derive timeseries of structural response for given transfer function
         INPUTS:
             :param f:    array_like
                 frequency vector
             :param H:    array_like
@@ -1578,17 +2019,32 @@
         y = np.fft.irfft(self.Xos*H*self.N*self.df,n=self.N)
         if 'var' not in kwargs.keys():
             kwargs = dict(kwargs,var = self.var.replace('x','y'))
         if 'unit' not in kwargs.keys():
             kwargs = dict(kwargs,unit = self.unit)        
         if 'name' not in kwargs.keys():
             kwargs = dict(kwargs,name = 'response for ' + self.name.replace('(','').replace(')',''))                     
-        outobj = timeseries(y,self.t,**kwargs)
+        # outobj = timeseries(y,self.t,**kwargs)
+        outobj = tsarr(y,fs=self.fs,**kwargs)
         return  outobj
-
+    
+    def der_scale2max(self,value = 1,**kwargs):
+        ''' derive timeseries scaled to reference value
+        INPUTS:
+            :param value:    scalar
+                value to scale max value to
+        OUTPUTS:  
+            outobj: timeseries object
+                scaled timeseries
+        ''' 
+        if 'var' not in kwargs.keys():
+            kwargs = dict(kwargs,var = self.var + '(scaled)')
+        outobj = tsarr(self.x/self.stat['max']*value,fs=self.fs,**kwargs)
+        return  outobj        
+        
     def der_zeropadded(self,zpfactor):
         ''' derive zeropadded timeseries
         INPUTS:
             :param tpfactor:    scalar
                 zero-padding factor
         OUTPUTS:  
             outobj: timeseries object
@@ -1597,15 +2053,15 @@
             A. Trapp, Q. Hoesch, P. Wolfsteiner, Effects of insufficient sampling on counting algorithms in vibration fatigue, Procedia Structural Integrity 38 (2022) 260–270            
         ''' 
         newN = int(np.ceil(self.N*zpfactor))
         Y = np.append(self.Xos, np.zeros(newN-self.N))
         y = np.fft.irfft(Y*newN*self.df,n=newN)
         t = np.linspace(0,self.T,newN+1)
         t = t[:-1]
-        outobj = timeseries(y,t)
+        outobj = tsarr(y,fs=self.fs)
         return  outobj 
 
     def get_ls(self,Nf = 10, func='acc2dis', D = 0.03,p_interp = 30, plot = True):
         # eval input resonant frequencies
         if np.isscalar(Nf):
             evalf  = np.linspace(0,round(self.fNy,0),Nf+2)
             evalf  = evalf[1:-1]
@@ -1615,20 +2071,17 @@
         check_df  = evalf[0]/100 
         if self.dfpsd > check_df:
             self.est_psd(df = check_df)
         # initialize
         ls, lsinterp = [],[]
 
         for ii in np.arange(len(evalf)):
-            resp,tf = self.der_sdofResponse(fD = evalf[ii],func = func, D = D)
-            ls.append({'si_x': resp.lk['si_x'], 'ni_x': resp.lk['ni_x'], 'max_ni': resp.lk['npeaks'],
-                       'si_X': resp.lk['si_X'], 'ni_X': resp.lk['ni_X'], 'fD': evalf[ii]})
-            # if isinstance(resp,qstimeseries):
-            #     qsdk.append({'si_x': resp.qs['si_X'], 'ni_x': resp.qs['ni_X']})
-
+            resp = self.der_sdofResponse(fD = evalf[ii],func = func, D = D)
+            ls.append({'si_x': resp.ls['si_x'], 'ni_x': resp.ls['ni_x'], 'max_ni': resp.ls['npeaks'],
+                       'si_X': resp.ls['si_X'], 'ni_X': resp.ls['ni_X'], 'fD': evalf[ii]})
 
         ni_interp = np.logspace(0,np.log10(0.9*min([x['max_ni'] for x in ls])),p_interp)
         ni_interp = ni_interp[ np.append(1,np.diff(ni_interp)) >= 1]
 
         for rsp in ls:
             si_interp = np.interp(ni_interp,rsp['ni_x'],rsp['si_x'])
             si_Interp = np.interp(ni_interp,rsp['ni_X'],rsp['si_X'])
@@ -1658,64 +2111,65 @@
             ax.set_xlabel('resonant frequency $f_D$ [Hz]')
             ax.set_ylabel('cumulated cycles (log) [-]')
             ax.set_zlabel('amplitude [$' + resp.var + '$]')
             ax.set_title('RFC vs. DK ($' + self.var + '$; log)')
             #ax.legend()
             plt.show()    
         return ls,lsinterp
-        
- ###############################################################################
-# Inheritance of timeseries for qstimeseries (quasi-stationary process) 
-class qstimeseries(timeseries):  
-    '''
-        Attributes
-        ----------
-        attributes from timeseries...
-        sigs:      list of timeseries objects ('stationary components')
-        R:         number of stationary processes
-        p:         portion of each processes
-        ---------- 
-        Methods
-        ---------- 
-        methods from timeseries...
-        est_qsLS(): estimate quasi-stationary load spectrum
-        ----------   
-    '''
+    # def __init__(self, inp,tukwin = 5e-4,**kwargs): 
+    #     for sig in inp:
+    #         x.append(sig.x*sp.signal.windows.tukey(sig.N,alpha=tukwin))  
+    #         N += sig.N   
+    #   self.R    = len(inp)
+    #   self.p    = [sig.N/N for sig in inp]
+           
+if __name__ == "__main__":  
+    xc1p1 = np.random.randn(20000)
+    xc1p2 = np.random.randn(10000)
+    xc1p3 = np.random.randn(5000)
+    xc2p1 = np.random.randn(20000)
+    xc2p2 = np.random.randn(10000)
+    xc2p3 = np.random.randn(5000)
+
+    c1 = [xc1p1,xc1p2,xc1p3]
+    c2 = [xc2p1,xc2p2,xc2p3]
+    x  = [c1,c2]
+
+    #%% signal definition
+    inp  = []                   # empty list to be filled with signal specifications
+    fpsd = np.arange(0,100+1)   # frequency vector for corresponding PSD
+
+    # stationary part 1
+    psd  = np.zeros(fpsd.shape)
+    psd[(fpsd >= 10) & (fpsd < 60)] = 1
+    inp.append({'fpsd': fpsd, 'psd': psd, 'T': 100, 'var': 'x_1'})
+
+    # stationary part 2
+    psd2 = np.zeros(fpsd.shape)
+    psd2[(fpsd >= 50) & (fpsd < 100)] = 1
+    inp.append({'fpsd': fpsd, 'psd': psd2, 'T': 100, 'var': 'x_2'})
+
+
+    scspdict = timeseries(inp[0])
+    scspdict.whos()
+    scspdict.plot()
+    scmpdict = timeseries(inp)
+    scmpdict.whos()
+    scmpdict.plot()
+    mcmpdict = timeseries([inp,inp,inp])
+    mcmpdict.whos()
+    mcmpdict.plot()
+
+    scmp = timeseries(c1,fs = 1200)
+    scmp.whos()
+    scmp.plot()
+    mcmp = timeseries(x,fs = 1200)
+    mcmp.whos()
+    mcmp.plot()
+    scsp = timeseries(xc1p1,fs = 1000)
+    scsp.whos()
+    scsp.plot()
+
 
-    def __init__(self, inp,tukwin = 5e-4,**kwargs): 
-        if type(inp) == list:
-            inp = [timeseries(psds) for psds in inp]
-        N = 0
-        x = []
-        for sig in inp:
-            x.append(sig.x*sp.signal.windows.tukey(sig.N,alpha=tukwin))  
-            N += sig.N   
-        fs = np.mean([sig.fs for sig in inp])
-        dt = 1/fs
-        t = np.arange(0,N*dt,dt)
-        x = np.concatenate(x)
-        minN = np.min((x.shape,t.shape))
-        self.sigs = inp 
-        super().__init__(x[:minN],t[:minN],**kwargs)  
-        self.R    = len(inp)
-        self.p    = [sig.N/N for sig in inp]
-        
-        
-    def est_qsLS(self):
-        ''' estimate quasi-stationary load spectrum
-        INPUTS:
-            ---     
-        SOURCES:
-            A. Trapp, P. Wolfsteiner, Fatigue assessment of non-stationary random loading in the frequency domain by a quasi-stationary Gaussian approximation, International Journal of Fatigue 148 (2021) 106214     
-        ''' 
-        self.qs = {'si_X': np.linspace(0,self.stat['maxvalue']*1.1,1000)}
-        self.qs['ni_X'] = np.zeros(self.qs['si_X'].shape)
-        for sig in self.sigs:
-            sig.est_ls(si_X = self.qs['si_X'])
-            self.qs['ni_X'] = self.qs['ni_X'] + sig.lk['ni_X']  
-        
-            
-                
 
 
 
-
```

### Comparing `pyRaTS-0.15/setup.py` & `pyRaTS-0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.rst', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyRaTS',                     
-    version='0.15',                        
+    version='0.20',                        
     author='Arvid Trapp',
     author_email='arvid.trapp@hm.edu',
     url='https://github.com/ArvidTrapp/pyRaTS',
     maintainer='Arvid Trapp, Peter Wolfsteiner',
     maintainer_email='arvid.trapp@hm.edu',                    
     description='processing of (RAndom) TimeSeries for vibration fatigue',
     long_description=long_description,
```

