# Comparing `tmp/pyjej-0.1.0.tar.gz` & `tmp/pyjej-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjej-0.1.0.tar", max compression
+gzip compressed data, was "pyjej-0.1.2.tar", max compression
```

## Comparing `pyjej-0.1.0.tar` & `pyjej-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6340 2023-05-24 19:10:39.662618 pyjej-0.1.0/README.md
--rw-r--r--   0        0        0      171 2023-05-24 19:10:03.865376 pyjej-0.1.0/pyjej/__main__.py
--rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.0/pyjej/selflib.py
--rw-r--r--   0        0        0     3006 2023-05-24 19:20:04.129146 pyjej-0.1.0/pyjej/tasks.py
--rw-r--r--   0        0        0      291 2023-05-24 19:11:46.840950 pyjej-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6841 1970-01-01 00:00:00.000000 pyjej-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7662 2023-05-24 20:03:42.364015 pyjej-0.1.2/README.md
+-rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.2/pyjej/__main__.py
+-rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.2/pyjej/selflib.py
+-rw-r--r--   0        0        0     3002 2023-05-24 20:06:14.371635 pyjej-0.1.2/pyjej/tasks.py
+-rw-r--r--   0        0        0      379 2023-05-24 20:07:59.571380 pyjej-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 pyjej-0.1.2/PKG-INFO
```

### Comparing `pyjej-0.1.0/README.md` & `pyjej-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,90 +9,122 @@
 -   Библиотека `pyyaml`
 
 ## Начало работы
 
 1. Клонируйте этот репозиторий на свой локальный компьютер.
 2. Установите необходимые зависимости, выполнив следующую команду:
     ```
-    pip install invoke pyyaml
+    poetry install
     ```
 3. Настройте информацию о сервере Jenkins в файле `inventory.yml`. Добавьте необходимую информацию о серверах Jenkins, с которыми вы хотите взаимодействовать.
 
+## Пример
+
+Вот пример использования задач:
+
+1. Экспорт всех заданий с сервера Jenkins:
+
+    ```
+    python -m pyjej job.export-all -s мой_сервер_jenkins
+    ```
+
+2. Создание задания на сервере Jenkins:
+
+    ```
+    python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    ```
+
+3. Обновление задания на сервере Jenkins:
+
+    ```
+    python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    ```
+
+4. Экспорт всех плагинов
+
+    ```
+    python -m pyjej plugins.export-all -s мой_сервер_jenkins
+    ```
+
+Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
+
 ## Использование
 
 ### tasks.py
 
-Этот файл содержит основные задачи для взаимодействия с Jenkins.
+В этом файле содержатся основные задачи для взаимодействия с Jenkins.
 
-#### Задача `export_all_jobs`
+#### Задача `job.export-all`
 
 Эта задача экспортирует все задания с указанного сервера Jenkins и сохраняет их в виде файлов XML.
 
 **Использование:**
 
-```
+```shell
 python -m pyjej job.export-all --server <имя_сервера>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 
-#### Задача `create_job`
+#### Задача `job.create`
 
 Эта задача создает конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
-```
-invoke job.create --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+```shell
+python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для создания.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
-#### Задача `update_job`
+#### Задача `job.update`
 
 Эта задача обновляет конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
-```
-invoke job.update --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+```shell
+python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для обновления.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
-### selflib.py
+#### Задача `plugins.export-all`
 
-Этот файл содержит вспомогательные функции, используемые задачами в `tasks.py`.
+Эта задача позволяет получить список всех установленных плагинов на указанном сервере Jenkins.
 
-## Пример
+**Использование:**
 
-Вот пример использования задач:
+```shell
+python -m pyjej plugins.export-all --server <имя_сервера>
+```
 
-1. Экспорт всех заданий с сервера Jenkins:
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 
-    ```
-    invoke job.export-all --server мой_сервер_jenkins
-    ```
+Результат выполнения команды будет выведен на экран. Если у команды не было ошибок, список плагинов будет сохранен в файле `data/<имя_сервера>/plains.txt`.
 
-2. Создание задания на сервере Jenkins:
+#### Задача `plugins.install`
 
-    ```
-    invoke job.create --server мой_сервер_jenkins --jobname моё_задание --in_folder входная_папка
-    ```
+Эта задача позволяет установить указанный плагин на сервере Jenkins.
 
-3. Обновление задания на сервере Jenkins:
-    ```
-    invoke job.update --server мой_сервер_jenkins --jobname моё_задание --in_folder входная_папка
-    ```
+**Использование:**
 
-Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
+```shell
+python -m pyjej plugins.install --server <имя_сервера> --plugin <имя_плагина>
+```
+
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
+-   `<имя_плагина>`: Имя плагина, который нужно установить.
+
+Результат выполнения команды будет выведен на экран.
 
 # Пример создания файла inventory.yml
 
 Файл `inventory.yml` используется для настройки подключения к серверам Jenkins в коде. В этой главе мы предоставим пример создания файла `inventory.yml` с фиктивными значениями.
 
 Пример содержимого файла `inventory.yml`:
