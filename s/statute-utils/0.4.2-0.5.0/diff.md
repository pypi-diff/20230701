# Comparing `tmp/statute_utils-0.4.2.tar.gz` & `tmp/statute_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.4.2.tar", max compression
+gzip compressed data, was "statute_utils-0.5.0.tar", max compression
```

## Comparing `statute_utils-0.4.2.tar` & `statute_utils-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.4.2/LICENSE
--rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.4.2/README.md
--rw-r--r--   0        0        0     1449 2023-06-25 10:37:56.128314 statute_utils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      361 2023-06-25 10:37:32.201516 statute_utils-0.4.2/statute_utils/__init__.py
--rw-r--r--   0        0        0     4210 2023-06-25 10:37:43.462905 statute_utils-0.4.2/statute_utils/main.py
--rw-r--r--   0        0        0     5167 2023-06-24 05:47:54.905008 statute_utils-0.4.2/statute_utils/models.py
--rw-r--r--   0        0        0     4431 2023-06-24 05:47:56.695048 statute_utils-0.4.2/statute_utils/names.py
--rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.4.2/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.4.2/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.4.2/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.4.2/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.4.2/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6615 2023-06-24 05:47:58.345784 statute_utils-0.4.2/statute_utils/serials.py
--rw-r--r--   0        0        0      327 2023-06-24 05:48:44.544520 statute_utils-0.4.2/statute_utils/statute/__init__.py
--rw-r--r--   0        0        0     9198 2023-06-24 05:48:08.172327 statute_utils-0.4.2/statute_utils/statute/category.py
--rw-r--r--   0        0        0     4423 2023-06-25 01:07:27.204571 statute_utils-0.4.2/statute_utils/statute/main.py
--rw-r--r--   0        0        0     4679 2023-06-23 10:46:22.018647 statute_utils-0.4.2/statute_utils/statute/rule.py
--rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.4.2/statute_utils/statute/short.py
--rw-r--r--   0        0        0     4667 2023-06-24 03:15:09.551113 statute_utils-0.4.2/statute_utils/statute/utils.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.0/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.0/README.md
+-rw-r--r--   0        0        0     1297 2023-07-01 04:37:03.663696 statute_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      431 2023-07-01 04:37:03.664040 statute_utils-0.5.0/statute_utils/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-01 04:37:03.664324 statute_utils-0.5.0/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     9093 2023-07-01 04:37:03.664630 statute_utils-0.5.0/statute_utils/components/category.py
+-rw-r--r--   0        0        0     1150 2023-07-01 04:37:03.664832 statute_utils-0.5.0/statute_utils/components/rule.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.0/statute_utils/components/short.py
+-rw-r--r--   0        0        0     4683 2023-07-01 04:37:03.665122 statute_utils-0.5.0/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     7805 2023-07-01 04:37:03.665405 statute_utils-0.5.0/statute_utils/main.py
+-rw-r--r--   0        0        0     2500 2023-07-01 04:37:03.665660 statute_utils-0.5.0/statute_utils/models.py
+-rw-r--r--   0        0        0    13202 2023-07-01 04:37:03.665877 statute_utils-0.5.0/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6682 2023-07-01 04:37:03.666097 statute_utils-0.5.0/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.0/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.0/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.0/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.0/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.0/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     4739 2023-07-01 04:37:03.666304 statute_utils-0.5.0/statute_utils/tree.py
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 statute_utils-0.5.0/PKG-INFO
```

### Comparing `statute_utils-0.4.2/LICENSE` & `statute_utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.2/README.md` & `statute_utils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.2/pyproject.toml` & `statute_utils-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.4.2"
+version = "0.5.0"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Intended Audience :: Legal Industry",
-  "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pydantic = ">=2.0b3"
 python-slugify = "^8.0"
-python-dateutil = "^2.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.1.15"
-types-Markdown = "^3.4"
-types-PyYAML = "^6.0"
 types-python-slugify = "^5.0"
-types-python-dateutil = "^2.8"
 ipykernel = "^6.23.2"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
```

### Comparing `statute_utils-0.4.2/statute_utils/models.py` & `statute_utils-0.5.0/statute_utils/tree.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,138 +1,140 @@
-import re
+import datetime
 from collections.abc import Iterator
-from re import Pattern
+from pathlib import Path
+from typing import NamedTuple
 
-from pydantic import Field
+import yaml
 
-from .recipes import split_digits
-from .statute import BaseCollection, BasePattern, Rule, StatuteSerialCategory, stx
+from .components import Rule, StatuteSerialCategory, StatuteTitle, set_node_ids, walk
 
