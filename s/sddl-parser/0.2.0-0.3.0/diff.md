# Comparing `tmp/sddl_parser-0.2.0.tar.gz` & `tmp/sddl_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddl_parser-0.2.0.tar", max compression
+gzip compressed data, was "sddl_parser-0.3.0.tar", max compression
```

## Comparing `sddl_parser-0.2.0.tar` & `sddl_parser-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      398 2023-06-27 21:46:46.042420 sddl_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3741 2023-06-27 21:44:17.810516 sddl_parser-0.2.0/README.md
--rw-r--r--   0        0        0       71 2023-06-27 15:03:35.127501 sddl_parser-0.2.0/sddl_parser/__init__.py
--rw-r--r--   0        0        0      517 2023-06-27 16:21:14.512040 sddl_parser-0.2.0/sddl_parser/api.py
--rw-r--r--   0        0        0     5151 2023-06-27 20:20:51.962626 sddl_parser-0.2.0/sddl_parser/dictionary.py
--rw-r--r--   0        0        0     5195 2023-06-27 20:56:57.890162 sddl_parser-0.2.0/sddl_parser/parser.py
--rw-r--r--   0        0        0    50423 2023-06-27 21:38:38.418293 sddl_parser-0.2.0/sddl_parser/rights_enums.py
--rw-r--r--   0        0        0      796 2023-06-27 20:10:00.050365 sddl_parser-0.2.0/sddl_parser/type_enums.py
--rw-r--r--   0        0        0     1439 2023-06-27 19:55:38.294366 sddl_parser-0.2.0/sddl_parser/types.py
--rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 sddl_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      455 2023-06-30 23:54:30.580370 sddl_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3782 2023-06-30 23:55:19.526760 sddl_parser-0.3.0/README.md
+-rw-r--r--   0        0        0       75 2023-06-30 20:12:20.818217 sddl_parser-0.3.0/sddl_parser/__init__.py
+-rw-r--r--   0        0        0    50688 2023-06-30 17:28:00.851573 sddl_parser-0.3.0/sddl_parser/ace_rights_enums.py
+-rw-r--r--   0        0        0     1526 2023-06-30 23:47:30.535387 sddl_parser-0.3.0/sddl_parser/api.py
+-rw-r--r--   0        0        0     1257 2023-06-30 22:00:15.446960 sddl_parser-0.3.0/sddl_parser/enums.py
+-rw-r--r--   0        0        0     5295 2023-06-30 23:27:33.678123 sddl_parser-0.3.0/sddl_parser/parser.py
+-rw-r--r--   0        0        0     2845 2023-06-30 21:01:35.039016 sddl_parser-0.3.0/sddl_parser/sid_enum.py
+-rw-r--r--   0        0        0     2647 2023-06-30 23:41:53.672836 sddl_parser-0.3.0/sddl_parser/types.py
+-rw-r--r--   0        0        0     5410 2023-06-30 23:09:49.290197 sddl_parser-0.3.0/sddl_parser/well_known_dictionary.py
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 sddl_parser-0.3.0/PKG-INFO
```

### Comparing `sddl_parser-0.2.0/README.md` & `sddl_parser-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,162 @@
-# Install
-```
-pip3 install sddl-parser
-```
-
-# Usage
-Parse an SDDL string
-
-```py
->> from sddl_parser import parse_sddl
->> sddl = "O:SYG:SYD:AI(A;ID;GA;;;SY)"
->> parse_sddl(sddl)
-SDDL(
-    owner="LOCAL_SYSTEM",
-    group="LOCAL_SYSTEM",
-    dacl=DACL(
-        flags=["SDDL_AUTO_INHERITED"],
-        aces=[
-            ACE(
-                type=AceType.ACCESS_ALLOWED,
-                flags=["INHERITED"],
-                object_guid="",
-                rights_int=268435456,
-                inherit_object_guid="",
-                sid="LOCAL_SYSTEM",
-                conditional_ace=None,
-                rights={GenericAccessRights.GENERIC_ALL},
-            )
-        ],
-    ),
-    sacl=None,
-)
-```
-
-Parse an ACE
-
-```py
->> from sddl_parser import parse_ace
->> ace = "(A;ID;0x10030;;;AC)"
->> parse_ace(ace)
-ACE(
-    type=AceType.ACCESS_ALLOWED,
-    flags=["INHERITED"],
-    object_guid="",
-    rights_int=65584,
-    inherit_object_guid="",
-    sid="ALL_APP_PACKAGES",
-    conditional_ace=None,
-    rights={
-        GenericAccessRights.ACCESS4,
-        GenericAccessRights.DELETE,
-        GenericAccessRights.ACCESS5,
-    },
-)
-```
-
-See that `GenericAccessRights.ACCESS4` is returned. That's an indication that the SDDL type should be specified. To get more accurate rights, use `.as_type()` on the object or pass the Rights object to the parse_ace function
-
-```py
->> from sddl_parser import parse_ace, FileAccessRights
->> ace = "(A;ID;0x1200a9;;;AC)"
->> # alternatively, run parse_ace(ace, FileAccessRights)
->> parse_ace(ace).as_type(FileAccessRights)
-ACE(
-    type=AceType.ACCESS_ALLOWED,
-    flags=["INHERITED"],
-    object_guid="",
-    rights_int=65584,
-    inherit_object_guid="",
-    sid="ALL_APP_PACKAGES",
-    conditional_ace=None,
-    rights={
-        FileAccessRights.FILE_WRITE_EA,
-        FileAccessRights.DELETE,
-        FileAccessRights.FILE_EXECUTE,
-    },
-)
-```
-
-All rights are IntEnums, so if you want to check for generic rights, `FileAccessRights.DELETE` is equivalent to `GenericAccessRights.DELETE`
-
-# Access Rights Available
-
-All right enums are given here
-
-```
->> from sddl_parser import rights_enums
->> for x in dir(rights_enums):
->>   print(i)
-AlpcAccessRights
-AuditAccessRights
-DebugAccessRights
-DesktopAccessRights
-DirectoryAccessRights
-DirectoryServiceAccessRights
-EnlistmentAccessRights
-EventAccessRights
-FileAccessRights
-FileDirectoryAccessRights
-FilterConnectionPortAccessRights
-FirewallAccessRights
-FirewallFilterAccessRights
-GenericAccessRights
-IoCompletionAccessRights
-JobAccessRights
-KeyAccessRights
-LsaAccountAccessRights
-LsaPolicyAccessRights
-LsaSecretAccessRights
-LsaTrustedDomainAccessRights
-MemoryPartitionAccessRights
-MutantAccessRights
-PrintSpoolerAccessRights
-ProcessAccessRights
-RegistryKeyAccessRights
-RegistryTransactionAccessRights
-ResourceManagerAccessRights
-SamAliasAccessRights
-SamDomainAccessRights
-SamGroupAccessRights
-SamServerAccessRights
-SamUserAccessRights
-SemaphoreAccessRights
-ServiceAccessRights
-ServiceControlManagerAccessRights
-SessionAccessRights
-SymbolicLinkAccessRights
-ThreadAccessRights
-TimerAccessRights
-TokenAccessRights
-TraceAccessRights
-TransactionAccessRights
-TransactionManagerAccessRights
-WindowStationAccessRights
-WnfAccessRights
-```
-
-# TODO
-1. Allow identifiers (D:, O:, S:) to be out of order. I haven't run into this on any SDDLs on my system, but I'm sure it exists somewhere out there
-
-# Thanks
-- Thanks to [An0ther0ne] for compiling the constants for ACEs
-- Thanks to [James Forshaw] for compiling access rights in NTApiDotNet
-
-
-[An0ther0ne]: https://github.com/An0ther0ne
-[James Forshaw]: https://twitter.com/tiraniddo
+Metadata-Version: 2.1
+Name: sddl-parser
+Version: 0.3.0
+Summary: Parse SDDL strings
+Author: Max Harley
+Author-email: maxh@maxh.io
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: parsy (>=2.1,<3.0)
+Description-Content-Type: text/markdown
+
+# Install
+```
+pip3 install sddl-parser
+```
+
+# Usage
+Parse an SDDL string
+
+```py
+>> from sddl_parser import parse_sddl
+>> sddl = "O:SYG:SYD:AI(A;ID;GA;;;SY)"
+>> parse_sddl(sddl)
+SDDL(
+    owner=SIDEnum.LOCAL_SYSTEM,
+    group=SIDEnum.LOCAL_SYSTEM,
+    dacl=ACL(
+        flags={SDDLFlags.SDDL_AUTO_INHERITED},
+        aces=[
+            ACE(
+                type=AceType.ACCESS_ALLOWED,
+                flags={AceFlags.INHERITED},
+                object_guid="",
+                rights_int=268435456,
+                inherit_object_guid="",
+                sid=SIDEnum.LOCAL_SYSTEM,
+                conditional_ace=None,
+                rights={GenericAccessRights.GENERIC_ALL},
+            )
+        ],
+    ),
+    sacl=None,
+)
+```
+
+Parse an ACE
+
+```py
+>> from sddl_parser import parse_ace
+>> ace = "(A;ID;0x10030;;;AC)"
+>> parse_ace(ace)
+ACE(
+    type=AceType.ACCESS_ALLOWED,
+    flags={AceFlags.INHERITED},
+    object_guid="",
+    rights_int=65584,
+    inherit_object_guid="",
+    sid=SIDEnum.ALL_APP_PACKAGES,
+    conditional_ace=None,
+    rights={
+        GenericAccessRights.ACCESS4,
+        GenericAccessRights.DELETE,
+        GenericAccessRights.ACCESS5,
+    },
+)
+```
+
+See that `GenericAccessRights.ACCESS4` is returned. That's an indication that the SDDL type should be specified. To get more accurate rights, use `.as_type()` on the object or pass the Rights object to the parse_ace function
+
+```py
+>> from sddl_parser import parse_ace, FileAccessRights
+>> ace = "(A;ID;0x1200a9;;;AC)"
+>> # alternatively, run parse_ace(ace, FileAccessRights)
+>> parse_ace(ace).as_type(FileAccessRights)
+ACE(
+    type=AceType.ACCESS_ALLOWED,
+    flags={AceFlags.INHERITED},
+    object_guid="",
+    rights_int=1179817,
+    inherit_object_guid="",
+    sid=SIDEnum.ALL_APP_PACKAGES,
+    conditional_ace=None,
+    rights={
+        FileAccessRights.FILE_EXECUTE,
+        FileAccessRights.FILE_READ_DATA,
+        FileAccessRights.FILE_READ_ATTRIBUTES,
+        FileAccessRights.READ_CONTROL,
+        FileAccessRights.SYNCHRONIZE,
+        FileAccessRights.FILE_GENERIC_EXECUTE,
+        FileAccessRights.FILE_READ_EA,
+        FileAccessRights.FILE_GENERIC_READ,
+    },
+)
+```
+
+All rights are IntEnums, so if you want to check for generic rights, `FileAccessRights.DELETE` is equivalent to `GenericAccessRights.DELETE`
+
+# Access Rights Available
+
+All right enums are given here
+
+```
+>> from sddl_parser import rights_enums
+>> for x in dir(rights_enums):
+>>   print(i)
+AlpcAccessRights
+AuditAccessRights
+DebugAccessRights
+DesktopAccessRights
+DirectoryAccessRights
+DirectoryServiceAccessRights
+EnlistmentAccessRights
+EventAccessRights
+FileAccessRights
+FileDirectoryAccessRights
+FilterConnectionPortAccessRights
+FirewallAccessRights
+FirewallFilterAccessRights
+GenericAccessRights
+IoCompletionAccessRights
+JobAccessRights
+KeyAccessRights
+LsaAccountAccessRights
+LsaPolicyAccessRights
+LsaSecretAccessRights
+LsaTrustedDomainAccessRights
+MemoryPartitionAccessRights
+MutantAccessRights
+PrintSpoolerAccessRights
+ProcessAccessRights
+RegistryKeyAccessRights
+RegistryTransactionAccessRights
+ResourceManagerAccessRights
+SamAliasAccessRights
+SamDomainAccessRights
+SamGroupAccessRights
+SamServerAccessRights
+SamUserAccessRights
+SemaphoreAccessRights
+ServiceAccessRights
+ServiceControlManagerAccessRights
+SessionAccessRights
+SymbolicLinkAccessRights
+ThreadAccessRights
+TimerAccessRights
+TokenAccessRights
+TraceAccessRights
+TransactionAccessRights
+TransactionManagerAccessRights
+WindowStationAccessRights
+WnfAccessRights
+```
+
+# Shoulders of Giants
+- [An0ther0ne]
+- [James Forshaw]
+
+[An0ther0ne]: https://github.com/An0ther0ne
+[James Forshaw]: https://twitter.com/tiraniddo
+
```

### Comparing `sddl_parser-0.2.0/sddl_parser/dictionary.py` & `sddl_parser-0.3.0/sddl_parser/well_known_dictionary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict
-from sddl_parser.rights_enums import (
+from sddl_parser.ace_rights_enums import (
     GenericAccessRights,
     FileAccessRights,
     RegistryKeyAccessRights,
 )
-from sddl_parser.type_enums import AceType
+from sddl_parser.sid_enum import SIDEnum
+from sddl_parser.enums import AceType, AceFlags, SDDLFlags
 
 # https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/628ebb1d-c509-4ea0-a10f-77ef97ca4586
 ACE_TYPE: Dict[str, AceType] = {
     "A": AceType.ACCESS_ALLOWED,
     "D": AceType.ACCESS_DENIED,
     "OA": AceType.ACCESS_ALLOWED_OBJECT,
     "OD": AceType.ACCESS_DENIED_OBJECT,
@@ -24,22 +25,23 @@
     "XU": AceType.SYSTEM_AUDIT_CALLBACK,
     "ZA": AceType.ACCESS_ALLOWED_CALLBACK_OBJECT,
     "TL": AceType.SYSTEM_PROCESS_TRUST_LABEL,
     "FL": AceType.SYSTEM_ACCESS_FILTER,
 }
 
 ACE_FLAGS = {
-    "CI": ("CONTAINER_INHERIT", "CONTAINER_INHERIT_ACE", 0x02),
-    "OI": ("OBJECT_INHERIT", "OBJECT_INHERIT_ACE", 0x01),
-    "NP": ("NO_PROPAGATE", "NO_PROPAGATE_INHERIT_ACE", 0x04),
-    "IO": ("INHERIT_ONLY", "INHERIT_ONLY_ACE", 0x08),
-    "ID": ("INHERITED", "INHERITED_ACE", 0x10),
-    "SA": ("AUDIT_SUCCESS", "SUCCESSFUL_ACCESS_ACE_FLAG", 0x40),
-    "FA": ("AUDIT_FAILURE", "FAILED_ACCESS_ACE_FLAG", 0x80),
-    # TODO: TP and CR missing - https://learn.microsoft.com/en-us/windows/win32/secauthz/ace-strings
+    "CI": AceFlags.CONTAINER_INHERIT,
+    "OI": AceFlags.OBJECT_INHERIT,
+    "NP": AceFlags.NO_PROPAGATE,
+    "IO": AceFlags.INHERIT_ONLY,
+    "ID": AceFlags.INHERITED,
+    "SA": AceFlags.AUDIT_SUCCESS,
+    "FA": AceFlags.AUDIT_FAILURE,
+    "TP": AceFlags.TRUST_PROTECTED_FILTER
+    # TODO: CR missing - https://learn.microsoft.com/en-us/windows/win32/secauthz/ace-strings
 }
 
 
 # https://github.com/tpn/winsdk-10/blob/master/Include/10.0.14393.0/shared/sddl.h#L123
 ACE_RIGHTS: Dict[str, int] = {
     "CC": GenericAccessRights.ACCESS0,
     "DC": GenericAccessRights.ACCESS1,
@@ -70,82 +72,82 @@
     "NR": 0x01,
     # SDDL_NO_WRITE_UP
     "NW": 0x02,
     # SDDL_NO_EXECUTE_UP
     "NX": 0x04,
 }
 
-SDDL_SIDS = {  # Well known SIDs
-    "AA": "ACCESS_CONTROL_ASSISTANCE_OPS",
-    "AC": "ALL_APP_PACKAGES",
-    "AN": "ANONYMOUS",
-    "AO": "ACCOUNT_OPERATORS",
-    "AP": "PROTECTED_USERS",
-    "AU": "AUTHENTICATED_USERS",
-    "BA": "BUILTIN_ADMINISTRATORS",
-    "BG": "BUILTIN_GUESTS",
-    "BO": "BACKUP_OPERATORS",
-    "BU": "BUILTIN_USERS",
-    "CA": "CERT_SERV_ADMINISTRATORS",
-    "CD": "CERTSVC_DCOM_ACCESS",
-    "CG": "CREATOR_GROUP",
-    "CN": "CLONEABLE_CONTROLLERS",
-    "CO": "CREATOR_OWNER",
-    "CY": "CRYPTO_OPERATORS",
-    "DA": "DOMAIN_ADMINISTRATORS",
-    "DC": "DOMAIN_COMPUTERS",
-    "DD": "DOMAIN_DOMAIN_CONTROLLERS",
-    "DG": "DOMAIN_GUESTS",
-    "DU": "DOMAIN_USERS",
-    "EA": "ENTERPRISE_ADMINS",
-    "ED": "ENTERPRISE_DOMAIN_CONTROLLERS",
-    "EK": "ENTERPRISE_KEY_ADMINS",
-    "ER": "EVENT_LOG_READERS",
-    "ES": "RDS_ENDPOINT_SERVERS",
-    "HA": "HYPER_V_ADMINS",
-    "HI": "ML_HIGH",
-    "IS": "IIS_USERS",
-    "IU": "INTERACTIVE",
-    "KA": "KEY_ADMINS",
-    "LA": "LOCAL_ADMIN",
-    "LG": "LOCAL_GUEST",
-    "LS": "LOCAL_SERVICE",
-    "LU": "PERFLOG_USERS",
-    "LW": "ML_LOW",
-    "ME": "ML_MEDIUM",
-    "MP": "ML_MEDIUM_PLUS",
-    "MU": "PERFMON_USERS",
-    "NO": "NETWORK_CONFIGURATION_OPS",
-    "NS": "NETWORK_SERVICE",
-    "NU": "NETWORK",
-    "OW": "OWNER_RIGHTS",
-    "PA": "GROUP_POLICY_ADMINS",
-    "PO": "PRINTER_OPERATORS",
-    "PS": "PERSONAL_SELF",
-    "PU": "POWER_USERS",
-    "RA": "RDS_REMOTE_ACCESS_SERVERS",
-    "RC": "RESTRICTED_CODE",
-    "RD": "REMOTE_DESKTOP",
-    "RE": "REPLICATOR",
-    "RM": "RMS__SERVICE_OPERATORS",
-    "RO": "ENTERPRISE_RO_DCs",
-    "RS": "RAS_SERVERS",
-    "RU": "ALIAS_PREW2KCOMPACC",
-    "SA": "SCHEMA_ADMINISTRATORS",
-    "SI": "ML_SYSTEM",
-    "SO": "SERVER_OPERATORS",
-    "SS": "SERVICE_ASSERTED",
-    "SU": "SERVICE",
-    "SY": "LOCAL_SYSTEM",
-    "UD": "USER_MODE_DRIVERS",
-    "WD": "EVERYONE",
-    "WR": "WRITE_RESTRICTED_CODE",
+# Well known SIDs
+SDDL_SIDS = {
+    "AA": SIDEnum.ACCESS_CONTROL_ASSISTANCE_OPS,
+    "AC": SIDEnum.ALL_APP_PACKAGES,
+    "AN": SIDEnum.ANONYMOUS,
+    "AO": SIDEnum.ACCOUNT_OPERATORS,
+    "AP": SIDEnum.PROTECTED_USERS,
+    "AU": SIDEnum.AUTHENTICATED_USERS,
+    "BA": SIDEnum.BUILTIN_ADMINISTRATORS,
+    "BG": SIDEnum.BUILTIN_GUESTS,
+    "BO": SIDEnum.BACKUP_OPERATORS,
+    "BU": SIDEnum.BUILTIN_USERS,
+    "CA": SIDEnum.CERT_SERV_ADMINISTRATORS,
+    "CD": SIDEnum.CERTSVC_DCOM_ACCESS,
+    "CG": SIDEnum.CREATOR_GROUP,
+    "CN": SIDEnum.CLONEABLE_CONTROLLERS,
+    "CO": SIDEnum.CREATOR_OWNER,
+    "CY": SIDEnum.CRYPTO_OPERATORS,
+    "DA": SIDEnum.DOMAIN_ADMINISTRATORS,
+    "DC": SIDEnum.DOMAIN_COMPUTERS,
+    "DD": SIDEnum.DOMAIN_DOMAIN_CONTROLLERS,
+    "DG": SIDEnum.DOMAIN_GUESTS,
+    "DU": SIDEnum.DOMAIN_USERS,
+    "EA": SIDEnum.ENTERPRISE_ADMINS,
+    "ED": SIDEnum.ENTERPRISE_DOMAIN_CONTROLLERS,
+    "EK": SIDEnum.ENTERPRISE_KEY_ADMINS,
+    "ER": SIDEnum.EVENT_LOG_READERS,
+    "ES": SIDEnum.RDS_ENDPOINT_SERVERS,
+    "HA": SIDEnum.HYPER_V_ADMINS,
+    "HI": SIDEnum.ML_HIGH,
+    "IS": SIDEnum.IIS_USERS,
+    "IU": SIDEnum.INTERACTIVE,
+    "KA": SIDEnum.KEY_ADMINS,
+    "LA": SIDEnum.LOCAL_ADMIN,
+    "LG": SIDEnum.LOCAL_GUEST,
+    "LS": SIDEnum.LOCAL_SERVICE,
+    "LU": SIDEnum.PERFLOG_USERS,
+    "LW": SIDEnum.ML_LOW,
+    "ME": SIDEnum.ML_MEDIUM,
+    "MP": SIDEnum.ML_MEDIUM_PLUS,
+    "MU": SIDEnum.PERFMON_USERS,
+    "NO": SIDEnum.NETWORK_CONFIGURATION_OPS,
+    "NS": SIDEnum.NETWORK_SERVICE,
+    "NU": SIDEnum.NETWORK,
+    "OW": SIDEnum.OWNER_RIGHTS,
+    "PA": SIDEnum.GROUP_POLICY_ADMINS,
+    "PO": SIDEnum.PRINTER_OPERATORS,
+    "PS": SIDEnum.PERSONAL_SELF,
+    "PU": SIDEnum.POWER_USERS,
+    "RA": SIDEnum.RDS_REMOTE_ACCESS_SERVERS,
+    "RC": SIDEnum.RESTRICTED_CODE,
+    "RD": SIDEnum.REMOTE_DESKTOP,
+    "RE": SIDEnum.REPLICATOR,
+    "RM": SIDEnum.RMS__SERVICE_OPERATORS,
+    "RO": SIDEnum.ENTERPRISE_RO_DCs,
+    "RS": SIDEnum.RAS_SERVERS,
+    "RU": SIDEnum.ALIAS_PREW2KCOMPACC,
+    "SA": SIDEnum.SCHEMA_ADMINISTRATORS,
+    "SI": SIDEnum.ML_SYSTEM,
+    "SO": SIDEnum.SERVER_OPERATORS,
+    "SS": SIDEnum.SERVICE_ASSERTED,
+    "SU": SIDEnum.SERVICE,
+    "SY": SIDEnum.LOCAL_SYSTEM,
+    "UD": SIDEnum.USER_MODE_DRIVERS,
+    "WD": SIDEnum.EVERYONE,
+    "WR": SIDEnum.WRITE_RESTRICTED_CODE,
 }
 
+
 SDDL_FLAGS = {
-    # Order matters because of the way the flags are checked
-    "PAI": "PROTECTED|SDDL_AUTO_INHERITED",
-    "AR": "SDDL_AUTO_INHERIT_REQ",
-    "AI": "SDDL_AUTO_INHERITED",
-    "P": "PROTECTED",
-    "": "NULL_DACL",
+    "AR": SDDLFlags.SDDL_AUTO_INHERIT_REQ,
+    "AI": SDDLFlags.SDDL_AUTO_INHERITED,
+    "P": SDDLFlags.PROTECTED,
+    "NO_ACCESS_CONTROL": SDDLFlags.NO_ACCESS_CONTROL,
 }
```

### Comparing `sddl_parser-0.2.0/sddl_parser/parser.py` & `sddl_parser-0.3.0/sddl_parser/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from parsy import string, regex, char_from, seq, test_char, Parser, generate
 from functools import reduce
 from operator import or_
 from typing import List, Dict, Any, Callable
 from functools import partial
-from sddl_parser.dictionary import (
+from sddl_parser.well_known_dictionary import (
     SDDL_SIDS,
     SDDL_FLAGS,
     ACE_TYPE,
     ACE_FLAGS,
     ACE_RIGHTS,
 )
-from sddl_parser.types import ACE, DACL, SDDL, SACL
+from sddl_parser.types import ACE, SDDL, ACL
+from sddl_parser.enums import SDDLFlags
 
 
 def parser_from_list(xs: List[str]) -> Parser:
     if not xs:
         raise ValueError("list is empty")
     return reduce(or_, map(string, xs))
 
@@ -63,26 +64,34 @@
 def parse_group() -> Parser:
     group_identifier = string("G:")
     return group_identifier >> parse_sid_field()
 
 
 sacl_identifier = string("S:")
 dacl_identifier = string("D:")
-sddl_flags = create_parser_from_dict(SDDL_FLAGS).map(lambda x: x.split("|"))
+
+
+def parse_sddl_flags() -> Parser:
+    def map_flags(xs: List[str]):
+        if xs == []:
+            return {SDDLFlags.NO_ACCESS_CONTROL}
+        return {SDDL_FLAGS[x] for x in xs}
+
+    return parser_from_list(list(SDDL_FLAGS)).many().map(map_flags)
+
 
 ace_types = create_parser_from_dict(ACE_TYPE, lambda xs, k: xs[k])
 
 
 def parse_ace_flags() -> Parser:
-    def flags_map(x: str) -> List[str]:
-        split_by_two = map("".join, zip(*[iter(x)] * 2))
-        return list(map(lambda x: ACE_FLAGS[x][0], split_by_two))
-
-    # TODO: Actually parse here instead of just grabbing till ;
-    return (take_till_char(";").map(flags_map)) | string("")
+    return (
+        parser_from_list(list(ACE_FLAGS.keys()))
+        .many()
+        .map(lambda xs: set(map(lambda x: ACE_FLAGS[x], xs)))
+    )
 
 
 def parse_ace_rights() -> Parser:
     hex_ace_rights = regex(r"0x[0-9a-fA-F]+").map(lambda x: int(x, 16))
 
     well_known_ace_rights = (
         parser_from_list(list(ACE_RIGHTS.keys()))
@@ -138,20 +147,20 @@
             conditional_ace=parse_conditional_ace().optional(),
         )
         << string(")")
     ).combine_dict(ACE)
 
 
 dacl = seq(
-    flags=dacl_identifier >> sddl_flags, aces=parse_ace_entry().many()
-).combine_dict(DACL)
+    flags=dacl_identifier >> parse_sddl_flags(), aces=parse_ace_entry().many()
+).combine_dict(ACL)
 
 sacl = seq(
-    flags=sacl_identifier >> sddl_flags, aces=parse_ace_entry().many()
-).combine_dict(SACL)
+    flags=sacl_identifier >> parse_sddl_flags(), aces=parse_ace_entry().many()
+).combine_dict(ACL)
 
 
 # https://learn.microsoft.com/en-us/windows/win32/secauthz/sid-strings?source=recommendations
 # Example: O:SYG:SYD:(A;ID;FA;;;SY)
 # TODO: Allow entries to be out of order.
 # Something like sddl_item = parse_owner() | parse_group() | dacl | sacl
 # Then sddl_entry = sddl_item.many(), then just map each type to a single object