```

### Comparing `pyjej-0.1.0/pyjej/selflib.py` & `pyjej-0.1.2/pyjej/selflib.py`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.0/pyjej/tasks.py` & `pyjej-0.1.2/pyjej/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 @task
 def create_job(ctx, server: str, jobname: str, in_folder):
     """Создать указанную Job на Jenkins"""
     base_command_cli = INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
     res: Result = ctx.run(
-        f"{base_command_cli} create-job {jobname}_i < {pathlib.Path('data', in_folder,'jobs',f'{jobname}.xml')}",
+        f"{base_command_cli} create-job {jobname} < {pathlib.Path('data', in_folder,'jobs',f'{jobname}.xml')}",
     )
     print(res)
 
 
 @task
 def update_job(ctx, server: str, jobname: str, in_folder):
     """Обновить указанный Job в Jenkins"""
     base_command_cli = INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
     res: Result = ctx.run(
-        f"{base_command_cli} update-job {jobname}_i < {pathlib.Path('data',in_folder,'jobs',f'{jobname}.xml')}",
+        f"{base_command_cli} update-job {jobname} < {pathlib.Path('data',in_folder,'jobs',f'{jobname}.xml')}",
     )
     print(res)
 
 
 @task
 def export_all_plugins(ctx, server: str):
     """Получить список всех плагинов"""
```

### Comparing `pyjej-0.1.0/PKG-INFO` & `pyjej-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyjej
-Version: 0.1.0
-Summary: 
-Author: Your Name
-Author-email: you@example.com
+Version: 0.1.2
+Summary: Проект для взаимодействия с Jenkins через CLI
+Author: Кустов Денис
+Author-email: kudv@pkzdrav.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: invoke (>=2.1.2,<3.0.0)
@@ -25,90 +25,122 @@
 -   Библиотека `pyyaml`
 
 ## Начало работы
 
 1. Клонируйте этот репозиторий на свой локальный компьютер.
 2. Установите необходимые зависимости, выполнив следующую команду:
     ```
-    pip install invoke pyyaml
+    poetry install
     ```
 3. Настройте информацию о сервере Jenkins в файле `inventory.yml`. Добавьте необходимую информацию о серверах Jenkins, с которыми вы хотите взаимодействовать.
 
+## Пример
+
+Вот пример использования задач:
+
+1. Экспорт всех заданий с сервера Jenkins:
+
+    ```
+    python -m pyjej job.export-all -s мой_сервер_jenkins
+    ```
+
+2. Создание задания на сервере Jenkins:
+
+    ```
+    python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    ```
+
+3. Обновление задания на сервере Jenkins:
+
+    ```
+    python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    ```
+
+4. Экспорт всех плагинов
+
+    ```
+    python -m pyjej plugins.export-all -s мой_сервер_jenkins
+    ```
+
+Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
+
 ## Использование
 
 ### tasks.py
 
-Этот файл содержит основные задачи для взаимодействия с Jenkins.
+В этом файле содержатся основные задачи для взаимодействия с Jenkins.
 
-#### Задача `export_all_jobs`
+#### Задача `job.export-all`
 
 Эта задача экспортирует все задания с указанного сервера Jenkins и сохраняет их в виде файлов XML.
 
 **Использование:**
 
-```
+```shell
 python -m pyjej job.export-all --server <имя_сервера>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 
-#### Задача `create_job`
+#### Задача `job.create`
 
 Эта задача создает конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
-```
-invoke job.create --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+```shell
+python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для создания.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
-#### Задача `update_job`
+#### Задача `job.update`
 
 Эта задача обновляет конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
-```
-invoke job.update --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+```shell
+python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для обновления.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
-### selflib.py
+#### Задача `plugins.export-all`
 
-Этот файл содержит вспомогательные функции, используемые задачами в `tasks.py`.
+Эта задача позволяет получить список всех установленных плагинов на указанном сервере Jenkins.
 
-## Пример
+**Использование:**
 
-Вот пример использования задач:
+```shell
+python -m pyjej plugins.export-all --server <имя_сервера>
+```
 
-1. Экспорт всех заданий с сервера Jenkins:
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 
-    ```
-    invoke job.export-all --server мой_сервер_jenkins
-    ```
+Результат выполнения команды будет выведен на экран. Если у команды не было ошибок, список плагинов будет сохранен в файле `data/<имя_сервера>/plains.txt`.
 
-2. Создание задания на сервере Jenkins:
+#### Задача `plugins.install`
 
-    ```
-    invoke job.create --server мой_сервер_jenkins --jobname моё_задание --in_folder входная_папка
-    ```
+Эта задача позволяет установить указанный плагин на сервере Jenkins.
 
-3. Обновление задания на сервере Jenkins:
-    ```
-    invoke job.update --server мой_сервер_jenkins --jobname моё_задание --in_folder входная_папка
-    ```
+**Использование:**
 
-Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
+```shell
+python -m pyjej plugins.install --server <имя_сервера> --plugin <имя_плагина>
+```
+
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
+-   `<имя_плагина>`: Имя плагина, который нужно установить.
+
+Результат выполнения команды будет выведен на экран.
 
 # Пример создания файла inventory.yml
 
 Файл `inventory.yml` используется для настройки подключения к серверам Jenkins в коде. В этой главе мы предоставим пример создания файла `inventory.yml` с фиктивными значениями.
 
 Пример содержимого файла `inventory.yml`:
```

