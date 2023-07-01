# Comparing `tmp/not1mm-23.6.30.tar.gz` & `tmp/not1mm-23.6.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.6.30.tar", last modified: Sat Jul  1 04:17:57 2023, max compression
+gzip compressed data, was "not1mm-23.6.30.1.tar", last modified: Sat Jul  1 04:43:38 2023, max compression
```

## Comparing `not1mm-23.6.30.tar` & `not1mm-23.6.30.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.940596 not1mm-23.6.30/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.30/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23262 2023-07-01 04:17:57.939596 not1mm-23.6.30/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22516 2023-07-01 04:16:01.000000 not1mm-23.6.30/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.859595 not1mm-23.6.30/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.30/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94445 2023-07-01 04:11:44.000000 not1mm-23.6.30/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    26505 2023-06-28 22:11:02.000000 not1mm-23.6.30/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.895596 not1mm-23.6.30/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.30/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   635340 2023-06-17 01:32:08.000000 not1mm-23.6.30/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.30/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.30/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.30/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.30/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.30/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.30/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  7127932 2023-06-21 20:52:19.000000 not1mm-23.6.30/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.30/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.6.30/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.30/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.30/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.30/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.30/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.30/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.30/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.30/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.30/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44985 2023-06-21 19:42:00.000000 not1mm-23.6.30/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18069 2023-06-30 21:41:06.000000 not1mm-23.6.30/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.6.30/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.30/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.920596 not1mm-23.6.30/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.30/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.30/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.30/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.30/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.30/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.30/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.30/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.30/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.30/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.30/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.30/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.30/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.30/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.30/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.30/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.30/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.30/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.30/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.30/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.30/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.30/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.30/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.30/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.30/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.30/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.30/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.30/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.30/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.30/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.30/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.30/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.30/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.30/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.30/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.30/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.30/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.30/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.30/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.30/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.30/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.30/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.30/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.30/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.30/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.30/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.30/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.30/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.30/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.30/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.30/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.30/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.30/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.927596 not1mm-23.6.30/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.30/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.30/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.30/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.30/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35883 2023-06-28 19:43:33.000000 not1mm-23.6.30/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.30/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.30/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.30/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.30/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.30/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.30/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.30/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.30/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.30/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.30/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.30/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-07-01 04:16:27.000000 not1mm-23.6.30/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.30/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.30/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.935596 not1mm-23.6.30/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.30/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.30/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.30/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.30/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.30/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.30/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.30/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.30/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.30/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.30/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.30/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14562 2023-07-01 04:14:02.000000 not1mm-23.6.30/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.30/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.30/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.30/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.30/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.30/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.30/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.30/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.30/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.30/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.937596 not1mm-23.6.30/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.30/not1mm/testing/fakeflrig.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.30/not1mm/testing/flrigclient.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 not1mm-23.6.30/not1mm/testing/multicast_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-06-28 22:12:28.000000 not1mm-23.6.30/not1mm/testing/n1mm_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.30/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.862595 not1mm-23.6.30/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23262 2023-07-01 04:17:57.000000 not1mm-23.6.30/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3647 2023-07-01 04:17:57.000000 not1mm-23.6.30/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-07-01 04:17:57.000000 not1mm-23.6.30/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-07-01 04:17:57.000000 not1mm-23.6.30/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-07-01 04:17:57.000000 not1mm-23.6.30/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-07-01 04:17:57.000000 not1mm-23.6.30/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1272 2023-07-01 04:16:36.000000 not1mm-23.6.30/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-07-01 04:17:57.940596 not1mm-23.6.30/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:17:57.938596 not1mm-23.6.30/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      471 2023-06-26 02:26:39.000000 not1mm-23.6.30/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.880134 not1mm-23.6.30.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.30.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23264 2023-07-01 04:43:38.880134 not1mm-23.6.30.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22516 2023-07-01 04:16:01.000000 not1mm-23.6.30.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.747132 not1mm-23.6.30.1/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.30.1/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94445 2023-07-01 04:11:44.000000 not1mm-23.6.30.1/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    26505 2023-06-28 22:11:02.000000 not1mm-23.6.30.1/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.781133 not1mm-23.6.30.1/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.30.1/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   635340 2023-06-17 01:32:08.000000 not1mm-23.6.30.1/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.30.1/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.30.1/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.30.1/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.30.1/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.30.1/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.30.1/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  7127932 2023-06-21 20:52:19.000000 not1mm-23.6.30.1/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.30.1/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.6.30.1/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.30.1/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.30.1/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.30.1/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.30.1/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.30.1/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44985 2023-06-21 19:42:00.000000 not1mm-23.6.30.1/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18069 2023-06-30 21:41:06.000000 not1mm-23.6.30.1/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.6.30.1/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.30.1/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.865134 not1mm-23.6.30.1/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.30.1/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.30.1/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.30.1/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.30.1/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.30.1/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.30.1/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.30.1/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.30.1/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.30.1/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.30.1/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.30.1/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.30.1/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.30.1/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.30.1/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.30.1/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.30.1/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.30.1/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.30.1/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.30.1/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.30.1/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.30.1/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.30.1/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.30.1/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.30.1/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.30.1/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.30.1/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.30.1/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.30.1/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.30.1/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.30.1/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.30.1/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.30.1/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.30.1/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.30.1/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.30.1/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.30.1/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.30.1/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.30.1/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.30.1/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.30.1/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.30.1/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.30.1/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.30.1/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.30.1/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.30.1/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.30.1/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.30.1/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.30.1/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.30.1/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.30.1/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.30.1/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.30.1/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.871134 not1mm-23.6.30.1/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.30.1/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.30.1/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.30.1/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.30.1/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35883 2023-06-28 19:43:33.000000 not1mm-23.6.30.1/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.30.1/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.30.1/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.30.1/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.30.1/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.30.1/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.30.1/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.30.1/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.30.1/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.30.1/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.30.1/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.30.1/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-07-01 04:42:28.000000 not1mm-23.6.30.1/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.30.1/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.30.1/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.878134 not1mm-23.6.30.1/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.30.1/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14705 2023-07-01 04:39:54.000000 not1mm-23.6.30.1/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.30.1/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.30.1/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.30.1/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.30.1/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.30.1/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.30.1/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.30.1/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.30.1/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.30.1/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.879134 not1mm-23.6.30.1/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.30.1/not1mm/testing/fakeflrig.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.30.1/not1mm/testing/flrigclient.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 not1mm-23.6.30.1/not1mm/testing/multicast_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-06-28 22:12:28.000000 not1mm-23.6.30.1/not1mm/testing/n1mm_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.30.1/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.755133 not1mm-23.6.30.1/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23264 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3647 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1274 2023-07-01 04:42:11.000000 not1mm-23.6.30.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-07-01 04:43:38.881134 not1mm-23.6.30.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.880134 not1mm-23.6.30.1/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      471 2023-06-26 02:26:39.000000 not1mm-23.6.30.1/testing/test.py
```

### Comparing `not1mm-23.6.30/LICENSE` & `not1mm-23.6.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/PKG-INFO` & `not1mm-23.6.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.30
+Version: 23.6.30.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `not1mm-23.6.30/README.md` & `not1mm-23.6.30.1/README.md`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/__main__.py` & `not1mm-23.6.30.1/not1mm/__main__.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/bandmap.py` & `not1mm-23.6.30.1/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.6.30.1/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/MASTER.SCP` & `not1mm-23.6.30.1/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/about.ui` & `not1mm-23.6.30.1/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/bandmap.ui` & `not1mm-23.6.30.1/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/configuration.ui` & `not1mm-23.6.30.1/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/contests.sql` & `not1mm-23.6.30.1/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/cty.json` & `not1mm-23.6.30.1/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/editcontact.ui` & `not1mm-23.6.30.1/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/editmacro.ui` & `not1mm-23.6.30.1/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/logwindow.ui` & `not1mm-23.6.30.1/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/main.ui` & `not1mm-23.6.30.1/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/new_contest.ui` & `not1mm-23.6.30.1/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/not1mm.html` & `not1mm-23.6.30.1/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/opon.ui` & `not1mm-23.6.30.1/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/0.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/1.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/2.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/3.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/4.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/5.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/6.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/7.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/73.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/8.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/9.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/a.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/again.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/b.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/c.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/contest.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/cq.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/d.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/e.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/f.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/g.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/h.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/i.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/j.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/k.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/l.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/m.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/n.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/nil.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/o.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/p.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/q.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/r.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/roger.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/s.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/space.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/t.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/u.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/v.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/w.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/x.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/y.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/phonetics/z.wav` & `not1mm-23.6.30.1/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/pickcontest.ui` & `not1mm-23.6.30.1/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/reddot.png` & `not1mm-23.6.30.1/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/data/settings.ui` & `not1mm-23.6.30.1/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/cat_interface.py` & `not1mm-23.6.30.1/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/cwinterface.py` & `not1mm-23.6.30.1/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/database.py` & `not1mm-23.6.30.1/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/edit_macro.py` & `not1mm-23.6.30.1/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/edit_station.py` & `not1mm-23.6.30.1/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/ham_utility.py` & `not1mm-23.6.30.1/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/lookup.py` & `not1mm-23.6.30.1/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/multicast.py` & `not1mm-23.6.30.1/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/n1mm.py` & `not1mm-23.6.30.1/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/settings.py` & `not1mm-23.6.30.1/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/lib/versiontest.py` & `not1mm-23.6.30.1/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/logwindow.py` & `not1mm-23.6.30.1/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.6.30.1/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.6.30.1/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.6.30.1/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/arrl_field_day.py` & `not1mm-23.6.30.1/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.6.30.1/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.6.30.1/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/canada_day.py` & `not1mm-23.6.30.1/not1mm/plugins/canada_day.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,19 +198,23 @@
     if result:
         return int(result.get("Points", 0))
     return 0
 
 
 def calc_score(self):
     """Return calculated score"""
