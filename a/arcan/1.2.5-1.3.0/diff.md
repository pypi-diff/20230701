# Comparing `tmp/arcan-1.2.5.tar.gz` & `tmp/arcan-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.2.5.tar", max compression
+gzip compressed data, was "arcan-1.3.0.tar", max compression
```

## Comparing `arcan-1.2.5.tar` & `arcan-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1711 2023-06-30 21:58:37.058627 arcan-1.2.5/LICENSE
--rw-r--r--   0        0        0     4003 2023-06-30 21:58:37.058627 arcan-1.2.5/README.md
--rw-r--r--   0        0        0      907 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/ml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-06-30 21:58:37.058627 arcan-1.2.5/arcan/session/__init__.py
--rw-r--r--   0        0        0       62 2023-06-30 21:58:37.058627 arcan-1.2.5/main.py
--rw-r--r--   0        0        0      735 2023-06-30 21:58:37.062627 arcan-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 arcan-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-06-30 23:04:03.659730 arcan-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5132 2023-06-30 23:04:03.659730 arcan-1.3.0/README.md
+-rw-r--r--   0        0        0      907 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/session/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-30 23:04:03.659730 arcan-1.3.0/main.py
+-rw-r--r--   0        0        0      735 2023-06-30 23:04:03.663730 arcan-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 arcan-1.3.0/PKG-INFO
```

### Comparing `arcan-1.2.5/LICENSE` & `arcan-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.2.5/README.md` & `arcan-1.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -154,10 +154,40 @@
 
 - [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
 - [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
 - [FastAPI Documentation](https://fastapi.tiangolo.com/) - learn about FastAPI features and API.
 
 You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!
 
+
+
+### The application does the following: 
+- authenticates users via Email and Password with Firebase,
+- allows a user (cashier or store owner) to create various categories for the products,
+- add and delete products from the application, and
+- record and track sales made daily.
+
+<img width="1280" alt="Sales Management Dashboard" src="https://github.com/dha-stix/arcan-app/assets/67129211/4f963dcd-f81d-4c88-8c9d-3ac05b132ffa">
+
+
+## Live Demo
+- [View Live Version](https://arcan-two.vercel.app/)
+- [YouTube Demo](https://www.youtube.com/watch?v=Vq1xlL1g9eY)
+
+## How-to Guide
+[Read article on DEV](https://dev.to/arshadayvid/how-i-built-a-sales-management-app-with-nextjs-13-typescript-and-firebase-16cb)
+
+## Installation
+- Clone the project repository. Don't forget to star the repo 😉
+- Run `npm install` to install its dependencies.
+- Start the development server by running `npm run dev`
+
+## Tools
+- [NextJS 13](https://nextjs.org/docs)
+- [Tailwind CSS](https://tailwindcss.com/)
+- [Firebase](https://firebase.google.com)
+- [React Icons](https://react-icons.github.io/react-icons)
+
 ### Attribution
 This is a forked implementation for the Github repositories. Check out the attribution list:
-https://github.com/digitros/nextjs-fastapi
+https://github.com/digitros/nextjs-fastapi
+https://github.com/dha-stix/instock-app
```

#### html2text {}

```diff
@@ -45,10 +45,23 @@
 #"fastapi-dev": "poetry install && python -m uvicorn api.index:app --reload",
 ## Learn More To learn more about Next.js, take a look at the following
 resources: - [Next.js Documentation](https://nextjs.org/docs) - learn about
 Next.js features and API. - [Learn Next.js](https://nextjs.org/learn) - an
 interactive Next.js tutorial. - [FastAPI Documentation](https://
 fastapi.tiangolo.com/) - learn about FastAPI features and API. You can check
 out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your
-feedback and contributions are welcome! ### Attribution This is a forked
-implementation for the Github repositories. Check out the attribution list:
-https://github.com/digitros/nextjs-fastapi
+feedback and contributions are welcome! ### The application does the following:
+- authenticates users via Email and Password with Firebase, - allows a user
+(cashier or store owner) to create various categories for the products, - add
+and delete products from the application, and - record and track sales made
+daily. [Sales Management Dashboard] ## Live Demo - [View Live Version](https://
+arcan-two.vercel.app/) - [YouTube Demo](https://www.youtube.com/
+watch?v=Vq1xlL1g9eY) ## How-to Guide [Read article on DEV](https://dev.to/
+arshadayvid/how-i-built-a-sales-management-app-with-nextjs-13-typescript-and-
+firebase-16cb) ## Installation - Clone the project repository. Don't forget to
+star the repo ð - Run `npm install` to install its dependencies. - Start the
+development server by running `npm run dev` ## Tools - [NextJS 13](https://
+nextjs.org/docs) - [Tailwind CSS](https://tailwindcss.com/) - [Firebase](https:
+//firebase.google.com) - [React Icons](https://react-icons.github.io/react-
+icons) ### Attribution This is a forked implementation for the Github
+repositories. Check out the attribution list: https://github.com/digitros/
+nextjs-fastapi https://github.com/dha-stix/instock-app
```

### Comparing `arcan-1.2.5/arcan/__init__.py` & `arcan-1.3.0/arcan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # %%
 from modal import Stub, web_endpoint
 from modal import Image, Stub, web_endpoint
 
-__version__ = "1.2.5"
+__version__ = "1.3.0"
 
 
 # %%
 # %%
 def get_arcan_version():
     try:
         import arcan
```

### Comparing `arcan-1.2.5/pyproject.toml` & `arcan-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcan"
-version = "1.2.5"
+version = "1.3.0"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "arcan.ai Non-Commercial Open Source License"
 readme = "README.md"
 packages = [
     {include = "arcan"},
     {include = "main.py"}
```

### Comparing `arcan-1.2.5/PKG-INFO` & `arcan-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.2.5
+Version: 1.3.0
 Summary: A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools
 License: arcan.ai Non-Commercial Open Source License
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -171,10 +171,40 @@
 
 - [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
 - [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
 - [FastAPI Documentation](https://fastapi.tiangolo.com/) - learn about FastAPI features and API.
 
 You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!
 
+
+
+### The application does the following: 
+- authenticates users via Email and Password with Firebase,
+- allows a user (cashier or store owner) to create various categories for the products,
+- add and delete products from the application, and
+- record and track sales made daily.
+
+<img width="1280" alt="Sales Management Dashboard" src="https://github.com/dha-stix/arcan-app/assets/67129211/4f963dcd-f81d-4c88-8c9d-3ac05b132ffa">
+
+
+## Live Demo
+- [View Live Version](https://arcan-two.vercel.app/)
+- [YouTube Demo](https://www.youtube.com/watch?v=Vq1xlL1g9eY)
+
+## How-to Guide
+[Read article on DEV](https://dev.to/arshadayvid/how-i-built-a-sales-management-app-with-nextjs-13-typescript-and-firebase-16cb)
+
+## Installation
+- Clone the project repository. Don't forget to star the repo 😉
+- Run `npm install` to install its dependencies.
+- Start the development server by running `npm run dev`
+
+## Tools
+- [NextJS 13](https://nextjs.org/docs)
+- [Tailwind CSS](https://tailwindcss.com/)
+- [Firebase](https://firebase.google.com)
+- [React Icons](https://react-icons.github.io/react-icons)
+
 ### Attribution
 This is a forked implementation for the Github repositories. Check out the attribution list:
 https://github.com/digitros/nextjs-fastapi
+https://github.com/dha-stix/instock-app
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arcan Version: 1.2.5 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.3.0 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
 modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
 License Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fastapi (>=0.98.0,<0.99.0) Requires-
@@ -55,10 +55,23 @@
 #"fastapi-dev": "poetry install && python -m uvicorn api.index:app --reload",
 ## Learn More To learn more about Next.js, take a look at the following
 resources: - [Next.js Documentation](https://nextjs.org/docs) - learn about
 Next.js features and API. - [Learn Next.js](https://nextjs.org/learn) - an
 interactive Next.js tutorial. - [FastAPI Documentation](https://
 fastapi.tiangolo.com/) - learn about FastAPI features and API. You can check
 out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your
-feedback and contributions are welcome! ### Attribution This is a forked
-implementation for the Github repositories. Check out the attribution list:
-https://github.com/digitros/nextjs-fastapi
+feedback and contributions are welcome! ### The application does the following:
+- authenticates users via Email and Password with Firebase, - allows a user
+(cashier or store owner) to create various categories for the products, - add
+and delete products from the application, and - record and track sales made
+daily. [Sales Management Dashboard] ## Live Demo - [View Live Version](https://
+arcan-two.vercel.app/) - [YouTube Demo](https://www.youtube.com/
+watch?v=Vq1xlL1g9eY) ## How-to Guide [Read article on DEV](https://dev.to/
+arshadayvid/how-i-built-a-sales-management-app-with-nextjs-13-typescript-and-
+firebase-16cb) ## Installation - Clone the project repository. Don't forget to
+star the repo ð - Run `npm install` to install its dependencies. - Start the
+development server by running `npm run dev` ## Tools - [NextJS 13](https://
+nextjs.org/docs) - [Tailwind CSS](https://tailwindcss.com/) - [Firebase](https:
+//firebase.google.com) - [React Icons](https://react-icons.github.io/react-
+icons) ### Attribution This is a forked implementation for the Github
+repositories. Check out the attribution list: https://github.com/digitros/
+nextjs-fastapi https://github.com/dha-stix/instock-app
```

