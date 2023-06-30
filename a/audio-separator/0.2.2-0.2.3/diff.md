# Comparing `tmp/audio_separator-0.2.2.tar.gz` & `tmp/audio_separator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.2.2.tar", max compression
+gzip compressed data, was "audio_separator-0.2.3.tar", max compression
```

## Comparing `audio_separator-0.2.2.tar` & `audio_separator-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.2.2/LICENSE
--rw-r--r--   0        0        0     6469 2023-06-30 22:31:30.149482 audio_separator-0.2.2/README.md
--rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.2.2/audio_separator/__init__.py
--rw-r--r--   0        0        0    10902 2023-06-30 22:32:23.003055 audio_separator-0.2.2/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.2.2/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     1695 2023-06-30 22:44:02.036737 audio_separator-0.2.2/audio_separator/utils/cli.py
--rw-r--r--   0        0        0     2135 2023-06-30 05:58:37.421373 audio_separator-0.2.2/audio_separator/utils/pyrb.py
--rw-r--r--   0        0        0    24840 2023-06-30 06:51:10.010639 audio_separator-0.2.2/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      672 2023-06-30 22:40:44.479802 audio_separator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 audio_separator-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6469 2023-06-30 22:31:30.149482 audio_separator-0.2.3/README.md
+-rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.2.3/audio_separator/__init__.py
+-rw-r--r--   0        0        0    11008 2023-06-30 22:48:43.228969 audio_separator-0.2.3/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.2.3/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     1726 2023-06-30 22:48:43.140580 audio_separator-0.2.3/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0     2041 2023-06-30 22:48:43.147133 audio_separator-0.2.3/audio_separator/utils/pyrb.py
+-rw-r--r--   0        0        0    24722 2023-06-30 22:48:43.362641 audio_separator-0.2.3/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      760 2023-06-30 22:50:14.138142 audio_separator-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 audio_separator-0.2.3/PKG-INFO
```

### Comparing `audio_separator-0.2.2/LICENSE` & `audio_separator-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.2/README.md` & `audio_separator-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.2/audio_separator/separator.py` & `audio_separator-0.2.3/audio_separator/separator.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,242 +9,252 @@
 import torch
 import librosa
 import numpy as np
 import onnxruntime as ort
 import soundfile as sf
 from audio_separator.utils import spec_utils
 
+
 def print_with_timestamp(message):
     timestamp = datetime.datetime.now().isoformat()
     print(f"{timestamp} - {message}")
 
+
 class Separator:
-    def __init__(self, audio_file_path, model_name='UVR_MDXNET_KARA_2', model_file_dir='/tmp/audio-separator-models/', output_dir=None):
+    def __init__(self, audio_file_path, model_name="UVR_MDXNET_KARA_2", model_file_dir="/tmp/audio-separator-models/", output_dir=None):
         self.model_name = model_name
         self.model_file_dir = model_file_dir
         self.output_dir = output_dir
 
         # Create the model directory if it does not exist
         os.makedirs(self.model_file_dir, exist_ok=True)
 
         self.audio_file_path = audio_file_path
         self.audio_file_base = os.path.splitext(os.path.basename(audio_file_path))[0]
 
         self.model_name = model_name
-        self.model_url = f'https://github.com/TRvlvr/model_repo/releases/download/all_public_uvr_models/{self.model_name}.onnx'
-        self.model_data_url = 'https://raw.githubusercontent.com/TRvlvr/application_data/main/mdx_model_data/model_data.json'
-        
+        self.model_url = f"https://github.com/TRvlvr/model_repo/releases/download/all_public_uvr_models/{self.model_name}.onnx"
+        self.model_data_url = "https://raw.githubusercontent.com/TRvlvr/application_data/main/mdx_model_data/model_data.json"
+
         self.wav_type_set = "PCM_16"
         self.is_normalization = False
         self.is_denoise = False
 
         self.chunks = 0
         self.margin = 44100
         self.adjust = 1
         self.dim_c = 4
         self.hop = 1024
 
         self.primary_source = None
         self.secondary_source = None
 
         warnings.filterwarnings("ignore")
-        self.cpu = torch.device('cpu')
-        self.device = torch.device('cpu')
-        self.run_type = ['CPUExecutionProvider']
+        self.cpu = torch.device("cpu")
+        self.device = torch.device("cpu")
+        self.run_type = ["CPUExecutionProvider"]
 
     def get_model_hash(self, model_path):
         try:
-            with open(model_path, 'rb') as f:
-                f.seek(- 10000 * 1024, 2)
+            with open(model_path, "rb") as f:
+                f.seek(-10000 * 1024, 2)
                 return hashlib.md5(f.read()).hexdigest()
         except:
-            return hashlib.md5(open(model_path,'rb').read()).hexdigest()
+            return hashlib.md5(open(model_path, "rb").read()).hexdigest()
 
     def separate(self):
-        model_path = os.path.join(self.model_file_dir, f'{self.model_name}.onnx')
+        model_path = os.path.join(self.model_file_dir, f"{self.model_name}.onnx")
         if not os.path.isfile(model_path):
-            print_with_timestamp(f'Model not found at path {model_path}, downloading...')
+            print_with_timestamp(f"Model not found at path {model_path}, downloading...")
             wget.download(self.model_url, model_path)
 
-        print_with_timestamp('Reading model settings...')
+        print_with_timestamp("Reading model settings...")
 
         model_hash = self.get_model_hash(model_path)
-        print_with_timestamp(f'Model {model_path} has hash {model_hash} ...')
-        
-        model_data_path = os.path.join(self.model_file_dir, 'model_data.json')
+        print_with_timestamp(f"Model {model_path} has hash {model_hash} ...")
+
+        model_data_path = os.path.join(self.model_file_dir, "model_data.json")
         if not os.path.isfile(model_data_path):
-            print_with_timestamp(f'Model data not found at path {model_data_path}, downloading...')
+            print_with_timestamp(f"Model data not found at path {model_data_path}, downloading...")
             wget.download(self.model_data_url, model_data_path)
 
         model_data_object = json.load(open(model_data_path))
         model_data = model_data_object[model_hash]
-        
+
         self.compensate = model_data["compensate"]
         self.dim_f = model_data["mdx_dim_f_set"]
-        self.dim_t = 2**model_data["mdx_dim_t_set"]
+        self.dim_t = 2 ** model_data["mdx_dim_t_set"]
         self.n_fft = model_data["mdx_n_fft_scale_set"]
         self.primary_stem = model_data["primary_stem"]
         self.secondary_stem = "Vocals" if self.primary_stem == "Instrumental" else "Instrumental"
 
-        print_with_timestamp(f'Set model data values: compensate = {self.compensate} primary_stem = {self.primary_stem} dim_f = {self.dim_f} dim_t = {self.dim_t} n_fft = {self.n_fft}') 
+        print_with_timestamp(
+            f"Set model data values: compensate = {self.compensate} primary_stem = {self.primary_stem} dim_f = {self.dim_f} dim_t = {self.dim_t} n_fft = {self.n_fft}"
+        )
 
-        print_with_timestamp('Loading model...')
+        print_with_timestamp("Loading model...")
         ort_ = ort.InferenceSession(model_path, providers=self.run_type)
-        self.model_run = lambda spek:ort_.run(None, {'input': spek.cpu().numpy()})[0]
+        self.model_run = lambda spek: ort_.run(None, {"input": spek.cpu().numpy()})[0]
 
         self.initialize_model_settings()