+STATUTE_DIR = Path().home().joinpath("code/corpus-statutes")
 
-class NamedPattern(BasePattern):
-    """A [`Rule`][rule-model] can be extracted from a `NamedPattern`"""
 
-    name: str
-    regex_base: str
-    rule: Rule
-
-    @property
-    def regex(self) -> str:
-        return stx(rf"(?P<{self.group_name}>{self.regex_base})")
-
-    @property
-    def group_name(self) -> str:
-        return self.rule.slug
-
-
-class NamedPatternCollection(BaseCollection):
-    """Each named legal title, not falling under the SerialNames Patterns,
-    will also have its own manually crafted regex string. Examples include
-    'the Spanish Civil Code' or the '1987 Constitution' or the
-    'Code of Professional Responsibility'.
-    """
-
-    collection: list[NamedPattern]
-
-    def extract_rules(self, text: str) -> Iterator[Rule]:
-        for m in self.pattern.finditer(text):
-            for named in self.collection:
-                if m.lastgroup == named.group_name:
-                    yield named.rule
-
-
-class SerialPattern(BasePattern):
-    """A [`Rule`][rule-model] can be extracted from a `SerialPattern`. The word _serial_
-    is employed because the documents representing rules are numbered consecutively.
-
-    Each serial pattern refers to a [`Statute Category`][statute-category-model],
-    e.g. `RA`, `CA`, etc. matched with a
-    [`Serial Identifier`][statute-serial-identifier].
-
-    Since a `SerialPattern` inherits from a [BasePattern][base-pattern], it includes
-    other fields declared in the latter model: `matches` and `excludes` bringing the
-    total number of fields to 5, viz.:
-
-    Field | Description | Example
-    --:|:--|:--
-    `cat` | [`Statute Category`][statute-category-model] | StatuteSerialCategory.RepublicAct
-    `regex_bases` | How do we pattern the category name? | ["r.a. no.", "Rep. Act. No."]
-    `regex_serials` | What digits are allowed | ["386", "11114"]
-    `matches` | Usable in parametized tests to determine whether the pattern declared matches the samples | ["Republic Act No. 7160", "R.A. 386 and 7160" ]
-    `excludes` | Usable in parametized tests to determine that the full pattern will not match | ["Republic Act No. 7160:", "RA 9337-"]
-    """  # noqa: E501
-
-    cat: StatuteSerialCategory = Field(
-        ...,
-        title="Statute Serial Category",
-        description=(
-            "A type of rule from the taxonomy enumerated under StatuteSerialCategory."
-        ),
-    )
-    regex_bases: list[str] = Field(
-        ...,
-        title="Prefix Label in Regex",
-        description=(
-            "There are too many ways to express a category name. There is a"
-            " need to generate various regex strings which, when combined with"
-            " the serial, can qualify for a serial rule."
-        ),
-    )
-    regex_serials: list[str] = Field(
-        ...,
-        title="Serial Identifiers in Regex",
-        description=(
-            "The possible values of serial numbers to be matched with the regex_bases."
-        ),
-    )
-
-    @property
-    def lines(self) -> Iterator[str]:
-        """Each regex string produced matches the serial rule. Note the line break
-        needs to be retained so that when printing `@regex`, the result is organized.
-        """
-        for base in self.regex_bases:
-            for idx in self.regex_serials:
-                yield rf"""({base}\s*{idx})
-                """
+class Statute(NamedTuple):
+    """A instance is dependent on a statute path from a fixed
+    `STATUTE_DIR`. The shape of the Python object will be different
+    from the shape of the dumpable `.yml` export."""
 
