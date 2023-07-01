# Comparing `tmp/llm_client-0.6.1.tar.gz` & `tmp/llm_client-0.6.2.tar.gz`

## Comparing `llm_client-0.6.1.tar` & `llm_client-0.6.2.tar`

### file list

```diff
@@ -1,309 +1,57 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.6.1/.DS_Store
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 llm_client-0.6.1/preformnce_banchmark.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.6.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/base_llm_client.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/__init__.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/ai21_client.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/aleph_alpha_client.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/anthropic_client.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/base_llm_api_client.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/google_client.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/huggingface_client.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/llm_api_client_factory.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_api_client/openai_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_client/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/llm_client/local_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/sync/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 llm_client-0.6.1/llm_client/sync/sync_llm_api_client_factory.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/pyvenv.cfg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/activate
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/activate.csh
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/activate.fish
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/convert-caffe2-to-onnx
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/convert-onnx-to-caffe2
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/deactivate.nu
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/docutils
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/f2py
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/f2py3
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/f2py3.11
--rwxr-xr-x   0        0        0     1696 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/get_objgraph
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/httpx
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/huggingface-cli
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/isympy
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/keyring
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/langchain
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/langchain-server
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/markdown-it
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/normalizer
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/openai
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pip
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pip3
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pip3.11
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pkginfo
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/publish.py
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/py.test
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pygmentize
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyproject-build
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyrsa-decrypt
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyrsa-encrypt
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyrsa-keygen
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyrsa-priv2pub
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyrsa-sign
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pyrsa-verify
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2html.py
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2man.py
--rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2odt.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/torchrun
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/tqdm
--rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/transformers-cli
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/twine
--rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/undill
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/wheel
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/wheel-3.11
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/wheel3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/bin/wheel3.11
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/etc/jupyter/nbconfig/notebook.d/jupyterlab-plotly.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/LICENSE.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/README.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
--rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
--rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
--rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/package.json
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-r--r--   0        0        0  3578814 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-r--r--   0        0        0    70520 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/style.js
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/third-party-licenses.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/extension.js
--rw-r--r--   0        0        0  3666905 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js.LICENSE.txt
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.6.1/new_venv/share/man/man1/isympy.1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/conftest.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/test_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/ai21_client/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/ai21_client/conftest.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/ai21_client/test_ai21.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/anthropic_client/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/anthropic_client/conftest.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/anthropic_client/test_anthropic_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/google_client/__init__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/google_client/conftest.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/google_client/test_google_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/huggingface_client/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/huggingface_client/conftest.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/huggingface_client/test_huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/openai_client/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/openai_client/conftest.py
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_api_client/openai_client/test_openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_client/local_client/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_client/local_client/conftest.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/llm_client/local_client/test_local_client.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/ai21/text_completion.json
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/ai21/tokenize.json
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/google/chat_completion.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/google/embedding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/google/text_completion.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/google/tokens_count.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/huggingface/text_completion.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/openai/chat_completion.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/resources/openai/text_completion.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.1/tests/test_utils/load_json_resource.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/Activate.ps1
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/activate
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/activate.csh
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/activate.fish
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/docutils
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/f2py
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/f2py3
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/f2py3.9
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/httpx
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/huggingface-cli
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/keyring
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/normalizer
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/openai
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pip
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pip3
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pip3.10
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pip3.9
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pkginfo
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/publish.py
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/py.test
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pygmentize
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyproject-build
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyrsa-decrypt
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyrsa-encrypt
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyrsa-keygen
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyrsa-priv2pub
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyrsa-sign
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pyrsa-verify
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/python -> python3.9
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/python3 -> python3.9
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/python3.9 -> /opt/miniconda3/bin/python3.9
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2html.py
--rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1107 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2html5.py
--rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2latex.py
--rwxr-xr-x   0        0        0      672 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2man.py
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2odt.py
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2s5.py
--rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rst2xml.py
--rwxr-xr-x   0        0        0      726 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/tqdm
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/transformers-cli
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_3_9/bin/twine
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/pyvenv.cfg
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/activate
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/activate.csh
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/activate.fish
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/deactivate.nu
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/normalizer
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/pip
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/pip3
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/pip3.11
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/py.test
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/wheel
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/wheel-3.11
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/wheel3
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_ai21/bin/wheel3.11
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/pyvenv.cfg
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/activate
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/activate.csh
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/activate.fish
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/deactivate.nu
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/f2py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/f2py3
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/f2py3.11
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/huggingface-cli
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/normalizer
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/pip
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/pip3
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/pip3.11
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/py.test
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/tqdm
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/transformers-cli
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/wheel
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/wheel-3.11
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/wheel3
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.1/venv_local/bin/wheel3.11
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.6.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.6.1/LICENSE
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 llm_client-0.6.1/README.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 llm_client-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 llm_client-0.6.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.6.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/base_llm_client.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/ai21_client.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/aleph_alpha_client.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/anthropic_client.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/base_llm_api_client.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/google_client.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/huggingface_client.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/llm_api_client_factory.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/openai_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_client/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_client/local_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/sync/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/sync/sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/conftest.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/test_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/ai21_client/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/ai21_client/conftest.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/ai21_client/test_ai21.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/anthropic_client/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/anthropic_client/conftest.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/anthropic_client/test_anthropic_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/google_client/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/google_client/conftest.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/google_client/test_google_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/huggingface_client/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/huggingface_client/conftest.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/huggingface_client/test_huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/openai_client/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/openai_client/conftest.py
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/openai_client/test_openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/local_client/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/local_client/conftest.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/local_client/test_local_client.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/ai21/text_completion.json
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/ai21/tokenize.json
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/chat_completion.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/embedding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/text_completion.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/tokens_count.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/huggingface/text_completion.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/openai/chat_completion.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/openai/text_completion.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/test_utils/load_json_resource.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.6.2/LICENSE
+-rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 llm_client-0.6.2/README.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 llm_client-0.6.2/PKG-INFO
```