-        print_with_timestamp('Running inference...')
+        print_with_timestamp("Running inference...")
         mdx_net_cut = True
         mix, raw_mix, samplerate = prepare_mix(self.audio_file_path, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
-        print_with_timestamp('Demixing...')
+        print_with_timestamp("Demixing...")
         source = self.demix_base(mix)[0]
 
-        print_with_timestamp(f'Saving {self.primary_stem} stem...')
-        primary_stem_path = os.path.join(f'{self.audio_file_base}_({self.primary_stem})_{self.model_name}.wav')
+        print_with_timestamp(f"Saving {self.primary_stem} stem...")
+        primary_stem_path = os.path.join(f"{self.audio_file_base}_({self.primary_stem})_{self.model_name}.wav")
         if not isinstance(self.primary_source, np.ndarray):
             self.primary_source = spec_utils.normalize(source, self.is_normalization).T
         self.write_audio(primary_stem_path, self.primary_source, samplerate)
 
-        print_with_timestamp(f'Saving {self.secondary_stem} stem...')
-        secondary_stem_path = os.path.join(f'{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.wav')
+        print_with_timestamp(f"Saving {self.secondary_stem} stem...")
+        secondary_stem_path = os.path.join(f"{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.wav")
         if not isinstance(self.secondary_source, np.ndarray):
             raw_mix = self.demix_base(raw_mix, is_match_mix=True)[0] if mdx_net_cut else raw_mix
-            self.secondary_source, raw_mix = spec_utils.normalize_two_stem(source*self.compensate, raw_mix, self.is_normalization)
-            self.secondary_source = (-self.secondary_source.T+raw_mix.T)
+            self.secondary_source, raw_mix = spec_utils.normalize_two_stem(source * self.compensate, raw_mix, self.is_normalization)
+            self.secondary_source = -self.secondary_source.T + raw_mix.T
         self.write_audio(secondary_stem_path, self.secondary_source, samplerate)
 
         torch.cuda.empty_cache()
         return primary_stem_path, secondary_stem_path
 
     def write_audio(self, stem_path, stem_source, samplerate):
         # If output_dir is specified, create it and join it with stem_path
         if self.output_dir:
             # Create the output directory if it does not exist
             os.makedirs(self.output_dir, exist_ok=True)
             stem_path = os.path.join(self.output_dir, stem_path)
-        
+
         sf.write(stem_path, stem_source, samplerate, subtype=self.wav_type_set)
 
     def initialize_model_settings(self):
-        self.n_bins = self.n_fft//2+1
-        self.trim = self.n_fft//2
-        self.chunk_size = self.hop * (self.dim_t-1)
+        self.n_bins = self.n_fft // 2 + 1
+        self.trim = self.n_fft // 2
+        self.chunk_size = self.hop * (self.dim_t - 1)
         self.window = torch.hann_window(window_length=self.n_fft, periodic=False).to(self.device)
-        self.freq_pad = torch.zeros([1, self.dim_c, self.n_bins-self.dim_f, self.dim_t]).to(self.device)
-        self.gen_size = self.chunk_size-2*self.trim
+        self.freq_pad = torch.zeros([1, self.dim_c, self.n_bins - self.dim_f, self.dim_t]).to(self.device)
+        self.gen_size = self.chunk_size - 2 * self.trim
 
     def initialize_mix(self, mix, is_ckpt=False):
         if is_ckpt:
             pad = self.gen_size + self.trim - ((mix.shape[-1]) % self.gen_size)
-            mixture = np.concatenate((np.zeros((2, self.trim), dtype='float32'),mix, np.zeros((2, pad), dtype='float32')), 1)
+            mixture = np.concatenate((np.zeros((2, self.trim), dtype="float32"), mix, np.zeros((2, pad), dtype="float32")), 1)
             num_chunks = mixture.shape[-1] // self.gen_size
-            mix_waves = [mixture[:, i * self.gen_size: i * self.gen_size + self.chunk_size] for i in range(num_chunks)]
+            mix_waves = [mixture[:, i * self.gen_size : i * self.gen_size + self.chunk_size] for i in range(num_chunks)]
         else:
             mix_waves = []
             n_sample = mix.shape[1]
-            pad = self.gen_size - n_sample%self.gen_size
-            mix_p = np.concatenate((np.zeros((2,self.trim)), mix, np.zeros((2,pad)), np.zeros((2,self.trim))), 1)
+            pad = self.gen_size - n_sample % self.gen_size
+            mix_p = np.concatenate((np.zeros((2, self.trim)), mix, np.zeros((2, pad)), np.zeros((2, self.trim))), 1)
             i = 0
             while i < n_sample + pad:
-                waves = np.array(mix_p[:, i:i+self.chunk_size])
+                waves = np.array(mix_p[:, i : i + self.chunk_size])
                 mix_waves.append(waves)
                 i += self.gen_size
-                
+
         mix_waves = torch.tensor(mix_waves, dtype=torch.float32).to(self.device)
 
         return mix_waves, pad
-    
+
     def demix_base(self, mix, is_ckpt=False, is_match_mix=False):
         chunked_sources = []
         for slice in mix:
             sources = []
             tar_waves_ = []
             mix_p = mix[slice]
             mix_waves, pad = self.initialize_mix(mix_p, is_ckpt=is_ckpt)
             mix_waves = mix_waves.split(1)
             pad = mix_p.shape[-1] if is_ckpt else -pad
             with torch.no_grad():
                 for mix_wave in mix_waves:
                     tar_waves = self.run_model(mix_wave, is_ckpt=is_ckpt, is_match_mix=is_match_mix)
                     tar_waves_.append(tar_waves)
-                tar_waves_ = np.vstack(tar_waves_)[:, :, self.trim:-self.trim] if is_ckpt else tar_waves_
+                tar_waves_ = np.vstack(tar_waves_)[:, :, self.trim : -self.trim] if is_ckpt else tar_waves_
                 tar_waves = np.concatenate(tar_waves_, axis=-1)[:, :pad]
                 start = 0 if slice == 0 else self.margin
                 end = None if slice == list(mix.keys())[::-1][0] or self.margin == 0 else -self.margin
-                sources.append(tar_waves[:,start:end]*(1/self.adjust))
+                sources.append(tar_waves[:, start:end] * (1 / self.adjust))
             chunked_sources.append(sources)
         sources = np.concatenate(chunked_sources, axis=-1)
-        
+
         return sources
 
     def run_model(self, mix, is_ckpt=False, is_match_mix=False):
-        
-        spek = self.stft(mix.to(self.device))*self.adjust
-        spek[:, :, :3, :] *= 0 
+        spek = self.stft(mix.to(self.device)) * self.adjust
+        spek[:, :, :3, :] *= 0
 
         if is_match_mix:
             spec_pred = spek.cpu().numpy()
         else:
-            spec_pred = -self.model_run(-spek)*0.5+self.model_run(spek)*0.5 if self.is_denoise else self.model_run(spek)
+            spec_pred = -self.model_run(-spek) * 0.5 + self.model_run(spek) * 0.5 if self.is_denoise else self.model_run(spek)
 
         if is_ckpt:
             return self.istft(spec_pred).cpu().detach().numpy()
-        else: 
-            return self.istft(torch.tensor(spec_pred).to(self.device)).to(self.cpu)[:,:,self.trim:-self.trim].transpose(0,1).reshape(2, -1).numpy()
-    
+        else:
+            return (
+                self.istft(torch.tensor(spec_pred).to(self.device))
+                .to(self.cpu)[:, :, self.trim : -self.trim]
+                .transpose(0, 1)
+                .reshape(2, -1)
+                .numpy()
+            )
+
     def stft(self, x):
         x = x.reshape([-1, self.chunk_size])
-        x = torch.stft(x, n_fft=self.n_fft, hop_length=self.hop, window=self.window, center=True,return_complex=True)
-        x=torch.view_as_real(x)
-        x = x.permute([0,3,1,2])
-        x = x.reshape([-1,2,2,self.n_bins,self.dim_t]).reshape([-1,self.dim_c,self.n_bins,self.dim_t])
-        return x[:,:,:self.dim_f]
+        x = torch.stft(x, n_fft=self.n_fft, hop_length=self.hop, window=self.window, center=True, return_complex=True)
+        x = torch.view_as_real(x)
+        x = x.permute([0, 3, 1, 2])
+        x = x.reshape([-1, 2, 2, self.n_bins, self.dim_t]).reshape([-1, self.dim_c, self.n_bins, self.dim_t])
+        return x[:, :, : self.dim_f]
 
     def istft(self, x, freq_pad=None):
-        freq_pad = self.freq_pad.repeat([x.shape[0],1,1,1]) if freq_pad is None else freq_pad
+        freq_pad = self.freq_pad.repeat([x.shape[0], 1, 1, 1]) if freq_pad is None else freq_pad
         x = torch.cat([x, freq_pad], -2)
-        x = x.reshape([-1,2,2,self.n_bins,self.dim_t]).reshape([-1,2,self.n_bins,self.dim_t])
-        x = x.permute([0,2,3,1])
-        x=x.contiguous()
-        x=torch.view_as_complex(x)
+        x = x.reshape([-1, 2, 2, self.n_bins, self.dim_t]).reshape([-1, 2, self.n_bins, self.dim_t])
+        x = x.permute([0, 2, 3, 1])
+        x = x.contiguous()
+        x = torch.view_as_complex(x)
         x = torch.istft(x, n_fft=self.n_fft, hop_length=self.hop, window=self.window, center=True)
-        return x.reshape([-1,2,self.chunk_size])
+        return x.reshape([-1, 2, self.chunk_size])
+
 
 def prepare_mix(mix, chunk_set, margin_set, mdx_net_cut=False, is_missing_mix=False):
     samplerate = 44100
 
     if not isinstance(mix, np.ndarray):
         mix, samplerate = librosa.load(mix, mono=False, sr=44100)
     else:
         mix = mix.T
 
     if mix.ndim == 1:
-        mix = np.asfortranarray([mix,mix])
+        mix = np.asfortranarray([mix, mix])
 
     def get_segmented_mix(chunk_set=chunk_set):
         segmented_mix = {}
-        
+
         samples = mix.shape[-1]
         margin = margin_set
-        chunk_size = chunk_set*44100
-        assert not margin == 0, 'margin cannot be zero!'
-        
+        chunk_size = chunk_set * 44100
+        assert not margin == 0, "margin cannot be zero!"
+
         if margin > chunk_size:
             margin = chunk_size
         if chunk_set == 0 or samples < chunk_size:
             chunk_size = samples
-        
+
         counter = -1
         for skip in range(0, samples, chunk_size):
-            counter+=1
+            counter += 1
             s_margin = 0 if counter == 0 else margin
-            end = min(skip+chunk_size+margin, samples)
-            start = skip-s_margin
-            segmented_mix[skip] = mix[:,start:end].copy()
+            end = min(skip + chunk_size + margin, samples)
+            start = skip - s_margin
+            segmented_mix[skip] = mix[:, start:end].copy()
             if end == samples:
                 break
-            
+
         return segmented_mix
-    
+
     segmented_mix = get_segmented_mix()
     raw_mix = get_segmented_mix(chunk_set=0) if mdx_net_cut else mix
     return segmented_mix, raw_mix, samplerate
```

### Comparing `audio_separator-0.2.2/audio_separator/utils/cli.py` & `audio_separator-0.2.3/audio_separator/utils/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,34 +9,38 @@
     timestamp = datetime.datetime.now().isoformat()
     print(f"{timestamp} - {message}")
 
 
 def main():
     parser = argparse.ArgumentParser(description="Separate audio file into different stems.")
 
-    parser.add_argument("audio_file", nargs='?', help="The audio file path to separate.", default=argparse.SUPPRESS)
-    parser.add_argument("--model_name", default='UVR_MDXNET_KARA_2', help="Optional model name to be used for separation.")
-    parser.add_argument("--model_file_dir", default='/tmp/audio-separator-models/', help="Optional model files directory.")
-    parser.add_argument("--output_dir", default=None, help="Optional directory where the separated files will be saved. If not specified, outputs to current dir.")
-    parser.add_argument('--version', action='store_true', help='Show the version number and exit')
+    parser.add_argument("audio_file", nargs="?", help="The audio file path to separate.", default=argparse.SUPPRESS)
+    parser.add_argument("--model_name", default="UVR_MDXNET_KARA_2", help="Optional model name to be used for separation.")
+    parser.add_argument("--model_file_dir", default="/tmp/audio-separator-models/", help="Optional model files directory.")
+    parser.add_argument(
+        "--output_dir",
+        default=None,
+        help="Optional directory where the separated files will be saved. If not specified, outputs to current dir.",
+    )
+    parser.add_argument("--version", action="store_true", help="Show the version number and exit")
 
     args = parser.parse_args()
 
     if args.version:
         version = pkg_resources.get_distribution("audio-separator").version
         print(f"audio-separator version: {version}")
         exit(0)
 
-    if not hasattr(args, 'audio_file'):
+    if not hasattr(args, "audio_file"):
         parser.print_help()
         exit(1)
 
-    print_with_timestamp(f'Separator beginning with input file: {args.audio_file}')
+    print_with_timestamp(f"Separator beginning with input file: {args.audio_file}")
 
     separator = Separator(args.audio_file, model_name=args.model_name, model_file_dir=args.model_file_dir, output_dir=args.output_dir)
     primary_stem_path, secondary_stem_path = separator.separate()
 
-    print_with_timestamp(f'Separation complete! Output files: {primary_stem_path} {secondary_stem_path}')
+    print_with_timestamp(f"Separation complete! Output files: {primary_stem_path} {secondary_stem_path}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `audio_separator-0.2.2/audio_separator/utils/pyrb.py` & `audio_separator-0.2.3/audio_separator/utils/pyrb.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 import subprocess
 import tempfile
 import six
 import numpy as np
 import soundfile as sf
 import sys
 
-if getattr(sys, 'frozen', False):
+if getattr(sys, "frozen", False):
     BASE_PATH_RUB = sys._MEIPASS
 else:
     BASE_PATH_RUB = os.path.dirname(os.path.abspath(__file__))
 
-__all__ = ['time_stretch', 'pitch_shift']
+__all__ = ["time_stretch", "pitch_shift"]
 
-__RUBBERBAND_UTIL = os.path.join(BASE_PATH_RUB, 'rubberband')
+__RUBBERBAND_UTIL = os.path.join(BASE_PATH_RUB, "rubberband")
 
 if six.PY2:
-    DEVNULL = open(os.devnull, 'w')
+    DEVNULL = open(os.devnull, "w")
 else:
     DEVNULL = subprocess.DEVNULL
 
-def __rubberband(y, sr, **kwargs):
 
+def __rubberband(y, sr, **kwargs):
     assert sr > 0
 
     # Get the input and output tempfile
-    fd, infile = tempfile.mkstemp(suffix='.wav')
+    fd, infile = tempfile.mkstemp(suffix=".wav")
     os.close(fd)
-    fd, outfile = tempfile.mkstemp(suffix='.wav')
+    fd, outfile = tempfile.mkstemp(suffix=".wav")
     os.close(fd)
 
     # dump the audio
     sf.write(infile, y, sr)
 
     try:
         # Execute rubberband
-        arguments = [__RUBBERBAND_UTIL, '-q']
+        arguments = [__RUBBERBAND_UTIL, "-q"]
 
         for key, value in six.iteritems(kwargs):
             arguments.append(str(key))
             arguments.append(str(value))
 
         arguments.extend([infile, outfile])
 
@@ -49,44 +49,42 @@
         y_out, _ = sf.read(outfile, always_2d=True)
 
         # make sure that output dimensions matches input
         if y.ndim == 1:
             y_out = np.squeeze(y_out)
 
     except OSError as exc:
-        six.raise_from(RuntimeError('Failed to execute rubberband. '
-                                    'Please verify that rubberband-cli '
-                                    'is installed.'),
-                       exc)
+        six.raise_from(RuntimeError("Failed to execute rubberband. " "Please verify that rubberband-cli " "is installed."), exc)
 
     finally:
         # Remove temp files
         os.unlink(infile)
         os.unlink(outfile)
 
     return y_out
 
+
 def time_stretch(y, sr, rate, rbargs=None):
     if rate <= 0:
-        raise ValueError('rate must be strictly positive')
+        raise ValueError("rate must be strictly positive")
 
     if rate == 1.0:
         return y
 
     if rbargs is None:
         rbargs = dict()
 
-    rbargs.setdefault('--tempo', rate)
+    rbargs.setdefault("--tempo", rate)
 
     return __rubberband(y, sr, **rbargs)
 
-def pitch_shift(y, sr, n_steps, rbargs=None):
 
+def pitch_shift(y, sr, n_steps, rbargs=None):
     if n_steps == 0:
         return y
 
     if rbargs is None:
         rbargs = dict()
 
-    rbargs.setdefault('--pitch', n_steps)
+    rbargs.setdefault("--pitch", n_steps)
 
     return __rubberband(y, sr, **rbargs)
```

### Comparing `audio_separator-0.2.2/audio_separator/utils/spec_utils.py` & `audio_separator-0.2.3/audio_separator/utils/spec_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,221 +7,230 @@
 import platform
 import traceback
 import datetime
 
 OPERATING_SYSTEM = platform.system()
 SYSTEM_ARCH = platform.platform()
 SYSTEM_PROC = platform.processor()
-ARM = 'arm'
+ARM = "arm"
 
-if OPERATING_SYSTEM == 'Windows':
+if OPERATING_SYSTEM == "Windows":
     from pyrubberband import pyrb
 else:
     from audio_separator.utils import pyrb
 
-if OPERATING_SYSTEM == 'Darwin':
-    wav_resolution = "polyphase" if SYSTEM_PROC == ARM or ARM in SYSTEM_ARCH else "sinc_fastest" 
+if OPERATING_SYSTEM == "Darwin":
+    wav_resolution = "polyphase" if SYSTEM_PROC == ARM or ARM in SYSTEM_ARCH else "sinc_fastest"
 else:
     wav_resolution = "sinc_fastest"
 
-MAX_SPEC = 'Max Spec'
-MIN_SPEC = 'Min Spec'
-AVERAGE = 'Average'
+MAX_SPEC = "Max Spec"
+MIN_SPEC = "Min Spec"
+AVERAGE = "Average"
+
 
 def print_with_timestamp(message):
     timestamp = datetime.datetime.now().isoformat()
     print(f"{timestamp} - {message}")
 
+
 def crop_center(h1, h2):
     h1_shape = h1.size()
     h2_shape = h2.size()
 
     if h1_shape[3] == h2_shape[3]:
         return h1
     elif h1_shape[3] < h2_shape[3]:
-        raise ValueError('h1_shape[3] must be greater than h2_shape[3]')
+        raise ValueError("h1_shape[3] must be greater than h2_shape[3]")
 
     s_time = (h1_shape[3] - h2_shape[3]) // 2
     e_time = s_time + h2_shape[3]
     h1 = h1[:, :, :, s_time:e_time]
 
     return h1
 
+
 def preprocess(X_spec):
     X_mag = np.abs(X_spec)
     X_phase = np.angle(X_spec)
 
     return X_mag, X_phase
 
+
 def make_padding(width, cropsize, offset):
     left = offset
     roi_size = cropsize - offset * 2
     if roi_size == 0:
         roi_size = cropsize
     right = roi_size - (width % roi_size) + left
 
     return left, right, roi_size
 
+
 def wave_to_spectrogram(wave, hop_length, n_fft, mid_side=False, mid_side_b2=False, reverse=False):
     if reverse:
         wave_left = np.flip(np.asfortranarray(wave[0]))
         wave_right = np.flip(np.asfortranarray(wave[1]))
     elif mid_side:
         wave_left = np.asfortranarray(np.add(wave[0], wave[1]) / 2)
         wave_right = np.asfortranarray(np.subtract(wave[0], wave[1]))
     elif mid_side_b2:
-        wave_left = np.asfortranarray(np.add(wave[1], wave[0] * .5))
-        wave_right = np.asfortranarray(np.subtract(wave[0], wave[1] * .5))
+        wave_left = np.asfortranarray(np.add(wave[1], wave[0] * 0.5))
+        wave_right = np.asfortranarray(np.subtract(wave[0], wave[1] * 0.5))
     else:
         wave_left = np.asfortranarray(wave[0])
         wave_right = np.asfortranarray(wave[1])
 
     spec_left = librosa.stft(wave_left, n_fft, hop_length=hop_length)
     spec_right = librosa.stft(wave_right, n_fft, hop_length=hop_length)
-    
+
     spec = np.asfortranarray([spec_left, spec_right])
 
     return spec
-   
+
+
 def wave_to_spectrogram_mt(wave, hop_length, n_fft, mid_side=False, mid_side_b2=False, reverse=False):
     import threading
 
     if reverse:
         wave_left = np.flip(np.asfortranarray(wave[0]))
         wave_right = np.flip(np.asfortranarray(wave[1]))
     elif mid_side:
         wave_left = np.asfortranarray(np.add(wave[0], wave[1]) / 2)
         wave_right = np.asfortranarray(np.subtract(wave[0], wave[1]))
     elif mid_side_b2:
-        wave_left = np.asfortranarray(np.add(wave[1], wave[0] * .5))
-        wave_right = np.asfortranarray(np.subtract(wave[0], wave[1] * .5))
+        wave_left = np.asfortranarray(np.add(wave[1], wave[0] * 0.5))
+        wave_right = np.asfortranarray(np.subtract(wave[0], wave[1] * 0.5))
     else:
         wave_left = np.asfortranarray(wave[0])
         wave_right = np.asfortranarray(wave[1])
-   
+
     def run_thread(**kwargs):
         global spec_left
         spec_left = librosa.stft(**kwargs)
 
-    thread = threading.Thread(target=run_thread, kwargs={'y': wave_left, 'n_fft': n_fft, 'hop_length': hop_length})
+    thread = threading.Thread(target=run_thread, kwargs={"y": wave_left, "n_fft": n_fft, "hop_length": hop_length})
     thread.start()
     spec_right = librosa.stft(wave_right, n_fft, hop_length=hop_length)
-    thread.join()   
-    
+    thread.join()
+
     spec = np.asfortranarray([spec_left, spec_right])
 
     return spec
-    
+
+
 def normalize(wave, is_normalize=False):
     """Save output music files"""
     maxv = np.abs(wave).max()
     if maxv > 1.0:
         print_with_timestamp(f"Normalization Set {is_normalize}: Input above threshold for clipping. Max:{maxv}")
         if is_normalize:
             print(f"The result was normalized.")
             wave /= maxv
         else:
             print(f"The result was not normalized.")
     else:
         print_with_timestamp(f"Normalization Set {is_normalize}: Input not above threshold for clipping. Max:{maxv}")
-    
+
     return wave
-    
+
+
 def normalize_two_stem(wave, mix, is_normalize=False):
     """Save output music files"""
-    
+
     maxv = np.abs(wave).max()
     max_mix = np.abs(mix).max()
-    
+
     if maxv > 1.0:
         print_with_timestamp(f"Normalization Set {is_normalize}: Primary source above threshold for clipping. Max:{maxv}")
         print_with_timestamp(f"Normalization Set {is_normalize}: Mixture above threshold for clipping. Max:{max_mix}")
         if is_normalize:
             print(f"The result was normalized.")
             wave /= maxv
             mix /= maxv
         else:
             print(f"The result was not normalized.")
     else:
         print_with_timestamp(f"Normalization Set {is_normalize}: Input not above threshold for clipping. Max:{maxv}")
-    
-    
+
     print_with_timestamp(f"Normalization Set {is_normalize}: Primary source - Max:{np.abs(wave).max()}")
     print_with_timestamp(f"Normalization Set {is_normalize}: Mixture - Max:{np.abs(mix).max()}")
-    
-    return wave, mix    
+
+    return wave, mix
+
 
 def combine_spectrograms(specs, mp):
-    l = min([specs[i].shape[2] for i in specs])    
-    spec_c = np.zeros(shape=(2, mp.param['bins'] + 1, l), dtype=np.complex64)
+    l = min([specs[i].shape[2] for i in specs])
+    spec_c = np.zeros(shape=(2, mp.param["bins"] + 1, l), dtype=np.complex64)
     offset = 0
-    bands_n = len(mp.param['band'])
-    
+    bands_n = len(mp.param["band"])
+
     for d in range(1, bands_n + 1):
-        h = mp.param['band'][d]['crop_stop'] - mp.param['band'][d]['crop_start']
-        spec_c[:, offset:offset+h, :l] = specs[d][:, mp.param['band'][d]['crop_start']:mp.param['band'][d]['crop_stop'], :l]
+        h = mp.param["band"][d]["crop_stop"] - mp.param["band"][d]["crop_start"]
+        spec_c[:, offset : offset + h, :l] = specs[d][:, mp.param["band"][d]["crop_start"] : mp.param["band"][d]["crop_stop"], :l]
         offset += h
-        
-    if offset > mp.param['bins']:
-        raise ValueError('Too much bins')
-        
+
+    if offset > mp.param["bins"]:
+        raise ValueError("Too much bins")
+
     # lowpass fiter
-    if mp.param['pre_filter_start'] > 0: # and mp.param['band'][bands_n]['res_type'] in ['scipy', 'polyphase']:   
+    if mp.param["pre_filter_start"] > 0:  # and mp.param['band'][bands_n]['res_type'] in ['scipy', 'polyphase']:
         if bands_n == 1:
-            spec_c = fft_lp_filter(spec_c, mp.param['pre_filter_start'], mp.param['pre_filter_stop'])
+            spec_c = fft_lp_filter(spec_c, mp.param["pre_filter_start"], mp.param["pre_filter_stop"])
         else:
-            gp = 1        
-            for b in range(mp.param['pre_filter_start'] + 1, mp.param['pre_filter_stop']):
-                g = math.pow(10, -(b - mp.param['pre_filter_start']) * (3.5 - gp) / 20.0)
+            gp = 1
+            for b in range(mp.param["pre_filter_start"] + 1, mp.param["pre_filter_stop"]):
+                g = math.pow(10, -(b - mp.param["pre_filter_start"]) * (3.5 - gp) / 20.0)
                 gp = g
                 spec_c[:, b, :] *= g
-                
+
     return np.asfortranarray(spec_c)
-    
-def spectrogram_to_image(spec, mode='magnitude'):
-    if mode == 'magnitude':
+
+
+def spectrogram_to_image(spec, mode="magnitude"):
+    if mode == "magnitude":
         if np.iscomplexobj(spec):
             y = np.abs(spec)
         else:
             y = spec
-        y = np.log10(y ** 2 + 1e-8)
-    elif mode == 'phase':
+        y = np.log10(y**2 + 1e-8)
+    elif mode == "phase":
         if np.iscomplexobj(spec):
             y = np.angle(spec)
         else:
             y = spec
 
     y -= y.min()
     y *= 255 / y.max()
     img = np.uint8(y)
 
     if y.ndim == 3:
         img = img.transpose(1, 2, 0)
-        img = np.concatenate([
-            np.max(img, axis=2, keepdims=True), img
-        ], axis=2)
+        img = np.concatenate([np.max(img, axis=2, keepdims=True), img], axis=2)
 
     return img
 
+
 def reduce_vocal_aggressively(X, y, softmask):
     v = X - y
     y_mag_tmp = np.abs(y)
     v_mag_tmp = np.abs(v)
 
     v_mask = v_mag_tmp > y_mag_tmp
     y_mag = np.clip(y_mag_tmp - v_mag_tmp * v_mask * softmask, 0, np.inf)
 
-    return y_mag * np.exp(1.j * np.angle(y))
+    return y_mag * np.exp(1.0j * np.angle(y))
+
 
 def merge_artifacts(y_mask, thres=0.01, min_range=64, fade_size=32):
     mask = y_mask
-    
+
     try:
         if min_range < fade_size * 2:
-            raise ValueError('min_range must be >= fade_size * 2')
+            raise ValueError("min_range must be >= fade_size * 2")
 
         idx = np.where(y_mask.min(axis=(0, 1)) > thres)[0]
         start_idx = np.insert(idx[np.where(np.diff(idx) != 1)[0] + 1], 0, idx[0])
         end_idx = np.append(idx[np.where(np.diff(idx) != 1)[0]], idx[-1])
         artifact_idx = np.where(end_idx - start_idx > min_range)[0]
         weight = np.zeros_like(y_mask)
         if len(artifact_idx) > 0:
@@ -229,339 +238,365 @@
             end_idx = end_idx[artifact_idx]
             old_e = None
             for s, e in zip(start_idx, end_idx):
                 if old_e is not None and s - old_e < fade_size:
                     s = old_e - fade_size * 2
 
                 if s != 0:
-                    weight[:, :, s:s + fade_size] = np.linspace(0, 1, fade_size)
+                    weight[:, :, s : s + fade_size] = np.linspace(0, 1, fade_size)
                 else:
                     s -= fade_size
 
                 if e != y_mask.shape[2]:
-                    weight[:, :, e - fade_size:e] = np.linspace(1, 0, fade_size)
+                    weight[:, :, e - fade_size : e] = np.linspace(1, 0, fade_size)
                 else:
                     e += fade_size
 
-                weight[:, :, s + fade_size:e - fade_size] = 1
+                weight[:, :, s + fade_size : e - fade_size] = 1
                 old_e = e
 
         v_mask = 1 - y_mask
         y_mask += weight * v_mask
-        
+
         mask = y_mask
     except Exception as e:
-        error_name = f'{type(e).__name__}'
-        traceback_text = ''.join(traceback.format_tb(e.__traceback__))
+        error_name = f"{type(e).__name__}"
+        traceback_text = "".join(traceback.format_tb(e.__traceback__))
         message = f'{error_name}: "{e}"\n{traceback_text}"'
-        print('Post Process Failed: ', message)
-        
+        print("Post Process Failed: ", message)
 
     return mask
 
+
 def align_wave_head_and_tail(a, b):
-    l = min([a[0].size, b[0].size])  
-    
-    return a[:l,:l], b[:l,:l]
-    
+    l = min([a[0].size, b[0].size])
+
+    return a[:l, :l], b[:l, :l]
+
+
 def spectrogram_to_wave(spec, hop_length, mid_side, mid_side_b2, reverse, clamp=False):
     spec_left = np.asfortranarray(spec[0])
     spec_right = np.asfortranarray(spec[1])
 
     wave_left = librosa.istft(spec_left, hop_length=hop_length)
     wave_right = librosa.istft(spec_right, hop_length=hop_length)
 
     if reverse:
         return np.asfortranarray([np.flip(wave_left), np.flip(wave_right)])
     elif mid_side:
         return np.asfortranarray([np.add(wave_left, wave_right / 2), np.subtract(wave_left, wave_right / 2)])
     elif mid_side_b2:
-        return np.asfortranarray([np.add(wave_right / 1.25, .4 * wave_left), np.subtract(wave_left / 1.25, .4 * wave_right)])
+        return np.asfortranarray([np.add(wave_right / 1.25, 0.4 * wave_left), np.subtract(wave_left / 1.25, 0.4 * wave_right)])
     else:
         return np.asfortranarray([wave_left, wave_right])
-    
+
+
 def spectrogram_to_wave_mt(spec, hop_length, mid_side, reverse, mid_side_b2):
     import threading
 
     spec_left = np.asfortranarray(spec[0])
     spec_right = np.asfortranarray(spec[1])
-    
+
     def run_thread(**kwargs):
         global wave_left
         wave_left = librosa.istft(**kwargs)
-        
-    thread = threading.Thread(target=run_thread, kwargs={'stft_matrix': spec_left, 'hop_length': hop_length})
+
+    thread = threading.Thread(target=run_thread, kwargs={"stft_matrix": spec_left, "hop_length": hop_length})
     thread.start()
     wave_right = librosa.istft(spec_right, hop_length=hop_length)
-    thread.join()   
-    
+    thread.join()
+
     if reverse:
         return np.asfortranarray([np.flip(wave_left), np.flip(wave_right)])
     elif mid_side:
         return np.asfortranarray([np.add(wave_left, wave_right / 2), np.subtract(wave_left, wave_right / 2)])
     elif mid_side_b2:
-        return np.asfortranarray([np.add(wave_right / 1.25, .4 * wave_left), np.subtract(wave_left / 1.25, .4 * wave_right)])
+        return np.asfortranarray([np.add(wave_right / 1.25, 0.4 * wave_left), np.subtract(wave_left / 1.25, 0.4 * wave_right)])
     else:
         return np.asfortranarray([wave_left, wave_right])
-    
+
+
 def cmb_spectrogram_to_wave(spec_m, mp, extra_bins_h=None, extra_bins=None):
-    bands_n = len(mp.param['band'])    
+    bands_n = len(mp.param["band"])
     offset = 0
 
     for d in range(1, bands_n + 1):
-        bp = mp.param['band'][d]
-        spec_s = np.ndarray(shape=(2, bp['n_fft'] // 2 + 1, spec_m.shape[2]), dtype=complex)
-        h = bp['crop_stop'] - bp['crop_start']
-        spec_s[:, bp['crop_start']:bp['crop_stop'], :] = spec_m[:, offset:offset+h, :]
-        
+        bp = mp.param["band"][d]
+        spec_s = np.ndarray(shape=(2, bp["n_fft"] // 2 + 1, spec_m.shape[2]), dtype=complex)
+        h = bp["crop_stop"] - bp["crop_start"]
+        spec_s[:, bp["crop_start"] : bp["crop_stop"], :] = spec_m[:, offset : offset + h, :]
+
         offset += h
-        if d == bands_n: # higher
-            if extra_bins_h: # if --high_end_process bypass
-                max_bin = bp['n_fft'] // 2
-                spec_s[:, max_bin-extra_bins_h:max_bin, :] = extra_bins[:, :extra_bins_h, :]
-            if bp['hpf_start'] > 0:
-                spec_s = fft_hp_filter(spec_s, bp['hpf_start'], bp['hpf_stop'] - 1)
+        if d == bands_n:  # higher
+            if extra_bins_h:  # if --high_end_process bypass
+                max_bin = bp["n_fft"] // 2
+                spec_s[:, max_bin - extra_bins_h : max_bin, :] = extra_bins[:, :extra_bins_h, :]
+            if bp["hpf_start"] > 0:
+                spec_s = fft_hp_filter(spec_s, bp["hpf_start"], bp["hpf_stop"] - 1)
             if bands_n == 1:
-                wave = spectrogram_to_wave(spec_s, bp['hl'], mp.param['mid_side'], mp.param['mid_side_b2'], mp.param['reverse'])
+                wave = spectrogram_to_wave(spec_s, bp["hl"], mp.param["mid_side"], mp.param["mid_side_b2"], mp.param["reverse"])
             else:
-                wave = np.add(wave, spectrogram_to_wave(spec_s, bp['hl'], mp.param['mid_side'], mp.param['mid_side_b2'], mp.param['reverse']))
+                wave = np.add(
+                    wave, spectrogram_to_wave(spec_s, bp["hl"], mp.param["mid_side"], mp.param["mid_side_b2"], mp.param["reverse"])
+                )
         else:
-            sr = mp.param['band'][d+1]['sr']
-            if d == 1: # lower
-                spec_s = fft_lp_filter(spec_s, bp['lpf_start'], bp['lpf_stop'])
-                wave = librosa.resample(spectrogram_to_wave(spec_s, bp['hl'], mp.param['mid_side'], mp.param['mid_side_b2'], mp.param['reverse']), bp['sr'], sr, res_type=wav_resolution)
-            else: # mid
-                spec_s = fft_hp_filter(spec_s, bp['hpf_start'], bp['hpf_stop'] - 1)
-                spec_s = fft_lp_filter(spec_s, bp['lpf_start'], bp['lpf_stop'])
-                wave2 = np.add(wave, spectrogram_to_wave(spec_s, bp['hl'], mp.param['mid_side'], mp.param['mid_side_b2'], mp.param['reverse']))
-                wave = librosa.resample(wave2, bp['sr'], sr, res_type=wav_resolution)
-        
+            sr = mp.param["band"][d + 1]["sr"]
+            if d == 1:  # lower
+                spec_s = fft_lp_filter(spec_s, bp["lpf_start"], bp["lpf_stop"])
+                wave = librosa.resample(
+                    spectrogram_to_wave(spec_s, bp["hl"], mp.param["mid_side"], mp.param["mid_side_b2"], mp.param["reverse"]),
+                    bp["sr"],
+                    sr,
+                    res_type=wav_resolution,
+                )
+            else:  # mid
+                spec_s = fft_hp_filter(spec_s, bp["hpf_start"], bp["hpf_stop"] - 1)
+                spec_s = fft_lp_filter(spec_s, bp["lpf_start"], bp["lpf_stop"])
+                wave2 = np.add(
+                    wave, spectrogram_to_wave(spec_s, bp["hl"], mp.param["mid_side"], mp.param["mid_side_b2"], mp.param["reverse"])
+                )
+                wave = librosa.resample(wave2, bp["sr"], sr, res_type=wav_resolution)
+
     return wave
 
+
 def fft_lp_filter(spec, bin_start, bin_stop):
     g = 1.0
     for b in range(bin_start, bin_stop):
         g -= 1 / (bin_stop - bin_start)
         spec[:, b, :] = g * spec[:, b, :]
-        
+
     spec[:, bin_stop:, :] *= 0
 
     return spec
 
+
 def fft_hp_filter(spec, bin_start, bin_stop):
     g = 1.0
     for b in range(bin_start, bin_stop, -1):
         g -= 1 / (bin_start - bin_stop)
         spec[:, b, :] = g * spec[:, b, :]
-    
-    spec[:, 0:bin_stop+1, :] *= 0
+
+    spec[:, 0 : bin_stop + 1, :] *= 0
 
     return spec
 
+
 def mirroring(a, spec_m, input_high_end, mp):
-    if 'mirroring' == a:
-        mirror = np.flip(np.abs(spec_m[:, mp.param['pre_filter_start']-10-input_high_end.shape[1]:mp.param['pre_filter_start']-10, :]), 1)
-        mirror = mirror * np.exp(1.j * np.angle(input_high_end))
-        
+    if "mirroring" == a:
+        mirror = np.flip(
+            np.abs(spec_m[:, mp.param["pre_filter_start"] - 10 - input_high_end.shape[1] : mp.param["pre_filter_start"] - 10, :]), 1
+        )
+        mirror = mirror * np.exp(1.0j * np.angle(input_high_end))
+
         return np.where(np.abs(input_high_end) <= np.abs(mirror), input_high_end, mirror)
-        
-    if 'mirroring2' == a:
-        mirror = np.flip(np.abs(spec_m[:, mp.param['pre_filter_start']-10-input_high_end.shape[1]:mp.param['pre_filter_start']-10, :]), 1)
+
+    if "mirroring2" == a:
+        mirror = np.flip(
+            np.abs(spec_m[:, mp.param["pre_filter_start"] - 10 - input_high_end.shape[1] : mp.param["pre_filter_start"] - 10, :]), 1
+        )
         mi = np.multiply(mirror, input_high_end * 1.7)
-        
+
         return np.where(np.abs(input_high_end) <= np.abs(mi), input_high_end, mi)
 
+
 def adjust_aggr(mask, is_non_accom_stem, aggressiveness):
-    aggr = aggressiveness['value']
+    aggr = aggressiveness["value"]
 
     if aggr != 0:
         if is_non_accom_stem:
             aggr = 1 - aggr
-    
+
         aggr = [aggr, aggr]
-    
-        if aggressiveness['aggr_correction'] is not None:
-            aggr[0] += aggressiveness['aggr_correction']['left']
-            aggr[1] += aggressiveness['aggr_correction']['right']
+
+        if aggressiveness["aggr_correction"] is not None:
+            aggr[0] += aggressiveness["aggr_correction"]["left"]
+            aggr[1] += aggressiveness["aggr_correction"]["right"]
 
         for ch in range(2):
-            mask[ch, :aggressiveness['split_bin']] = np.power(mask[ch, :aggressiveness['split_bin']], 1 + aggr[ch] / 3)
-            mask[ch, aggressiveness['split_bin']:] = np.power(mask[ch, aggressiveness['split_bin']:], 1 + aggr[ch])
+            mask[ch, : aggressiveness["split_bin"]] = np.power(mask[ch, : aggressiveness["split_bin"]], 1 + aggr[ch] / 3)
+            mask[ch, aggressiveness["split_bin"] :] = np.power(mask[ch, aggressiveness["split_bin"] :], 1 + aggr[ch])
 
         # if is_non_accom_stem:
         #     mask = (1.0 - mask)
-        
+
     return mask
 
+
 def stft(wave, nfft, hl):
     wave_left = np.asfortranarray(wave[0])
     wave_right = np.asfortranarray(wave[1])
     spec_left = librosa.stft(wave_left, nfft, hop_length=hl)
     spec_right = librosa.stft(wave_right, nfft, hop_length=hl)
     spec = np.asfortranarray([spec_left, spec_right])
 
     return spec
 
+
 def istft(spec, hl):
     spec_left = np.asfortranarray(spec[0])
     spec_right = np.asfortranarray(spec[1])
     wave_left = librosa.istft(spec_left, hop_length=hl)
     wave_right = librosa.istft(spec_right, hop_length=hl)
     wave = np.asfortranarray([wave_left, wave_right])
 
     return wave
 
-def spec_effects(wave, algorithm='Default', value=None):
-    spec = [stft(wave[0],2048,1024), stft(wave[1],2048,1024)]
-    if algorithm == 'Min_Mag':
+
+def spec_effects(wave, algorithm="Default", value=None):
+    spec = [stft(wave[0], 2048, 1024), stft(wave[1], 2048, 1024)]
+    if algorithm == "Min_Mag":
         v_spec_m = np.where(np.abs(spec[1]) <= np.abs(spec[0]), spec[1], spec[0])
-        wave = istft(v_spec_m,1024)
-    elif algorithm == 'Max_Mag':
+        wave = istft(v_spec_m, 1024)
+    elif algorithm == "Max_Mag":
         v_spec_m = np.where(np.abs(spec[1]) >= np.abs(spec[0]), spec[1], spec[0])
-        wave = istft(v_spec_m,1024)
-    elif algorithm == 'Default':
-        wave = (wave[1] * value) + (wave[0] * (1-value))
-    elif algorithm == 'Invert_p':
+        wave = istft(v_spec_m, 1024)
+    elif algorithm == "Default":
+        wave = (wave[1] * value) + (wave[0] * (1 - value))
+    elif algorithm == "Invert_p":
         X_mag = np.abs(spec[0])
-        y_mag = np.abs(spec[1])            
-        max_mag = np.where(X_mag >= y_mag, X_mag, y_mag)  
-        v_spec = spec[1] - max_mag * np.exp(1.j * np.angle(spec[0]))
-        wave = istft(v_spec,1024)
-            
-    return wave      
+        y_mag = np.abs(spec[1])
+        max_mag = np.where(X_mag >= y_mag, X_mag, y_mag)
+        v_spec = spec[1] - max_mag * np.exp(1.0j * np.angle(spec[0]))
+        wave = istft(v_spec, 1024)
+
+    return wave
+
 
 def spectrogram_to_wave_no_mp(spec, n_fft=2048, hop_length=1024):
     wave = librosa.istft(spec, n_fft=n_fft, hop_length=hop_length)
-    
+
     if wave.ndim == 1:
-        wave = np.asfortranarray([wave,wave])
+        wave = np.asfortranarray([wave, wave])
 
     return wave
 
+
 def wave_to_spectrogram_no_mp(wave):
-    
     spec = librosa.stft(wave, n_fft=2048, hop_length=1024)
-    
+
     if spec.ndim == 1:
-        spec = np.asfortranarray([spec,spec])
+        spec = np.asfortranarray([spec, spec])
 
     return spec
 
+
 def invert_audio(specs, invert_p=True):
-    
     ln = min([specs[0].shape[2], specs[1].shape[2]])
-    specs[0] = specs[0][:,:,:ln]
-    specs[1] = specs[1][:,:,:ln]
-        
+    specs[0] = specs[0][:, :, :ln]
+    specs[1] = specs[1][:, :, :ln]
+
     if invert_p:
         X_mag = np.abs(specs[0])
-        y_mag = np.abs(specs[1])            
-        max_mag = np.where(X_mag >= y_mag, X_mag, y_mag)  
-        v_spec = specs[1] - max_mag * np.exp(1.j * np.angle(specs[0]))
+        y_mag = np.abs(specs[1])
+        max_mag = np.where(X_mag >= y_mag, X_mag, y_mag)
+        v_spec = specs[1] - max_mag * np.exp(1.0j * np.angle(specs[0]))
     else:
         specs[1] = reduce_vocal_aggressively(specs[0], specs[1], 0.2)
         v_spec = specs[0] - specs[1]
 
     return v_spec
 
+
 def invert_stem(mixture, stem):
-    
     mixture = wave_to_spectrogram_no_mp(mixture)
     stem = wave_to_spectrogram_no_mp(stem)
     output = spectrogram_to_wave_no_mp(invert_audio([mixture, stem]))
 
     return -output.T
 
-def ensembling(a, specs):   
+
+def ensembling(a, specs):
     for i in range(1, len(specs)):
         if i == 1:
             spec = specs[0]
 
         ln = min([spec.shape[2], specs[i].shape[2]])
-        spec = spec[:,:,:ln]
-        specs[i] = specs[i][:,:,:ln]
-        
+        spec = spec[:, :, :ln]
+        specs[i] = specs[i][:, :, :ln]
+
         if MIN_SPEC == a:
             spec = np.where(np.abs(specs[i]) <= np.abs(spec), specs[i], spec)
         if MAX_SPEC == a:
-            spec = np.where(np.abs(specs[i]) >= np.abs(spec), specs[i], spec)  
+            spec = np.where(np.abs(specs[i]) >= np.abs(spec), specs[i], spec)
         if AVERAGE == a:
-            spec = np.where(np.abs(specs[i]) == np.abs(spec), specs[i], spec)  
+            spec = np.where(np.abs(specs[i]) == np.abs(spec), specs[i], spec)
 
     return spec
 
-def ensemble_inputs(audio_input, algorithm, is_normalization, wav_type_set, save_path):
 
+def ensemble_inputs(audio_input, algorithm, is_normalization, wav_type_set, save_path):
     wavs_ = []
-    
+
     if algorithm == AVERAGE:
         output = average_audio(audio_input)
         samplerate = 44100
     else:
         specs = []
-        
-        for i in range(len(audio_input)):  
+
+        for i in range(len(audio_input)):
             wave, samplerate = librosa.load(audio_input[i], mono=False, sr=44100)
             wavs_.append(wave)
             spec = wave_to_spectrogram_no_mp(wave)
             specs.append(spec)
-        
+
         wave_shapes = [w.shape[1] for w in wavs_]
         target_shape = wavs_[wave_shapes.index(max(wave_shapes))]
-        
+
         output = spectrogram_to_wave_no_mp(ensembling(algorithm, specs))
         output = to_shape(output, target_shape.shape)
 
     sf.write(save_path, normalize(output.T, is_normalization), samplerate, subtype=wav_type_set)
 
+
 def to_shape(x, target_shape):
     padding_list = []
     for x_dim, target_dim in zip(x.shape, target_shape):
-        pad_value = (target_dim - x_dim)
-        pad_tuple = ((0, pad_value))
+        pad_value = target_dim - x_dim
+        pad_tuple = (0, pad_value)
         padding_list.append(pad_tuple)
-    
-    return np.pad(x, tuple(padding_list), mode='constant')
+
+    return np.pad(x, tuple(padding_list), mode="constant")
+
 
 def to_shape_minimize(x: np.ndarray, target_shape):
-    
     padding_list = []
     for x_dim, target_dim in zip(x.shape, target_shape):
-        pad_value = (target_dim - x_dim)
-        pad_tuple = ((0, pad_value))
+        pad_value = target_dim - x_dim
+        pad_tuple = (0, pad_value)
         padding_list.append(pad_tuple)
-    
-    return np.pad(x, tuple(padding_list), mode='constant')
 
-def augment_audio(export_path, audio_file, rate, is_normalization, wav_type_set, save_format=None, is_pitch=False):
+    return np.pad(x, tuple(padding_list), mode="constant")
 
+
+def augment_audio(export_path, audio_file, rate, is_normalization, wav_type_set, save_format=None, is_pitch=False):
     wav, sr = librosa.load(audio_file, sr=44100, mono=False)
 
     if wav.ndim == 1:
-        wav = np.asfortranarray([wav,wav])
+        wav = np.asfortranarray([wav, wav])
 
     if is_pitch:
         wav_1 = pyrb.pitch_shift(wav[0], sr, rate, rbargs=None)
         wav_2 = pyrb.pitch_shift(wav[1], sr, rate, rbargs=None)
     else:
         wav_1 = pyrb.time_stretch(wav[0], sr, rate, rbargs=None)
         wav_2 = pyrb.time_stretch(wav[1], sr, rate, rbargs=None)
 
     if wav_1.shape > wav_2.shape:
         wav_2 = to_shape(wav_2, wav_1.shape)
     if wav_1.shape < wav_2.shape:
         wav_1 = to_shape(wav_1, wav_2.shape)
-        
+
     wav_mix = np.asfortranarray([wav_1, wav_2])
-    
+
     sf.write(export_path, normalize(wav_mix.T, is_normalization), sr, subtype=wav_type_set)
     save_format(export_path)
-    
+
+
 def average_audio(audio):
-    
     waves = []
     wave_shapes = []
     final_waves = []
 
     for i in range(len(audio)):
         wave = librosa.load(audio[i], sr=44100, mono=False)
         waves.append(wave[0])
@@ -573,124 +608,127 @@
     final_waves.append(target_shape)
 
     for n_array in waves:
         wav_target = to_shape(n_array, target_shape.shape)
         final_waves.append(wav_target)
 
     waves = sum(final_waves)
-    waves = waves/len(audio)
+    waves = waves / len(audio)
 
     return waves
-    
+
+
 def average_dual_sources(wav_1, wav_2, value):
-    
     if wav_1.shape > wav_2.shape:
         wav_2 = to_shape(wav_2, wav_1.shape)
     if wav_1.shape < wav_2.shape:
         wav_1 = to_shape(wav_1, wav_2.shape)
 
-    wave = (wav_1 * value) + (wav_2 * (1-value))
+    wave = (wav_1 * value) + (wav_2 * (1 - value))
 
     return wave
-    
+
+
 def reshape_sources(wav_1: np.ndarray, wav_2: np.ndarray):
-    
     if wav_1.shape > wav_2.shape:
         wav_2 = to_shape(wav_2, wav_1.shape)
     if wav_1.shape < wav_2.shape:
         ln = min([wav_1.shape[1], wav_2.shape[1]])
-        wav_2 = wav_2[:,:ln]
+        wav_2 = wav_2[:, :ln]
 
     ln = min([wav_1.shape[1], wav_2.shape[1]])
-    wav_1 = wav_1[:,:ln]
-    wav_2 = wav_2[:,:ln]
+    wav_1 = wav_1[:, :ln]
+    wav_2 = wav_2[:, :ln]
 
     return wav_2
-    
-def align_audio(file1, file2, file2_aligned, file_subtracted, wav_type_set, is_normalization, command_Text, progress_bar_main_var, save_format):
+
+
+def align_audio(
+    file1, file2, file2_aligned, file_subtracted, wav_type_set, is_normalization, command_Text, progress_bar_main_var, save_format
+):
     def get_diff(a, b):
         corr = np.correlate(a, b, "full")
         diff = corr.argmax() - (b.shape[0] - 1)
         return diff
-  
+
     progress_bar_main_var.set(10)
-    
+
     # read tracks
     wav1, sr1 = librosa.load(file1, sr=44100, mono=False)
     wav2, sr2 = librosa.load(file2, sr=44100, mono=False)
     wav1 = wav1.transpose()
     wav2 = wav2.transpose()
 
     command_Text(f"Audio file shapes: {wav1.shape} / {wav2.shape}\n")
-    
+
     wav2_org = wav2.copy()
     progress_bar_main_var.set(20)
-    
+
     command_Text("Processing files... \n")
-    
-  # pick random position and get diff
-    
-    counts = {}       # counting up for each diff value
+
+    # pick random position and get diff
+
+    counts = {}  # counting up for each diff value
     progress = 20
-    
+
     check_range = 64
 
-    base = (64 / check_range)
+    base = 64 / check_range
 
     for i in range(check_range):
         index = int(random.uniform(44100 * 2, min(wav1.shape[0], wav2.shape[0]) - 44100 * 2))
-        shift = int(random.uniform(-22050,+22050))
-        samp1 = wav1[index      :index      +44100, 0]          # currently use left channel
-        samp2 = wav2[index+shift:index+shift+44100, 0]
+        shift = int(random.uniform(-22050, +22050))
+        samp1 = wav1[index : index + 44100, 0]  # currently use left channel
+        samp2 = wav2[index + shift : index + shift + 44100, 0]
         progress += 1 * base
         progress_bar_main_var.set(progress)
         diff = get_diff(samp1, samp2)
         diff -= shift
-        
+
     if abs(diff) < 22050:
         if not diff in counts:
             counts[diff] = 0
         counts[diff] += 1
-  
-  # use max counted diff value
+
+    # use max counted diff value
     max_count = 0
-    est_diff  = 0
+    est_diff = 0
     for diff in counts.keys():
         if counts[diff] > max_count:
             max_count = counts[diff]
             est_diff = diff
-    
+
     command_Text(f"Estimated difference is {est_diff} (count: {max_count})\n")
 
     progress_bar_main_var.set(90)
-    
+
     audio_files = []
 
     def save_aligned_audio(wav2_aligned):
         command_Text(f"Aligned File 2 with File 1.\n")
         command_Text(f"Saving files... ")
         sf.write(file2_aligned, normalize(wav2_aligned, is_normalization), sr2, subtype=wav_type_set)
         save_format(file2_aligned)
         min_len = min(wav1.shape[0], wav2_aligned.shape[0])
         wav_sub = wav1[:min_len] - wav2_aligned[:min_len]
         audio_files.append(file2_aligned)
         return min_len, wav_sub
-    
-  # make aligned track 2
+
+    # make aligned track 2
     if est_diff > 0:
         wav2_aligned = np.append(np.zeros((est_diff, 2)), wav2_org, axis=0)
         min_len, wav_sub = save_aligned_audio(wav2_aligned)
     elif est_diff < 0:
         wav2_aligned = wav2_org[-est_diff:]
         min_len, wav_sub = save_aligned_audio(wav2_aligned)
     else:
         command_Text(f"Audio files already aligned.\n")
         command_Text(f"Saving inverted track... ")
         min_len = min(wav1.shape[0], wav2.shape[0])
         wav_sub = wav1[:min_len] - wav2[:min_len]
 
     wav_sub = np.clip(wav_sub, -1, +1)
-  
+
     sf.write(file_subtracted, normalize(wav_sub, is_normalization), sr1, subtype=wav_type_set)
     save_format(file_subtracted)
-  
-    progress_bar_main_var.set(95)
+
+    progress_bar_main_var.set(95)
```

### Comparing `audio_separator-0.2.2/pyproject.toml` & `audio_separator-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.2.2"
+version = "0.2.3"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 
 [tool.poetry.dependencies]
@@ -17,10 +17,16 @@
 torch = "^1.13"
 wget = "^3"
 six = "^1.16"
 
 [tool.poetry.scripts]
 audio-separator = 'audio_separator.utils.cli:main'
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+
+[tool.black]
+line-length = 140
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `audio_separator-0.2.2/PKG-INFO` & `audio_separator-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.2.2
+Version: 0.2.3
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

