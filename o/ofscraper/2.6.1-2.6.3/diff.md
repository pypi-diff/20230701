# Comparing `tmp/ofscraper-2.6.1.tar.gz` & `tmp/ofscraper-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.6.1.tar", max compression
+gzip compressed data, was "ofscraper-2.6.3.tar", max compression
```

## Comparing `ofscraper-2.6.1.tar` & `ofscraper-2.6.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2023-06-27 15:23:52.029471 ofscraper-2.6.1/LICENSE
--rw-r--r--   0        0        0     2862 2023-06-27 15:23:52.029471 ofscraper-2.6.1/README.md
--rw-r--r--   0        0        0      607 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8281 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/archive.py
--rw-r--r--   0        0        0     4920 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     2859 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     9111 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9871 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5640 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11761 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3909 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3205 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8815 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    14097 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/commands/check.py
--rw-r--r--   0        0        0     4937 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    13452 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6337 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4973 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      696 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7683 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27766 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1139 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    11211 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8950 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10803 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    19529 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3376 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     6442 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9615 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/of.py
--rw-r--r--   0        0        0    11732 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-27 15:23:52.041472 ofscraper-2.6.1/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0    29248 2023-06-27 15:23:52.041472 ofscraper-2.6.1/ofscraper/utils/table.py
--rw-r--r--   0        0        0     6089 2023-06-27 15:23:52.041472 ofscraper-2.6.1/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1696 2023-06-27 15:24:34.413645 ofscraper-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 ofscraper-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-01 17:49:04.668305 ofscraper-2.6.3/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-01 17:49:04.668305 ofscraper-2.6.3/README.md
+-rw-r--r--   0        0        0      607 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8526 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     5019 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2859 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9222 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    10084 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5672 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11976 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3909 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3408 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8918 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    14531 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     4942 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    13717 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6339 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     5037 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      696 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7683 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27832 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1209 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    11211 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8986 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10803 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    20240 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3376 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     6486 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9615 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/of.py
+-rw-r--r--   0        0        0    11732 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0    29248 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/table.py
+-rw-r--r--   0        0        0     5811 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1759 2023-07-01 17:49:35.624240 ofscraper-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 ofscraper-2.6.3/PKG-INFO
```

### Comparing `ofscraper-2.6.1/LICENSE` & `ofscraper-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/README.md` & `ofscraper-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/__init__.py` & `ofscraper-2.6.3/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/__version__.py` & `ofscraper-2.6.3/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/api/archive.py` & `ofscraper-2.6.3/ofscraper/api/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
+import ssl
+import certifi
 import math
 import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
@@ -43,41 +45,41 @@
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
     if timestamp:
-        log.debug(arrow.get(math.trunc(float(timestamp))))
         timestamp=str(timestamp)
         ep = constants.archivedNextEP
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.archivedEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
+        
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:       
+        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:  
             if r.ok:
                 progress.remove_task(task)
                 posts =( await r.json())['list']
                 log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
                 if not posts:
                     posts= []
                 if len(posts)==0:
                     log.debug(f" {log_id} -> number of post found 0")
                 elif len(posts)>0:
                     log.debug(f"{log_id} -> number of archived post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-                    log.debug(f"{log_id} -> first ID {posts[0]['id']}")
-                    log.debug(f"{log_id} -> last ID {posts[-1]['id']}")        
+                    log.debug(f"{log_id} -> found archived post IDs {list(map(lambda x:x.get('id'),posts))}")
+       
                     if required_ids==None:
                         attempt.set(0)
                         tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
                     else:
                         [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
 
 
@@ -151,16 +153,18 @@
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Archived Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
-        cache.set(f"archived_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"archived_{model_id}",list(map(lambda x:{"id":x.get("id"),"postedAtPrecise":x.get("postedAtPrecise")},unduped)),expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"archived_check_{model_id}{model_id}",unduped,expire=constants.CHECK_EXPIRY)
+
         cache.close()
     elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"archived_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
-
+        cache.set(f"archived_check_{model_id}{model_id}",[],expire=constants.CHECK_EXPIRY) 
         cache.close()
         log.debug("Some post where not retrived resetting cache")
 
     return unduped
```

### Comparing `ofscraper-2.6.1/ofscraper/api/highlights.py` & `ofscraper-2.6.3/ofscraper/api/highlights.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import logging
 import contextvars
 import aiohttp
+import ssl
+import certifi
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -69,24 +71,24 @@
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
     headers=auth.make_headers(auth.read_auth())
   
 
     url_stories = constants.highlightsWithStoriesEP.format(user_id)
     url_story = constants.highlightsWithAStoryEP.format(user_id)
-    r_one=await c.request("get",url_story ,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=auth.create_sign(url_story , headers))
-    r_multiple=await c.request("get",url_stories ,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=auth.create_sign(url_stories , headers))
+    r_one=await c.request("get",url_story ,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.create_sign(url_story , headers))
+    r_multiple=await c.request("get",url_stories ,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.create_sign(url_stories , headers))
     
     # highlights_, stories
     sem.release()
     if  r_multiple.ok and r_one.ok:
         attempt.set(0)
-        log.debug(f"[bold]Highlight Post Count without Dupes[/bold] {len(await r_multiple.json())} found")
-        log.debug(f"[bold]Story Post Count without Dupes[/bold] {len(await r_one.json())} found")
         highlights_, stories =get_highlightList(await r_multiple.json()),await r_one.json()
+        log.debug(f"highlights: -> found highlights ids {list(map(lambda x:x.get('id'),highlights_))}")
+        log.debug(f"highlights: -> found stories ids {list(map(lambda x:x.get('id'),stories))}") 
         job_progress.remove_task(task)
 
     else:
         job_progress.remove_task(task)
         r_multiple.raise_for_status()
         r_one.raise_for_status()
     return  highlights_, stories
```

### Comparing `ofscraper-2.6.1/ofscraper/api/init.py` & `ofscraper-2.6.3/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/api/me.py` & `ofscraper-2.6.3/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/api/messages.py` & `ofscraper-2.6.3/ofscraper/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
 import aiohttp
 import logging
+import ssl
+import certifi
 import contextvars
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
@@ -106,15 +108,15 @@
     for message in responseArray:
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
         oldmsgset.discard(message["id"])       
         unduped.append(message)
     if len(oldmsgset)==0 and not (args_.getargs().before or args_.getargs().after):
-        cache.set(f"messages_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"messages_{model_id}",list(map(lambda x:{"id":x.get("id"),"createdAt":x.get("createdAt") or x.get("postedAt") },unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"message_check_{model_id}",oldmessages,expire=constants.CHECK_EXPIRY)
 
         cache.close()
     elif len(oldmsgset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"messages_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
         cache.set(f"message_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
         cache.close()
@@ -132,31 +134,32 @@
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'}{url}")
 
 
     async with sem:
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
             task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
             
             if r.ok:
 
                 messages = (await r.json())['list']
                 log_id=f"offset messageid:{message_id if message_id else 'init id'}"
                 if not messages:
                     messages=[]
                 if len(messages)==0:
                     log.debug(f"{log_id} -> number of messages found 0")
                 elif len(messages)>0:
                     log.debug(f"{log_id} -> number of messages found {len(messages)}")
                     log.debug(f"{log_id} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
-                    log.debug(f"{log_id} -> first ID {messages[0]['id']}")
                     log.debug(f"{log_id} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
-                    log.debug(f"{log_id} -> last ID {messages[-1]['id']}")    
+                    log.debug(f"{log_id} -> found message ids {list(map(lambda x:x.get('id'),messages))}")
+
+
                     if (arrow.get( messages[-1].get("createdAt") or messages[-1].get("postedAt")).float_timestamp<(args_.getargs().after or arrow.get(0)).float_timestamp):
                         attempt.set(0)
                     elif required_ids==None:
                         attempt.set(0)
                         tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'])))
                     else:
                         [required_ids.discard(ele["id"]) for ele in messages]
```

### Comparing `ofscraper-2.6.1/ofscraper/api/paid.py` & `ofscraper-2.6.3/ofscraper/api/paid.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
+import ssl
+import certifi
 import aiohttp
 import logging
 import contextvars
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
@@ -94,22 +96,23 @@
     media = None
     attempt.set(attempt.get(0) + 1)
     url = constants.purchased_contentEP.format(offset,username)
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
     headers=auth.make_headers(auth.read_auth())
     headers=auth.create_sign(url, headers)
-    async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+    async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
         sem.release()
         if r.ok:
             data=await r.json()
             attempt.set(0)
             media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
             log.debug(f"offset:{offset} -> media found {len(media)}")
             log.debug(f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }")
+            log.debug(f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
             if  data.get("hasMore"):
                 offset += len(media)
                 tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress,offset=offset)))
             job_progress.remove_task(task)
 
         else:
             log.debug(f"[bold]paid request status code:[/bold]{r.status}")
@@ -169,15 +172,15 @@
     log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
     for post in output:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Paid Post count[/bold] {len(unduped)} found")
-    cache.set(f"purchased_all",output,expire=constants.RESPONSE_EXPIRY)
+    cache.set(f"purchased_all",list(map(lambda x:x.get("id"),unduped)),expire=constants.RESPONSE_EXPIRY)
     cache.close()
     return unduped
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_all_paid(c,job_progress,offset=0,count=0,required=0):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
@@ -187,15 +190,15 @@
     media = None
     attempt.set(attempt.get(0) + 1)
     await sem.acquire()
     url = constants.purchased_contentALL.format(offset)
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} offset={offset}",visible=True)
     headers=auth.make_headers(auth.read_auth())
     headers=auth.create_sign(url, headers)
-    async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+    async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
         sem.release()
         if r.ok:
             attempt.set(0) 
             log_id=f"offset {offset or 0}:"
             data=await r.json()   
             job_progress.remove_task(task)
             media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
@@ -205,16 +208,16 @@
                 media=[]
             if len(media)==0:
                 log.debug(f"{log_id} -> number of post found 0")
             elif len(media)>0:
                 log.debug(f"{log_id} -> number of post found {len(media)}")
                 log.debug(f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}")
                 log.debug(f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}")
-                log.debug(f"{log_id} -> first ID {media[0]['id']}")
-                log.debug(f"{log_id} -> last ID {media[-1]['id']}")
+                log.debug(f"{log_id} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
+
                 if required==0:
                     attempt.set(0)
                     tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media))))
 
                 elif len(count)<len(required):
                     tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media),required=required,count=count+len(media))))
```

### Comparing `ofscraper-2.6.1/ofscraper/api/pinned.py` & `ofscraper-2.6.3/ofscraper/api/pinned.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
+import ssl
+import certifi
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
 import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
@@ -51,29 +53,30 @@
         ep=constants.timelinePinnedEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:         
+        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:         
             if r.ok:
                 progress.remove_task(task)
                 posts =( await r.json())['list']
                 log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
                 if not posts:
                     posts= []
                 if len(posts)==0:
                     log.debug(f"{log_id} -> number of pinned post f found 0")
                 else:
                     log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-                    log.debug(f"{log_id} -> first ID {posts[0]['id']}")
-                    log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
+                    log.debug(f"{log_id} -> found pinned post IDs {list(map(lambda x:x.get('id'),posts))}")
+
+  
                 #post infinite loops            
                 # elif required_ids==None:
                 #     attempt.set(0)
                     # tasks.append(asyncio.create_task(scrape_pinned_posts(headers, model_id,progress,timestamp=posts[0]['postedAtPrecise'])))
             else:
                     log.debug(f"[bold]pinned request status code:[/bold]{r.status}")
                     log.debug(f"[bold]pinned response:[/bold] {await r.text()}")
```

### Comparing `ofscraper-2.6.1/ofscraper/api/posts.py` & `ofscraper-2.6.3/ofscraper/api/posts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 import logging
 import aiohttp
 import arrow
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_result
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
 import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
 import ofscraper.constants as constants
 import ofscraper.utils.config as config
 
 
+
 log=logging.getLogger(__package__)
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None):
         self._post = post
         self._model_id = int(model_id)
         self._username = username
@@ -59,15 +61,15 @@
     def responsetype_(self):
         return self._responsetype_
 
     @property
     def responsetype(self):
         if self.archived:
             if config.get_archived_responsetype(config.read_config()) == "":
