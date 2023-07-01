# Comparing `tmp/sphractal-0.4.2.tar.gz` & `tmp/sphractal-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.4.2.tar", max compression
+gzip compressed data, was "sphractal-0.4.3.tar", max compression
```

## Comparing `sphractal-0.4.2.tar` & `sphractal-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,27 @@
--rw-r--r--   0        0        0     1082 2023-06-30 03:23:36.162883 sphractal-0.4.2/LICENSE
--rw-r--r--   0        0        0     2767 2023-06-30 03:23:36.162883 sphractal-0.4.2/README.md
--rw-r--r--   0        0        0     1428 2023-06-30 03:24:30.958639 sphractal-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1394 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/__init__.py
--rw-r--r--   0        0        0    21060 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     3821 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      279 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8813 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     7909 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11480 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/utils.py
--rw-r--r--   0        0        0    94223 2023-06-30 03:23:36.234883 sphractal-0.4.2/tests/fixtures.py
--rw-r--r--   0        0        0    10966 2023-06-30 03:23:36.234883 sphractal-0.4.2/tests/test_sphractal.py
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 sphractal-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-01 08:12:27.577598 sphractal-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2925 2023-07-01 08:12:27.577598 sphractal-0.4.3/README.md
+-rw-r--r--   0        0        0     1978 2023-07-01 08:13:11.260939 sphractal-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/3DbinImBCcpu.cpp
+-rw-r--r--   0        0        0     3111 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/3DbinImBCgpu.cpp
+-rw-r--r--   0        0        0     2084 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/README.txt
+-rw-r--r--   0        0        0     3581 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCPU.cpp
+-rw-r--r--   0        0        0      979 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCPU.h
+-rw-r--r--   0        0        0     4378 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA2D.cu
+-rw-r--r--   0        0        0     1056 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA2D.cuh
+-rw-r--r--   0        0        0     4947 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA3D.cu
+-rw-r--r--   0        0        0     1056 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA3D.cuh
+-rw-r--r--   0        0        0     5867 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA4D.cu
+-rw-r--r--   0        0        0     1056 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA4D.cuh
+-rw-r--r--   0        0        0    10330 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/test.cpp
+-rw-r--r--   0        0        0     1394 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    21444 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     3821 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      279 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8881 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8119 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11480 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94223 2023-07-01 08:12:27.641597 sphractal-0.4.3/tests/fixtures.py
+-rw-r--r--   0        0        0    17404 2023-07-01 08:12:27.641597 sphractal-0.4.3/tests/test_sphractal.py
+-rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 sphractal-0.4.3/PKG-INFO
```

### Comparing `sphractal-0.4.2/LICENSE` & `sphractal-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.2/README.md` & `sphractal-0.4.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Sphractal
 
