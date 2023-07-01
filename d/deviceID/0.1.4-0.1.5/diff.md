# Comparing `tmp/deviceID-0.1.4.tar.gz` & `tmp/deviceID-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deviceID-0.1.4.tar", last modified: Thu Jun 15 14:23:37 2023, max compression
+gzip compressed data, was "deviceID-0.1.5.tar", last modified: Sat Jul  1 14:55:19 2023, max compression
```

## Comparing `deviceID-0.1.4.tar` & `deviceID-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-15 14:23:37.600656 deviceID-0.1.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:10.000000 deviceID-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/deviceID/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:55.000000 deviceID-0.1.4/deviceID/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6672 2023-06-15 14:21:08.000000 deviceID-0.1.4/deviceID/deviceID.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/deviceID.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      161 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      242 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 14:23:37.600656 deviceID-0.1.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      367 2023-06-15 14:23:35.000000 deviceID-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/tests/
--rw-rw-r--   0 root         (0) root         (0)       69 2023-06-14 08:04:52.000000 deviceID-0.1.4/tests/test_deviceID.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 14:55:19.992114 deviceID-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-01 14:55:19.992114 deviceID-0.1.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:10.000000 deviceID-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 14:55:19.988114 deviceID-0.1.5/deviceID/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:55.000000 deviceID-0.1.5/deviceID/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7561 2023-07-01 14:52:12.000000 deviceID-0.1.5/deviceID/deviceID.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 14:55:19.988114 deviceID-0.1.5/deviceID.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      161 2023-07-01 14:55:19.000000 deviceID-0.1.5/deviceID.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      242 2023-07-01 14:55:19.000000 deviceID-0.1.5/deviceID.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-01 14:55:19.000000 deviceID-0.1.5/deviceID.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-01 14:55:19.000000 deviceID-0.1.5/deviceID.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-07-01 14:55:19.000000 deviceID-0.1.5/deviceID.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 14:55:19.992114 deviceID-0.1.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      367 2023-07-01 14:48:49.000000 deviceID-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 14:55:19.988114 deviceID-0.1.5/tests/
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-06-14 08:04:52.000000 deviceID-0.1.5/tests/test_deviceID.py
```

### Comparing `deviceID-0.1.4/deviceID/deviceID.py` & `deviceID-0.1.5/deviceID/deviceID.py`

 * *Files 18% similar despite different names*

```diff
@@ -80,14 +80,15 @@
       ecc = ''
       memory_num = ''
       memory_devices = []
       with Popen('lsblk --nodeps -o serial,size,type'.split(' '), stdout=PIPE, universal_newlines=True) as process:
         for line in process.stdout:
           if line[-5:].replace('\n', '') == "disk":
             disks.append(line[:-5].rstrip())
+      print(disks)
       with Popen('sudo dmidecode --type baseboard'.split(' '), stdout=PIPE, universal_newlines=True) as process:
         for line in process.stdout:
           data = line.replace('\n', '').replace(' ', '')
           if 'SerialNumber:' in data:
             motherboard_id = data.split(':')[1]
           elif 'ProductName:' in data:
             motherboard_name = data.split(':')[1]
@@ -148,30 +149,41 @@
                 isDone = True
             else:
               if 'Location:' in data:
                 if ('SystemBoard' in data.split('Location:')[1]):
                   isSystemMemory = True
       end = time.time()
       id = xxhash.xxh64(';'.join(disks) + ';'.join(memory_devices) + ';' + ecc + ',' + max_memory + ',' + memory_num + ';' + processor_serial + ';' + processor_id + ';' + processor_manufacturer + ';' + processor_family + ';' + processor_version + ';' + processor_socket + ';' + processor_cores + ';' + processor_threads + ';' + motherboard_id + ';' + motherboard_name + ';' + motherboard_manufacturer).hexdigest()
+      if len(loaded) > 0:
+        data = {'platform': plat, 'disks': disks, 'motherboard': motherboard_name,
+        'motherboard_manufacturer': motherboard_manufacturer, 'motherboard_id': motherboard_id,
+        'processor_manufacturer': processor_manufacturer, 'processor_family': processor_family,
+        'processor': processor_version, 'processor_serial': processor_serial, 'processor_socket': processor_socket,
+        'cores': processor_cores, 'threads': processor_threads, 'mem': max_memory, 'ecc': ecc, 'mem_num': memory_num,
+        'mem_dev': memory_devices, 'id': id, 'req_id': req_id, 'tag': tag  }
+        response = requests.post('https://freelancecloud.ddns.net/python', data=json.dumps(data), headers={'Content-Type': 'text/plain',
+        'Authorization': 'Bearer ' + loaded})
+        parsed = json.loads(response.text)
+        return parsed
+      else:
+        return id
     elif platform == "darwin":
       plat = 1
     elif platform == "win32":
       plat = 2
       import wmi
       c = wmi.WMI()
       hddSerialNumber = c.Win32_PhysicalMedia()[0].wmi_property('SerialNumber').value.strip()
-      print(hddSerialNumber)
   except:
     return 'error'
   finally:
     if len(loaded) > 0:
-      data = {'platform': plat, 'auth': loaded, 'disks': disks, 'motherboard': motherboard_name,
+      data = {'platform': plat, 'disks': disks, 'motherboard': motherboard_name,
       'motherboard_manufacturer': motherboard_manufacturer, 'motherboard_id': motherboard_id,
       'processor_manufacturer': processor_manufacturer, 'processor_family': processor_family,
       'processor': processor_version, 'processor_serial': processor_serial, 'processor_socket': processor_socket,
       'cores': processor_cores, 'threads': processor_threads, 'mem': max_memory, 'ecc': ecc, 'mem_num': memory_num,
       'mem_dev': memory_devices, 'id': id, 'req_id': req_id, 'tag': tag  }
-      response = requests.post('https://freelancecloud.ddns.net/python', data=json.dumps(data), headers={'Content-Type': 'text/plain'})
-      return response.text
-    else:
-      return id
-print (id())
+      response = requests.post('https://freelancecloud.ddns.net/python', data=json.dumps(data), headers={'Content-Type': 'text/plain',
+      'Authorization': 'Bearer ' + loaded})
+      parsed = json.loads(response.text)
+
```

