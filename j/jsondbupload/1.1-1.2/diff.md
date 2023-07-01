# Comparing `tmp/jsondbupload-1.1.tar.gz` & `tmp/jsondbupload-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsondbupload-1.1.tar", max compression
+gzip compressed data, was "jsondbupload-1.2.tar", max compression
```

## Comparing `jsondbupload-1.1.tar` & `jsondbupload-1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6265 2023-03-12 04:27:33.832000 jsondbupload-1.1/README.md
--rw-r--r--   0        0        0       38 2022-04-04 16:26:06.000000 jsondbupload-1.1/jsondbupload/__init__.py
--rw-r--r--   0        0        0     6221 2023-03-12 04:24:45.836000 jsondbupload-1.1/jsondbupload/jsondbupload.py
--rw-r--r--   0        0        0      407 2023-03-12 04:28:49.428000 jsondbupload-1.1/pyproject.toml
--rw-r--r--   0        0        0     7300 2023-03-12 04:30:46.202548 jsondbupload-1.1/setup.py
--rw-r--r--   0        0        0     6852 2023-03-12 04:30:46.202916 jsondbupload-1.1/PKG-INFO
+-rw-r--r--   0        0        0     6265 2023-03-12 04:27:33.832000 jsondbupload-1.2/README.md
+-rw-r--r--   0        0        0       38 2022-04-04 16:26:06.000000 jsondbupload-1.2/jsondbupload/__init__.py
+-rw-r--r--   0        0        0     6341 2023-07-01 06:57:57.912000 jsondbupload-1.2/jsondbupload/jsondbupload.py
+-rw-r--r--   0        0        0      407 2023-07-01 07:05:02.240000 jsondbupload-1.2/pyproject.toml
+-rw-r--r--   0        0        0     7300 2023-07-01 07:07:16.504305 jsondbupload-1.2/setup.py
+-rw-r--r--   0        0        0     6852 2023-07-01 07:07:16.504760 jsondbupload-1.2/PKG-INFO
```

### Comparing `jsondbupload-1.1/README.md` & `jsondbupload-1.2/README.md`

 * *Files identical despite different names*

### Comparing `jsondbupload-1.1/jsondbupload/jsondbupload.py` & `jsondbupload-1.2/jsondbupload/jsondbupload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json, os
 import jstyleson
 
 class JsonDBUpload(object):
-	def __init__(self, db, logger=None):
+	def __init__(self, db, logger=None, model=None):
 		self.db = db
 		self.logger = logger
 
-		self.tables_dict = {table.__tablename__: table for table in db.Model.__subclasses__()}
+		if model:
+			self.tables_dict = {table.__tablename__: table for table in model.__subclasses__()}
+		else:
+			self.tables_dict = {table.__tablename__: table for table in db.Model.__subclasses__()}
 
 	#########################################################################################################
 	#	Load values from config files to database tables
 	def update_tables_from_file(self, data_file):
 
 		if not os.path.exists(data_file):
 			raise Exception( f"Cannot find file {[data_file]}.  Working directory is [{os.path.curdir}] (absolute path: {os.path.realpath( os.path.curdir)} )")