```

### Comparing `sddl_parser-0.2.0/sddl_parser/rights_enums.py` & `sddl_parser-0.3.0/sddl_parser/ace_rights_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from enum import IntEnum
 
-# TODO: Maybe when I get bored one day, I'll make a class for subclassing enums. Why isn't that implemented already? Probably a good reason
-
 
 class GenericAccessRights(IntEnum):
     ACCESS0 = 0x1
     ACCESS1 = 0x2
     ACCESS2 = 0x4
     ACCESS3 = 0x8
     ACCESS4 = 0x10
@@ -156,41 +154,14 @@
         GenericAccessRights.STANDARD_RIGHTS_EXECUTE
         | FILE_READ_ATTRIBUTES
         | FILE_EXECUTE
         | SYNCHRONIZE
     )
 
 
-class FileDirectoryAccessRights(IntEnum):
-    """
-    https://learn.microsoft.com/en-us/windows/win32/fileio/file-access-rights-constants
-    """
-
-    FILE_LIST_DIRECTORY = GenericAccessRights.ACCESS0
-    FILE_ADD_FILE = GenericAccessRights.ACCESS1
-    FILE_ADD_SUBDIRECTORY = GenericAccessRights.ACCESS2
-    FILE_READ_EA = GenericAccessRights.ACCESS3
-    FILE_WRITE_EA = GenericAccessRights.ACCESS4
-    FILE_TRAVERSE = GenericAccessRights.ACCESS5
-    FILE_DELETE_CHILD = GenericAccessRights.ACCESS6
-    FILE_READ_ATTRIBUTES = GenericAccessRights.ACCESS7
-    FILE_WRITE_ATTRIBUTES = GenericAccessRights.ACCESS8
-    GENERIC_READ = GenericAccessRights.GENERIC_READ
-    GENERIC_WRITE = GenericAccessRights.GENERIC_WRITE
-    GENERIC_EXECUTE = GenericAccessRights.GENERIC_EXECUTE
-    GENERIC_ALL = GenericAccessRights.GENERIC_ALL
-    DELETE = GenericAccessRights.DELETE
-    READ_CONTROL = GenericAccessRights.READ_CONTROL
-    WRITE_DAC = GenericAccessRights.WRITE_DAC
-    WRITE_OWNER = GenericAccessRights.WRITE_OWNER
-    SYNCHRONIZE = GenericAccessRights.SYNCHRONIZE
-    MAXIMUM_ALLOWED = GenericAccessRights.MAXIMUM_ALLOWED
-    ACCESS_SYSTEM_SECURITY = GenericAccessRights.ACCESS_SYSTEM_SECURITY
-
-
 class RegistryKeyAccessRights(IntEnum):
     """
     https://learn.microsoft.com/en-us/windows/win32/sysinfo/registry-key-security-and-access-rights
     """
 
     KEY_QUERY_VALUE = GenericAccessRights.ACCESS0
     KEY_SET_VALUE = GenericAccessRights.ACCESS1