-                return "achived"
+                return "archived"
             return config.get_archived_responsetype(config.read_config())
 
         else:
             response=config.read_config().get("responsetype", {}).get(self._responsetype_) 
             if  response == "":
                 return self._responsetype_.capitalize()
             elif  response == None:
@@ -362,27 +364,30 @@
     def linked(self):
         return None
 
     @property
     def media(self):
         return self._media
     @property
+    @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
     async def parse_mpd(self): 
         if not self.mpd:
             return
       
         params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
                                     sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as session:
             headers=auth.make_headers(auth.read_auth())
             headers=auth.create_sign(self.mpd, headers) 
             async with session.request("get",self.mpd,headers=headers,params=params) as r:
                 if not r.ok:
                     return None
                 return MPEGDASHParser.parse(await r.text())
+ 
+    
     @property
     def license(self):
         if not self.mpd:
             return None
         responsetype=self.post.post["responseType"]
         if responsetype in ["timeline","archived","pinned"]:
             responsetype="post"
```

### Comparing `ofscraper-2.6.1/ofscraper/api/profile.py` & `ofscraper-2.6.3/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/api/subscriptions.py` & `ofscraper-2.6.3/ofscraper/api/subscriptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 from itertools import chain
+import ssl
+import certifi
 import logging
 import aiohttp
 from rich.console import Console
 import arrow
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import subscriptionsEP,NUM_TRIES
@@ -31,17 +33,18 @@
 
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_subscriptions(headers, offset=0) -> list:
     async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,sock_connect=None, sock_read=None)) as c: 
         url = subscriptionsEP.format(offset)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
             if r.ok:
                 subscriptions = await r.json()