```

### Comparing `jsondbupload-1.1/setup.py` & `jsondbupload-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['jstyleson>=0.0.2,<0.0.3']
 
 setup_kwargs = {
     'name': 'jsondbupload',
-    'version': '1.1',
+    'version': '1.2',
     'description': 'Insert records to relational database from json file',
     'long_description': '# Json DB Upload: Upload to a database from a JSON file\n\nModule enables a user to insert records into a database from a json file and also enables insertion into tables with foreign keys.  Hence, if you need to table A first, then key the primary keys from that to table B, this is possible from JsonDBUpload!\n\n\n### What problem does this solve?\nWhen you have a new application there are times where you need to insert some initial set of records.  Or there maybe a time where you need to synchronise data selectively between data stores of sorts. This is where this module can be of use.  It can help to insert records in any relational database which has a connection to it via sqlaclchemy\n\n### How does it do this?\nThe module takes in an argument of a json file (or a list-dictionary), and then proceeds to insert records one by one.  The json file must contain the table name, and label and foreign keys.\n\nThere are two key paramaters:\n1. A database session - this is from Flask SQLAlchemy\n2. An optional logger module (e.g. such as https://pypi.org/project/mclogger/ )\n\n### How to install?\nJSONDBUpload is avaialble through PyPi or you may use git:\n\n```\npip install jsondbupoad\n```\n\nOr, through git:\n```\ngit clone https://github.com/pub12/jsondbupload.git\n```\n\n### How to use jsondbupload?\nThe module is relatively easy to use.  All that is required is a file, and a database session.  The file format is as follows:\n```\n[\n\t{\t\t\n\t\t"table_name":"<table name>", \n\t\t"foreign_keys":[ { "<field name in current table>":"<table name of foreign table>.<field name>"} ],\n\t\t"data":[\n\t\t\t\t\t{"<field name>":"<field value>", ... },\n\t\t\t\t\t....\n\t\t]\n\t}\n]\n```\n\nThere are three key fields:\n* table_name: the name of the table to update\n* foreign_keys: a list of foreign key lookup from current file - this entry is optional\n* data: data to update\n\nHere\'s a working example to update 3 tables.  Firstly this is the sqlalchmey schema:\n```\nclass Author(db.Model):\n\t__tablename__ = \'author\' \n\tid = db.Column(db.Integer(), primary_key=True)\n\tname = db.Column(db.Integer() )\n\nclass Book(db.Model):\n\t__tablename__ = \'book\' \n\tid = db.Column(db.Integer(), primary_key=True)\n\tname = db.Column(db.Integer() )\n\tauthor_id = db.Column( db.Integer()  , db.ForeignKey( \'author.id\'  ) )\n\t_author = db.relationship("Author", backref=db.backref("author" ), lazy=\'joined\')\n\n\nclass Bookset(db.Model):\n\t__tablename__ = \'bookset\' \n\tid = db.Column(db.Integer(), primary_key=True)\n\tname = db.Column(db.Integer() )\n```\n\nAnd here\'s the json data to be used, this is in a file called `db_upload_file.json` (this can be any filename of course):\n```\n[\n\t{\t\t\n\t\t"table_name":"author", \n\t\t"data":[\n\t\t\t\t\t{"id":"AA_1", "name":"James"  },\n\t\t\t\t\t{"id":"AA_2", "name":"Moneypenny" }\n\t\t]\n\t},\n\t{\t\t\n\t\t"table_name":"book", \n\t\t"foreign_keys":[ { "author_id":"author.id"} ],\n\t\t"data":[\n\t\t\t\t\t{"id":"BB_1", "author_id":"AA_1", "name":"Never say Never"  },\n\t\t\t\t\t{"id":"BB_2", "author_id":"AA_2", "name":"Goldeneye" }\n\t\t]\n\t},\n\t{\t\t\n\t\t"table_name":"bookset", \n\t\t"data":[\n\t\t\t\t\t{"id":"", "name":"Best of Bond"  }\n\t\t]\n\t}\n]\n```\n\nIn this example, we have:\n* Updates to table `author` with two rows.  Please note, that in the database schema the field `id` is a primary key with automatic values so the entries will be ignored.\n* Updates to table `book` has a foreign key linkage where `author_id` is supposed to link to table `book.id` and the temporary values are linked to the table `author` by the `foreign_keys` description.\n* Update to table `bookset` is much simpler where the `name` field is specified, and the primary key `id` has no entry as any value given to it will be ignored anyway as it is a primary key.\n\n\nFinally, this is the code:\n```\nfrom jsondbupload import JsonDBUpload\nfrom flask import Flask\nfrom flask_sqlalchemy import SQLAlchemy, Model\n\nfrom mclogger import MCLogger\n\n#Define the table methods\nclass Author(db.Model):\n\t__tablename__ = \'author\' \n\tid = db.Column(db.Integer(), primary_key=True)\n\tname = db.Column(db.Integer() )\n\nclass Book(db.Model):\n\t__tablename__ = \'book\' \n\tid = db.Column(db.Integer(), primary_key=True)\n\tname = db.Column(db.Integer() )\n\tauthor_id = db.Column( db.Integer()  , db.ForeignKey( \'author.id\'  ) )\n\t_author = db.relationship("Author", backref=db.backref("author" ), lazy=\'joined\')\n\n\nclass Bookset(db.Model):\n\t__tablename__ = \'bookset\' \n\tid = db.Column(db.Integer(), primary_key=True)\n\tname = db.Column(db.Integer() )\n\t\n#Instantiate flask\napp = Flask(__name__)\napp.config[\'SQLALCHEMY_DATABASE_URI\'] = \'sqlite:///test.db\'\napp.config[\'SQLALCHEMY_TRACK_MODIFICATIONS\'] = False\ndb = SQLAlchemy(app)\n\n#Create logger - this is from https://pypi.org/project/mclogger/\nlogger = MCLogger( \'test_log.text\').getLogger()\n\n#>>>> Two lines to ulaod json data!  It will also do the commit to the database.  The logger is optional and will show on screen what\'s happening under the hood.\nj2db = JsonDBUpload( db, logger )\nj2db.update_tables_from_file(  \'db_upload_file.json\' )\n#>>>>>\n\n#After inserts, this will print out the records updated\nauth_list = db.session.query( Author ).all()\nfor item in auth_list:\n\tprint( item.name )\n\n```\n\n\n\n### Class JsonDBUpload Methods overview\n\n- #### __init__(db, logger=None)\n\tCreate instance of the JsonDBUpload instance.  \n\t\n\t- *db*: A reference to the SQLAlchemy database object reference with link already open to the database\n\t- *logger*:  The logger is an optional entry of the module `logging` or any sub-class of that such as `mclogger`.  If provided, it\'ll show a color log in the console of all the inserts\n\n- #### update_tables_from_file(filename )\n\tUpdate the database tables specfied in a given json file\n\n\t- *filename*: A string reference to the filename with relative or absolute path\n\n- #### update_tables_from_dict( data )\n\tUpdate the database tables specfied in a given list of dictionaries\n\n\t- *data*: A list of dictionaries with table names for each.  Format must be as follows:\n\t```\n\n\t[\n\t\t{\t\t\n\t\t\t"table_name":"<table name>", \n\t\t\t"foreign_keys":[ { "<field name in current table>":"<table name of foreign table>.<field name>"} ],\n\t\t\t"data":[\n\t\t\t\t\t\t{"<field name>":"<field value>", ... },\n\t\t\t\t\t\t....\n\t\t\t]\n\t\t}\n\t]\n\t```\n\n### Change Log\n## Version 1.0.6\n- Added ability to use single line and multiline comments in json file using jstyleson library\n',
     'author': 'pub12',
     'author_email': 'pubudu79@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pub12/jsondbupload',
```

### Comparing `jsondbupload-1.1/PKG-INFO` & `jsondbupload-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsondbupload
-Version: 1.1
+Version: 1.2
 Summary: Insert records to relational database from json file
 Home-page: https://github.com/pub12/jsondbupload
 License: MIT
 Author: pub12
 Author-email: pubudu79@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