### Comparing `llm_client-0.6.1/.github/workflows/test.yml` & `llm_client-0.6.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/__init__.py` & `llm_client-0.6.2/llm_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 from llm_client.base_llm_client import BaseLLMClient
 
 # load api clients
 try:
     from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
     from llm_client.llm_api_client.llm_api_client_factory import LLMAPIClientFactory, LLMAPIClientType
```

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/ai21_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/ai21_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/aleph_alpha_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/aleph_alpha_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/anthropic_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/anthropic_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from typing import Optional
 
-from anthropic import count_tokens
+from anthropic import AsyncAnthropic
 
 from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
 from llm_client.consts import PROMPT_KEY
 
 COMPLETE_PATH = "complete"
 BASE_URL = "https://api.anthropic.com/v1/"
 COMPLETIONS_KEY = "completion"
 AUTH_HEADER = "x-api-key"
 ACCEPT_HEADER = "Accept"
+VERSION_HEADER = "anthropic-version"
 ACCEPT_VALUE = "application/json"
 MAX_TOKENS_KEY = "max_tokens_to_sample"
 
 
 class AnthropicClient(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
+        self._anthropic = AsyncAnthropic()
+        if self._headers.get(VERSION_HEADER) is None:
+            self._headers[VERSION_HEADER] = self._anthropic.default_headers[VERSION_HEADER]
         self._headers[ACCEPT_HEADER] = ACCEPT_VALUE
         self._headers[AUTH_HEADER] = self._api_key
 
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: Optional[int] = None,
                               temperature: float = 1,
                               **kwargs) -> \
             list[str]:
@@ -36,8 +40,8 @@
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
         return [response_json[COMPLETIONS_KEY]]
 
     async def get_tokens_count(self, text: str, **kwargs) -> int:
-        return count_tokens(text)
+        return await self._anthropic.count_tokens(text)
```

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/base_llm_api_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/base_llm_api_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/google_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/google_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/huggingface_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/huggingface_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/llm_api_client_factory.py` & `llm_client-0.6.2/llm_client/llm_api_client/llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_api_client/openai_client.py` & `llm_client-0.6.2/llm_client/llm_api_client/openai_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/llm_client/local_client.py` & `llm_client-0.6.2/llm_client/llm_client/local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/llm_client/sync/sync_llm_api_client_factory.py` & `llm_client-0.6.2/llm_client/sync/sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/test_llm_api_client_factory.py` & `llm_client-0.6.2/tests/llm_api_client/test_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/ai21_client/conftest.py` & `llm_client-0.6.2/tests/llm_api_client/ai21_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/ai21_client/test_ai21.py` & `llm_client-0.6.2/tests/llm_api_client/ai21_client/test_ai21.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/anthropic_client/conftest.py` & `llm_client-0.6.2/tests/llm_api_client/openai_client/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,34 @@
+from unittest.mock import MagicMock, patch
+
 import pytest
+from aiohttp import ClientSession
 
-from llm_client import AnthropicClient
-from llm_client.llm_api_client.anthropic_client import BASE_URL, COMPLETE_PATH
 from llm_client.llm_api_client.base_llm_api_client import LLMAPIClientConfig
+from llm_client.llm_api_client.openai_client import OpenAIClient
 
 
 @pytest.fixture
 def model_name():
-    return "claude-v1"
+    return "ada"
+
+
+@pytest.fixture
+def openai_mock():
+    with patch("llm_client.llm_api_client.openai_client.openai") as openai_mock:
+        yield openai_mock
 
 
 @pytest.fixture