+[![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
+
 ## Description
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Current
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### To be Done
-* Complete `tests/`.
+* Set path for exeDir.
 * Publish to Conda.
 * Nested multiprocessing.
 * Better looking plots, allow figure size to be specified, allow choice for 'paper' and 'presentation'.
 * Consider transforming xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 
 ## Installation
```

### Comparing `sphractal-0.4.2/pyproject.toml` & `sphractal-0.4.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.4.2"
+version = "0.4.3"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
-authors = ["Jonathan Yik Chang Ting"]
+authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-include = ["tests/*"]
+homepage = "https://github.com/Jon-Ting/sphractal"
+repository = "https://github.com/Jon-Ting/sphractal"
+documentation = "https://sphractal.readthedocs.io/en/latest/"
+keywords = ["box-counting", "box-count", "fractal", "dimension", "sphere", "surface"]
+classifiers = [
+    "Intended Audience :: Science/Research", 
+    "Natural Language :: English", 
+    "Operating System :: OS Independent", 
+    "Programming Language :: C++", 
+    "Programming Language :: Python :: 3", 
+    "Topic :: Scientific/Engineering", 
+]
+include = ["tests/*", "src/fbc/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 matplotlib = ">=3.7.1"
 statsmodels = ">=0.14.0"
 scipy = {version = ">=1.11.0", python = ">=3.9,<3.13"}
 numba = ">=0.57.1"
```

### Comparing `sphractal-0.4.2/src/sphractal/__init__.py` & `sphractal-0.4.3/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.2/src/sphractal/boxCnt.py` & `sphractal-0.4.3/src/sphractal/boxCnt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from concurrent.futures import ProcessPoolExecutor as Pool
 from math import log10
 from os import mkdir, system
 from os.path import isdir
+from warnings import warn
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 import numpy as np
 from statsmodels.api import OLS, add_constant
 
 from sphractal.surfExact import findTargetAtoms, MIN_VAL_FROM_BOUND, scanAllAtoms, writeBoxCoords
@@ -57,17 +58,17 @@
     verbose : bool
         Whether to display the details.
     genPCD : bool, optional
         Whether to generate pcd file for box-counting using MATLAB code written by Kazuaki Iida.
     
     Returns
     -------
-    scaleChange : list
+    scales : list
         Box lengths.
-    cntChange : list
+    counts : list
         Number of boxes that cover the surface of interest, as represented by the voxels in the 3D binary image.
 
     Examples
     --------
     >>> eles, rads, xyzs, _, minxyz, maxxyz = readXYZ('example.xyz')
     >>> neighs, _ = findNN(rads, xyzs, minxyz, maxxyz, 2.5)
     >>> surfs = findSurf(xyzs, neighs, 'alphaShape', 5.0)
@@ -83,27 +84,29 @@
     - 16384 -> 8192 GB
     Further details about maximum grid size and memory estimation could be found in original codes of the authors in
     {SPHRACTAL_DIR_PATH}/src/fbc/test.cpp.
     As a reference, when 8192 grids are used, allocation of memory took 25 min; while the CPU algorithm runs for 18 min.
     """
     if verbose:
         print(f"  Approximating the surface with {numPoint} point clouds for each atom...")
+    if not isdir(writeFileDir):
+        mkdir(writeFileDir)
 
     genSurfPoints(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                   npName, writeFileDir,
                   radType, numPoint, gridNum,
                   rmInSurf, vis, verbose, genPCD)
     system(f"{exeDir}/3DbinImBC{procUnit}.exe {gridNum} {writeFileDir}/surfVoxelIdxs.txt "
            f"{writeFileDir}/surfVoxelBoxCnts.txt")
-    scaleChange, cntChange = [], []
+    scales, counts = [], []
     with open(f"{writeFileDir}/surfVoxelBoxCnts.txt", 'r') as f:
         for line in f:
-            scaleChange.append(log10(1 / int(line.split()[0])))
-            cntChange.append(log10(int(line.split()[1])))
-    return scaleChange[::-1], cntChange[::-1]
+            scales.append(log10(1 / int(line.split()[0])))
+            counts.append(log10(int(line.split()[1])))
+    return scales[::-1], counts[::-1]
 
 
 # @annotate('getSphereBoxCnts', color='blue')
 def getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                      maxRange, minMaxBoxLens, minXYZ, npName, writeFileDir='boxCntOutputs', numBoxLenSample=10,
                      rmInSurf=True, writeBox=True, verbose=False, boxLenConc=False, maxWorkers=2):
     """
@@ -144,33 +147,37 @@
         Whether to parallelise the box-counting across different box lengths.
     maxWorkers : int, optional
         Maximum number of processes to spawn for parallelisation of box-counting across different box lengths, only used
         if 'boxLenConc' is True.
     
     Returns
     -------
-    scaleChange : list
+    scales : list
         Box lengths.
-    cntChange : list
+    counts : list
         Number of boxes that cover the exact spherical surface of interest.
     
     Examples
     --------
     >>> eles, rads, xyzs, _, minxyz, maxxyz = readXYZ('example.xyz')
     >>> neighs, _ = findNN(rads, xyzs, minxyz, maxxyz, 1.2)
     >>> surfs = findSurf(xyzs, neighs, 'alphaShape', 2.0)
     >>> scales, counts = getSphereBoxCnts(eles, rads, surfs, xyzs, neighs, 100, (0.2, 1), minxyz, 'example')
     """
     if verbose:
         print(f"  Representing the surface by treating each atom as exact spheres...")
         print(f"    (1/eps)    (# bulk)    (# surf)")
+    if writeBox:
+        if not isdir(writeFileDir):
+            mkdir(writeFileDir)
+
     atomsIdxs = atomsSurfIdxs if rmInSurf else findTargetAtoms(atomsNeighIdxs)
     overallBoxLen = maxRange + MIN_VAL_FROM_BOUND * 2
     allLensSurfBoxs, allLensBulkBoxs, allLensSurfCnts, allLensBulkCnts = [], [], [], []
-    scaleChange, scanBoxLens, scanAllAtomsInps = [], [], []
+    scales, scanBoxLens, scanAllAtomsInps = [], [], []
     approxScanBoxLens = np.geomspace(minMaxBoxLens[1], minMaxBoxLens[0], num=numBoxLenSample)
     for approxScanBoxLen in approxScanBoxLens:  # Evenly reduced box lengths on log scale
         magnFac = int(overallBoxLen / approxScanBoxLen)
         scanBoxLen = overallBoxLen / magnFac
         scanAllAtomsInp = (magnFac, scanBoxLen, atomsIdxs, minXYZ,
                            atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, 
                            rmInSurf, verbose)
@@ -179,80 +186,82 @@
         else:
             scanAllAtomsResult = scanAllAtoms(scanAllAtomsInp) 
             allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
             allLensSurfBoxs.append(allAtomsSurfBoxs)
             allLensBulkBoxs.append(allAtomsBulkBoxs)
             allLensSurfCnts.append(len(allAtomsSurfBoxs))
 
-        scaleChange.append(log10(magnFac / overallBoxLen))
+        scales.append(log10(magnFac / overallBoxLen))
         scanBoxLens.append(scanBoxLen)
 
     if boxLenConc:
         with Pool(max_workers=maxWorkers) as pool:
             for scanAllAtomsResult in pool.map(scanAllAtoms, scanAllAtomsInps):
                 allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
                 allLensSurfBoxs.append(allAtomsSurfBoxs)
                 allLensBulkBoxs.append(allAtomsBulkBoxs)
                 allLensSurfCnts.append(len(allAtomsSurfBoxs))
-    cntChange = [log10(sCnt) if sCnt != 0 else np.nan for sCnt in allLensSurfCnts]
+    counts = [log10(sCnt) if sCnt != 0 else np.nan for sCnt in allLensSurfCnts]
 
     if writeBox:
         writeBoxCoords(atomsEle, atomsXYZ, allLensSurfBoxs, allLensBulkBoxs, minXYZ, scanBoxLens, writeFileDir, npName)
-    return scaleChange, cntChange
+    return scales, counts
 
 
 # @annotate('findSlope', color='green')
-def findSlope(scaleChange, cntChange, npName='', writeFileDir='boxCntOutputs', lenRange='trim',
-              minSampleNum=5, confIntPerc=95, visReg=True, saveFig=False, showPlot=False):
+def findSlope(scales, counts, npName='', writeFileDir='boxCntOutputs', lenRange='trim',
+              minSampleNum=5, confLvl=95, visReg=True, saveFig=False, showPlot=False):
     """
     Compute the slope (box counting dimension) from the box-counting data collected.
 
     Parameters
     ----------
-    scaleChange : list
+    scales : list
         Box lengths.
-    cntChange : list
+    counts : list
         Number of boxes that cover the exact spherical surface of interest.
     npName : str, optional
         Identifier of the measured object, which forms part of the output file name, ideally unique.
     writeFileDir : str, optional
         Path to the directory to store the output files.
     lenRange : {'trim', 'full'}, optional
         Range of box lengths to include for determining the box-counting dimension. Choosing 'trim' finds the highest 
         coefficient of determination by iteratively removing the box counts obtained using boxes of extreme sizes.
     minSampleNum : int, optional
         Minimum number of box count data points to be retained for slope estimation from the linear regression fitting.
-    confIntPerc : Union[int, float]
+    confLvl : Union[int, float]
         Confidence level of confidence interval in percentage.
     visReg : bool, optional
         Whether to generate figures from the linear regression fitting process.
     saveFig : bool, optional
-        Whether to save the plots generated.
+        Whether to save the plots generated, only works when 'visReg' is True.
     showPlot : bool, optional
-        Whether to show the plots generated.
+        Whether to show the plots generated, only works when 'visReg' is True.
     
     Returns
     -------
     r2score : float
         Coefficient of determination from determination of the dimension of point clouds surface.
     boxCntDim : float
         Box-counting dimension of the point clouds representation of the surface.
     slopeCI : tuple
         Confidence interval of the box-counting dimension of the point clouds surface.
     """
-    while np.nan in cntChange:
-        nanIdx = cntChange.index(np.nan)
-        del cntChange[nanIdx]
-        del scaleChange[nanIdx]
-    firstPointIdx, lastPointIdx, removeSmallBoxes = 0, len(scaleChange), True  # countChange.count(countChange[0])
-
-    alphaCI = 1 - confIntPerc/100
-    r2score, boxCntDim, slopeCI, r2scorePrev, boxCntDimPrev, slopeCIPrev = 0.0, 0.0, (0.0, 0.0), 0.0, 0.0, (0.0, 0.0)
-    while len(scaleChange[firstPointIdx:lastPointIdx]) > minSampleNum:
-        x, y = scaleChange[firstPointIdx:lastPointIdx], cntChange[firstPointIdx:lastPointIdx]
+    while np.nan in counts:
+        nanIdx = counts.index(np.nan)
+        del counts[nanIdx]
+        del scales[nanIdx]
+    firstPointIdx, lastPointIdx, removeSmallBoxes = 0, len(scales), True  # countChange.count(countChange[0])
+
+    if abs(confLvl) > 100:
+        warn(f"Confidence level out of range, confidence intervals are unreliable! 'confLvl' should be within [0, 100) instead of {confLvl}")
+    alphaCI = 1 - confLvl/100
+    r2score, boxCntDim, slopeCI, r2scorePrev, boxCntDimPrev, slopeCIPrev = 0.0, 0.0, np.array((np.inf, np.inf)), 0.0, 0.0, np.array((np.inf, np.inf))
+    while len(scales[firstPointIdx:lastPointIdx]) > minSampleNum:
+        x, y = scales[firstPointIdx:lastPointIdx], counts[firstPointIdx:lastPointIdx]
         regModel = OLS(endog=y, exog=add_constant(x)).fit()
         r2score, boxCntDim, slopeCI = regModel.rsquared, regModel.params[1], regModel.conf_int(alpha=alphaCI)[1]
         yPred = regModel.predict()  # Returns ndarray, allowing subtraction later
         if visReg:
             plt.close()
             _, ax = plt.subplots()
             ax.scatter(x, y)
@@ -260,15 +269,15 @@
             predOLS = regModel.get_prediction()
             lowCIvals, upCIvals = predOLS.summary_frame()['mean_ci_lower'], predOLS.summary_frame()['mean_ci_upper']
             ax.plot(x, upCIvals, 'r--')
             ax.plot(x, lowCIvals, 'r--')
             ax.set_xlabel('log(1/r)')
             ax.set_ylabel('log(N)')
             ax.yaxis.set_major_formatter(FormatStrFormatter('% 1.1f'))
-            ax.set_title(f"{npName} R2: {r2score:.3f}, D_Box: {boxCntDim:.3f}, {confIntPerc}% CI: "
+            ax.set_title(f"{npName} R2: {r2score:.3f}, D_Box: {boxCntDim:.3f}, {confLvl}% CI: "
                       f"[{slopeCI[0]:.3f}, {slopeCI[1]:.3f}]");
         # Removal of next point (beware of weird behaviour in middle range)
         # lstSqErrs = np.subtract(y, yPred) ** 2
         # if len(y) % 2 == 0:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2:].sum()
         # else:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2 + 1:].sum()
@@ -282,29 +291,31 @@
             else:
                 if round(r2score, 3) < round(r2scorePrev, 3):
                     return r2scorePrev, boxCntDimPrev, slopeCIPrev
                 firstPointIdx += 1
         if saveFig:
             boxCntDimsDir = f"{writeFileDir}/boxCntDims"
             if not isdir(boxCntDimsDir):
+                if not isdir(writeFileDir):
+                    mkdir(writeFileDir)
                 mkdir(boxCntDimsDir)
             plt.savefig(f"{boxCntDimsDir}/{npName}_boxCntDim.png")
         if showPlot:
             plt.show()
         r2scorePrev, boxCntDimPrev, slopeCIPrev = r2score, boxCntDim, slopeCI
         if lenRange == 'full':
             break
     return r2score, boxCntDim, slopeCI
 
 
 # @annotate('runCase', color='cyan')
 # @estDuration
 def runBoxCnt(xyzFilePath, 
               radType='atomic', calcBL=False, findSurfOption='alphaShape', alphaMult=2.0,
-              writeFileDir='boxCntOutputs', lenRange='trim', minSampleNum=5, confIntPerc=95, 
+              writeFileDir='boxCntOutputs', lenRange='trim', minSampleNum=5, confLvl=95, 
               rmInSurf=True, vis=True, saveFig=False, showPlot=False, verbose=False,
               runPointCloudBoxCnt=True, numPoints=300, gridNum=1024, exeDir='../bin', procUnit='cpu', genPCD=False,
               runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, writeBox=True, 
               boxLenConc=False, maxWorkers=2):
     """
     Run box-counting algorithm on the surface of a given object consisting of a set of spheres represented as either
     point clouds or exact spherical surface.
@@ -325,15 +336,15 @@
     writeFileDir : str, optional
         Path to the directory to store the output files.
     lenRange : {'trim', 'full'}, optional
         Range of box lengths to include for determining the box-counting dimension. Choosing 'trim' finds the highest 
         coefficient of determination by iteratively removing the box counts obtained using boxes of extreme sizes.
     minSampleNum : int, optional
         Minimum number of box count data points to be retained for slope estimation from the linear regression fitting.
-    confIntPerc : Union[int, float], optional
+    confLvl : Union[int, float], optional
         Confidence level of confidence interval in percentage.
     rmInSurf : bool, optional
         Whether to remove the surface points on the inner surface.
     vis : bool, optional
         Whether to generate output files for visualisation.
     saveFig : bool, optional
         Whether to save the plots generated, only used if 'vis' is True.
@@ -402,22 +413,22 @@
         mkdir(writeFileDir)
     if runPointCloudBoxCnt:
         scalesPC, countsPC = getVoxelBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                                              testCase, writeFileDir, exeDir, procUnit,
                                              radType, numPoints, gridNum,
                                              rmInSurf, vis, verbose, genPCD)
         r2PC, bcDimPC, confIntPC = findSlope(scalesPC, countsPC, f"{testCase}_PC", writeFileDir, lenRange,
-                                             minSampleNum, confIntPerc, vis, saveFig, showPlot)
+                                             minSampleNum, confLvl, vis, saveFig, showPlot)
     if runExactSphereBoxCnt:
         minAtomRad = atomsRad.min()
         scalesES, countsES = getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                                               maxRange, (minAtomRad * minLenMult, minAtomRad * maxLenMult),
                                               minXYZ, testCase, writeFileDir, numBoxLenSample,
                                               rmInSurf, writeBox, verbose, boxLenConc, maxWorkers)
         r2ES, bcDimES, confIntES = findSlope(scalesES, countsES, f"{testCase}_ES", writeFileDir, lenRange,
-                                             minSampleNum, confIntPerc, vis, saveFig, showPlot)
+                                             minSampleNum, confLvl, vis, saveFig, showPlot)
     if verbose:
         if runPointCloudBoxCnt:
             print(f"  Point clouds  D_Box: {bcDimPC:.4f} [{confIntPC[0]:.4f}, {confIntPC[1]:.4f}],  R2: {r2PC:.4f}")
         if runExactSphereBoxCnt:
             print(f"  Exact surface D_Box: {bcDimES:.4f} [{confIntES[0]:.4f}, {confIntES[1]:.4f}],  R2: {r2ES:.4f}")
     return r2PC, bcDimPC, confIntPC, r2ES, bcDimES, confIntES
