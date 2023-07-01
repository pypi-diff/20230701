# Comparing `tmp/kanonym4text-0.1.4.tar.gz` & `tmp/kanonym4text-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanonym4text-0.1.4.tar", last modified: Thu Jun 29 12:33:51 2023, max compression
+gzip compressed data, was "kanonym4text-1.1.5.tar", last modified: Sat Jul  1 16:20:13 2023, max compression
```

## Comparing `kanonym4text-0.1.4.tar` & `kanonym4text-1.1.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-06-29 12:33:51.377794 kanonym4text-0.1.4/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      660 2023-06-29 12:33:51.377794 kanonym4text-0.1.4/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     4398 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/README.md
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-06-29 12:33:51.373794 kanonym4text-0.1.4/kanonym4text/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       54 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/__init__.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-06-29 12:33:51.377794 kanonym4text-0.1.4/kanonym4text/data/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/data/5000_most_common_words_by_order.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    10752 2023-06-29 09:26:44.000000 kanonym4text-0.1.4/kanonym4text/k_anonym_text.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-06-29 12:33:51.377794 kanonym4text-0.1.4/kanonym4text/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13374 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8761 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6128 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      855 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11197 2023-06-29 09:26:32.000000 kanonym4text-0.1.4/kanonym4text/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3187 2023-06-28 20:28:34.000000 kanonym4text-0.1.4/kanonym4text/utils/utilization_utils.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-06-29 12:33:51.373794 kanonym4text-0.1.4/kanonym4text.egg-info/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      660 2023-06-29 12:33:51.000000 kanonym4text-0.1.4/kanonym4text.egg-info/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      685 2023-06-29 12:33:51.000000 kanonym4text-0.1.4/kanonym4text.egg-info/SOURCES.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-06-29 12:33:51.000000 kanonym4text-0.1.4/kanonym4text.egg-info/dependency_links.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-06-29 12:33:51.000000 kanonym4text-0.1.4/kanonym4text.egg-info/requires.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       19 2023-06-29 12:33:51.000000 kanonym4text-0.1.4/kanonym4text.egg-info/top_level.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-06-29 12:33:51.377794 kanonym4text-0.1.4/setup.cfg
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1335 2023-06-29 12:32:50.000000 kanonym4text-0.1.4/setup.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-06-29 12:33:51.377794 kanonym4text-0.1.4/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-06-28 09:31:23.000000 kanonym4text-0.1.4/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13378 2023-06-28 11:14:10.000000 kanonym4text-0.1.4/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8761 2023-06-28 09:31:24.000000 kanonym4text-0.1.4/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6111 2023-06-29 09:19:28.000000 kanonym4text-0.1.4/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      953 2023-06-29 09:23:37.000000 kanonym4text-0.1.4/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11195 2023-06-28 09:31:23.000000 kanonym4text-0.1.4/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3161 2023-06-29 09:23:03.000000 kanonym4text-0.1.4/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:20:13.701461 kanonym4text-1.1.5/
+-rw-rw-rw-   0        0        0     1090 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      879 2023-07-01 16:20:13.700501 kanonym4text-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5151 2023-07-01 16:13:23.000000 kanonym4text-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 16:20:13.556563 kanonym4text-1.1.5/kanonym4text/
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:43:33.000000 kanonym4text-1.1.5/kanonym4text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:20:13.604468 kanonym4text-1.1.5/kanonym4text/data/
+-rw-rw-rw-   0        0        0    40665 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/data/5000_most_common_words_by_order.txt
+-rw-rw-rw-   0        0        0    11472 2023-07-01 15:36:00.000000 kanonym4text-1.1.5/kanonym4text/k_anonym_text.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:20:13.636462 kanonym4text-1.1.5/kanonym4text/utils/
+-rw-rw-rw-   0        0        0      397 2023-07-01 15:44:56.000000 kanonym4text-1.1.5/kanonym4text/utils/__init__.py
+-rw-rw-rw-   0        0        0    13374 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0     8761 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     6128 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      855 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/utils/models.py
+-rw-rw-rw-   0        0        0    11195 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     3187 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/kanonym4text/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:20:13.591497 kanonym4text-1.1.5/kanonym4text.egg-info/
+-rw-rw-rw-   0        0        0      879 2023-07-01 16:20:13.000000 kanonym4text-1.1.5/kanonym4text.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-07-01 16:20:13.000000 kanonym4text-1.1.5/kanonym4text.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 16:20:13.000000 kanonym4text-1.1.5/kanonym4text.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-07-01 16:20:13.000000 kanonym4text-1.1.5/kanonym4text.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-01 16:20:13.000000 kanonym4text-1.1.5/kanonym4text.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 16:20:13.702465 kanonym4text-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2023-07-01 15:59:11.000000 kanonym4text-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:20:13.699498 kanonym4text-1.1.5/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:18:12.000000 kanonym4text-1.1.5/utils/__init__.py
+-rw-rw-rw-   0        0        0    13378 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0     8761 2023-06-28 20:14:13.000000 kanonym4text-1.1.5/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     6132 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      939 2023-06-28 20:14:13.000000 kanonym4text-1.1.5/utils/models.py
+-rw-rw-rw-   0        0        0    11195 2023-06-28 20:14:13.000000 kanonym4text-1.1.5/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     3191 2023-06-29 05:38:36.000000 kanonym4text-1.1.5/utils/utilization_utils.py
```

### Comparing `kanonym4text-0.1.4/kanonym4text/k_anonym_text.py` & `kanonym4text-1.1.5/kanonym4text/k_anonym_text.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,290 +1,296 @@
-#!/usr/bin/python3
-
-"""
-K-anonymity for texts
-"""
-
-# Info
-__author__ = 'Lior Treiman and Hadas Neuman'
-__version__ = '1.1'
-__date__ = '3/6/23'
-
-# Imports
-import sys
-import pandas as pd
-import numpy as np
-import re
-import os
-import argparse
-import time
-import warnings
-import logging
-import pkg_resources
-warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
-
-
-def anonymize_llm(df: pd.DataFrame, k: int, col: str='txt', plot: bool=False, n_jobs: int = 1, verbose: int=0):
-    """
-    Uses LLM methods to preform anonymization
-    """
-    from kanonym4text.utils import llm_utils, utilization_utils, anonym_utils
-
-    # TEMP
-    prefix = 'temp_prefix_llm' # TEMP
-    init_logger(verbose)
-    logging.info(f'{os.path.basename(__file__)} {__version__} LLM pipeline')
-
-    # Adding number of characters
-    num_chars_col = 'Num_characters'
-    df[num_chars_col] = df[col].str.len()
-    docs = df[col]
-    
-    logging.info(f'Number of documents: {len(docs)}')
-    logging.info(f'Average number of characters in documents: {df[num_chars_col].mean()} maximum characters in a document {df[num_chars_col].max()}')
-
-    # Runing the anonymization
-    annon_docs, _ = llm_utils.run_anonymization_on_txt(docs, k, n_jobs)
-    df['anonymized_text'] = annon_docs
-
-    curr_k, non_anon_indexes = anonym_utils.get_anonym_degree(docs=annon_docs, min_k=k)
-    out_str = f'Anonymity after reduction:{curr_k}  number of un-anonymized documents: {len(non_anon_indexes)}'
-    logging.info(out_str)  # Logging
-
-    # Logging the un-anonymized documents
-    if len(non_anon_indexes) > 0: 
-        out_str = f'Un-anonymized documents: {non_anon_indexes}'
-        logging.info(out_str)  # Logging
-
-    # Utilization utils
-    if plot:
-        plot_prefix = prefix
-    else:
-        plot_prefix = None
-    mean_dist = utilization_utils.get_mean_semantice_distance_for_corpus(df[col], df['anonymized_text'], prefix=plot_prefix)
-    out_str = f'Mean semantic distance before and after the anonymization process: {mean_dist}'
-    logging.info(out_str)  # Logging
-
-    logging.info('Done')  # Logging
-    return df, mean_dist
-
-
-def get_prefix(arguments):
-    """
-    Creates a prefix based on the input file and k.
-    """
-    # Removing extension
-    if arguments.out:
-        file = arguments.out
-    else:
-        file = arguments.file
-
-    _, file_extension = os.path.splitext(file)
-    base_name = os.path.basename(file).replace(file_extension, '')
-    prefix = f'{base_name}_k{arguments.k}_stop_{arguments.num_stop}'
-
-    if arguments.sample:
-         prefix += f'_sample_of_{arguments.sample}'
-
-    # LLM
-    if arguments.llm:
-        prefix += '_llm'
-    
-
-    return prefix
-
-
-def init_logger(verbose):
-    """
-    Initiating the logger
-    """
-    # log_name = f'logs/{prefix}.log'
-    logging.basicConfig(
-    level=max(0, 30 - (verbose*10)),
-    format='%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s')
-
-
-def print_size(var, var_name):
-    """
-    Prints the variable size to the log
-    """
-    logging.debug(f'The size of {var_name}: {sys.getsizeof(var)/1000000}MB')
-
-
-def get_data_path():
-    # Credit: https://medium.com/@vuillaut/python-package-and-access-data-in-your-module-d05e72f58785
-    # f1 = pkg_resources.get_resource_filename(__name__, 'data/5000_most_common_words_by_order.txt')
-    relative_file = 'data/5000_most_common_words_by_order.txt'
-    file_name = pkg_resources.resource_filename('kanonym4text', relative_file)
-    return file_name
-
-
-# def run_anonym(arguments):
-def anonymize(df: pd.DataFrame, k: int, col: str='txt', plot: bool=False, wemodel: str = 'glove-twitter-25',
-                num_stop: int = 1000, n_jobs: int = 1, verbose: int=0):
-    """
-    The main function. Runs the anonymization.
-    """
-    init_logger(verbose)
-    logging.info(f'{os.path.basename(__file__)} {__version__} WE pipeline')
-
-    from kanonym4text.utils import nlp_utils, cluster_utils, utilization_utils, anonym_utils, models
-
-    logging.info(f'Word embedding model: {wemodel}')  # Logging
-
-    # Uploading the word embedding model
-    if wemodel == 'glove-twitter-25':
-        cos = False
-    else:
-        cos = True
-    
-    wemodel = models.upload_we_model(wemodel)
-    if wemodel is None:
-        exit(1) 
-
-    # TEMP
-    prefix = 'temp_prefix' # TEMP
-    
-    logging.info(f'Number of documents: {df.shape[0]}')  # Logging
-
-    # Getting the stopword list
-    short_stopword_list = nlp_utils.stopwords.words('english')
-    stop_file = get_data_path()
-    long_stopword_list = nlp_utils.get_list_from_file(stop_file, num_stop)
-    if long_stopword_list:
-        long_stopword_list = list(set(short_stopword_list + long_stopword_list))
-    else:
-        logging.error(f'Could not read the stop word file.')
-        exit(1)
-
-    out_str = f'Stopword list contains {len(long_stopword_list)} words'
-    logging.info(out_str)  # Logging
-
-    # Creating the word dictionary and word list
-    word_dict = nlp_utils.create_word_dict(df[col], long_stopword_list)  # this function takes too long need to make more efficient
-    out_str = f'Number of unique words in dataset: {len(word_dict)}'
-    logging.info(out_str)  # Logging
-
-    # Run clustering
-    cluster_dict, dist_dict, _ = cluster_utils.run_clustering(word_dict, stop_list=long_stopword_list, wemodel=wemodel, cosine=cos, n_jobs=n_jobs)
-    out_str = f'Number of DBSCAN clusters:\t {len(cluster_dict)}'
-    logging.info(out_str)  # Logging
-
-    # Generalization
-    df, _, long_stopword_list = nlp_utils.replace_words_in_df(df, cluster_dict, dist_dict, word_dict, 
-                                                              col, wemodel=wemodel, stop_list = long_stopword_list)
-    out_str = f'Generalization completed.'
-    logging.info(out_str)  # Logging
-    
-    # Find k neighbors
-    neighbor_list = anonym_utils.ckmeans_clustering(docs=df['anon_txt'], k=k, n_jobs=n_jobs, stop_list=short_stopword_list)
-
-    out_str = f'Found {len(neighbor_list)} groups of {k} neighbors'
-    logging.info(out_str)  # Logging
-
-    # Reduction
-    force_anon_txt_annoy = anonym_utils.force_anonym(docs=df['anon_txt'], neighbor_list=neighbor_list, stop_list=long_stopword_list)
-
-    # Testing success
-    curr_k, non_anon_indexes = anonym_utils.get_anonym_degree(docs=force_anon_txt_annoy, min_k=k, stop_list=long_stopword_list)
-    out_str = f'Anonymity after reduction:{curr_k}  number of un-anonymized documents: {len(non_anon_indexes)}'
-    logging.info(out_str)  # Logging
-
-    # Logging the un-anonymized documents
-    if len(non_anon_indexes) > 0: 
-        out_str = f'Un-anonymized documents: {non_anon_indexes}'
-        logging.info(out_str)  # Logging
-
-    # Adding the anonymized corpus to the dataframe
-    anonym_col = 'force_anon_txt'
-    df[anonym_col] = force_anon_txt_annoy
-    del(force_anon_txt_annoy)  # Freeing space
-    df = anonym_utils.add_neighbor_list_to_df(df, neighbor_list)
-    # Counting the number of words and *
-    df['num_of_words_after_forcing'] = df['force_anon_txt'].apply(lambda x: len(re.findall(r'\w+', x)))
-    df['num_of_deleting_after_forcing'] = df['force_anon_txt'].apply(lambda x: len(re.findall(r'\*', x)))
-
-    # Utilization utils
-    if plot:
-        plot_prefix = prefix
-    else:
-        plot_prefix = None
-    mean_dist = utilization_utils.get_mean_semantice_distance_for_corpus(df[col], df[anonym_col], prefix=plot_prefix)
-    out_str = f'Mean semantic distance before and after the anonymization process: {mean_dist}'
-    logging.info(out_str)  # Logging
-    
-    logging.info('Done')  # Logging
-    return df, mean_dist
-
-
-def parse_args():
-    """
-    Defines the ArgumentParser
-    :return: The parser
-    """
-    parser_func = argparse.ArgumentParser(description='Converts dot tree to newick tree format')
-    parser_func.add_argument('-f', '--file', help='Input CSV file', required=True)
-
-    parser_func.add_argument('-k', help='The k anonymity degree',  required=True)
-    parser_func.add_argument('-s', '--stop', help='Stop word list file. default=data/1000_most_common_words.txt', 
-                             default='data/5000_most_common_words_by_order.txt')
-    parser_func.add_argument('--col', help='Text column. Default - txt', default='txt')
-    parser_func.add_argument('--out', help='Output file name. default - based on input file and k')
-    parser_func.add_argument('--llm', action="store_true",
-                             help='Use LLM methods. default: False')
-    parser_func.add_argument('--plot', action="store_true",
-                             help='Plot semantic distance before and after the anonymization. default: False')
-    parser_func.add_argument('--sample', 
-                             help='Take only the first N rows. For debugging.', type=int)
-    parser_func.add_argument('--wemodel', 
-                             help='Word embedding model.', default='fasttext-wiki-news-subwords-300')
-    parser_func.add_argument('--num_stop', 
-                             help='Number of stop words, ordered by frequency. Must be between 0-5000. default 1000', type=int, default='1000')
-    parser_func.add_argument('--n_jobs',
-                             help='The number of parallel jobs to run. -1 means using all processors. default -1', 
-                             type=int, default=1)
-    parser_func.add_argument('--verbose', type=int, default=0,
-                             help='Prevent the program from displaying screen output. default: 0')
-    parser_func.add_argument('-version', action='version', version='%(prog)s:' + ' %s-%s' % (__version__, __date__))
-    return parser_func
-
-
-def run_from_command_line():
-    """
-    Runs the functions from command line
-    """
-    parser = parse_args()
-    args = parser.parse_args()
-
-    # getting the input arguments
-    input_file = args.file  # Input database
-    k = int(args.k)  # Desired k degree
-    col = args.col  # The text columns  
-
-    # df from csv
-    df = pd.read_csv(input_file)
-    if args.sample:
-        df = df.head(args.sample)
-
-    prefix = get_prefix(args) 
-
-    if not args.llm:
-        df, mean_dist = anonymize(df=df, k=k, col=col, plot=args.plot, num_stop=args.num_stop, wemodel=args.wemodel, n_jobs=args.n_jobs, verbose=args.verbose)
-    else:
-        df, mean_dist = anonymize_llm(df=df, k=k, col=col, plot=args.plot, n_jobs=args.n_jobs, verbose=args.verbose)
-    
-    print('Mean semantic distance:', mean_dist)
-    # Saving
-    if args.out:
-        output_name = args.out
-    else:
-        output_name = f'{prefix}_anonymized.csv'
-    out_file = 'outputs/' + output_name
-    df.to_csv(out_file, index=False)
-    
-
-if __name__ == "__main__":    
-    start_time = time.time()
-    run_from_command_line()
-    print(f'Running time: {round((time.time() - start_time),2)} seconds')
-    
+#!/usr/bin/python3
+
+"""
+K-anonymity for texts
+"""
+
+# Info
+__author__ = 'Lior Trieman and Hadas Neuman'
+__version__ = '1.1'
+__date__ = '1/7/23'
+
+# Imports
+import sys
+import pandas as pd
+import numpy as np
+import re
+import os
+import argparse
+import time
+import warnings
+import logging
+import pkg_resources
+warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
+
+
+def llm_method(df: pd.DataFrame, k: int, col: str = 'txt', plot: bool = False, n_jobs: int = 1, verbose: int = 0):
+    """
+    Uses LLM methods to preform anonymization
+    """
+    from utils import llm_utils, utilization_utils, anonym_utils
+
+    # TEMP
+    prefix = 'temp_prefix_llm'  # TEMP
+    init_logger(verbose)
+    # logging.info('Start LLM pipeline')  # Logging
+    logging.info(f'{os.path.basename(__file__)} {__version__} LLM pipeline')
+
+    # Adding number of characters
+    num_chars_col = 'Num_characters'
+    df[num_chars_col] = df[col].str.len()
+    docs = df[col]
+
+    logging.info(f'Number of documents: {len(docs)}')
+    logging.info(
+        f'Average number of characters in documents: {df[num_chars_col].mean()} maximum characters in a document {df[num_chars_col].max()}')
+
+    # Runing the anonymization
+    annon_docs, _ = llm_utils.run_anonymization_on_txt(docs, k, n_jobs)
+    df['anonymized_text'] = annon_docs
+
+    curr_k, non_anon_indexes = anonym_utils.get_anonym_degree(docs=annon_docs, min_k=k)
+    out_str = f'Anonymity after reduction:{curr_k}  number of un-anonymized documents: {len(non_anon_indexes)}'
+    logging.info(out_str)  # Logging
+
+    # Logging the un-anonymized documents
+    if len(non_anon_indexes) > 0:
+        out_str = f'Un-anonymized documents: {non_anon_indexes}'
+        logging.info(out_str)  # Logging
+
+    # Utilization utils
+    if plot:
+        plot_prefix = prefix
+    else:
+        plot_prefix = None
+    mean_dist = utilization_utils.get_mean_semantice_distance_for_corpus(df[col], df['anonymized_text'],
+                                                                         prefix=plot_prefix)
+    out_str = f'Mean semantic distance before and after the anonymization process: {mean_dist}'
+    logging.info(out_str)  # Logging
+
+    logging.info('Done')  # Logging
+    return df, mean_dist
+
+
+def get_prefix(arguments):
+    """
+    Creates a prefix based on the input file and k.
+    """
+    # Removing extension
+    if arguments.out:
+        file = arguments.out
+    else:
+        file = arguments.file
+
+    _, file_extension = os.path.splitext(file)
+    base_name = os.path.basename(file).replace(file_extension, '')
+    prefix = f'{base_name}_k{arguments.k}_stop_{arguments.num_stop}'
+
+    if arguments.sample:
+         prefix += f'_sample_of_{arguments.sample}'
+    # LLM
+    if arguments.llm:
+        prefix += '_llm'
+    return prefix
+
+
+def init_logger(verbose):
+    """
+    Initiating the logger
+    """
+    # log_name = f'logs/{prefix}.log'
+    logging.basicConfig(
+        level=max(0, 30 - (verbose*10)),
+        format='%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s')
+
+
+def print_size(var, var_name):
+    """
+    Prints the variable size to the log
+    """
+    logging.debug(f'The size of {var_name}: {sys.getsizeof(var)/1000000}MB')
+
+
+def get_data_path():
+    # Credit: https://medium.com/@vuillaut/python-package-and-access-data-in-your-module-d05e72f58785
+    # f1 = pkg_resources.get_resource_filename(__name__, 'data/5000_most_common_words_by_order.txt')
+    relative_file = 'data/5000_most_common_words_by_order.txt'
+    file_name = pkg_resources.resource_filename('kanonym4text', relative_file)
+    return file_name
+
+
+def anonymize(df: pd.DataFrame, k: int, col: str = 'txt', plot: bool = False,
+              wemodel: str = 'fasttext-wiki-news-subwords-300',
+              num_stop: int = 1000, n_jobs: int = 1, verbose: int = 0):
+    """
+    The main function. Runs the anonymization.
+    """
+    init_logger(verbose)
+    logging.info(f'{os.path.basename(__file__)} {__version__} WE pipeline')
+
+    from kanonym4text.utils import nlp_utils, cluster_utils, utilization_utils, anonym_utils, models
+
+    logging.info(f'Word embedding model: {wemodel}')  # Logging
+
+    # Uploading the word embedding model
+    if wemodel == 'glove-twitter-25':  # default model
+        cos = False
+    else:
+        cos = True
+    
+    wemodel = models.upload_we_model(wemodel)
+    if wemodel is None:
+        exit(1) 
+
+    # TEMP
+    prefix = 'temp_prefix' # TEMP
+    
+    logging.info(f'Number of documents: {df.shape[0]}')  # Logging
+
+    # Getting the stopword list
+    short_stopword_list = nlp_utils.stopwords.words('english')
+    stop_file = get_data_path()
+    long_stopword_list = nlp_utils.get_list_from_file(stop_file, num_stop)
+    if long_stopword_list:
+        long_stopword_list = list(set(short_stopword_list + long_stopword_list))
+    else:
+        logging.error(f'Could not read the stop word file.')
+        exit(1)
+
+    out_str = f'Stopword list contains {len(long_stopword_list)} words'
+    logging.info(out_str)  # Logging
+
+    # Creating the word dictionary and word list
+    word_dict = nlp_utils.create_word_dict(df[col], long_stopword_list)
+    # this function takes too long need to make more efficient
+    out_str = f'Number of unique words in dataset: {len(word_dict)}'
+    logging.info(out_str)  # Logging
+
+    # Run clustering
+    cluster_dict, dist_dict, _ = cluster_utils.run_clustering(word_dict,
+                                                              stop_list=long_stopword_list,
+                                                              wemodel=wemodel,
+                                                              cosine=cos, n_jobs=n_jobs)
+    out_str = f'Number of DBSCAN clusters:\t {len(cluster_dict)}'
+    logging.info(out_str)  # Logging
+
+    # Generalization
+    df, _, long_stopword_list = nlp_utils.replace_words_in_df(df, cluster_dict,
+                                                              dist_dict, word_dict,
+                                                              col, wemodel=wemodel,
+                                                              stop_list=long_stopword_list)
+    out_str = f'Generalization completed.'
+    logging.info(out_str)  # Logging
+    
+    # Find k neighbors
+    neighbor_list = anonym_utils.ckmeans_clustering(docs=df['anon_txt'],
+                                                    k=k, n_jobs=n_jobs,
+                                                    stop_list=short_stopword_list)
+
+    out_str = f'Found {len(neighbor_list)} groups of {k} neighbors'
+    logging.info(out_str)  # Logging
+
+    # Reduction
+    force_anon_txt_annoy = anonym_utils.force_anonym(docs=df['anon_txt'], neighbor_list=neighbor_list, stop_list=long_stopword_list)
+
+    # Testing success
+    curr_k, non_anon_indexes = anonym_utils.get_anonym_degree(docs=force_anon_txt_annoy, min_k=k, stop_list=long_stopword_list)
+    out_str = f'Anonymity after reduction:{curr_k}  number of un-anonymized documents: {len(non_anon_indexes)}'
+    logging.info(out_str)  # Logging
+
+    # Logging the un-anonymized documents
+    if len(non_anon_indexes) > 0: 
+        out_str = f'Un-anonymized documents: {non_anon_indexes}'
+        logging.info(out_str)  # Logging
+
+    # Adding the anonymized corpus to the dataframe
+    anonym_col = 'force_anon_txt'
+    df[anonym_col] = force_anon_txt_annoy
+    del(force_anon_txt_annoy)  # Freeing space
+    df = anonym_utils.add_neighbor_list_to_df(df, neighbor_list)
+    # Counting the number of words and *
+    df['num_of_words_after_forcing'] = df['force_anon_txt'].apply(lambda x: len(re.findall(r'\w+', x)))
+    df['num_of_deleting_after_forcing'] = df['force_anon_txt'].apply(lambda x: len(re.findall(r'\*', x)))
+
+    # Utilization utils
+    if plot:
+        plot_prefix = prefix
+    else:
+        plot_prefix = None
+    mean_dist = utilization_utils.get_mean_semantice_distance_for_corpus(df[col], df[anonym_col], prefix=plot_prefix)
+    out_str = f'Mean semantic distance before and after the anonymization process: {mean_dist}'
+    logging.info(out_str)  # Logging
+    
+    logging.info('Done')  # Logging
+    return df, mean_dist
+
+
+def parse_args():
+    """
+    Defines the ArgumentParser
+    :return: The parser
+    """
+    parser_func = argparse.ArgumentParser(description='Converts dot tree to newick tree format')
+    parser_func.add_argument('-f', '--file', help='Input CSV file', required=True)
+
+    parser_func.add_argument('-k', help='The k anonymity degree',  required=True)
+    parser_func.add_argument('-s', '--stop', help='Stop word list file. default=data/1000_most_common_words.txt', 
+                             default='data/5000_most_common_words_by_order.txt')
+    parser_func.add_argument('--col', help='Text column. Default - txt', default='txt')
+    parser_func.add_argument('--out', help='Output file name. default - based on input file and k')
+    parser_func.add_argument('--llm', action="store_true",
+                             help='Use LLM methods. default: False')
+    parser_func.add_argument('--plot', action="store_true",
+                             help='Plot semantic distance before and after the anonymization. default: False')
+    parser_func.add_argument('--sample', 
+                             help='Take only the first N rows. For debugging.', type=int)
+    parser_func.add_argument('--wemodel', 
+                             help='Word embedding model.', default='fasttext-wiki-news-subwords-300')
+    parser_func.add_argument('--num_stop', 
+                             help='Number of stop words, ordered by frequency. Must be between 0-5000. default 1000', type=int, default='1000')
+    parser_func.add_argument('--n_jobs',
+                             help='The number of parallel jobs to run. -1 means using all processors. default -1', 
+                             type=int, default=1)
+    parser_func.add_argument('--verbose', type=int, default=0,
+                             help='Prevent the program from displaying screen output. default: 0')
+    parser_func.add_argument('-version', action='version', version='%(prog)s:' + ' %s-%s' % (__version__, __date__))
+    return parser_func
+
+
+def run_from_command_line():
+    """
+    Runs the functions from command line
+    """
+    parser = parse_args()
+    args = parser.parse_args()
+
+    # getting the input arguments
+    input_file = args.file  # Input database
+    k = int(args.k)  # Desired k degree
+    col = args.col  # The text columns  
+
+    # df from csv
+    df = pd.read_csv(input_file)
+    if args.sample:
+        df = df.head(args.sample)
+
+    prefix = get_prefix(args) 
+
+    if not args.llm:
+        df, mean_dist = anonymize(df=df, k=k, col=col, plot=args.plot, num_stop=args.num_stop, wemodel=args.wemodel, n_jobs=args.n_jobs, verbose=args.verbose)
+
+    print('Mean semantic distance:', mean_dist)
+    # Saving
+    if args.out:
+        output_name = args.out
+    else:
+        output_name = f'{prefix}_anonymized.csv'
+    out_file = 'outputs/' + output_name
+    df.to_csv(out_file, index=False)
+    
+
+if __name__ == "__main__":    
+    start_time = time.time()
+    run_from_command_line()
+    print(f'Running time: {round((time.time() - start_time),2)} seconds')
+
```

### Comparing `kanonym4text-0.1.4/kanonym4text/utils/anonym_utils.py` & `kanonym4text-1.1.5/kanonym4text/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/kanonym4text/utils/cluster_utils.py` & `kanonym4text-1.1.5/kanonym4text/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/kanonym4text/utils/llm_utils.py` & `kanonym4text-1.1.5/kanonym4text/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/kanonym4text/utils/models.py` & `kanonym4text-1.1.5/kanonym4text/utils/models.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/kanonym4text/utils/nlp_utils.py` & `kanonym4text-1.1.5/kanonym4text/utils/nlp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 
 short_stopword_list = None
 long_stopword_list = None
 
 nlp = spacy.load('en_core_web_sm', disable=['ner', 'parser'])  # disabling Named Entity Recognition for speed
 # we_model = models.we_model
 