-def config(client_session, model_name):
-    return LLMAPIClientConfig("top-secret-api-key", client_session, default_model=model_name)
+def config(model_name):
+    return LLMAPIClientConfig("fake-api-key", MagicMock(ClientSession), default_model=model_name)
 
 
 @pytest.fixture
-def llm_client(config):
-    return AnthropicClient(config)
+def open_ai_client(config):
+    return OpenAIClient(config)
 
 
 @pytest.fixture
-def complete_url():
-    return BASE_URL + COMPLETE_PATH
+def tiktoken_mock():
+    with patch("llm_client.llm_api_client.openai_client.tiktoken") as tiktoken_mock:
+        yield tiktoken_mock
```

### Comparing `llm_client-0.6.1/tests/llm_api_client/anthropic_client/test_anthropic_client.py` & `llm_client-0.6.2/tests/llm_api_client/anthropic_client/test_anthropic_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,114 @@
-from unittest.mock import patch
-
 import pytest
 
-from llm_client import LLMAPIClientFactory, LLMAPIClientType, AnthropicClient
+from llm_client import LLMAPIClientFactory, LLMAPIClientType
 from llm_client.consts import PROMPT_KEY, MODEL_KEY
 from llm_client.llm_api_client.anthropic_client import AUTH_HEADER, COMPLETIONS_KEY, MAX_TOKENS_KEY, ACCEPT_HEADER, \
-    ACCEPT_VALUE
+    ACCEPT_VALUE, VERSION_HEADER, AnthropicClient
 
 
 @pytest.mark.asyncio
 async def test_get_llm_api_client__with_anthropic(config):
     del config.session
     async with LLMAPIClientFactory() as llm_api_client_factory:
         actual = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.ANTHROPIC, **config.__dict__)
 
     assert isinstance(actual, AnthropicClient)
 
 
 @pytest.mark.asyncio
-async def test_text_completion__sanity(mock_aioresponse, llm_client, complete_url):
+async def test_text_completion__sanity(mock_aioresponse, llm_client, complete_url, anthropic_version):
+    mock_aioresponse.post(
+        complete_url,
+        payload={COMPLETIONS_KEY: "completion text"}
+    )
+
+    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
+
+    assert actual == ["completion text"]
+    mock_aioresponse.assert_called_once_with(complete_url, method='POST',
+                                             headers={AUTH_HEADER: llm_client._api_key,
+                                                      ACCEPT_HEADER: ACCEPT_VALUE,
+                                                      VERSION_HEADER: anthropic_version},
+                                             json={PROMPT_KEY: 'These are a few of my favorite',
+                                                   MAX_TOKENS_KEY: 10, "temperature": 1,
+                                                   MODEL_KEY: llm_client._default_model},
+                                             raise_for_status=True)
+
+
+@pytest.mark.asyncio
+async def test_text_completion__with_version_header(mock_aioresponse, config, complete_url):
     mock_aioresponse.post(
         complete_url,
         payload={COMPLETIONS_KEY: "completion text"}
     )
+    config.headers[VERSION_HEADER] = "1.0.0"
+    llm_client = AnthropicClient(config)
 
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
-                                                      ACCEPT_HEADER: ACCEPT_VALUE},
+                                                      ACCEPT_HEADER: ACCEPT_VALUE,
+                                                      VERSION_HEADER: "1.0.0"},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
                                                    MAX_TOKENS_KEY: 10, "temperature": 1,
                                                    MODEL_KEY: llm_client._default_model},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__without_max_tokens_raise_value_error(mock_aioresponse, llm_client):
     with pytest.raises(ValueError):
         await llm_client.text_completion(prompt="These are a few of my favorite")
 
 
 @pytest.mark.asyncio
-async def test_text_completion__override_model(mock_aioresponse, llm_client, complete_url):
+async def test_text_completion__override_model(mock_aioresponse, llm_client, complete_url, anthropic_version):
     new_model_name = "claude-instant"
     mock_aioresponse.post(
         complete_url,
         payload={COMPLETIONS_KEY: "completion text"}
     )
 
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", model=new_model_name,
                                               max_tokens=10)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
-                                                      ACCEPT_HEADER: ACCEPT_VALUE},
+                                                      ACCEPT_HEADER: ACCEPT_VALUE,
+                                                      VERSION_HEADER: anthropic_version},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
                                                    MAX_TOKENS_KEY: 10, "temperature": 1,
                                                    MODEL_KEY: new_model_name},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
