# Comparing `tmp/unrollcuda-0.0.6.tar.gz` & `tmp/unrollcuda-0.0.7.tar.gz`

## Comparing `unrollcuda-0.0.6.tar` & `unrollcuda-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,30 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/build.sh
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/df
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/requirements.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/upload.sh
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/docker/Dockerfile
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/docker/build.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/docker/check_gpu.sh
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/docker/requirements.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/docker/run.sh
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/docker/stop.sh
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/examples/cross.cu
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/examples/cross.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/examples/invert.cu
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/examples/invert.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/examples/mem_test.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/examples/unrollcuda_test.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/src/unrollcuda/__init__.py
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/src/unrollcuda/unrollcuda.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/LICENSE
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 unrollcuda-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/build.sh
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/df
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/upload.sh
+-rw-r--r--   0        0        0   354039 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/assets/cross.png
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/docker/Dockerfile
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/docker/build.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/docker/check_gpu.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/docker/requirements.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/docker/run.sh
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/docker/stop.sh
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/cross.cu
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/cross.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/elementwise_mul.cu
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/elementwise_mul.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/elementwise_mul_1.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/elementwise_mul_rev0.cu
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/invert.cu
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/invert.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/mem_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/nsight-sys.sh
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/requirements.txt
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/unrollcuda_test.py
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/examples/archive/unrollcuda_test_1.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/src/unrollcuda/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/src/unrollcuda/unrollcuda.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/LICENSE
+-rw-r--r--   0        0        0    11504 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 unrollcuda-0.0.7/PKG-INFO
```

### Comparing `unrollcuda-0.0.6/examples/cross.cu` & `unrollcuda-0.0.7/examples/invert.cu`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+#define MAX_DIMENSIONS 4 // Set the number of dimensions accordingly to your array
+
 __global__ void unroll(
     bool *arr,
     unsigned int *shape,
     unsigned long long gpu_arr_size,
     unsigned long long shape_total,
     unsigned long long dimensions_count,
     unsigned long long step,
     unsigned char order,
     unsigned long long batch_start
 )
 {
     unsigned long long idx = threadIdx.x + blockIdx.x * blockDim.x;
     unsigned long long idx_full;
     unsigned int i = 0;
-    unsigned int *indices = new unsigned int[dimensions_count]; // array to hold the computed indices
+    unsigned int indices[MAX_DIMENSIONS];
     unsigned long long tmp;
     
     idx_full = i * step + idx;
 
     while (idx_full < shape_total && idx_full < gpu_arr_size)
     {
         tmp = idx_full + batch_start; // add batch_start to account for the offset
@@ -30,22 +32,21 @@
             tmp /= shape[dimension];
         }
         //printf("idx_full: %llu, idx: %llu, batch_start: %llu\n", idx_full, idx, batch_start);
         
         for (unsigned int j = 0; j < dimensions_count; ++j)
         {
             // j is the dimension
-            // Your code there ++
-            if (indices[j] == 1)
-            {
-                // Set true if any index equals to 1
-                arr[idx_full] = true;
-                break;
-            }
-            // Your code there --
+            
+            // Your code ++
+            // Invert the value in arr
+            arr[idx_full] = !arr[idx_full];
+            // Your code --
+
+            break;
         }
         i += 1;
         idx_full = i * step + idx;
     }
     // Free the memory
     delete[] indices;
 }
```