```

### Comparing `sphractal-0.4.2/src/sphractal/constants.py` & `sphractal-0.4.3/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.2/src/sphractal/data/example.xyz` & `sphractal-0.4.3/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.2/src/sphractal/surfExact.py` & `sphractal-0.4.3/src/sphractal/surfExact.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,16 @@
 # @annotate('writeBoxCoords', color='yellow')
 def writeBoxCoords(atomsEle, atomsXYZ, allSurfBoxs, allBulkBoxs, minXYZ, scanBoxLens,
                    writeFileDir, npName):
     """Write out coordinates of scanned boxes."""
     minX, minY, minZ = minXYZ
     boxCoordsDir = f"{writeFileDir}/boxCoords"
     if not isdir(boxCoordsDir):
+        if not isdir(writeFileDir):
+            mkdir(writeFileDir)
         mkdir(boxCoordsDir)
     with open(f"{boxCoordsDir}/{npName}_boxCoords.xyz", 'w') as f:
         for (i, scanBoxLen) in enumerate(scanBoxLens):
             if i != 0:
                 f.write('\n')
             f.write(f"{len(atomsEle) + len(allSurfBoxs[i]) + len(allBulkBoxs[i])}\n")
             for (j, atomXYZ) in enumerate(atomsXYZ):
```

### Comparing `sphractal-0.4.2/src/sphractal/surfPointClouds.py` & `sphractal-0.4.3/src/sphractal/surfPointClouds.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,28 +86,32 @@
 
 
 # @annotate('writePCD', color='yellow')
 def writePCD(writeFileDir, npName, surfPointXYZs):
     """Generate a pcd file required for 3D box-counting using MATLAB code written by Kazuaki Iida."""
     surfPointsDir = f"{writeFileDir}/surfPoints"
     if not isdir(surfPointsDir):
