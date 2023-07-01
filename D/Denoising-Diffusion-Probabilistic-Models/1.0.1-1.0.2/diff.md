# Comparing `tmp/Denoising_Diffusion_Probabilistic_Models-1.0.1-py3-none-any.whl.zip` & `tmp/Denoising_Diffusion_Probabilistic_Models-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9647 bytes, number of entries: 11
--rw-r--r--  2.0 unx     6979 b- defN 23-Jun-25 11:47 diffusion/DDMFunctions.py
--rw-r--r--  2.0 unx    10005 b- defN 23-Jun-25 11:47 diffusion/Network.py
--rw-r--r--  2.0 unx     1192 b- defN 23-Jun-25 11:47 diffusion/Scheduler.py
--rw-r--r--  2.0 unx      134 b- defN 23-Jun-25 11:47 diffusion/Test.py
--rw-r--r--  2.0 unx     3457 b- defN 23-Jun-25 11:47 diffusion/Train.py
--rw-r--r--  2.0 unx      189 b- defN 23-Jun-25 11:47 diffusion/__init__.py
--rw-r--r--  2.0 unx      355 b- defN 23-Jun-25 11:47 diffusion/diffusion_process.py
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD
-11 files, 23822 bytes uncompressed, 7963 bytes compressed:  66.6%
+Zip file size: 9716 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     7135 b- defN 23-Jul-01 08:06 diffusion/DDMFunctions.py
+-rw-r--r--  2.0 unx    10005 b- defN 23-Jul-01 08:06 diffusion/Network.py
+-rw-r--r--  2.0 unx     1192 b- defN 23-Jul-01 08:06 diffusion/Scheduler.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Jul-01 08:06 diffusion/Test.py
+-rw-r--r--  2.0 unx     3457 b- defN 23-Jul-01 08:06 diffusion/Train.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Jul-01 08:06 diffusion/__init__.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Jul-01 08:06 diffusion/diffusion_process.py
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-01 08:07 Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 08:07 Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-01 08:07 Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-01 08:07 Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/RECORD
+11 files, 23978 bytes uncompressed, 8032 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: diffusion/__init__.py
 Comment: 
 
 Filename: diffusion/diffusion_process.py
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/METADATA
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/WHEEL
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/top_level.txt
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## diffusion/DDMFunctions.py

```diff
@@ -47,14 +47,17 @@
 
         # 事後確率 q(x_{t-1} | x_t, x_0)の計算
         self.posterior_variance = self.betas * (1. - self.alphas_cumprod_prev) / (1. - self.alphas_cumprod)
 
         self.noise_list = []
 
     def extract(self, a, t, x_shape):
+        """
+        バッチのインデックスに対して適切なtインデックスを抽出します。
+        """
         batch_size = t.shape[0]
         out = a.gather(-1, t.cpu())
         return out.reshape(batch_size, *((1,) * (len(x_shape) - 1))).to(t.device)
 
 
     def reverse_transform(self, im):
         im = im.squeeze().numpy().transpose(1, 2, 0)
@@ -63,15 +66,15 @@
         return im
 
 
     # @title 画像の表示の定義
     def plot(self, x_noisy, timestep=None):
         noisy_image = self.reverse_transform(x_noisy)
         if timestep is not None:
-            text = "Step:" + str(timestep)
+            text = "Step:" + str(timestep + 1)
             plt.text(0, 0, text, fontdict=None, bbox=dict(facecolor='white', alpha=1))
         plt.axis('off')
         plt.imshow(noisy_image)
         plt.show()
 
     def p_losses(self, denoise_model, x_start, t, noise=None, loss_type="l1"):
         if noise is None:
@@ -190,17 +193,19 @@
 
     def transforms(self, examples):
        examples["pixel_values"] = [transform(image.convert("L")) for image in examples["image"]]
        del examples["image"]
     
        return examples
 
-    # 教材確認用
-    # 画像を指定のサイズに切り取って、値域を0-255 から -1.0 - +1.0 に変換
     def transform_(self, image_size):
+        """
+        教材確認用
+        画像を指定のサイズに切り取って、値域を0-255 から -1.0 - +1.0 に変換
+        """
         return Compose([
             Resize(image_size),
             CenterCrop(image_size),
             ToTensor(),
             Lambda(lambda t: (t * 2) - 1),
         ])
```

## Comparing `Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD` & `Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-diffusion/DDMFunctions.py,sha256=KBh012fZb7RmvP45K0Oh33VDagNOWbhDhSZ4Zv5QLGk,6979
+diffusion/DDMFunctions.py,sha256=g-zuVqnkr_D8T9Ns8kw2qMHWCYjmnMgNGaxxfiOCL4w,7135
 diffusion/Network.py,sha256=DBIyc-o6Q0ScwT6ITI6MNauX3As0vl-hhK2MIPVkEfU,10005
 diffusion/Scheduler.py,sha256=d9TpBH7yrX8QPqNnEhJ04ULLTNGQMdPOg28HWyqtRug,1192
 diffusion/Test.py,sha256=7TsJJE83SWWspqaav9ZmbgYbkXjMleVJyehPdoBkqRk,134
 diffusion/Train.py,sha256=pr7OKXCSX1hk_vIIHmnspl_4az9_b4-cIkS04ut_06k,3457
 diffusion/__init__.py,sha256=HhslOaOBONU0AL5pSzfZesj7SfohsvKoEmoHoKehicQ,189
 diffusion/diffusion_process.py,sha256=XciyhvrGX1an4p0QywgOq3Q3HjAXcKGYVJS7YodIcrw,355
-Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/METADATA,sha256=rvNjTCy27_iKp0941Io-MrphDjwH_XF6U287DbTxZ0M,430
-Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
-Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD,,
+Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/METADATA,sha256=6fge18kx7Ai2oFd_TCG1JXCt5KccX0K3qfAz4rWTUZk,430
+Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
+Denoising_Diffusion_Probabilistic_Models-1.0.2.dist-info/RECORD,,
```

