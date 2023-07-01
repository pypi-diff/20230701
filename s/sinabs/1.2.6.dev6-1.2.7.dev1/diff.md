# Comparing `tmp/sinabs-1.2.6.dev6.tar.gz` & `tmp/sinabs-1.2.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinabs-1.2.6.dev6.tar", last modified: Fri Jun 30 20:46:45 2023, max compression
+gzip compressed data, was "sinabs-1.2.7.dev1.tar", last modified: Sat Jul  1 17:26:10 2023, max compression
```

## Comparing `sinabs-1.2.6.dev6.tar` & `sinabs-1.2.7.dev1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.209720 sinabs-1.2.6.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.189720 sinabs-1.2.6.dev6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.193720 sinabs-1.2.6.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    30047 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-30 20:46:45.209720 sinabs-1.2.6.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.193720 sinabs-1.2.6.dev6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.193720 sinabs-1.2.6.dev6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/_static/sinabs-logo-lowercase-whitebg.png
--rw-r--r--   0 runner    (1001) docker     (123)    80008 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/_static/sinabs-logo-lowercase.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/_templates/class_activation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/_templates/class_layer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/about/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/about/differences.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/about/info.md
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/about/release_notes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/activation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/from_torch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/layers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/network.rst
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/synopcounter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/contact.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/gallery/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/layers/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/layers/plot_alif.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/layers/plot_exp_leaky.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/layers/plot_iaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/layers/plot_lif.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/layers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/gallery/spike_fns/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/spike_fns/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/spike_fns/plot_maxspike.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/spike_fns/plot_multispike.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/spike_fns/plot_singlespike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.197720 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/plot_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/plot_heaviside.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/plot_multigaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/plot_periodicexponential.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/gallery/surrogate_grad_fns/plot_singleexponential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.201720 sinabs-1.2.6.dev6/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/getting_started/fundamentals.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/getting_started/iaf_neuron_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/getting_started/python_pyenv_pipenv.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/getting_started/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.201720 sinabs-1.2.6.dev6/docs/how_tos/
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/how_tos/activations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/how_tos/how_tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)    58127 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/how_tos/synops_loss_ann.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/how_tos/synops_loss_snn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.201720 sinabs-1.2.6.dev6/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/plugins/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.201720 sinabs-1.2.6.dev6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/tutorials/LeNet_5_EngChinese.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/tutorials/bptt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    48781 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/tutorials/nmnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/tutorials/weight_scaling.md
--rw-r--r--   0 runner    (1001) docker     (123)    27612 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/docs/tutorials/weight_transfer_mnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-30 20:46:45.209720 sinabs-1.2.6.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.201720 sinabs-1.2.6.dev6/sinabs/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.205720 sinabs-1.2.6.dev6/sinabs/activation/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/activation/quantize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/activation/reset_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/activation/spike_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/activation/surrogate_gradient_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/cnnutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/from_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.205720 sinabs-1.2.6.dev6/sinabs/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/alif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/crop2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/exp_leak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.205720 sinabs-1.2.6.dev6/sinabs/layers/functional/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/functional/alif.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/functional/lif.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/iaf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/lif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/neuromorphic_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/pool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/quantize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/stateful_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/layers/to_spike.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.205720 sinabs-1.2.6.dev6/sinabs/onnx/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/onnx/get_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/synopcounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/sinabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.205720 sinabs-1.2.6.dev6/sinabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/sinabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-30 20:46:45.000000 sinabs-1.2.6.dev6/sinabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/sinabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/sinabs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/sinabs.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/sinabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 20:46:44.000000 sinabs-1.2.6.dev6/sinabs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.209720 sinabs-1.2.6.dev6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.209720 sinabs-1.2.6.dev6/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/models/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_alif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_batch_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_crop2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_exp_leak.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_from_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_iaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_img2spk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_lif.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_maxpooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_network_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_neuromorphic_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_normalize_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_quantize.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_reshaping.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_sig2spk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_stateful_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_surrogate_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_synops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_to_spike_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:46:45.209720 sinabs-1.2.6.dev6/tests/weights/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 20:46:38.000000 sinabs-1.2.6.dev6/tests/weights/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.392227 sinabs-1.2.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.380226 sinabs-1.2.7.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.380226 sinabs-1.2.7.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    30125 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-01 17:26:10.392227 sinabs-1.2.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.380226 sinabs-1.2.7.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.380226 sinabs-1.2.7.dev1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/_static/sinabs-logo-lowercase-whitebg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80008 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/_static/sinabs-logo-lowercase.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.380226 sinabs-1.2.7.dev1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/_templates/class_activation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/_templates/class_layer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/about/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/about/differences.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/about/info.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/about/release_notes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/activation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/from_torch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/layers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/network.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/synopcounter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/contact.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/gallery/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/layers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/layers/plot_alif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/layers/plot_exp_leaky.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/layers/plot_iaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/layers/plot_lif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/layers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/gallery/spike_fns/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/spike_fns/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/spike_fns/plot_maxspike.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/spike_fns/plot_multispike.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/spike_fns/plot_singlespike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/plot_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/plot_heaviside.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/plot_multigaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/plot_periodicexponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/gallery/surrogate_grad_fns/plot_singleexponential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/getting_started/fundamentals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/getting_started/iaf_neuron_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/getting_started/python_pyenv_pipenv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/getting_started/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/how_tos/
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/how_tos/activations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/how_tos/how_tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    58127 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/how_tos/synops_loss_ann.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/how_tos/synops_loss_snn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/plugins/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.384226 sinabs-1.2.7.dev1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/tutorials/LeNet_5_EngChinese.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/tutorials/bptt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    48768 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/tutorials/nmnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/tutorials/weight_scaling.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27612 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/docs/tutorials/weight_transfer_mnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-01 17:26:10.392227 sinabs-1.2.7.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.388226 sinabs-1.2.7.dev1/sinabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.388226 sinabs-1.2.7.dev1/sinabs/activation/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/activation/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/activation/reset_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/activation/spike_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/activation/surrogate_gradient_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/cnnutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/from_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.388226 sinabs-1.2.7.dev1/sinabs/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/alif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/crop2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/exp_leak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.388226 sinabs-1.2.7.dev1/sinabs/layers/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/functional/alif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/functional/lif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/iaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/lif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/neuromorphic_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/pool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/stateful_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/layers/to_spike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.388226 sinabs-1.2.7.dev1/sinabs/onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/onnx/get_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/synopcounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/sinabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.388226 sinabs-1.2.7.dev1/sinabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 17:26:10.000000 sinabs-1.2.7.dev1/sinabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.392227 sinabs-1.2.7.dev1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.392227 sinabs-1.2.7.dev1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/models/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_alif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_batch_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_crop2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_exp_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_iaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_img2spk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_lif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_maxpooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_network_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_neuromorphic_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_normalize_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_reshaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_sig2spk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_stateful_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_surrogate_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_synops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_to_spike_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:26:10.392227 sinabs-1.2.7.dev1/tests/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 17:26:07.000000 sinabs-1.2.7.dev1/tests/weights/README.txt
```

### Comparing `sinabs-1.2.6.dev6/.github/workflows/ci-pipeline.yml` & `sinabs-1.2.7.dev1/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/AUTHORS` & `sinabs-1.2.7.dev1/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Felix Bauer <felix.bauer@synsense.ai>
 Gregor Lenz <gregor.lenz@synsense.ai>
 Gregor Lenz <mail@lenzgregor.com>
 Martino Sorbaro <martino.sorbaro@ed.ac.uk>
 Martino Sorbaro <martino.sorbaro@posteo.net>
 Massimo Bortone <massimo.bortone@aictx.ai>
 MurphyWu <waitxxxx@126.com>