+        if not isdir(writeFileDir):
+            mkdir(writeFileDir)
         mkdir(surfPointsDir)
     with open(f"{surfPointsDir}/{npName}_surfPoints.pcd", 'w') as f:
         f.write('# .PCD v.7 - Point Cloud Data file format\nVERSION .7')
         f.write('\nFIELDS x y z\nSIZE 4 4 4\nTYPE F F F\nCOUNT 1 1 1\n')
         f.write(f"WIDTH {len(surfPointXYZs)}\nHEIGHT 1\nPOINTS {len(surfPointXYZs)}\nDATA ascii\n")
         for xyz in surfPointXYZs:
             f.write(f"{xyz[0]} {xyz[1]} {xyz[2]}\n")
 
 
 # @annotate('writeSurfPoints', color='blue')
 def writeSurfPoints(writeFileDir, npName, atomsSurfIdxs, atomsXYZ, surfPointXYZs, nonSurfPointXYZs):
     """Generate an xyz file for visualisation of classified point clouds."""
     surfPointsDir = f"{writeFileDir}/surfPoints"
     if not isdir(surfPointsDir):
+        if not isdir(writeFileDir):
+            mkdir(writeFileDir)
         mkdir(surfPointsDir)
     with open(f"{surfPointsDir}/{npName}_surfPoints.xyz", 'w') as f:
         f.write(f"{len(surfPointXYZs) + len(nonSurfPointXYZs) + len(atomsSurfIdxs)}\n\n")
         for (i, xyz) in enumerate(surfPointXYZs):
             f.write(f"OU {xyz[0]} {xyz[1]} {xyz[2]} {i}\n")
         for (i, xyz) in enumerate(nonSurfPointXYZs):
             f.write(f"IN {xyz[0]} {xyz[1]} {xyz[2]} {i}\n")