### Comparing `unrollcuda-0.0.6/examples/invert.cu` & `unrollcuda-0.0.7/examples/elementwise_mul_rev0.cu`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+// Define MAX_DIMENSIONS as the maximum value dimensions_count can have
+//#define MAX_DIMENSIONS 10 
+
 __global__ void unroll(
-    bool *arr,
+    unsigned int *arr0,
+    unsigned int *arr1,
     unsigned int *shape,
     unsigned long long gpu_arr_size,
     unsigned long long shape_total,
     unsigned long long dimensions_count,
     unsigned long long step,
     unsigned char order,
-    unsigned long long batch_start
+    unsigned long long batch_start    
 )
 {
     unsigned long long idx = threadIdx.x + blockIdx.x * blockDim.x;
+    // if (idx==0) printf("gpu_arr_size: %llu, shape_total: %llu, dimensions_count: %llu, step: %llu, order: %u, batch_start: %llu\n", gpu_arr_size, shape_total, dimensions_count, step, order, batch_start);
     unsigned long long idx_full;
-    unsigned int i = 0;
+    unsigned long long i = 0;
     unsigned int *indices = new unsigned int[dimensions_count]; // array to hold the computed indices
+    // Declare indices as a fixed-size array in shared memory
+    //__shared__ unsigned int indices[MAX_DIMENSIONS];
     unsigned long long tmp;
     
     idx_full = i * step + idx;
 
     while (idx_full < shape_total && idx_full < gpu_arr_size)
     {
         tmp = idx_full + batch_start; // add batch_start to account for the offset
@@ -32,16 +39,19 @@
         //printf("idx_full: %llu, idx: %llu, batch_start: %llu\n", idx_full, idx, batch_start);
         
         for (unsigned int j = 0; j < dimensions_count; ++j)
         {
             // j is the dimension
             
             // Your code ++
-            // Invert the value in arr
-            arr[idx_full] = !arr[idx_full];
+            // Multiply elementwise
+            //if (j==2) 
+            //printf("j: %u, indices[j]: %u, arr1[idx_full]: %u, arr0[idx_full]: %u\n", j, indices[j], arr1[idx_full], arr0[idx_full]);
+            if (idx==0) printf("j: %u, indices[j]: %u, arr1[idx_full]: %u, arr0[idx_full]: %u\n", j, indices[j], arr1[idx_full], arr0[idx_full]);
+            arr0[idx_full] = arr0[idx_full] * arr1[idx_full];
             // Your code --
 
             break;
         }
         i += 1;
         idx_full = i * step + idx;
     }
```

### Comparing `unrollcuda-0.0.6/examples/invert.py` & `unrollcuda-0.0.7/examples/invert.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numpy as np
 import unrollcuda as uc
 
 
 def main():
         
-    dimensions = [3, 4, 7, 12]
+    dimensions = [2000, 100, 100, 100]
     shape = [int(size) for size in dimensions]
     # random boolean values
     arr = np.random.choice(
         a=[False, True],
         size=shape,
         p=[0.5, 0.5],
         )
     print('Array shape: ', arr.shape)
+    print('Array size: ', arr.size)
     
     # Read the kernel code from the file
     with open('invert.cu', 'r') as f:
         kernel_code = f.read()
     # Define the unrollcuda instance
     ker = uc.kernel(kernel_code)
     # Call inference
```

### Comparing `unrollcuda-0.0.6/examples/mem_test.py` & `unrollcuda-0.0.7/examples/mem_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import unrollcuda_test as uc
+import unrollcuda as uc
 import psutil
 
 
 def main():
     # Define the unrollcuda instance
     ker = uc.kernel()
 
@@ -20,8 +20,7 @@
     ram_memory = psutil.virtual_memory().available/1024**3
     # Format to x.xx
     ram_memory = "{:.2f}".format(ram_memory)
     print('RAM memory available: ',ram_memory,'Gb')
 
 if __name__ == '__main__':
     main()
-
```

### Comparing `unrollcuda-0.0.6/src/unrollcuda/__init__.py` & `unrollcuda-0.0.7/src/unrollcuda/__init__.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.6/LICENSE` & `unrollcuda-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.6/pyproject.toml` & `unrollcuda-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","numpy","pycuda"]
 build-backend = "hatchling.build"
 
 [project]
 name = "unrollcuda"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Aleksei Iurasov", email="format37@gmail.com" },
 ]
 description = "Loop unrolling and batching for CUDA"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