-    @property
-    def group_name(self) -> str:
-        return rf"serial_{self.cat.name}"
-
-    @property
-    def regex(self) -> str:
-        return rf"(?P<{self.group_name}>{r'|'.join(self.lines)})"
-
-    @property
-    def digits_in_match(self) -> Pattern:
-        return re.compile(r"|".join(self.regex_serials))
-
-
-class SerialPatternCollection(BaseCollection):
-    """Each category-based, serial-numbered, legal title will have a
-    regex string, e.g. Republic Act is a category, a serial number for
-    this category is 386 representing the Philippine Civil Code."""
-
-    collection: list[SerialPattern]
-
-    def extract_rules(self, text: str) -> Iterator[Rule]:
-        """Each `m`, a python Match object, represents a
-        serial pattern category with possible ambiguous identifier found.
-
-        So running `m.group(0)` should yield the entire text of the
-        match which consists of (a) the definitive category;
-        and (b) the ambiguous identifier.
-
-        The identifier is ambiguous because it may be a compound one,
-        e.g. 'Presidential Decree No. 1 and 2'. In this case, there
-        should be 2 matches produced not just one.
-
-        This function splits the identifier by commas `,` and the
-        word `and` to get the individual component identifiers.
-        """
-        for match in self.pattern.finditer(text):
-            for sp in self.collection:
-                if match.lastgroup == sp.group_name:
-                    if candidates := sp.digits_in_match.search(match.group(0)):
-                        for d in split_digits(candidates.group(0)):
-                            yield Rule(cat=sp.cat, id=d)
+    titles: list[StatuteTitle]
+    rule: Rule
+    variant: int
+    date: datetime.date
+    units: list[dict]
+
+    def __str__(self) -> str:
+        return f"{self.rule.__str__()}, {self.date.strftime('%b %d, %Y')}"
+
+    def __repr__(self) -> str:
+        return "/".join(
+            [
+                self.rule.cat.value,
+                self.rule.num,
+                self.date.isoformat(),
+                f"{str(self.variant)}.yml",
+            ]
+        )
+
+    @property
+    def slug(self):
+        return self.__repr__().removesuffix(".yml").replace("/", "-")
+
+    def make_title_rows(self) -> Iterator[dict[str, str]]:
+        for counter, title in enumerate(self.titles, start=1):
+            yield {
+                "id": f"{self.slug}-{counter}",
+                "statute_id": self.slug,
+                "cat": title.category.name.lower(),
+                "text": title.text,
+            }
+
+    def make_row(self) -> dict:
+        """All nodes in the tree are marked by a material path.
+
+        The units key is manipulated to add a root node. This is
+        useful for repeals and other changes since affecting the root node, affects all nodes.
+
+        The root node for every key should be `1.`
+        """  # noqa: E501
+        set_node_ids(self.units)
+        return {
+            "id": self.slug,
+            "cat": self.rule.cat.value,
+            "num": self.rule.num,
+            "date": self.date,
+            "variant": self.variant,
+            "units": [{"num": "1.", "units": self.units}],
+        }
+
+    def to_file(self) -> Path:
+        """Orders the different key, value pairs for a yaml dump operation.
+        Ensures that each node in the tree is properly (rather than alphabetically)
+        ordered."""
+        f = STATUTE_DIR.joinpath(self.__repr__())
+        f.parent.mkdir(parents=True, exist_ok=True)
+        data: dict = self._asdict()
+        data["units"] = walk(data["units"])
+        text = yaml.dump(data, width=60)  # see representer added in walk
+        f.write_text(text)
+        return f
+
+    @classmethod
+    def from_file(cls, file: Path):
+        """Assumes strict path routing structure: `cat` / `num` / `date` / `variant`.yml,
+        e.g. `ra/386/1946-06-18/1.yml` where each file contains the following metadata, the
+        mandatory ones being "title" and "units". See example:
+
+        ```yaml
+        title: An Act to Ordain and Institute the Civil Code of the Philippines
+        aliases:
+        - New Civil Code
+        - Civil Code of 1950
+        short: Civil Code of the Philippines
+        units:
+        - item: Container 1
+          caption: Preliminary Title
+          units:
+            - item: Chapter 1
+              caption: Effect and Application of Laws
+              units:
+                - item: Article 1
+                  content: >-
+                    This Act shall be known as the "Civil Code of the Philippines."
+                    (n)
+                - item: Article 2
+                  content: >-
+                    Laws shall take effect after fifteen days following the
+                    completion of their publication either in the Official
+                    Gazette or in a newspaper of general circulation in the
+                    Philippines, unless it is otherwise provided. (1a)
+        ```
+        """  # noqa: E501
+        cat, num, date, variant = file.parts[-4:]
+        _date = [int(i) for i in date.split("-")]
+
+        data = yaml.safe_load(file.read_bytes())
+        official = data.get("title")
+        if not official:
+            return None
+
+        category = StatuteSerialCategory(cat)
+        if not category:
+            return None
+
+        serial = category.serialize(num)
+        if not serial:
+            return None
+
+        return cls(
+            rule=Rule(cat=category, num=num),
+            variant=int(variant.removesuffix(".yml")),
+            date=datetime.date(year=_date[0], month=_date[1], day=_date[2]),
+            units=data.get("units"),
+            titles=list(
+                StatuteTitle.generate(
+                    official=official,
+                    serial=serial,
+                    short=data.get("short"),
+                    aliases=data.get("aliases"),
+                )
+            ),
+        )
```

### Comparing `statute_utils-0.4.2/statute_utils/recipes/digits.py` & `statute_utils-0.5.0/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.2/statute_utils/recipes/spain.py` & `statute_utils-0.5.0/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.2/statute_utils/serials.py` & `statute_utils-0.5.0/statute_utils/models_serials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .models import SerialPattern, SerialPatternCollection
+from .components import (
+    StatuteSerialCategory,
+    add_blg,
+    add_num,
+    limited_acts,
+    ltr,
+)
+from .models import SerialPattern
 from .recipes import (
     ACT_DIGITS,
     BP_DIGITS,
     CA_DIGITS,
     PD_DIGITS_PLUS,
     RA_DIGITS,
     digitize,
 )