-def get_list_from_file(file_name, num):
+def get_list_from_file(file_name, num=None):
     """"
     Reads a file with words (each word on different line) and returns a list of these words.
     """
     try:
         with open(file_name, 'r') as file:
             
             # reading the file
             data = file.read()
             
             # replacing end splitting the text 
             # when newline ('\n') is seen.
             word_list = data.split("\n")
 
             # Take only part of the words
-            if (num >= 0) and (num < len(word_list)):
+            if num and (num < len(word_list)):
                 word_list = word_list[:num]
     
     except Exception as e:
         logging.error(f'Could not read the file {file_name}: {e}')
         word_list = None
     return word_list
```

### Comparing `kanonym4text-0.1.4/kanonym4text/utils/utilization_utils.py` & `kanonym4text-1.1.5/kanonym4text/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/kanonym4text.egg-info/SOURCES.txt` & `kanonym4text-1.1.5/kanonym4text.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 kanonym4text/__init__.py
 kanonym4text/k_anonym_text.py
 kanonym4text.egg-info/PKG-INFO
 kanonym4text.egg-info/SOURCES.txt
 kanonym4text.egg-info/dependency_links.txt
```

### Comparing `kanonym4text-0.1.4/setup.py` & `kanonym4text-1.1.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-from setuptools import setup, find_packages
-
-VERSION = '0.1.4'
-DESCRIPTION = 'k-anonymity for texts'
-LONG_DESCRIPTION = 'A package that applies k-anonymity on extual documents.'
-
-# Setting up
-setup(
-    name="kanonym4text",
-    version=VERSION,
-    author="Lior Trieman, Hadas Neuman",
-    author_email="liortr30@gmail.com, hadas.doron@gmail.com",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    # package_dir={'kanonym4text': 'kanonym4text'},
-    install_requires=[
-        'numpy==1.23.0',
-        'pandas==1.5.3',
-        'matplotlib==3.7.1',
-        'gensim==4.3.1',
-        'torch==2.0.1',
-        'transformers==4.29.0',
-        'sentence-transformers==2.2.2',
-        'spacy==3.5.3',
-        'nltk==3.8.1',
-        'annoy==1.17.2',
-        'k-means-constrained==0.7.2'
-    ],
-    keywords=['python', 'k-anonymity', 'privacy', 'NLP'],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ],
-    package_data={
-        'kanonym4text': ['data/5000_most_common_words_by_order.txt']}
-)
-
+from setuptools import setup, find_packages
+
+VERSION = '1.1.5'
+DESCRIPTION = 'k-anonymity for texts'
+LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymize corpus'
+
+# Setting up
+setup(
+    name="kanonym4text",
+    version=VERSION,
+    author="Lior Trieman, Hadas Neuman",
+    author_email="liortr30@gmail.com, hadas.doron@gmail.com",
+    url='https://github.com/neumanh/K-anonymity-fot-texts/tree/build_pack',
+
+    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/1.1.5.tar.gz',
+
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    # package_dir={'kanonym4text': 'kanonym4text'},
+    install_requires=[
+        'numpy==1.23.0',
+        'pandas==1.5.3',
+        'matplotlib==3.7.1',
+        'gensim==4.3.1',
+        'torch==2.0.1',
+        'transformers==4.29.0',
+        'sentence-transformers==2.2.2',
+        'spacy==3.5.3',
+        'nltk==3.8.1',
+        'annoy==1.17.2',
+        'k-means-constrained==0.7.2'
+    ],
+    keywords=['python', 'k-anonymity', 'privacy', 'NLP'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+        'License :: OSI Approved :: MIT License',
+
+    ],
+    package_data={
+        'kanonym4text': ['data/5000_most_common_words_by_order.txt']}
+)
+
```

### Comparing `kanonym4text-0.1.4/utils/anonym_utils.py` & `kanonym4text-1.1.5/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/utils/cluster_utils.py` & `kanonym4text-1.1.5/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/utils/llm_utils.py` & `kanonym4text-1.1.5/utils/llm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for i in indexes:
         print(origina_docs[i])
     print('\nAfter:')
     for i in indexes:
         print(new_docs[i])
 
 
