# Comparing `tmp/SecureMessaging-1.0.2-py3-none-any.whl.zip` & `tmp/SecureMessaging-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5941 bytes, number of entries: 5
--rw-r--r--  2.0 unx    12558 b- defN 23-Jul-01 17:10 SecureMessaging.py
--rw-r--r--  2.0 unx     2852 b- defN 23-Jul-01 17:11 SecureMessaging-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 17:11 SecureMessaging-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 17:11 SecureMessaging-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      406 b- defN 23-Jul-01 17:11 SecureMessaging-1.0.2.dist-info/RECORD
-5 files, 15924 bytes uncompressed, 5183 bytes compressed:  67.5%
+Zip file size: 5500 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    12558 b- defN 23-Jul-01 17:36 SecureMessaging.py
+-rw-r--r--  2.0 unx     1799 b- defN 23-Jul-01 17:45 SecureMessaging-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 17:45 SecureMessaging-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 17:45 SecureMessaging-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      406 b- defN 23-Jul-01 17:45 SecureMessaging-1.0.4.dist-info/RECORD
+5 files, 14871 bytes uncompressed, 4742 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: SecureMessaging.py
 Comment: 
 
-Filename: SecureMessaging-1.0.2.dist-info/METADATA
+Filename: SecureMessaging-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: SecureMessaging-1.0.2.dist-info/WHEEL
+Filename: SecureMessaging-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: SecureMessaging-1.0.2.dist-info/top_level.txt
+Filename: SecureMessaging-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: SecureMessaging-1.0.2.dist-info/RECORD
+Filename: SecureMessaging-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SecureMessaging.py

```diff
@@ -174,15 +174,15 @@
 
         serialized_data = pickle.dumps(data)
         s.sendall(serialized_data)
         print("\nSent encrypted message, key and MAC")
 
 
 
-def recieve_message():
+def receive_message():
     global rng
     rng = "True"
     BUFFER_LIMIT = 1024 * 10
     server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     server.bind(('0.0.0.0', 5555))
     server.listen(1)
     print('To User: I will be back when bear connects, sorry about that. I am once again, currently eating a salad, who knew I could get fat off of these, anyway see you when bear connects! -Tom')
@@ -260,15 +260,15 @@
     while True:
         if rng == "False":
             receive_thread = threading.Thread(target=receive_message, daemon=True)
             receive_thread.start()
         time.sleep(1)  # Adjust the sleep duration based on your requirements
 
 
-def transcieve_message():
+def transceive_message():
     receive_thread = threading.Thread(target=receive_message, daemon=True)
     receive_thread.start()
     check_receive_thread = threading.Thread(target=check_receive, daemon=True)
     check_receive_thread.start()
 
     with patch_stdout():
         # Prompt for the IP address
```