+Nogay Kuepelioglu <nogay.kuepelioglu@synsense.ai>
 Nogay Küpelioglu <nogay.kuepelioglu@synsense.ai>
 Nogay Küpelioğlu <kupelioglun@mef.edu.tr>
 Nogay Küpelioğlu <nogay.kuepelioglu@synsense.ai>
 Sadique Sheik <sadique.sheik@ai-ctx.com>
 Sadique Sheik <sadique.sheik@aictx.ai>
 Sadique Sheik <sadique.sheik@synsense.ai>
 Yalun_Hu <yalun.hu@synsense.ai>
```

### Comparing `sinabs-1.2.6.dev6/ChangeLog` & `sinabs-1.2.7.dev1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+* Fix issue #99, add unit test
+
+v1.2.6
+------
+
+* change nmnist tutorial title
 * added NMNIST tutorial
 * Unit test for periodic exponential gradient
 * Generate periodic exponential surrogate gradient correctly for different thresholds. Solves issue #97
 * Add none type comparison to spike\_threshold and min\_v\_mem
 
 v1.2.5
 ------
```

### Comparing `sinabs-1.2.6.dev6/LICENSE` & `sinabs-1.2.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/PKG-INFO` & `sinabs-1.2.7.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinabs
-Version: 1.2.6.dev6
+Version: 1.2.7.dev1
 Summary: SynSense Spiking Neural Network simulator for deep neural networks (DNNs).
 Home-page: UNKNOWN
 Author: SynSense (formerly AiCTX)
 Author-email: sinabs@synsense.ai
 License: GNU AGPLv3
 Project-URL: Source code, https://github.com/synsense/sinabs
 Project-URL: Documentation, https://readthedocs.org/projects/sinabs/