-def sum_text_basic(doc_list, tokenizer, gen_model):
+def sum_text_0(doc_list, tokenizer, gen_model):
     # define the input sentences
     #input_text = '. '.join(doc_list)
     input_text = ''
     for doc in doc_list:
        input_text = f'{input_text}\n- {doc}. ' 
 
     # preprocess the input sentences
@@ -39,15 +39,15 @@
     for doc in doc_list:
        input_text = f'{input_text}{i}: {doc}. ' 
        i += 1
     
     # print('doc_list:', doc_list)
     # preprocess the input sentences
     prompt = prompt_builder(doc_list)
-    input_ids = tokenizer.encode(prompt, return_tensors="pt")
+    input_ids = tokenizer.encode(prompt, return_tensors="pt", show_progress_bar=False)
 
     # generate the summary sentence
     output_ids = gen_model.generate(input_ids=input_ids, max_length=32, num_beams=4, early_stopping=True)
     output = tokenizer.decode(output_ids[0], skip_special_tokens=True)
 
     return output
```

### Comparing `kanonym4text-0.1.4/utils/models.py` & `kanonym4text-1.1.5/utils/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import gensim.downloader as api
 import nltk
 from nltk.sentiment import SentimentIntensityAnalyzer
 import logging
 
-# nltk.download('vader_lexicon', quiet=True)  # download necessary data for sentiment analysis
+# nltk.download('vader_lexicon')  # download necessary data for sentiment analysis
 nltk.download('stopwords', quiet=True)
 nltk.download('punkt', quiet=True)
 
-# # Instantiate sentiment analyzer
-# analyzer = SentimentIntensityAnalyzer()
+# Instantiate sentiment analyzer
+analyzer = SentimentIntensityAnalyzer()
+
 
 def upload_we_model(model_name):
     # From GloVe
     # model_name = 'glove-twitter-25'
 
     possible_models = list(api.info()['models'].keys())
     if model_name not in possible_models:
```

### Comparing `kanonym4text-0.1.4/utils/nlp_utils.py` & `kanonym4text-1.1.5/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.4/utils/utilization_utils.py` & `kanonym4text-1.1.5/utils/utilization_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import numpy as np
 from numpy.linalg import norm
 from sentence_transformers import SentenceTransformer
 import logging
 
 from utils import models
 
+analyzer = models.analyzer
+
 def get_mean_semantice_distance_for_corpus(cor1, cor2, prefix=None):
     """
     Calculates the distance for each pair of documents
     """
     sem_model = SentenceTransformer('sentence-transformers/all-MiniLM-L12-v1')
     cor1_embed = sem_model.encode(cor1, show_progress_bar=False)
     cor2_embed = sem_model.encode(cor2, show_progress_bar=False)
```