-async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, complete_url):
+async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, complete_url, anthropic_version):
     mock_aioresponse.post(
         complete_url,
         payload={COMPLETIONS_KEY: "completion text"}
     )
 
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10, temperature=0.5)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
-                                                      ACCEPT_HEADER: ACCEPT_VALUE},
+                                                      ACCEPT_HEADER: ACCEPT_VALUE,
+                                                      VERSION_HEADER: anthropic_version},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
                                                    MAX_TOKENS_KEY: 10,
                                                    MODEL_KEY: llm_client._default_model,
                                                    "temperature": 0.5},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
-async def test_get_tokens_count__sanity(llm_client):
-    with patch("llm_client.llm_api_client.anthropic_client.count_tokens") as mock_count_tokens:
-        actual = await llm_client.get_tokens_count(text="These are a few of my favorite things!")
+async def test_get_tokens_count__sanity(llm_client, number_of_tokens, mock_anthropic):
+    actual = await llm_client.get_tokens_count(text="These are a few of my favorite things!")
 
-        assert actual == mock_count_tokens.return_value
-        mock_count_tokens.assert_called_once_with("These are a few of my favorite things!")
+    assert actual == 10
+    mock_anthropic.return_value.count_tokens.assert_awaited_once_with("These are a few of my favorite things!")
```

### Comparing `llm_client-0.6.1/tests/llm_api_client/google_client/conftest.py` & `llm_client-0.6.2/tests/llm_api_client/google_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/google_client/test_google_client.py` & `llm_client-0.6.2/tests/llm_api_client/google_client/test_google_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/huggingface_client/conftest.py` & `llm_client-0.6.2/tests/llm_api_client/huggingface_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/huggingface_client/test_huggingface.py` & `llm_client-0.6.2/tests/llm_api_client/huggingface_client/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_api_client/openai_client/test_openai.py` & `llm_client-0.6.2/tests/llm_api_client/openai_client/test_openai.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_client/local_client/conftest.py` & `llm_client-0.6.2/tests/llm_client/local_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/llm_client/local_client/test_local_client.py` & `llm_client-0.6.2/tests/llm_client/local_client/test_local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/tests/resources/ai21/text_completion.json` & `llm_client-0.6.2/tests/resources/ai21/text_completion.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/.gitignore` & `llm_client-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/LICENSE` & `llm_client-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.1/README.md` & `llm_client-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # LLM-Client-SDK
 [![Test](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/github/license/uripeled2/llm-client-sdk.svg)](https://opensource.org/licenses/MIT)
 
-LLM-Client-SDK is an SDK for communicating with generative AI large language models
+LLM-Client-SDK is an SDK for seamless integration with generative AI large language models
 (We currently support - OpenAI, Google, AI21, HuggingfaceHub, Aleph Alpha, Anthropic,
 Local models with transformers - and many more soon).
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
```

### Comparing `llm_client-0.6.1/pyproject.toml` & `llm_client-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "tiktoken >=0.3.3",
     "dataclasses_json >= 0.5.0"
 ]
 huggingface = [
     "transformers >= 4.0.0"
 ]
 anthropic = [
-    "anthropic >= 0.2.0"
+    "anthropic >= 0.3.2"
 ]
 google = [
     "google-generativeai >= 0.1.0"
 ]
 api = [
     "llm-client[openai,huggingface,anthropic,google]"
 ]
```

### Comparing `llm_client-0.6.1/PKG-INFO` & `llm_client-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: SDK for using LLM
 Project-URL: Homepage, https://github.com/uripeled2/llm-client-sdk
 Author-email: Uri Peled <uripeled2@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: aiohttp<4.0.0,>=3.0.0
 Provides-Extra: all
 Requires-Dist: llm-client[api,local,sync]; extra == 'all'
 Provides-Extra: anthropic
-Requires-Dist: anthropic>=0.2.0; extra == 'anthropic'
+Requires-Dist: anthropic>=0.3.2; extra == 'anthropic'
 Provides-Extra: api
 Requires-Dist: llm-client[anthropic,google,huggingface,openai]; extra == 'api'
 Provides-Extra: google
 Requires-Dist: google-generativeai>=0.1.0; extra == 'google'
 Provides-Extra: huggingface
 Requires-Dist: transformers>=4.0.0; extra == 'huggingface'
 Provides-Extra: local
@@ -41,15 +41,15 @@
 Requires-Dist: pytest-mock; extra == 'test'
 Description-Content-Type: text/markdown
 
 # LLM-Client-SDK
 [![Test](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/github/license/uripeled2/llm-client-sdk.svg)](https://opensource.org/licenses/MIT)
 
-LLM-Client-SDK is an SDK for communicating with generative AI large language models
+LLM-Client-SDK is an SDK for seamless integration with generative AI large language models
 (We currently support - OpenAI, Google, AI21, HuggingfaceHub, Aleph Alpha, Anthropic,
 Local models with transformers - and many more soon).
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
```