@@ -340,14 +311,18 @@
     WRITE_OWNER = GenericAccessRights.WRITE_OWNER
     SYNCHRONIZE = GenericAccessRights.SYNCHRONIZE
     MAXIMUM_ALLOWED = GenericAccessRights.MAXIMUM_ALLOWED
     ACCESS_SYSTEM_SECURITY = GenericAccessRights.ACCESS_SYSTEM_SECURITY
 
 
 class FileDirectoryAccessRights(IntEnum):
+    """
+    https://learn.microsoft.com/en-us/windows/win32/fileio/file-access-rights-constants
+    """
+
     FILE_LIST_DIRECTORY = GenericAccessRights.ACCESS0
     FILE_ADD_FILE = GenericAccessRights.ACCESS1
     FILE_ADD_SUBDIRECTORY = GenericAccessRights.ACCESS2
     FILE_READ_EA = GenericAccessRights.ACCESS3
     FILE_WRITE_EA = GenericAccessRights.ACCESS4
     FILE_TRAVERSE = GenericAccessRights.ACCESS5
     FILE_DELETE_CHILD = GenericAccessRights.ACCESS6
@@ -1086,7 +1061,59 @@
     GENERIC_ALL = GenericAccessRights.GENERIC_ALL
     DELETE = GenericAccessRights.DELETE
     READ_CONTROL = GenericAccessRights.READ_CONTROL
     WRITE_DAC = GenericAccessRights.WRITE_DAC
     WRITE_OWNER = GenericAccessRights.WRITE_OWNER
     MAXIMUM_ALLOWED = GenericAccessRights.MAXIMUM_ALLOWED
     ACCESS_SYSTEM_SECURITY = GenericAccessRights.ACCESS_SYSTEM_SECURITY
