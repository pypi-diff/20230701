# Comparing `tmp/cloci-0.0.9.tar.gz` & `tmp/cloci-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloci-0.0.9.tar", last modified: Wed Jun 28 23:00:12 2023, max compression
+gzip compressed data, was "cloci-0.1.0.tar", last modified: Sat Jul  1 02:42:50 2023, max compression
```

## Comparing `cloci-0.0.9.tar` & `cloci-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.821971 cloci-0.0.9/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    34207 2023-06-21 18:37:49.000000 cloci-0.0.9/LICENSE
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     4367 2023-06-28 23:00:12.819971 cloci-0.0.9/PKG-INFO
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3894 2023-06-21 18:37:25.000000 cloci-0.0.9/README.md
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      696 2023-06-21 18:37:25.000000 cloci-0.0.9/TODO.md
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.696979 cloci-0.0.9/cloci/
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.732017 cloci-0.0.9/cloci/cloci.egg-info/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     4367 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/PKG-INFO
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      532 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/SOURCES.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/dependency_links.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      107 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/requires.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       10 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/top_level.txt
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.777976 cloci-0.0.9/cloci/lib/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:01.000000 cloci-0.0.9/cloci/lib/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    27794 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/evo_conco.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    18698 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/generate_nulls.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16702 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/hgp2hgx.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74109 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/hgx2hlgs.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    36251 2023-05-30 17:06:24.000000 cloci-0.0.9/cloci/lib/input_parsing.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    39842 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/output_data.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     7114 2023-05-30 17:03:59.000000 cloci-0.0.9/cloci/lib/treecalcs.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.815973 cloci-0.0.9/cloci/tools/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:06.000000 cloci-0.0.9/cloci/tools/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23144 2023-05-04 18:14:28.000000 cloci-0.0.9/cloci/tools/cloci2enrich.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13698 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/tools/cloci2stats.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     9802 2023-06-16 22:09:29.000000 cloci-0.0.9/cloci/tools/hlg2biofile.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17241 2023-06-16 22:09:33.000000 cloci-0.0.9/cloci/tools/hlg2hlg_net.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2023-06-28 23:00:12.822974 cloci-0.0.9/setup.cfg
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1249 2023-06-28 23:00:11.000000 cloci-0.0.9/setup.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.826247 cloci-0.1.0/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      107 2023-07-01 02:42:18.000000 cloci-0.1.0/.gitignore
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    34207 2023-06-21 18:37:49.000000 cloci-0.1.0/LICENSE
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    43924 2023-07-01 02:42:50.824253 cloci-0.1.0/PKG-INFO
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3894 2023-06-21 18:37:25.000000 cloci-0.1.0/README.md
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      740 2023-06-30 00:13:59.000000 cloci-0.1.0/TODO.md
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.689251 cloci-0.1.0/archive/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    73986 2023-04-12 16:22:58.000000 cloci-0.1.0/archive/hgx2gcfs.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74097 2023-04-12 16:22:58.000000 cloci-0.1.0/archive/hgx2hlgs.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.693251 cloci-0.1.0/cloci/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    46352 2023-07-01 02:39:13.000000 cloci-0.1.0/cloci/cloci.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.747260 cloci-0.1.0/cloci/lib/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:01.000000 cloci-0.1.0/cloci/lib/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    27794 2023-06-28 00:57:46.000000 cloci-0.1.0/cloci/lib/evo_conco.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    18698 2023-06-28 00:57:46.000000 cloci-0.1.0/cloci/lib/generate_nulls.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16702 2023-06-28 00:57:46.000000 cloci-0.1.0/cloci/lib/hgp2hgx.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74109 2023-06-28 00:57:46.000000 cloci-0.1.0/cloci/lib/hgx2hlgs.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    36251 2023-05-30 17:06:24.000000 cloci-0.1.0/cloci/lib/input_parsing.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    37967 2023-06-30 16:53:27.000000 cloci-0.1.0/cloci/lib/output_data.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     7114 2023-05-30 17:03:59.000000 cloci-0.1.0/cloci/lib/treecalcs.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.781253 cloci-0.1.0/cloci/tools/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:39:38.000000 cloci-0.1.0/cloci/tools/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23167 2023-07-01 02:39:15.000000 cloci-0.1.0/cloci/tools/cloci2enrich.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13966 2023-07-01 02:39:16.000000 cloci-0.1.0/cloci/tools/cloci2stats.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16906 2023-07-01 02:39:22.000000 cloci-0.1.0/cloci/tools/hg2hg_net.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     9825 2023-07-01 02:39:16.000000 cloci-0.1.0/cloci/tools/hlg2biofile.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17264 2023-07-01 02:39:16.000000 cloci-0.1.0/cloci/tools/hlg2hlg_net.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.716256 cloci-0.1.0/cloci.egg-info/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    43924 2023-07-01 02:42:50.000000 cloci-0.1.0/cloci.egg-info/PKG-INFO
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      684 2023-07-01 02:42:50.000000 cloci-0.1.0/cloci.egg-info/SOURCES.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2023-07-01 02:42:50.000000 cloci-0.1.0/cloci.egg-info/dependency_links.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      250 2023-07-01 02:42:50.000000 cloci-0.1.0/cloci.egg-info/entry_points.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       23 2023-07-01 02:42:50.000000 cloci-0.1.0/cloci.egg-info/requires.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        6 2023-07-01 02:42:50.000000 cloci-0.1.0/cloci.egg-info/top_level.txt
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:42:50.812249 cloci-0.1.0/etc/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    75323 2023-06-16 22:03:00.000000 cloci-0.1.0/etc/boundaries.png
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)   307022 2023-06-16 22:03:00.000000 cloci-0.1.0/etc/pipeline.png
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    42013 2023-06-16 22:03:00.000000 cloci-0.1.0/etc/recovery.png
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1218 2023-07-01 02:42:11.000000 cloci-0.1.0/pyproject.toml
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2023-07-01 02:42:50.826257 cloci-0.1.0/setup.cfg
```

### Comparing `cloci-0.0.9/LICENSE` & `cloci-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/PKG-INFO` & `cloci-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: cloci
-Version: 0.0.9
-Summary: Function-agnostic gene cluster detection
-Home-page: https://github.com/xonq/cloci/
-Author: xonq
-Author-email: konkelzach@protonmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.0,<4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## NOTE
 Extensive alpha testing has been conducted, though this software is in a beta state. Errors are expected, often rerunning without changing parameters is sufficient to resume appropriately. 
 Kindly raise git issues for errors - if you can find the bug, even better! This software will have longterm maintenance, but maintenance is currently not the priority. Documentation is currently lacking, please be patient as I build out the repository and wiki.
 
 Please also note that this software interfaces with the comparative genomics software suite, Mycotools. I am hopeful you will find Mycotools useful. Please find its manuscript and the [associated repository](https://gitlab.com/xonq/mycotools).
 
 <br />
```

### Comparing `cloci-0.0.9/TODO.md` & `cloci-0.1.0/TODO.md`

 * *Files 17% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 	- [ ] High percentage of 1 domain/reference cluster
 - [ ] Convert sliding window to nucleotide-based slide
 - [ ] Account for alternate splicing appropriately
 - [ ] Implement probabilistic pass for 2 HG HG combinations
 - [ ] Account for duplicates of HGs on edge of cluster
 - [ ] Add Pfam extraction feature
 - [ ] Add GO extraction feature
+- [ ] Output networks as interactable files
```

### Comparing `cloci-0.0.9/cloci/lib/evo_conco.py` & `cloci-0.1.0/cloci/lib/evo_conco.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/cloci/lib/generate_nulls.py` & `cloci-0.1.0/cloci/lib/generate_nulls.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/cloci/lib/hgp2hgx.py` & `cloci-0.1.0/cloci/lib/hgp2hgx.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/cloci/lib/hgx2hlgs.py` & `cloci-0.1.0/cloci/lib/hgx2hlgs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/cloci/lib/input_parsing.py` & `cloci-0.1.0/cloci/lib/input_parsing.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/cloci/lib/output_data.py` & `cloci-0.1.0/cloci/lib/output_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -502,68 +502,16 @@
     return ann_res, failed_omes
 
 
 def annotate_clusters(genes_list, #gff_path, prot_path, 
                       ome, ome_dir, gene2hg, prefix = 'hlg',
                       ann_res = {}):
 
-#    gff_dir, fa_dir = ome_dir + ome + '/gff/', ome_dir + ome + '/fa/'
- #   if not os.path.isdir(gff_dir):
-  #      os.mkdir(gff_dir)
-   # if not os.path.isdir(fa_dir):
-    #    os.mkdir(fa_dir)
-
- #   clus_gffs, clus_fas, clus_anns, scafs, svg_dict = [], [], {}, set(), {}
-#    gff_list, prot_dict = gff2list(gff_path), fa2dict(prot_path)
-#    print('\t' + ome, flush = True)
- #   for genes in genes_list:
-  #      clus_gffs.append([[]])
-   #     clus_fas.append({})
-    #    clus_ann = ''
-     #   for gene in genes:
-      #      geneCoord = None
-       #     geneGff = grabGffAcc(gff_list, gene)
-        #    for entry in geneGff:
-         #       if entry['type'].lower() == 'gene':
-          #          geneCoord = (int(entry['start']), int(entry['end']), entry['strand'])
-           # geneFa = prot_dict[gene]
-            #if gene in ann_res:
-             #   pfamStr = ';Pfam=' + '|'.join([
-              #      (hit[0] + '-' + hit[1]).replace('|','&') for hit in ann_res[gene]
-               #     ])
-                #clus_ann += pfamStr[6:]
-#            else:
- #               pfamStr = ''
-  #          clus_ann += ','
-   #         try:
-    #            ogStr = ';OG=' + str(gene2hg[gene])
-     #       except KeyError: # gene not in an OG or is a singleton
-      #          ogStr = ';OG='
-       #     for entry in geneGff:
-        #        if entry['type'] == 'gene' or entry['type'].lower() == 'mrna':
-         #           entry['attributes'] += pfamStr + ogStr
-          #  geneFa['description'] = pfamStr[6:]
-           # clus_gffs[-1][0].extend(geneGff)
-            #clus_fas[-1][gene] = geneFa
-#        scaf_prep = clus_gffs[-1][0][0]['seqid']
- #       scaf = scaf_prep[:20]
-  #      if scaf_prep != scaf:
-   #         scaf = scaf_prep[:20] + '..'
-    #    count = 0
-     #   while scaf + '_' + str(count) in scafs:
-      #      count += 1
-       # name = scaf + '_' + str(count)
-        #scafs.add(name)
-#        clus_anns[name] = clus_ann[:-1]
- #       clus_gffs[-1].append(name)
-#        svg_dict[name] = copy.deepcopy(t_svg_dict)
-#        with open(gff_dir + name + '.gff3', 'w') as out:
- #           out.write(list2gff(clus_gffs[-1][0]))
-  #      with open(fa_dir + name + '.fa', 'w') as out:
-   #         out.write(dict2fa(clus_fas[-1]))
+    if not os.path.isfile(f'{ome_dir}{ome}/{prefix}.tsv'):
+        return
 
     with open(ome_dir + ome + f'/{prefix}.tsv.tmp', 'w') as out:
         out.write('#name\thgs\tgenes\tgcfs\tpfams\n')
         with open(ome_dir + ome + f'/{prefix}.tsv', 'r') as raw:
             for line in raw:
                 if not line.startswith('#'):
                     clus_d = line.split()
@@ -572,15 +520,15 @@
                     anns = ['|'.join([y[1] if y else '' for y in x]) \
                             if x else '' for x in anns_p]
                     ann_str = ';'.join(anns)
                     out.write('\t'.join(clus_d + [ann_str]) + '\n')
     shutil.move(f'{ome_dir}{ome}/{prefix}.tsv.tmp', 
                 f'{ome_dir}{ome}/{prefix}.tsv')
 
-    return ome#, svg_dict
+#    return ome#, svg_dict
 #    return ome, clus_gffs, clus_fas, svg_dict
 
 
 def output_hgxs(hgx2dist, hgx2omes, hgx2i, i2ome, out_dir):
     maxhgxd = max(hgx2dist.values())
     minhgxd = min(hgx2dist.values())
 
@@ -732,14 +680,16 @@
             except TypeError:
                  if hgx2omes2gcl[hgxc][omesc] >= gcl_thresh \
                     and omes2patch[omesc] >= patch_thresh \
                     and hgx2omes2id[hgxc][omesc] >= id_perc:
                     gcfs[hlg] = locs
                     gcf_omes[hlg] = omesc
                     gcf_hgxs[hlg] = hgxc
+            except KeyError:
+                eprint(f'\tWARNING: missing from proxies and removed: {omesc, hgxc}')
         return gcfs, gcf_omes, gcf_hgxs
     else:
         return hlgs, hlg_omes, hlg_hgxs
 
 def threshold_hlg_wopos(gcl_thresh, patch_thresh, id_perc, hlgs,
                        hlg_hgxs, hlg_omes, omes2patch,
                        hgx2omes2gcl, hgx2omes2id):
@@ -942,17 +892,17 @@
             pass
 #             annotate_clusters_cmds.append([genes, #gff_path, pro_path, 
  #                                  ome, out_dir + 'ome/', gene2hg,
    #                                prefix])
 
 
     with mp.get_context('fork').Pool(processes = cpus) as pool:
-        clus_info = pool.starmap(annotate_clusters, 
-                                 tqdm(annotate_clusters_cmds, 
-                                      total = len(annotate_clusters_cmds)))
+        pool.starmap(annotate_clusters, 
+                             tqdm(annotate_clusters_cmds, 
+                                  total = len(annotate_clusters_cmds)))
         pool.close()
         pool.join()
 
 
 def output_hlgs(db, wrk_dir, hlgs, hlg_omes, i2ome, out_dir, hlg_hgxs,
          omes2dist, omes2patch, hgx2omes2gcl, hgx2omes2id, hgx2omes2pos, 
          gene2hg, plusminus, ome2i, hlg2clan, dist_thresh, gcl_thresh,
@@ -994,7 +944,10 @@
         gcf_genes = write_ome_output('gcf', gcfs, out_dir, db, cpus, gene2hg)
    
     if pfam_path or ipr_path:    
         print('\nX. Annotating clusters', flush = True)
 
     annotation_mngr(hlg_genes, db, wrk_dir, pfam_path, ipr_path, 
                     gene2hg, out_dir, prefix = 'hlg', cpus = cpus)
+    if dist_thresh or gcl_thresh or patch_thresh or id_perc or pos_perc:
+        annotation_mngr(hlg_genes, db, wrk_dir, pfam_path, ipr_path, 
+                        gene2hg, out_dir, prefix = 'gcf', cpus = cpus)
```

### Comparing `cloci-0.0.9/cloci/lib/treecalcs.py` & `cloci-0.1.0/cloci/lib/treecalcs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.9/cloci/tools/cloci2enrich.py` & `cloci-0.1.0/cloci/tools/cloci2enrich.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,15 +495,15 @@
                 WriteOutput(ref_scores[2], thresh, out_base + '_hvt.ref.go.tsv', go2pfam = True)
         else:
             scoresDict = GetPopResults(ome2genes2pfam, ome2clus_genes2pfam, taxonGenes, taxonClusGenes, pool)
             print(f'\tWriting', flush = True)
 
             WriteOutput(scoresDict, thresh, out_base + '.pfam.tsv', go2onto = None)
 
-if __name__ == '__main__':
+def cli():
 
     parser = argparse.ArgumentParser(description = 'cloci2pfam enrichment')
     parser.add_argument('-a', '--alpha', help = 'Overall Bonferonni corrected alpha; DEFAULT: 0.05',
         type = float, default = 0.05)
     parser.add_argument('-d', '--db', help = 'cloci mycotools db input', required = True)
     parser.add_argument('-r', '--rank', help = 'taxon rank', required = True)
     parser.add_argument('-c', '--cloci_dir', help = 'cloci output dir', required = True)
@@ -552,7 +552,11 @@
     pool = mp.Pool(processes = args.cpu)
     main(db, args.alpha, args.rank.lower(), cloci_dir, pfam_dir, out_dir, pfam2go_path, 
          go_file, go_terms, pool = pool, top_hit = args.top_hit)
     pool.close()
     pool.join()
 
     sys.exit(0)
+
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `cloci-0.0.9/cloci/tools/cloci2stats.py` & `cloci-0.1.0/cloci/tools/cloci2stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     return -sum([v/len_anns * log(v/len_anns) for v in ann_counts.values()])
             
 
 def calc_stats(ome, f, gff_path, alia = None):
     genes_in_clus = []
     hlgs = []
     overall_anns = []
+    if not os.path.isfile(f):
+        return None, None, None, None, None, None, None
  #   ind_shannons = []
     with open(f, 'r') as raw:
         for line in raw:
             if not line.startswith('#'):
                 try:
                     data = line.rstrip().split('\t')
                     clus_id, hgs, genes, t_hlgs = data[0],data[1],data[2],data[3]
@@ -109,14 +111,16 @@
                                     'csb': [], 'pds': [], 'sd': [],
                                     'mean_g': [], 'med_g': [], 'pc': []})
 
     with open(tmp_path, 'w') as out:
         out.write('tip\ttmd\tgcl\tmmi\tmmp\tcsb\tpds\tpc\tdivers\ttaxon\n')
         if rank == 'ome':
             for ome, hlgs, mean_gic, median_gic, pc, alia, shan in ome_stats:
+                if not ome:
+                    continue
                 prox = [hlg2data[hlg] for hlg in set(hlgs)]
                 tax_dict[ome]['tmd'].extend([x[0] for x in prox])
                 tax_dict[ome]['gcl'].extend([x[1] for x in prox])
                 tax_dict[ome]['mmi'].extend([x[2] for x in prox])
                 tax_dict[ome]['mmp'].extend([x[3] for x in prox])
                 tax_dict[ome]['csb'].extend([x[4] for x in prox])
                 tax_dict[ome]['pds'].extend([x[5] for x in prox])
@@ -130,16 +134,18 @@
                         + f'{sum(tax_dict[ome]["mmi"])/len(tax_dict[ome]["mmi"])}\t' \
                         + f'{sum(tax_dict[ome]["mmp"])/len(tax_dict[ome]["mmp"])}\t' \
                         + f'{sum(tax_dict[ome]["csb"])/len(tax_dict[ome]["csb"])}\t' \
                         + f'{sum(tax_dict[ome]["pds"])/len(tax_dict[ome]["pds"])}\t' \
                         + f'{pc}\t{sd}\t\n')
         else:
             for ome, hlgs, mean_gic, median_gic, pc, alia, shan in ome_stats:
+                if not ome:
+                    continue
                 tax = db[ome]['taxonomy'][rank]
-                prox = [hlg2data[hlg] for hlg in set(hlgs)]
+                prox = [hlg2data[hlg] for hlg in set(hlgs) if hlg in hlg2data]                        
                 tmd = [x[0] for x in prox]
                 gcl = [x[1] for x in prox]
                 mmi = [x[2] for x in prox]
                 mmp = [x[3] for x in prox]
                 csb = [x[4] for x in prox]
                 pds = [x[5] for x in prox]
 
@@ -282,22 +288,22 @@
   #      if os.path.isfile(tmp_file):
    #         os.remove(tmp_file)
         print('\nWriting GCF stats', flush = True)
         out_f = cloci_dir + 'gcf_stats.' + rank 
         output_stats(out_f, gcf_stats)
 
 
-if __name__ == '__main__':
+def cli():
     ranks = ['ome', 'kingdom', 'phylum', 'subphylum', 'class', 'order', 'family', 'genus', 'species']
     parser = argparse.ArgumentParser(description = 'Summarize CLOCI output for taxonomic rank')
     parser.add_argument('-i', '--input', required = True, help = 'CLOCI input directory')
     parser.add_argument('-r', '--rank', help = f'{ranks}; DEFAULT: ome')
     parser.add_argument('-d', '--mtdb', help = 'MycotoolsDB')
 #    parser.add_argument('-g', '--gamma', action = 'store_true',
-        help = 'Calculate gamma and beta diversity')
+   #     help = 'Calculate gamma and beta diversity')
  #   parser.add_argument('-a', '--annotations', 
    #     help = '[-g] Directory of tbl-formatted Pfam annotations for gamma diversity, labeled <ome>.out')
   #  parser.add_argument('-p', '--pfam', help = '[-g] Pfam.hmm path')
 
 
     parser.add_argument('-c', '--cpu', type = int)
     args = parser.parse_args()
@@ -310,8 +316,12 @@
 #    if args.gamma:
  #       findExecs(['hmmsearch', exit = set('hmmsearch')])
 
 
     main(format_path(args.input), mtdb(format_path(args.mtdb)), rank, cpus = args.cpu)
   #       gamma = False, ann_dir = format_path(args.annotations), 
    #      pfam = format_path(args.pfam),    
-   sys.exit(0)
+    sys.exit(0)
+
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `cloci-0.0.9/cloci/tools/hlg2biofile.py` & `cloci-0.1.0/cloci/tools/hlg2biofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         with mp.Pool(processes = cpus) as pool:
             pool.starmap(compile_ome_faas,
                          tqdm(((db[ome]['faa'], ome, hlg2genes, out_dir, bool(omes)) \
                               for ome, hlg2genes in ome_res), total = len(ome_res)))
         
 
 
-if __name__ == '__main__':
+def cli():
     parser = argparse.ArgumentParser(description = 'Parse CLOCI output and ' \
            + 'generate biofiles. "-" for stdin; -g specifies GCFs, all HLGs by default')
 
     in_opt = parser.add_argument_group('Input parameters')
     in_opt.add_argument('-c', '--cloci_dir', help = 'CLOCI output dir', required = True)
     in_opt.add_argument('-g', '--gcf', action = 'store_true', help = 'Generate files for GCFs')
     in_opt.add_argument('-o', '--ome', help = 'Generate files for all ome(s) HLG/GCFs')
@@ -241,7 +241,11 @@
             print('\nOutputting specified GCFs', flush = True)
         else:
             print('\nOutputting specified HLGs', flush = True)
 
     main(db, run_dir, out_dir, omes, hlgs, args.gcf, 
          args.gbk, args.gff, args.faa, args.cpu)
     sys.exit(0)
+
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `cloci-0.0.9/cloci/tools/hlg2hlg_net.py` & `cloci-0.1.0/cloci/tools/hlg2hlg_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
         locI2name = {k: i02i1[v] for k, v in locI2name.items()}
 
     make_network(out_file, adj_arr, modules, nl2ol, img, 
                  annotate, font_size, locI2color, locI2name, scale)
     print(f'\nNetwork outputted to {out_file}', flush = True)
 
 
-if __name__ == '__main__':
+def cli():
     ranks = ['kingdom', 'phylum', 'subphylum', 'class', 'order', 'family', 'genus']
     img_exts = ['pdf', 'png', 'ps', 'svg']
     net_exts = ['dot', 'gml', 'graphml', 'gt', 'xml']
     parser = argparse.ArgumentParser(
         description = 'Cloci locus-locus similarity network. Will output all clans if no -c/-f'
         )
     parser.add_argument('-i', '--input', help = 'Completed Cloci directory', required = True)
@@ -448,7 +448,11 @@
         colors = []
     
     main(clans, hlgs, format_path(in_dir, force_dir = True), 
          args.min, args.passing, db, rank, ext = ext, img = img,
          annotate_loc = args.annotate_loc, annotate_hlg = args.annotate_hlg,
          highlight = locids, scale = args.scale, chrono = args.convert,
          font_size = args.font_size, colors = colors)
+
+
+if __name__ == '__main__':
+    cli()
```