```

### Comparing `sinabs-1.2.6.dev6/README.md` & `sinabs-1.2.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/Makefile` & `sinabs-1.2.7.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/_static/sinabs-logo-lowercase-whitebg.png` & `sinabs-1.2.7.dev1/docs/_static/sinabs-logo-lowercase-whitebg.png`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/_static/sinabs-logo-lowercase.png` & `sinabs-1.2.7.dev1/docs/_static/sinabs-logo-lowercase.png`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/about/contributing.md` & `sinabs-1.2.7.dev1/docs/about/contributing.md`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/about/differences.md` & `sinabs-1.2.7.dev1/docs/about/differences.md`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/about/release_notes.md` & `sinabs-1.2.7.dev1/docs/about/release_notes.md`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/api/activation.rst` & `sinabs-1.2.7.dev1/docs/api/activation.rst`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/api/layers.rst` & `sinabs-1.2.7.dev1/docs/api/layers.rst`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/conf.py` & `sinabs-1.2.7.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/gallery/layers/plot_lif.py` & `sinabs-1.2.7.dev1/docs/gallery/layers/plot_lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/gallery/layers/utils.py` & `sinabs-1.2.7.dev1/docs/gallery/layers/utils.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/getting_started/fundamentals.rst` & `sinabs-1.2.7.dev1/docs/getting_started/fundamentals.rst`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/getting_started/iaf_neuron_model.ipynb` & `sinabs-1.2.7.dev1/docs/getting_started/iaf_neuron_model.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/getting_started/install.rst` & `sinabs-1.2.7.dev1/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/getting_started/python_pyenv_pipenv.rst` & `sinabs-1.2.7.dev1/docs/getting_started/python_pyenv_pipenv.rst`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/getting_started/quickstart.ipynb` & `sinabs-1.2.7.dev1/docs/getting_started/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/how_tos/activations.ipynb` & `sinabs-1.2.7.dev1/docs/how_tos/activations.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/how_tos/synops_loss_ann.ipynb` & `sinabs-1.2.7.dev1/docs/how_tos/synops_loss_ann.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/how_tos/synops_loss_snn.ipynb` & `sinabs-1.2.7.dev1/docs/how_tos/synops_loss_snn.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/index.md` & `sinabs-1.2.7.dev1/docs/index.md`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/tutorials/LeNet_5_EngChinese.ipynb` & `sinabs-1.2.7.dev1/docs/tutorials/LeNet_5_EngChinese.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/tutorials/bptt.ipynb` & `sinabs-1.2.7.dev1/docs/tutorials/bptt.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/tutorials/nmnist.ipynb` & `sinabs-1.2.7.dev1/docs/tutorials/nmnist.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991776315789473%*

 * *Differences: {"'cells'": "{0: {'source': ['# Training NMNIST for deployment on Speck using EXODUS']}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# End to end tutorial of training and deploying an SNN using EXODUS"
+                "# Training NMNIST for deployment on Speck using EXODUS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
```

### Comparing `sinabs-1.2.6.dev6/docs/tutorials/weight_scaling.md` & `sinabs-1.2.7.dev1/docs/tutorials/weight_scaling.md`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/docs/tutorials/weight_transfer_mnist.ipynb` & `sinabs-1.2.7.dev1/docs/tutorials/weight_transfer_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/setup.cfg` & `sinabs-1.2.7.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/activation/quantize.py` & `sinabs-1.2.7.dev1/sinabs/activation/quantize.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/activation/reset_mechanism.py` & `sinabs-1.2.7.dev1/sinabs/activation/reset_mechanism.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/activation/spike_generation.py` & `sinabs-1.2.7.dev1/sinabs/activation/spike_generation.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/activation/surrogate_gradient_fn.py` & `sinabs-1.2.7.dev1/sinabs/activation/surrogate_gradient_fn.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/cnnutils.py` & `sinabs-1.2.7.dev1/sinabs/cnnutils.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/conversion.py` & `sinabs-1.2.7.dev1/sinabs/conversion.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/from_torch.py` & `sinabs-1.2.7.dev1/sinabs/from_torch.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/__init__.py` & `sinabs-1.2.7.dev1/sinabs/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/alif.py` & `sinabs-1.2.7.dev1/sinabs/layers/alif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/crop2d.py` & `sinabs-1.2.7.dev1/sinabs/layers/crop2d.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/exp_leak.py` & `sinabs-1.2.7.dev1/sinabs/layers/exp_leak.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/functional/alif.py` & `sinabs-1.2.7.dev1/sinabs/layers/functional/alif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/functional/lif.py` & `sinabs-1.2.7.dev1/sinabs/layers/functional/lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/iaf.py` & `sinabs-1.2.7.dev1/sinabs/layers/iaf.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/lif.py` & `sinabs-1.2.7.dev1/sinabs/layers/lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/neuromorphic_relu.py` & `sinabs-1.2.7.dev1/sinabs/layers/neuromorphic_relu.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/pool2d.py` & `sinabs-1.2.7.dev1/sinabs/layers/pool2d.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/reshape.py` & `sinabs-1.2.7.dev1/sinabs/layers/reshape.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/stateful_layer.py` & `sinabs-1.2.7.dev1/sinabs/layers/stateful_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/layers/to_spike.py` & `sinabs-1.2.7.dev1/sinabs/layers/to_spike.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/network.py` & `sinabs-1.2.7.dev1/sinabs/network.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/onnx/get_graph.py` & `sinabs-1.2.7.dev1/sinabs/onnx/get_graph.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs/synopcounter.py` & `sinabs-1.2.7.dev1/sinabs/synopcounter.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         # it is flattened (B*T,C,H,W) or unflattened (B,T,C,H,W)
         unflattened_shape = None
         for layer in self.model.modules():
             if isinstance(layer, sl.SqueezeMixin):
                 unflattened_shape = (layer.batch_size, layer.num_timesteps)
 
         for layer in self.model.modules():
-            if isinstance(layer, sl.StatefulLayer):
+            if isinstance(layer, sl.StatefulLayer) and layer.does_spike:
                 layer.acc_output = torch.tensor(0)
                 layer.n_batches = 0
                 handle = layer.register_forward_hook(spiking_hook)
                 self.handles.append(handle)
             if isinstance(layer, torch.nn.Conv2d):
                 layer.accumulated_synops = torch.tensor(0)
                 layer.synops = torch.tensor(0)
```

### Comparing `sinabs-1.2.6.dev6/sinabs/utils.py` & `sinabs-1.2.7.dev1/sinabs/utils.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/sinabs.egg-info/PKG-INFO` & `sinabs-1.2.7.dev1/sinabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinabs
-Version: 1.2.6.dev6
+Version: 1.2.7.dev1
 Summary: SynSense Spiking Neural Network simulator for deep neural networks (DNNs).
 Home-page: UNKNOWN
 Author: SynSense (formerly AiCTX)
 Author-email: sinabs@synsense.ai
 License: GNU AGPLv3
 Project-URL: Source code, https://github.com/synsense/sinabs
 Project-URL: Documentation, https://readthedocs.org/projects/sinabs/
```

### Comparing `sinabs-1.2.6.dev6/sinabs.egg-info/SOURCES.txt` & `sinabs-1.2.7.dev1/sinabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_activations.py` & `sinabs-1.2.7.dev1/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_alif.py` & `sinabs-1.2.7.dev1/tests/test_alif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_batch_mismatch.py` & `sinabs-1.2.7.dev1/tests/test_batch_mismatch.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_conversion.py` & `sinabs-1.2.7.dev1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_copy.py` & `sinabs-1.2.7.dev1/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_exp_leak.py` & `sinabs-1.2.7.dev1/tests/test_exp_leak.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_from_model.py` & `sinabs-1.2.7.dev1/tests/test_from_model.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_iaf.py` & `sinabs-1.2.7.dev1/tests/test_iaf.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_lif.py` & `sinabs-1.2.7.dev1/tests/test_lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_maxpooling.py` & `sinabs-1.2.7.dev1/tests/test_maxpooling.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_network_class.py` & `sinabs-1.2.7.dev1/tests/test_network_class.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_neuromorphic_relu.py` & `sinabs-1.2.7.dev1/tests/test_neuromorphic_relu.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_normalize_weights.py` & `sinabs-1.2.7.dev1/tests/test_normalize_weights.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_onnx.py` & `sinabs-1.2.7.dev1/tests/test_onnx.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_quantize.py` & `sinabs-1.2.7.dev1/tests/test_quantize.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_reshaping.py` & `sinabs-1.2.7.dev1/tests/test_reshaping.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_stateful_layer.py` & `sinabs-1.2.7.dev1/tests/test_stateful_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_surrogate_gradients.py` & `sinabs-1.2.7.dev1/tests/test_surrogate_gradients.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_synops_counter.py` & `sinabs-1.2.7.dev1/tests/test_synops_counter.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,14 +178,34 @@
     assert (output == input_).all()
     assert model_stats["firing_rate"] == 0.25
     assert layer_stats["firing_rate"] == 0.25
     assert layer_stats["firing_rate_per_neuron"].shape == (4, 4)
     assert layer_stats["firing_rate_per_neuron"].mean() == 0.25
 
 
+def test_nonspiking_stateful_layer():
+    model = nn.Sequential(sl.IAF(), sl.ExpLeak(tau_mem=10))
+    input_ = torch.eye(4).unsqueeze(0).unsqueeze(0)
+
+    analyzer = sinabs.SNNAnalyzer(model)
+    output = model(input_)
+    model_stats = analyzer.get_model_statistics(average=True)
+    assert model_stats["firing_rate"] == 0.25
+    
+    layer_stats = analyzer.get_layer_statistics(average=True)
+    # ExpLeak layer should not show up in spiking or parameter stats
+    assert "1" not in layer_stats["spiking"]
+    assert "1" not in layer_stats["parameter"]
+    
+    spiking_layer_stats = layer_stats["spiking"]["0"]
+    assert spiking_layer_stats["firing_rate"] == 0.25
+    assert spiking_layer_stats["firing_rate_per_neuron"].shape == (4, 4)
+    assert spiking_layer_stats["firing_rate_per_neuron"].mean() == 0.25
+
+
 def test_spiking_layer_firing_rate_across_batches():
     layer = sl.IAF()
     input1 = torch.eye(4).unsqueeze(0).unsqueeze(0)
     input2 = 2 * torch.eye(4).unsqueeze(0).unsqueeze(0)
 
     analyzer = sinabs.SNNAnalyzer(layer)
     output = layer(input1)
```

### Comparing `sinabs-1.2.6.dev6/tests/test_to_spike_layer.py` & `sinabs-1.2.7.dev1/tests/test_to_spike_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-1.2.6.dev6/tests/test_utils.py` & `sinabs-1.2.7.dev1/tests/test_utils.py`

 * *Files identical despite different names*