+
+
+# TODO: Maybe when I get bored one day, I'll make a class for subclassing enums. Why isn't that implemented already? Probably a good reason
+
+AllRightsT = (
+    AlpcAccessRights
+    | AuditAccessRights
+    | DebugAccessRights
+    | DesktopAccessRights
+    | DirectoryAccessRights
+    | DirectoryServiceAccessRights
+    | EnlistmentAccessRights
+    | EventAccessRights
+    | FileAccessRights
+    | FileDirectoryAccessRights
+    | FilterConnectionPortAccessRights
+    | FirewallAccessRights
+    | FirewallFilterAccessRights
+    | GenericAccessRights
+    | IoCompletionAccessRights
+    | JobAccessRights
+    | KeyAccessRights
+    | LsaAccountAccessRights
+    | LsaPolicyAccessRights
+    | LsaSecretAccessRights
+    | LsaTrustedDomainAccessRights
+    | MemoryPartitionAccessRights
+    | MutantAccessRights
+    | PrintSpoolerAccessRights
+    | ProcessAccessRights
+    | RegistryKeyAccessRights
+    | RegistryTransactionAccessRights
+    | ResourceManagerAccessRights
+    | SamAliasAccessRights
+    | SamDomainAccessRights
+    | SamGroupAccessRights
+    | SamServerAccessRights
+    | SamUserAccessRights
+    | SemaphoreAccessRights
+    | ServiceAccessRights
+    | ServiceControlManagerAccessRights
+    | SessionAccessRights
+    | SymbolicLinkAccessRights
+    | ThreadAccessRights
+    | TimerAccessRights
+    | TokenAccessRights
+    | TraceAccessRights
+    | TransactionAccessRights
+    | TransactionManagerAccessRights
+    | WindowStationAccessRights
+    | WnfAccessRights
+)
```

### Comparing `sddl_parser-0.2.0/sddl_parser/type_enums.py` & `sddl_parser-0.3.0/sddl_parser/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,27 @@
-from enum import IntEnum
+from enum import IntEnum, Enum, auto
+
+
+class SDDLFlags(Enum):
+    SDDL_AUTO_INHERIT_REQ = auto()
+    SDDL_AUTO_INHERITED = auto()
+    PROTECTED = auto()
+    NO_ACCESS_CONTROL = auto()
+
+
+class AceFlags(IntEnum):
+    OBJECT_INHERIT = 0x01
+    CONTAINER_INHERIT = 0x02
+    NO_PROPAGATE = 0x04
+    INHERIT_ONLY = 0x08
+    INHERITED = 0x10
+    AUDIT_SUCCESS = 0x40
+    TRUST_PROTECTED_FILTER = 0x40
+    AUDIT_FAILURE = 0x80
+    # CRITICAL_ACE_FLAG - Can't find this value
 
 
 class AceType(IntEnum):
     ACCESS_ALLOWED = 0x0
     ACCESS_DENIED = 0x1
     SYSTEM_AUDIT = 0x2
     SYSTEM_ALARM = 0x3
```