+                log.debug(f"usernames offset {offset}: usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}")      
                 return subscriptions
             r.raise_for_status()
 
 def parse_subscriptions(subscriptions: list) -> list:
     datenow=arrow.now()
     data = [
         {"name":profile['username']
```

### Comparing `ofscraper-2.6.1/ofscraper/api/timeline.py` & `ofscraper-2.6.3/ofscraper/api/timeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
 import logging
+import ssl
+import certifi
 import contextvars
 import math
 import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
@@ -54,31 +56,31 @@
         ep=constants.timelineEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
             if r.ok:
                 progress.remove_task(task)
                 posts = (await r.json())['list']
                 log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
                 if not posts:
                     posts= []
                 if len(posts)==0:
                     log.debug(f"{log_id} -> number of post found 0")
 
 
                 elif len(posts)>0:
                     log.debug(f"{log_id} -> number of post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-                    log.debug(f"{log_id} -> first ID {posts[0]['id']}")
-                    log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
+
+                    log.debug(f"{log_id} -> found postids {list(map(lambda x:x.get('id'),posts))}")
 
                     if required_ids==None:
                         attempt.set(0)
                         tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
                     else:
                         [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
                         #try once more to get id if only 1 left
@@ -153,15 +155,15 @@
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
-        cache.set(f"timeline_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"timeline_{model_id}",list(map(lambda x:{"id":x.get("id"),"postedAtPrecise":x.get("postedAtPrecise")},unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"timeline_check_{model_id}",unduped,expire=constants.CHECK_EXPIRY)
         cache.close()
     elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
         cache.set(f"timeline_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
 
         cache.close()
```

### Comparing `ofscraper-2.6.1/ofscraper/commands/check.py` & `ofscraper-2.6.3/ofscraper/commands/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,30 +109,43 @@
                 log.info(f"Getting Full Timeline for {user_name}")
                 model_id = profile.get_id( user_name)
             elif name_match2:
                 user_name = name_match2.group(0)
                 model_id = profile.get_id( user_name)
             else:
                 continue
+            if user_dict.get(user_name):
+                continue
         
             oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
+            user_dict[user_name] = {}
+            user_dict[user_name] = user_dict[user_name] or []
             if len(oldtimeline) > 0 and not args.force:
-                user_dict[user_name] = oldtimeline
-            elif not user_dict.get(user_name):
+                user_dict[user_name].extend(oldtimeline)
+            else:
                 user_dict[user_name] = {}
                 user_dict[user_name] = user_dict[user_name] or []
-                user_dict[user_name].extend(asyncio.run(
-                    timeline.get_timeline_post( model_id)))
-                user_dict[user_name].extend(asyncio.run(
-                    pinned.get_pinned_post( model_id)))
-                user_dict[user_name].extend(asyncio.run(
-                    archive.get_archived_post( model_id)))
+                data=asyncio.run(
+                    timeline.get_timeline_post( model_id))
+                user_dict[user_name].extend(data)
+                cache.set(
+                    f"timeline_check_{model_id}", data, expire=constants.CHECK_EXPIRY)
+                cache.close()
+            
+            oldarchive = cache.get(f"archived_check_{model_id}", default=[])
+            if len( oldarchive) > 0 and not args.force:
+                user_dict[user_name].extend(oldarchive)
+            else:
+                data=asyncio.run(
+                    archive.get_archived_post( model_id))
+                user_dict[user_name].extend(data)
                 cache.set(
-                    f"timeline_check_{model_id}", user_dict[user_name], expire=constants.CHECK_EXPIRY)
+                    f"archived_check_{model_id}", data, expire=constants.CHECK_EXPIRY)
                 cache.close()
+            
                 
 
         # individual links
         for ele in list(filter(lambda x: re.search(f"onlyfans.com/{constants.NUMBER_REGEX}+/{constants.USERNAME_REGEX}+$", x), links)):
             name_match = re.search(f"/({constants.USERNAME_REGEX}+$)", ele)
             num_match = re.search(f"/({constants.NUMBER_REGEX}+)", ele)
             if name_match and num_match:
@@ -196,15 +209,15 @@
         oldmessages = cache.get(f"message_check_{model_id}", default=[])
         log.debug(f"Number of messages in cache {len(oldmessages)}")
         
         if len(oldmessages) > 0 and not args.force:
             messages = oldmessages
         else:
             messages = asyncio.run(
-                messages_.get_messages(headers,  model_id))
+                messages_.get_messages( model_id))
             cache.set(f"message_check_{model_id}",
                         messages, expire=constants.CHECK_EXPIRY)
         oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
         paid = None
         # paid content
         if len(oldpaid) > 0 and not args.force:
             paid = oldpaid
```

### Comparing `ofscraper-2.6.1/ofscraper/commands/manual.py` & `ofscraper-2.6.3/ofscraper/commands/manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     media_dict=get_media_from_urls(urls)
     log.debug(f"Media dict length {len(list(media_dict.values()))}")
     for value in media_dict.values():
         if len(value)==0:
             continue
         model_id =value[0].post.model_id
         username=value[0].post.username
-        log.info(f"Downloading individual for {username}")
+        log.info(f"Downloading individual media for{username}")
         operations.create_tables(model_id,username)
         operations.write_profile_table(model_id,username)
         asyncio.run(download.process_dicts(
         username,
         model_id,
         value,
         ))
```

### Comparing `ofscraper-2.6.1/ofscraper/commands/scraper.py` & `ofscraper-2.6.3/ofscraper/commands/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,29 @@
         args.posts=[]
         result_main_prompt = prompts.main_prompt()
      
         #download
         if result_main_prompt == 0:
             check_auth()
             check_config()
-            process_post()     
+            run(process_post)
+
 
         # like a user's posts
         elif result_main_prompt == 1:
-            check_auth()
-            process_like()
+            check_auth()  
+            check_config()
+            run(process_like)
+
         # Unlike a user's posts
         elif result_main_prompt == 2:
-            check_auth()
-            process_unlike()
+            check_auth()  
+            check_config()
+            run(process_unlike)
+
         
         elif result_main_prompt == 3:
             # Edit `auth.json` file
             auth.edit_auth()
         
         elif result_main_prompt == 4:
             # Edit `config.json` file
@@ -121,15 +126,15 @@
 def process_post_user_first():
      with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         if args.users_first:
             output=[]
-            userdata=userselector.getselected_usernames()
+            userdata=userselector.getselected_usernames(rescan=False)
             length=len(userdata)
             for count,ele in enumerate(userdata):
                 log.debug(f"getting content for {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id( ele["name"])
@@ -154,19 +159,19 @@
                 value,
                 ))  
 def normal_post_process():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=userselector.getselected_usernames() if "None" not in args.posts else []
+        userdata=userselector.getselected_usernames(rescan=False)
         length=len(userdata)
         for count,ele in enumerate(userdata):
-            log.debug(f"Getting content+downloading {count+1}/{length} model")
             if args.posts:
+                log.info(f"Progress {count+1}/{length} model")
                 log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
             try:
                 model_id = profile.get_id( ele["name"])
                 operations.create_tables(model_id,ele['name'])
                 operations.write_profile_table(model_id,ele['name'])
                 combined_urls=OF.process_areas( ele, model_id)
                 asyncio.run(download.process_dicts(
@@ -198,15 +203,15 @@
             
 
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=userselector.getselected_usernames()
+        userdata=userselector.getselected_usernames(rescan=False)
         with stdout.lowstdout():
             for ele in list(filter(lambda x: x["active"],userdata)):
                     model_id = profile.get_id( ele["name"])
                     posts = like.get_posts(model_id)
                     unfavorited_posts = like.filter_for_unfavorited(posts)  
                     unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)   
                     log.debug(f"[bold]Number of unliked posts left after date filters[/bold] {len(unfavorited_posts)}")
@@ -215,15 +220,15 @@
                     like.like( model_id, ele["name"], post_ids)
 
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=userselector.getselected_usernames()
+        userdata=userselector.getselected_usernames(rescan=False)
         with stdout.lowstdout():
             for ele in list(filter(lambda x: x["active"],userdata)):
                     model_id = profile.get_id( ele["name"])
                     posts = like.get_posts( model_id)
                     favorited_posts = like.filter_for_favorited(posts)
                     favorited_posts=filters.timeline_array_filter(favorited_posts) 
                     log.debug(f"[bold]Number of liked posts left after date filters[/bold] {len(favorited_posts)}")
@@ -239,37 +244,42 @@
 
 
 
 ## run script once or on schedule based on args
 def run(*functs):
     # get usernames prior to potentially supressing output
     check_auth()
-    userselector.getselected_usernames()
-   
     if args.output=="PROMPT":
         log.info(f"[bold]silent-mode on[/bold]")    
     if args.daemon:
         log.info(f"[bold]daemon mode on[/bold]")   
     run_helper(*functs)
 
 
 def run_helper(*functs):
     # run each function once
-    [funct() for funct in functs]    
-    if args.daemon:
-        global jobqueue
-        jobqueue=queue.Queue()
+    global jobqueue
+    jobqueue=queue.Queue()
+    [jobqueue.put(funct) for funct in functs]
+    if args.daemon:   
         worker_thread = threading.Thread(target=set_schedule,args=[*functs])
         worker_thread.start()
         # Check if jobqueue has function
         while True:
+            log.debug(schedule.jobs)
             job_func = jobqueue.get()
             job_func()
             jobqueue.task_done()
-            log.debug(schedule.jobs)
+            userselector.getselected_usernames(rescan=True)
+            
+            #update selected user
+    else:
+        userselector.getselected_usernames(rescan=True,reset=True)
+        [(jobqueue.get())() for funct in functs]
+            
                 
 def check_auth():
     status=None
     while status!="UP":
         headers = auth.make_headers(auth.read_auth())
         status=init.getstatus(headers)
         if status=="DOWN":
```

### Comparing `ofscraper-2.6.1/ofscraper/constants.py` & `ofscraper-2.6.3/ofscraper/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,16 @@
             "paid":"Messages",
             "stories":"Stories",
             "highlights":"Stories",
             "profile":"Profile",
             "pinned":"Posts"
         }
 NUM_TRIES=10
+
+
 RESPONSE_EXPIRY=5000000
 CHECK_EXPIRY=86400
 DAILY_EXPIRY=86400
 HOURLY_EXPIRY=3600
 DISCORDWAIT=5
 OF_MIN=15
 OF_MAX=50
```

### Comparing `ofscraper-2.6.1/ofscraper/db/operations.py` & `ofscraper-2.6.3/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/db/queries.py` & `ofscraper-2.6.3/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/interaction/like.py` & `ofscraper-2.6.3/ofscraper/interaction/like.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import random
 import time
 import logging
+import ssl
+import certifi
 from typing import Union
 import asyncio
 import aiohttp
 
 from tenacity import retry,stop_after_attempt,wait_random
 
 from rich.progress import Progress
@@ -123,15 +125,15 @@
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def _like_request(c,id,model_id):
     async with sem:
         url = favoriteEP.format(id, model_id)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("post",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.request("post",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
             if r.ok:
                 return id                  
             log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
             log.debug(f"[bold]timeline response:[/bold] {await r.text()}")
             log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
             r.raise_for_status()
```

### Comparing `ofscraper-2.6.1/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.6.3/ofscraper/prompts/prompt_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Press enter when done"
 """
 FUZZY_INSTRUCTION=\
 """
 KeyBindings
 Toggle all: Ctrl+r
 Toggle single: Shift +Right /Home +Right / pageDown +Right
-Ctrl-Z: Change Sorting/Filters (keeps selections)
+Ctrl+Z: Change Sorting/Filters (keeps selections)
 
 Press Enter When Done
 Parantheses indicates number of selected user
 [Sort-Type: {sort}] [Descending: {desc}] [Account-Type {type}] [Subscription Status {status}] [Renewal {renewal}]
 """
 
 SCRAPE_PAID=\
```

### Comparing `ofscraper-2.6.1/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.6.3/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/prompts/prompts.py` & `ofscraper-2.6.3/ofscraper/prompts/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,19 +181,20 @@
 
     if pythonver<3.9 or pythonver>=3.11:
         console.print("\nNote: Browser Extractions only works with default browser profile\n\n")
         questions = [
             {
                 'type': 'list',
                 'message':msg ,
-                'choices':["Enter Each Field Manually","Paste From Cookie Helper", Separator(line="-----------\nBrowser Extractions"),"Chrome","Chromium","Firefox","Opera","Opera GX","Edge","Chromium","Brave","Vivaldi","Safari"],
+                'choices':["Enter Each Field Manually","Paste From M-rcus\' OnlyFans-Cookie-Helper", Separator(line="-----------\nBrowser Extractions"),"Chrome","Chromium","Firefox","Opera","Opera GX","Edge","Chromium","Brave","Vivaldi","Safari"],
                 "default":"Enter Each Field Manually",
 
             }
         ]
+        
 
     else:
         console.print("\nNote:To enable automatic extraction install ofscraper with python 3.9 or 3.10\n\n")
         msg="Select how to retrive auth information"
         questions = [
         {
             'type': 'list',
@@ -580,15 +581,15 @@
     return answers
 def reset_username_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
-            'message': "Do you want to reset username option",
+            'message': "Do you want to reset username selection",
             'choices':["Yes","No"]
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 def mp4_prompt(config_):
@@ -731,15 +732,15 @@
                                 
                         }
                             
     
     )
         
     answers=p.execute()
-    return answers,p
+    return list(map(lambda x:x["name"],answers or [])),p
         
 
 def model_selectorHelper(count,x):
     format='YYYY-MM-DD'
     expired=arrow.get(x['expired']).format(format) if x['expired'] else None
     renewed=arrow.get(x['renewed']).format(format)  if x['renewed'] else None
     subscribed=arrow.get(x['subscribed']).format(format)  if x['subscribed'] else None
```

### Comparing `ofscraper-2.6.1/ofscraper/utils/args.py` & `ofscraper-2.6.3/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/auth.py` & `ofscraper-2.6.3/ofscraper/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,27 +95,27 @@
                 'x-bc': ''
             }
         }
 
     browserSelect=browser_prompt()
 
     auth= auth or defaultAuth
-    if  browserSelect!="Enter Each Field Manually" and browserSelect!="Paste From Cookie Helper":
+    if  browserSelect!="Enter Each Field Manually" and browserSelect!="Paste From M-rcus\' OnlyFans-Cookie-Helper":
         temp=requests.utils.dict_from_cookiejar(getattr(browser_cookie3, browserSelect.lower())(domain_name="onlyfans"))
         auth=auth or  defaultAuth
         for key in ["sess","auth_id","auth_uid_"]:
             auth["auth"][key]=temp.get(key,"")
         console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",style="yellow")
         if not auth["auth"].get("x-bc"):
             auth["auth"]["x-bc"]=xbc_prompt()
         auth["auth"]["user_agent"]= user_agent_prompt(auth["auth"].get("user_agent") or "")
 
 
  
-    elif browserSelect=="Paste From Cookie Helper":
+    elif browserSelect=="Paste From M-rcus\' OnlyFans-Cookie-Helper":
         auth=auth_full_paste()
         auth["auth"]["app-token"]="33d57ade8c02dbc5a333db99ff9ae26a"
         for key in ["username","support_2fa","active","email","password","hashed"]:
             auth["auth"].pop(key)
         auth["auth"]["x-bc"]=auth["auth"].pop("x_bc")
         tempCookie=auth["auth"].pop("cookie")
         for ele in tempCookie.split(";"):
```

### Comparing `ofscraper-2.6.1/ofscraper/utils/binaries.py` & `ofscraper-2.6.3/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/config.py` & `ofscraper-2.6.3/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/dates.py` & `ofscraper-2.6.3/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/download.py` & `ofscraper-2.6.3/ofscraper/utils/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 import asyncio
 import math
 import pathlib
 from random import randint
 import platform
 import shutil
+import ssl
+import certifi
 import traceback
 import re
 import logging
 import aiohttp
 import contextvars
 import json
 import subprocess
@@ -129,15 +131,14 @@
                                         p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
         overall_progress.remove_task(task1)
     log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
     return photo_count+video_count+audio_count,skipped
 def retry_required(value):
     return value == ('skipped', 1)
 
-@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def download(c,ele,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)  
     try:
             with paths.set_directory(paths.getmediadir(ele,username,model_id)):
                 if ele.url:
                     return await main_download_helper(c,ele,pathlib.Path(".").absolute(),file_size_limit,username,model_id,progress)
                 elif ele.mpd:
@@ -145,41 +146,23 @@
                 else:
                     return None
     except Exception as e:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
 async def main_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
-    url=ele.url
     path_to_file=None
     async with sem:
-            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
             log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
-            async with c.request("get",url,allow_redirects=True,verify_ssl=False,cookies=None) as r:
-                if r.ok:
-                    rheaders=r.headers
-                    total = int(rheaders['Content-Length'])
-                    if file_size_limit>0 and total > int(file_size_limit): 
-                            return 'skipped', 1       
-                    content_type = rheaders.get("content-type").split('/')[-1]
-                    filename=paths.createfilename(ele,username,model_id,content_type)
-                    path_to_file = paths.truncate(pathlib.Path(path,f"{filename}"))                 
-                    pathstr=str(path_to_file)
-                    temp=paths.truncate(f"{path_to_file}.part")
-                    pathlib.Path(temp).unlink(missing_ok=True)
-                    task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
-                    with open(temp, 'wb') as f:                           
-                        progress.update(task1,visible=True )
-                        async for chunk in r.content.iter_chunked(1024):
-                            f.write(chunk)
-                            progress.update(task1, advance=len(chunk))
-                        progress.remove_task(task1) 
+            total ,temp,path_to_file=await main_download_downloader(c,ele,path,file_size_limit,username,model_id,progress)
+            if int(file_size_limit)>0 and total > int(file_size_limit): 
+                return "skipped",1
+
     
-                else:
-                    r.raise_for_status()
+
     if not pathlib.Path(temp).exists():
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {temp} was not created") 
         return "skipped",1
     elif abs(total-pathlib.Path(temp).absolute().stat().st_size)>500:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         return "skipped",1 
     else:
@@ -193,81 +176,63 @@
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
             operations.write_media_table(ele,path_to_file,model_id,username)
         set_cache_helper(ele)
         return ele.mediatype,total
 
+async def main_download_downloader(c,ele,path,file_size_limit,username,model_id,progress):
+    url=ele.url
+    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
+    async with c.request("get",url,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=None) as r:
+            if r.ok:
+                rheaders=r.headers
+                total = int(rheaders['Content-Length'])
+                if file_size_limit>0 and total > int(file_size_limit): 
+                        return total ,None,None    
+                content_type = rheaders.get("content-type").split('/')[-1]
+                filename=paths.createfilename(ele,username,model_id,content_type)
+                path_to_file = paths.truncate(pathlib.Path(path,f"{filename}"))                 
+                pathstr=str(path_to_file)
+                temp=paths.truncate(f"{path_to_file}.part")
+                pathlib.Path(temp).unlink(missing_ok=True)
+                task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
+                with open(temp, 'wb') as f:                           
+                    progress.update(task1,visible=True )
+                    async for chunk in r.content.iter_chunked(1024):
+                        f.write(chunk)
+                        progress.update(task1, advance=len(chunk))
+                    progress.remove_task(task1)  
+                return total ,temp,path_to_file
+            else:
+                r.raise_for_status()  
+
+
+
+
 async def alt_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
     async with sem:
         log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {ele.mpd}")
-        video = None
-        audio = None
-        base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
-        mpd=await ele.parse_mpd
         path_to_file = paths.truncate(pathlib.Path(path,f'{paths.createfilename(ele,username,model_id,"mp4")}'))
         temp_path=paths.truncate(pathlib.Path(path,f"temp_{ele.id or ele.filename_}_{randint(100,999)}.mp4"))
-        for period in mpd.periods:
-            for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
-                kId=None
-                for prot in adapt_set.content_protections:
-                    if prot.value==None:
-                        kId = prot.pssh[0].pssh 
-                        break
-                maxquality=max(map(lambda x:x.height,adapt_set.representations))
-                for repr in adapt_set.representations:
-                    name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
-                    if repr.height==maxquality:
-                        video={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video","name":name}
-                        break
-            for adapt_set in filter(lambda x:x.mime_type=="audio/mp4",period.adaptation_sets):             
-                kId=None
-                name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
-                for prot in adapt_set.content_protections:
-                    if prot.value==None:
-                        kId = prot.pssh[0].pssh 
-                        logger.updateSenstiveDict(kId,"pssh_code")
-                        break
-                for repr in adapt_set.representations:
-                    name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
-                    audio={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio","name":name}
-                    break
-            for item in [audio,video]:
-                url=f"{base_url}{item['origname']}"
-                log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
-                params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
-                async with c.request("get",url,params=params,allow_redirects=True,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=auth.make_headers(auth.read_auth())) as r:
-                    if r.ok:
-                        rheaders=r.headers
-                        total = int(rheaders['Content-Length'])
-                        item["total"]=total
-                        if file_size_limit>0 and total > int(file_size_limit): 
-                                return 'skipped', 1       
-                        temp= paths.truncate(pathlib.Path(path,f"{item['name']}.part"))
-                        temp.unlink(missing_ok=True)
-                        item["path"]=temp
-                        pathstr=str(temp)
-                        task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
-                        with open(temp, 'wb') as f:                           
-                            progress.update(task1,visible=True )
-                            async for chunk in r.content.iter_chunked(1024):
-                                f.write(chunk)
-                                progress.update(task1, advance=len(chunk))
-                            progress.remove_task(task1) 
-                    else:
-                        r.raise_for_status()
-    log.debug(f"Media:{ele.id} Post:{ele.postid} video name:{video['name']}")
-    log.debug(f"Media:{ele.id} Post:{ele.postid} audio name:{audio['name']}")
+        audio,video=await alt_download_preparer(ele)
+        audio=await alt_download_downloader(audio,c,ele,path,file_size_limit,progress)
+        if file_size_limit>0 and int(audio["total"]) > int(file_size_limit): 
+            return 'skipped', 1
+        video=await alt_download_downloader(video,c,ele,path,file_size_limit,progress)
+        if int(file_size_limit)>0 and int(video["total"]) > int(file_size_limit): 
+            return 'skipped', 1       
+          
     for item in [audio,video]:
         if not pathlib.Path(item["path"]).exists():
                 log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['path']} was not created") 
                 return "skipped",1
         elif abs(item["total"]-pathlib.Path(item['path']).absolute().stat().st_size)>500:
-            log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {total} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
+            log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {item['total']} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
             return "skipped",1 
                 
     for item in [audio,video]:
         key=await key_helper(c,item["pssh"],ele.license,ele.id)
         if key==None:
             log.debug(f"Media:{ele.id} Post:{ele.postid} Could not get key")
             return "skipped",1 
@@ -299,17 +264,75 @@
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
         log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
         operations.write_media_table(ele,path_to_file,model_id,username)
-    set_cache_helper(ele)
-    return ele.mediatype,total
+    return ele.mediatype,audio["total"]+video["total"]
+
+async def alt_download_preparer(ele):
+    mpd=await ele.parse_mpd
+    for period in mpd.periods:
+                for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
+                    kId=None
+                    for prot in adapt_set.content_protections:
+                        if prot.value==None:
+                            kId = prot.pssh[0].pssh 
+                            break
+                    maxquality=max(map(lambda x:x.height,adapt_set.representations))
+                    for repr in adapt_set.representations:
+                        name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
+                        if repr.height==maxquality:
+                            video={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video","name":name}
+                            break
+                for adapt_set in filter(lambda x:x.mime_type=="audio/mp4",period.adaptation_sets):             
+                    kId=None
+                    name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
+                    for prot in adapt_set.content_protections:
+                        if prot.value==None:
+                            kId = prot.pssh[0].pssh 
+                            logger.updateSenstiveDict(kId,"pssh_code")
+                            break
+                    for repr in adapt_set.representations:
+                        name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
+                        audio={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio","name":name}
+                        break
+    return audio,video
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
+async def alt_download_downloader(item,c,ele,path,file_size_limit,progress):
+    base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
+    url=f"{base_url}{item['origname']}"
+    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
+    params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
+    async with c.request("get",url,params=params,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.make_headers(auth.read_auth())) as r:
+        if r.ok:
+            rheaders=r.headers
+            total = int(rheaders['Content-Length'])
+            item["total"]=total
+            temp= paths.truncate(pathlib.Path(path,f"{item['name']}.part"))
+            temp.unlink(missing_ok=True)
+            item["path"]=temp
+            if file_size_limit>0 and total > int(file_size_limit): 
+                    return  item
+            pathstr=str(temp)
+            task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
+            with open(temp, 'wb') as f:                           
+                progress.update(task1,visible=True )
+                async for chunk in r.content.iter_chunked(1024):
+                    f.write(chunk)
+                    progress.update(task1, advance=len(chunk))
+                progress.remove_task(task1)
+            return item
+        else:
+            r.raise_for_status()
+
+
 
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def key_helper(c,pssh,licence_url,id):
     out=cache.get(licence_url)
     log.debug(f"ID:{id} pssh: {pssh!=None}")
     log.debug(f"ID:{id} licence: {licence_url}")
     if not out:
         headers=auth.make_headers(auth.read_auth())
         headers["cookie"]=auth.get_cookies()
@@ -322,15 +345,15 @@
             'proxy': '',
             'cache': True,
         }
 
 
                  
 
-        async with c.request("post",'https://cdrm-project.com/wv',json=json_data,verify_ssl=False,allow_redirects=True,cookies=None) as r:
+        async with c.request("post",'https://cdrm-project.com/wv',json=json_data,ssl=ssl.create_default_context(cafile=certifi.where()),allow_redirects=True,cookies=None) as r:
             httpcontent=await r.text()
             log.debug(f"ID:{id} key_response: {httpcontent}")
             soup = BeautifulSoup(httpcontent, 'html.parser')
             out=soup.find("li").contents[0]
             cache.set(licence_url,out, expire=2592000)
             cache.close()
     return out
```

### Comparing `ofscraper-2.6.1/ofscraper/utils/encoding.py` & `ofscraper-2.6.3/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/exit.py` & `ofscraper-2.6.3/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/filters.py` & `ofscraper-2.6.3/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/logger.py` & `ofscraper-2.6.3/ofscraper/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,29 +152,30 @@
             "PROMPT":"CRITICAL",
             "STATS":"ERROR",
             "LOW":"WARNING",
             "NORMAL":"INFO",
             "DEBUG":"DEBUG"}.get(input,100)
 
 def init_logger(log):
+    format=' \[%(module)s.%(funcName)s:%(lineno)d]  %(message)s'
     log.setLevel(1)
     addtrackback()
     # # #log file
       # #discord
     cord=DiscordHandler()
     cord.setLevel(getLevel(args.getargs().discord))
     cord.setFormatter(SensitiveFormatter('%(message)s'))
     #console
     sh=RichHandler(rich_tracebacks=True,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False,console=console.shared_console)
     sh.setLevel(getLevel(args.getargs().output))
-    sh.setFormatter(SensitiveFormatter('%(message)s'))
+    sh.setFormatter(SensitiveFormatter(format))
     sh.addFilter(NoDebug())
     tx=TextHandler()
     tx.setLevel(getLevel(args.getargs().output))
-    tx.setFormatter(SensitiveFormatter('%(message)s'))
+    tx.setFormatter(SensitiveFormatter(format))
     log.addHandler(cord)
     log.addHandler(sh)
     log.addHandler(tx)
     if args.getargs().log!="OFF":
         stream=open(paths.getlogpath(), encoding='utf-8',mode="a",)
         fh=logging.StreamHandler(stream)
         fh.setLevel(getLevel(args.getargs().log))
@@ -182,15 +183,15 @@
         fh.addFilter(NoDebug())
         log.addHandler(fh)
 
     
     if args.getargs().output=="DEBUG":
         sh2=RichHandler(rich_tracebacks=True, console=console.shared_console,markup=True,tracebacks_show_locals=True,show_time=False)
         sh2.setLevel(args.getargs().output)
-        sh2.setFormatter(SensitiveFormatter('%(message)s'))
+        sh2.setFormatter(SensitiveFormatter(format))
         sh2.addFilter(DebugOnly())
         log.addHandler(sh2)
     if args.getargs().log=="DEBUG":
         fh2=logging.StreamHandler(stream)
         fh2.setLevel(getLevel(args.getargs().log))
         fh2.setFormatter(LogFileFormatter('%(asctime)s - %(levelname)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
         fh2.addFilter(DebugOnly())
```

### Comparing `ofscraper-2.6.1/ofscraper/utils/of.py` & `ofscraper-2.6.3/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/paths.py` & `ofscraper-2.6.3/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/profiles.py` & `ofscraper-2.6.3/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/separate.py` & `ofscraper-2.6.3/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/stdout.py` & `ofscraper-2.6.3/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/table.py` & `ofscraper-2.6.3/ofscraper/utils/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.1/ofscraper/utils/userselector.py` & `ofscraper-2.6.3/ofscraper/utils/userselector.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,64 +14,57 @@
 import ofscraper.api.subscriptions as subscriptions
 import ofscraper.api.me as me
 import ofscraper.utils.auth as auth
 import ofscraper.utils.args as args_
 import ofscraper.utils.stdout as stdout
 
 
-selectedusers=None
+parsed_subscriptions=None
 log=logging.getLogger(__package__)
 args=args_.getargs()
 
-def getselected_usernames():
-    #username list will be retrived once per daemon run
-    # manual prompt will need to recertify options every call
-    global selectedusers
-    scraper_bool=len(args.posts)>0 or args.action
-    #always return with correct args
+def getselected_usernames(rescan=False,reset=False):
+    #username list will be retrived every time reset==True
+    global parsed_subscriptions
     if "Skip" in args.posts:
         return []
-    if selectedusers and scraper_bool:
-            return selectedusers
-    if scraper_bool:
-        selectedusers=selectuserhelper()
-    #create in these situations
-    #set at least once
-    elif args.username and not selectedusers:
-        selectedusers=selectuserhelper()
-    elif not selectedusers and not scraper_bool:
-        selectedusers=selectuserhelper()
-    elif selectedusers and not scraper_bool:
-        if prompts.reset_username_prompt()=="Yes":  
-            selectedusers=selectuserhelper()
-    return selectedusers
+    if reset==True and args.username and parsed_subscriptions:
+        if prompts.reset_username_prompt()=="Yes":
+           parsed_subscriptions=None
+           args.username=None
+           args_.changeargs(args)
+    if rescan==True:
+        parsed_subscriptions=None
+    if not parsed_subscriptions or not args.username:
+        selectuserhelper()
 
+    usernameset=set(args.username)
+    return list(filter(lambda x:x["name"] in usernameset,parsed_subscriptions)) if args.username!="ALL" else parsed_subscriptions
+    
 def selectuserhelper():
     headers = auth.make_headers(auth.read_auth())
     subscribe_count = process_me(headers)
-    parsed_subscriptions = get_models(headers, subscribe_count)
-    if args.username and "ALL" in args.username:
-        filter_subscriptions=filterNSort(parsed_subscriptions )
-        selectedusers=filter_subscriptions
-        
-    elif args.username:
-        selectedusers=list(filter(lambda x:x["name"] in args.username,parsed_subscriptions))
-    #manually select usernames
-    else:
+    global parsed_subscriptions
+    all_subs = get_models(headers, subscribe_count)
+    if not args.username: 
         selected=None
         while True:
-            filter_subscriptions=filterNSort(parsed_subscriptions)
-            selectedusers,p= get_model(filter_subscriptions,selected)
-            if selectedusers!=None:
+            parsed_subscriptions=filterNSort( all_subs )
+            selectedusers,p= get_model(parsed_subscriptions ,selected)
+            if len(selectedusers)!=0:
+                args.username=selectedusers
+                args_.changeargs(args)
                 break
-
             setfilter()
             setsort()
             selected=p.selected_choices
-    return selectedusers or []
+    else:
+        parsed_subscriptions=filterNSort( all_subs )
+
+   
 
 
 
         
 
         
 
@@ -88,42 +81,42 @@
         args=prompts.modify_sort_prompt(args)
 
 def filterNSort(usernames):
 
 
     #paid/free
     filterusername=usernames
-    log.debug(f"Init username length: {len(filterusername)}")
+    log.debug(f"username count no filters: {len(filterusername)}")
     dateNow=arrow.now()
     if args.account_type=="paid":
         filterusername=list(filter(lambda x:(x.get("price") or 0)>0,filterusername))
-        log.debug(f"+paid filter username length: {len(filterusername)}")
+        log.debug(f"+paid filter username count: {len(filterusername)}")
 
     elif args.account_type=="free":
         filterusername=list(filter(lambda x:(x.get("price") or 0)==0,filterusername))    
-        log.debug(f"+free filter username length: {len(filterusername)}")
+        log.debug(f"+free filter username count: {len(filterusername)}")
     
     if args.renewal=="active":
         filterusername=list(filter(lambda x:x.get("renewed")!=None,filterusername))
-        log.debug(f"+active renewal filter username length: {len(filterusername)}")
+        log.debug(f"+active renewal filter username count: {len(filterusername)}")
 
     elif args.renewal=="disabled":
         filterusername=list(filter(lambda x:x.get("renewed")==None,filterusername))  
-        log.debug(f"+disabled renewal filter username length: {len(filterusername)}")
+        log.debug(f"+disabled renewal filter username count: {len(filterusername)}")
 
     if args.sub_status=="active":
         filterusername=list(filter(lambda x:x.get("subscribed")!=None,filterusername)) 
-        log.debug(f"+active subscribtion filter username length: {len(filterusername)}")
+        log.debug(f"+active subscribtion filter username count: {len(filterusername)}")
 
     elif args.sub_status=="expired":
         filterusername=list(filter(lambda x:x.get("subscribed")==None,filterusername))
-        log.debug(f"+expired subscribtion filter username length: {len(filterusername)}")
+        log.debug(f"+expired subscribtion filter username count: {len(filterusername)}")
 
     filterusername=list(filter(lambda x:x["name"] not in args.excluded_username ,filterusername))
-    log.debug(f"final length with all filters: {len(filterusername)}")
+    log.debug(f"final username count with all filters: {len(filterusername)}")
     if len(filterusername)==0:
         raise Exception("You have filtered the user list to zero\nPlease Select less restrictive filters")
     return sort_models_helper(filterusername)      
 
 
 
 def sort_models_helper(models):
```

### Comparing `ofscraper-2.6.1/pyproject.toml` & `ofscraper-2.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.6.1"
+version = "2.6.3"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
@@ -49,14 +49,18 @@
 
 
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx-argparse = "^0.4.0"
 
+
+[tool.poetry.group.testing.dependencies]
+coverage = "^7.2.7"
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
 ofscraper = "ofscraper.start:main"
```

### Comparing `ofscraper-2.6.1/PKG-INFO` & `ofscraper-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.6.1
+Version: 2.6.3
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