+    mults = show_mults(self)
     result = self.database.fetch_points()
     if result is not None:
         score = result.get("Points", "0")
         if score is None:
             score = "0"
+        if int(mults) > 0:
+            contest_points = int(score) * int(mults)
+            return contest_points
         contest_points = int(score)
         return contest_points
     return 0
 
 
 def adif(self):
     """
```

### Comparing `not1mm-23.6.30/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.6.30.1/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.6.30.1/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/cwt.py` & `not1mm-23.6.30.1/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/general_logging.py` & `not1mm-23.6.30.1/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/jidx_cw.py` & `not1mm-23.6.30.1/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/jidx_ph.py` & `not1mm-23.6.30.1/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/plugins/winter_field_day.py` & `not1mm-23.6.30.1/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/testing/fakeflrig.py` & `not1mm-23.6.30.1/not1mm/testing/fakeflrig.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/testing/flrigclient.py` & `not1mm-23.6.30.1/not1mm/testing/flrigclient.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/testing/multicast_listener.py` & `not1mm-23.6.30.1/not1mm/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/testing/n1mm_listener.py` & `not1mm-23.6.30.1/not1mm/testing/n1mm_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm/testing/test.py` & `not1mm-23.6.30.1/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/not1mm.egg-info/PKG-INFO` & `not1mm-23.6.30.1/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.30
+Version: 23.6.30.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `not1mm-23.6.30/not1mm.egg-info/SOURCES.txt` & `not1mm-23.6.30.1/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30/pyproject.toml` & `not1mm-23.6.30.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.6.30"
+version = "23.6.30.1"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