-from .statute import (
-    StatuteSerialCategory,
-    add_blg,
-    add_num,
-    limited_acts,
-    ltr,
-)
 
 """MODERN"""
 
 ra = SerialPattern(
     cat=StatuteSerialCategory.RepublicAct,
     regex_bases=[
         add_num(ltr("R", "A")),
@@ -233,25 +233,26 @@
     regex_serials=[r"10-15-1991"],
     matches=["Resolution of the Court En Banc dated 10-15-1991"],
 )
 """
 ## Resolution of the Court Rule Pattern
 """
 
-
-SerializedRules = SerialPatternCollection(
-    collection=[
-        ra,
-        ca,
-        act,
-        eo,
-        pd,
-        bp,
-        loi,
-        rule_am,
-        rule_bm,
-        sc_cir,
-        oca_cir,
-        veto,
-        rule_reso,
-    ]
-)
+SERIAL_COLLECTION = [
+    ra,
+    ca,
+    act,
+    eo,
+    pd,
+    bp,
+    loi,
+    rule_am,
+    rule_bm,
+    sc_cir,
+    oca_cir,
+    veto,
+    rule_reso,
+]
+"""Each category-based / serial-numbered legal title will have a
+regex string, e.g. Republic Act is a category, a serial number for
+this category is 386 representing the Civil Code.
+"""
```

### Comparing `statute_utils-0.4.2/statute_utils/statute/category.py` & `statute_utils-0.5.0/statute_utils/components/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
 from enum import StrEnum, auto
-
-from pydantic import BaseModel, ConfigDict
+from typing import NamedTuple
 
 
 class StatuteTitleCategory(StrEnum):
     """
-    A [`Rule`][rule-model] in the Philippines involves various denominations.
+    A Rule in the Philippines involves various denominations.
     It can be referred to by its
 
     1. `official` title
     2. `serial` title
     3. `short` title
     4. `alias` titles
 
@@ -28,18 +27,14 @@
     Serial = auto()
     Alias = auto()
     Short = auto()
 
 
 class StatuteSerialCategory(StrEnum):
     """
-    ## Application
-    This concerns the `serial` title described by the [`Statute Title Category`][statute-title-category-model].
-
-    ## Concept
     It would be difficult to identify rules if they were arbitrarily named
     without a fixed point of reference. For instance the _Civil Code of the
     Philippines_,  an arbitrary collection of letters, would be hard to find
     if laws were organized alphabetically.
 
     Fortunately, each Philippine `serial`-title rule belongs to an
     assignable `StatuteSerialCategory`:
@@ -172,14 +167,16 @@
                 raise SyntaxWarning(f"{idx=} invalid serial of {self}")
 
             case StatuteSerialCategory.RulesOfCourt:
                 if idx in ["1918", "1940", "1964"]:
                     return f"{idx} Rules of Court"
                 elif idx in ["cpr"]:
                     return "Code of Professional Responsibility"
+                elif idx in ["cpra"]:
+                    return "Code of Professional Responsibility and Accountability"
                 raise SyntaxWarning(f"{idx=} invalid serial of {self}")
 
             case StatuteSerialCategory.VetoMessage:
                 """No need to specify No.; understood to mean a Republic Act"""
                 return f"Veto Message - {idx}"
 
             case StatuteSerialCategory.ResolutionEnBanc:
@@ -213,18 +210,17 @@
 
             case _:
                 # no need to uppercase pure digits
                 target_digit = idx if idx.isdigit() else idx.upper()
                 return f"{uncamel(self)} No. {target_digit}"
 
 
-class StatuteTitle(BaseModel):
+class StatuteTitle(NamedTuple):
     """Will be used to populate the database; assumes a fixed `statute_id`."""
 
-    model_config = ConfigDict(use_enum_values=True)
     category: StatuteTitleCategory
     text: str
 
     @classmethod
     def generate(
         cls,
         official: str | None = None,
@@ -238,9 +234,10 @@
         if serial:
             yield cls(category=StatuteTitleCategory.Serial, text=serial)
 
         if aliases:
             for title in aliases:
                 if title and title != "":
                     yield cls(category=StatuteTitleCategory.Alias, text=title)
+
         if short:
             yield cls(category=StatuteTitleCategory.Short, text=short)
```

### Comparing `statute_utils-0.4.2/statute_utils/statute/short.py` & `statute_utils-0.5.0/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.2/statute_utils/statute/utils.py` & `statute_utils-0.5.0/statute_utils/components/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,47 @@
 from collections.abc import Iterator
 
 import yaml
 
 
+def set_node_ids(
+    nodes: list[dict],
+    parent_id: str = "1.",
+    child_key: str = "units",
+):
+    """Recursive function updates nodes in place since list/dicts are mutable.
+    Assumes that the nodes reprsent a deeply nested json, e.g.
+
+    For each node in the `nodes` list, it will add a new `id` key and will
+    increment according to its place in the tree structure.
+
+    If node id "1.1." has child nodes, the first child node will be "1.1.1.".
+
+    A trailing period is necessary for materialized paths. Otherwise a string
+    with  `value like '%'` where the value is 1.1 will also match 1.11
+
+    The root of the tree will always be "1.", unless the `parent_id` is
+    set to a different string.
+
+    The child key of the tree will always be "units", unless the `child_key`
+    is set to a different string.
+
+    Args:
+        nodes (list[dict]): The list of dicts that
+        parent_id (str, optional): The root node id. Defaults to "1.".
+        child_key (str, optional): The node which represents a list of children nodes.
+            Defaults to "units".
+    """
+    if isinstance(nodes, list):
+        for counter, node in enumerate(nodes, start=1):
+            node["id"] = f"{parent_id}{str(counter)}."
+            if node.get(child_key, None):
+                set_node_ids(node[child_key], node["id"], child_key)
+
+
 class literal(str):
     pass
 
 
 def literal_presenter(dumper, data):
     return dumper.represent_scalar("tag:yaml.org,2002:str", data, style=">")
 
@@ -52,15 +87,15 @@
             if node.get("units", None):
                 walked_units = walk(node["units"])
                 data.append(("units", walked_units))
             revised_nodes.append(dict(data))
     return revised_nodes
 
 
-def stx(regex_text: str):
+def make_regex_readable(regex_text: str):
     """Remove indention of raw regex strings. This makes regex more readable when using
     rich.Syntax(<target_regex_string>, "python")"""
     return rf"""
 {regex_text}
 """
 
 
@@ -110,42 +145,7 @@
     r"REPUBLIC",
     r"Commonwealth",
     r"COMMONWEALTH",
 ]
 """If the word act is preceded by these phrases, do not consider the same to be a
 legacy act of congress."""
 limited_acts = not_prefixed_by_any(rf"{add_num(r'Acts?')}", NON_ACT_INDICATORS)
-
-
-def set_node_ids(
-    nodes: list[dict],
-    parent_id: str = "1.",
-    child_key: str = "units",
-):
-    """Recursive function updates nodes in place since list/dicts are mutable.
-    Assumes that the nodes reprsent a deeply nested json, e.g.
-
-    For each node in the `nodes` list, it will add a new `id` key and will
-    increment according to its place in the tree structure.
-
-    If node id "1.1." has child nodes, the first child node will be "1.1.1.".
-
-    A trailing period is necessary for materialized paths. Otherwise a string
-    with  `value like '%'` where the value is 1.1 will also match 1.11
-
-    The root of the tree will always be "1.", unless the `parent_id` is
-    set to a different string.
-
-    The child key of the tree will always be "units", unless the `child_key`
-    is set to a different string.
-
-    Args:
-        nodes (list[dict]): The list of dicts that
-        parent_id (str, optional): The root node id. Defaults to "1.".
-        child_key (str, optional): The node which represents a list of children nodes.
-            Defaults to "units".
-    """
-    if isinstance(nodes, list):
-        for counter, node in enumerate(nodes, start=1):
-            node["id"] = f"{parent_id}{str(counter)}."
-            if node.get(child_key, None):
-                set_node_ids(node[child_key], node["id"], child_key)
```

### Comparing `statute_utils-0.4.2/PKG-INFO` & `statute_utils-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.4.2
+Version: 0.5.0
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=2.0b3)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-slugify (>=8.0,<9.0)
 Project-URL: Documentation, https://justmars.github.io/statute-utils
 Project-URL: Repository, https://github.com/justmars/statute-utils
 Description-Content-Type: text/markdown
 
 # statute-utils
```

