# Comparing `tmp/qtgql-0.119.0.tar.gz` & `tmp/qtgql-0.119.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.0.tar", max compression
+gzip compressed data, was "qtgql-0.119.1.tar", max compression
```

## Comparing `qtgql-0.119.0.tar` & `qtgql-0.119.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-05-24 10:34:56.987851 qtgql-0.119.0/LICENSE
--rw-r--r--   0        0        0     1901 2023-05-24 10:34:56.987851 qtgql-0.119.0/README.md
--rw-r--r--   0        0        0     4363 2023-05-24 10:35:21.272295 qtgql-0.119.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1700 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    11706 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3500 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2065 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      413 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17696 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    10489 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1506 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      541 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     2826 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     2785 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     2034 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-05-24 10:34:57.003852 qtgql-0.119.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 qtgql-0.119.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 15:09:49.035745 qtgql-0.119.1/LICENSE
+-rw-r--r--   0        0        0     1805 2023-05-24 15:09:49.035745 qtgql-0.119.1/README.md
+-rw-r--r--   0        0        0     4363 2023-05-24 15:10:06.287816 qtgql-0.119.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1761 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    11706 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3631 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2065 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      413 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17696 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    10489 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1566 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      541 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     2826 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     2869 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     2028 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.1/PKG-INFO
```

### Comparing `qtgql-0.119.0/LICENSE` & `qtgql-0.119.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/README.md` & `qtgql-0.119.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 This project is currently under development, and **it is not** production ready,
 You can play-around and tell us what is wrong / missing / awesome :smile:.
 
 [Visit the docs for more info](https://nrbnlulu.github.io/qtgql/) (WIP)
 
 
 ### Features
-- [ ] object types, for each field there is a corresponding `Property`
+- [x] object types, for each field there is a corresponding `Q_PROPERTY`
 - [ ] enums
 - [ ] custom scalars
 - [ ] Unions
 - [ ] interfaces
 - [ ] Garbage collection
-- [ ] Type-safe Mutation handlers
-- [ ] Type-safe Query handlers: queries your server when a component uses this query (or imperatively fetched).
-- [ ] Query updates: fetch the same query multiple times would not instantiate everything from scratch
+- [ ] Type-safe operation handlers
+  - [x] Query.
+  - [ ] Mutations.
+  - [ ] Subscriptions.
+- [ ] updates: fetch the same query multiple times would not instantiate everything from scratch
 it would compare the current data with data received and emit __only__ the signals that are needed.
 - [x] Native-Qt client implementation of "[graphql-transport-ws](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md)" protocol (supports subscriptions) - You can provide your own network layer though.
-- [ ] Mutations.
-- [ ] Subscriptions.
 - [ ] Fully typed input variables.
```

### Comparing `qtgql-0.119.0/pyproject.toml` & `qtgql-0.119.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.0"
+version = "0.119.1"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.119.0/qtgqlcodegen/cli.py` & `qtgql-0.119.1/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.1/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-from typing import Any
+from functools import cached_property
 from typing import NewType
 from typing import Optional
 
 from attr import define
 
 CType = NewType("CType", str)
 
 
-@define
+@define(slots=False)
 class BuiltinScalar:
     tp: CType
-    default_value: Any
+    defaults_member_name: str
     graphql_name: str
     from_json_convertor: str
 
+    @cached_property
+    def default_value(self) -> str:
+        return f"qtgql::bases::DEFAULTS::{self.defaults_member_name}"
+
 
 class _BuiltinScalars:
     INT = BuiltinScalar(
         CType("int"),
-        "qtgql::DEFAULTS::INT",
+        "INT",
         graphql_name="Int",
         from_json_convertor="toInt()",
     )
     FLOAT = BuiltinScalar(
         CType("float"),
-        "qtgql::DEFAULTS::FLOAT",
+        "FLOAT",
         graphql_name="Float",
         from_json_convertor="toDouble()",
     )
     STRING = BuiltinScalar(
         CType("QString"),
-        "qtgql::DEFAULTS::STRING",
+        "STRING",
         graphql_name="String",
         from_json_convertor="toString()",
     )
     ID = BuiltinScalar(
         CType("QString"),
-        "qtgql::DEFAULTS::ID",
+        "ID",
         graphql_name="ID",
         from_json_convertor="toString()",
     )
     BOOLEAN = BuiltinScalar(
         CType("bool"),
-        "qtgql::DEFAULTS::BOOL",
+        "BOOL",
         graphql_name="Boolean",
         from_json_convertor="toBool()",
     )
     UUID = BuiltinScalar(
         CType("QUuid"),
-        "qtgql::DEFAULTS::UUID",
+        "UUID",
         graphql_name="UUID",
         from_json_convertor="toVariant().toUuid()",
     )
 
     @classmethod
     def __iter__(cls):
         for name, member in cls.__dict__.items():
```

### Comparing `qtgql-0.119.0/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.1/qtgqlcodegen/compiler/operation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.1/qtgqlcodegen/compiler/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,19 @@
     types: list[QtGqlObjectTypeDefinition]
     interfaces: list[QtGqlInterfaceDefinition]
     input_objects: list[QtGqlInputObjectTypeDefinition]
     config: QtGqlConfig
 
     @property
     def dependencies(self) -> list[str]:
-        return [f"#include {scalar.include_path}" for scalar in self.config.custom_scalars.values()]
+        ret: list[str] = []
+        for scalar in self.config.custom_scalars.values():
+            if scalar.include_path not in ret:
+                ret.append(scalar.include_path)
+        return [f"#include {inc}" for inc in ret]
 
     @property
     def custom_scalars(self) -> list[str]:
         return [scalar.graphql_name for scalar in self.config.custom_scalars.values()]
 
 
 @define(slots=False)
```

### Comparing `qtgql-0.119.0/qtgqlcodegen/config.py` & `qtgql-0.119.1/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.1/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/introspection.py` & `qtgql-0.119.1/qtgqlcodegen/introspection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/objecttype.py` & `qtgql-0.119.1/qtgqlcodegen/objecttype.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.1/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,37 +8,37 @@
     deserialized_type: str
     property_type: str
     include_path: str
 
 
 # An ISO-8601 encoded datetime.
 DateTimeScalarDefinition = CustomScalarDefinition(
-    type_name="qtgql::DateTimeScalar",
+    type_name="qtgql::customscalars::DateTimeScalar",
     graphql_name="DateTime",
     deserialized_type="QDateTime",
     property_type="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 DateScalarDefinition = CustomScalarDefinition(
-    type_name="qtgql::DateScalar",
+    type_name="qtgql::customscalars::DateScalar",
     graphql_name="Date",
     deserialized_type="QDate",
     property_type="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 TimeScalarDefinition = CustomScalarDefinition(
-    type_name="qtgql::TimeScalar",
+    type_name="qtgql::customscalars::TimeScalar",
     graphql_name="Time",
     deserialized_type="QTime",
     property_type="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 
 DecimalScalarDefinition = CustomScalarDefinition(
-    type_name="qtgql::DecimalScalar",
+    type_name="qtgql::customscalars::DecimalScalar",
     graphql_name="Decimal",
     deserialized_type="QString",
     property_type="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
```

### Comparing `qtgql-0.119.0/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.1/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.119.1/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.1/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 {% import "macros.jinja.hpp" as macros -%}
 #pragma once
 #include "./schema.hpp"
-#include <qtgql/gqlwstransport/operationhandler.hpp>
+#include <qtgql/gqlwstransport/gqlwstransport.hpp>
+
 namespace 👉 context.config.env_name 👈{
 namespace 👉context.ns👈{
 
-inline const qtgql::OperationMetadata OPERATION_METADATA = qtgql::OperationMetadata{
+inline const qtgql::bases::OperationMetadata OPERATION_METADATA = qtgql::bases::OperationMetadata{
         "👉 context.operation.name 👈",
         {
                 👉 context.operation.root_field.as_conf_string() 👈
         }
 };
 
 
@@ -20,39 +21,39 @@
  */
     Q_GADGET
 std::shared_ptr<👉context.schema_ns👈::👉 t.definition.name 👈> m_inst;
 
 public:
 
 👉 t.name 👈(const QJsonObject& data,
-const qtgql::SelectionsConfig& config){
+const qtgql::bases::SelectionsConfig& config){
     m_inst = 👉context.schema_ns👈::👉 t.definition.name 👈::from_json(data, config, OPERATION_METADATA);
 
 }
 {%- for f in t.fields.values() %}
 inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
     return m_inst->👉 f.definition.getter_name 👈();
 };
 {% endfor -%}
 };
 {% endfor %}
 
-class 👉 context.operation.name 👈: public qtgql::OperationHandlerABC {
+class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC {
     Q_OBJECT
 Q_PROPERTY(const 👉 context.operation.root_field.property_type 👈* data READ get_data NOTIFY dataChanged);
 
 std::unique_ptr<👉 context.operation.root_field.property_type 👈> m_data;
 
 inline const QString &ENV_NAME() override{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
 public:
 
-👉 context.operation.name 👈(): qtgql::OperationHandlerABC(qtgql::GqlWsTrnsMsgWithID(qtgql::OperationPayload(
+👉 context.operation.name 👈(): qtgql::gqlwstransport::OperationHandlerABC(qtgql::gqlwstransport::GqlWsTrnsMsgWithID(qtgql::gqlwstransport::OperationPayload(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
         ))){};
 
 inline const QUuid &operation_id() const override{
 return m_message_template.op_id;
 }
```

### Comparing `qtgql-0.119.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.1/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 {% import "macros.jinja.hpp" as macros -%}
 #pragma once
 #include <QObject>
 #include <QJsonObject>
 #include <memory>
-#include <qtgql/bases/objecttype.hpp>
-#include <qtgql/bases/metadata.hpp>
-#include <qtgql/bases/constants.hpp>
-{% for dep in context.dependencies %}
+
+#include <qtgql/bases/bases.hpp>
+{% for dep in context.dependencies -%}
 👉 dep 👈
 {% endfor %}
 
 namespace 👉 context.config.env_name 👈{
 
 // ----------- Object Types -----------
 {% for type in context.types %}
 {%- set base_class -%}{% if type.has_id_field %}ObjectTypeABCWithID{% else %}ObjectTypeABC{% endif %}{%- endset -%}
-class 👉 type.name 👈 : public qtgql::👉 base_class 👈{
+class 👉 type.name 👈 : public qtgql::bases::👉 base_class 👈{
 protected:
 static auto & INST_STORE() {
-    static qtgql::ObjectStore<👉 type.name 👈> _store;
+    static qtgql::bases::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
 
 👉 macros.props(type) 👈
 public:
 inline static const QString TYPE_NAME = "👉 type.name 👈";
 👉 type.name 👈 (QObject* parent = nullptr)
-: qtgql::👉 base_class 👈::👉 base_class 👈(parent) {};
+: qtgql::bases::👉 base_class 👈::👉 base_class 👈(parent) {};
 
 
 static std::shared_ptr<👉 type.name 👈> from_json(const QJsonObject& data,
-                                 const qtgql::SelectionsConfig& config,
-                                 const qtgql::OperationMetadata& metadata){
+                                 const qtgql::bases::SelectionsConfig& config,
+                                 const qtgql::bases::OperationMetadata& metadata){
 auto inst = std::make_shared<👉 type.name 👈>();
 {% for f in type.fields -%}
 {% set assign_to %} inst->👉 f.private_name 👈 {% endset %}
 👉macros.deserialize_field(f, assign_to)👈
 {% endfor %}
 
 {% if type.id_is_optional %}
 if (inst->id) {
-  auto record = NodeRecord(node = inst, retainers = set())
+  auto record = qtgql::bases::NodeRecord(node = inst, retainers = set())
                     .retain(metadata.operation_name)
                         cls.INST_STORE.add_record(record)
 }
 {% elif type.has_id_field and not type.id_is_optional %}
-auto record = std::make_shared<qtgql::NodeRecord<👉 type.name 👈>>(inst);
+auto record = std::make_shared<qtgql::bases::NodeRecord<👉 type.name 👈>>(inst);
 record->retain(metadata.operation_name);
 INST_STORE().add_record(record);
 {% endif %}
 return inst;
   };
 {% endfor %}
 
-void loose(const qtgql::OperationMetadata &metadata){throw "not implemented";};
+void loose(const qtgql::bases::OperationMetadata &metadata){throw "not implemented";};
 void update(const QJsonObject &data,
-            const qtgql::SelectionsConfig &selections){throw "not implemented";};
+            const qtgql::bases::SelectionsConfig &selections){throw "not implemented";};
 
 };
 
 }
```

### Comparing `qtgql-0.119.0/qtgqlcodegen/utils.py` & `qtgql-0.119.1/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.0/PKG-INFO` & `qtgql-0.119.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.0
+Version: 0.119.1
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -37,22 +37,22 @@
 This project is currently under development, and **it is not** production ready,
 You can play-around and tell us what is wrong / missing / awesome :smile:.
 
 [Visit the docs for more info](https://nrbnlulu.github.io/qtgql/) (WIP)
 
 
 ### Features
-- [ ] object types, for each field there is a corresponding `Property`
+- [x] object types, for each field there is a corresponding `Q_PROPERTY`
 - [ ] enums
 - [ ] custom scalars
 - [ ] Unions
 - [ ] interfaces
 - [ ] Garbage collection
-- [ ] Type-safe Mutation handlers
-- [ ] Type-safe Query handlers: queries your server when a component uses this query (or imperatively fetched).
-- [ ] Query updates: fetch the same query multiple times would not instantiate everything from scratch
+- [ ] Type-safe operation handlers
+  - [x] Query.
+  - [ ] Mutations.
+  - [ ] Subscriptions.
+- [ ] updates: fetch the same query multiple times would not instantiate everything from scratch
 it would compare the current data with data received and emit __only__ the signals that are needed.
 - [x] Native-Qt client implementation of "[graphql-transport-ws](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md)" protocol (supports subscriptions) - You can provide your own network layer though.
-- [ ] Mutations.
-- [ ] Subscriptions.
 - [ ] Fully typed input variables.
```