@@ -117,14 +121,16 @@
 
 
 # @annotate('writeSurfVoxels', color='green')
 def writeSurfVoxels(writeFileDir, npName, surfVoxelXYZs):
     """Generate an xyz file useful for visualisation of computed surface voxels."""
     surfVoxelsDir = f"{writeFileDir}/surfVoxels"
     if not isdir(surfVoxelsDir):
+        if not isdir(writeFileDir):
+            mkdir(writeFileDir)
         mkdir(surfVoxelsDir)
     with open(f"{surfVoxelsDir}/{npName}_surfVoxels.xyz", 'w') as f:
         f.write(f"{len(surfVoxelXYZs)}\n\n")
         for (i, xyz) in enumerate(surfVoxelXYZs):
             f.write(f"VX {xyz[0]} {xyz[1]} {xyz[2]} {i}\n")
```

### Comparing `sphractal-0.4.2/src/sphractal/utils.py` & `sphractal-0.4.3/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.2/tests/fixtures.py` & `sphractal-0.4.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.2/PKG-INFO` & `sphractal-0.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.4.2
+Version: 0.4.3
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
+Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
+Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
+Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: numba (>=0.57.1)
 Requires-Dist: numpy (>=1.22,<1.25)
 Requires-Dist: scipy (>=1.11.0) ; python_version >= "3.9" and python_version < "3.13"
 Requires-Dist: statsmodels (>=0.14.0)
+Project-URL: Documentation, https://sphractal.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/Jon-Ting/sphractal
 Description-Content-Type: text/markdown
 
 # Sphractal
 
+[![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
+
 ## Description
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Current
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### To be Done
-* Complete `tests/`.
+* Set path for exeDir.
 * Publish to Conda.
 * Nested multiprocessing.
 * Better looking plots, allow figure size to be specified, allow choice for 'paper' and 'presentation'.
 * Consider transforming xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 
 ## Installation
```

