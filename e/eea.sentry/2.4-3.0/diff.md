# Comparing `tmp/eea.sentry-2.4.zip` & `tmp/eea.sentry-3.0.zip`

## zipinfo {}

```diff
@@ -1,202 +1,252 @@
-Zip file size: 93676 bytes, number of entries: 200
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/
--rw-r--r--  2.0 unx       38 b- defN 22-Feb-17 13:58 eea.sentry-2.4/setup.cfg
--rw-r--r--  2.0 unx     2280 b- defN 22-Feb-17 13:58 eea.sentry-2.4/CONTRIBUTING.md
--rw-r--r--  2.0 unx     6955 b- defN 22-Feb-17 13:58 eea.sentry-2.4/PKG-INFO
--rw-r--r--  2.0 unx     4338 b- defN 22-Feb-17 13:58 eea.sentry-2.4/README.rst
--rw-r--r--  2.0 unx     1841 b- defN 22-Feb-17 13:58 eea.sentry-2.4/setup.py
--rw-r--r--  2.0 unx      126 b- defN 22-Feb-17 13:58 eea.sentry-2.4/MANIFEST.in
--rw-r--r--  2.0 unx       59 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6955 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        4 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/not-zip-safe
--rw-r--r--  2.0 unx       66 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/top_level.txt
--rw-r--r--  2.0 unx     4214 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea.sentry.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     1626 b- defN 22-Feb-17 13:58 eea.sentry-2.4/docs/HISTORY.txt
--rw-r--r--  2.0 unx      909 b- defN 22-Feb-17 13:58 eea.sentry-2.4/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 22-Feb-17 13:58 eea.sentry-2.4/docs/LICENSE.GPL
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/
--rw-r--r--  2.0 unx       80 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/cache/
--rw-r--r--  2.0 unx        4 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/version.txt
--rw-r--r--  2.0 unx      605 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/configure.zcml
--rw-r--r--  2.0 unx      850 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/setuphandlers.py
--rw-r--r--  2.0 unx      235 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/interfaces.py
--rw-r--r--  2.0 unx      832 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/processors.py
--rw-r--r--  2.0 unx      328 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/README.txt
--rw-r--r--  2.0 unx     1539 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles.zcml
--rw-r--r--  2.0 unx     6540 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/locales/de/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx      715 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/upgrades/configure.zcml
--rw-r--r--  2.0 unx       17 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/upgrades/__init__.py
--rw-r--r--  2.0 unx     1539 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/tests/base.py
--rw-r--r--  2.0 unx      660 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/js/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/zpt/
--rw-r--r--  2.0 unx      831 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/configure.zcml
--rw-r--r--  2.0 unx     3907 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/sentry.py
--rw-r--r--  2.0 unx       16 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/__init__.py
--rw-r--r--  2.0 unx     1446 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/js/sentry.js
--rw-r--r--  2.0 unx    99019 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/js/bundle.tracing.min.js
--rw-r--r--  2.0 unx      304 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/browser/zpt/sentry.pt
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/common/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/plone5/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/plone4/
--rw-r--r--  2.0 unx      120 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/uninstall/browserlayer.xml
--rw-r--r--  2.0 unx       87 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/common/metadata.xml
--rw-r--r--  2.0 unx      138 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/common/browserlayer.xml
--rw-r--r--  2.0 unx      158 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/plone5/metadata.xml
--rw-r--r--  2.0 unx      819 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/plone5/registry.xml
--rw-r--r--  2.0 unx      158 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/plone4/metadata.xml
--rw-r--r--  2.0 unx      279 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/profiles/plone4/jsregistry.xml
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/kgs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/plone5/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/plone4/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/eea/
--rw-r--r--  2.0 unx     2475 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/kgs/00_install_addon.js
--rw-r--r--  2.0 unx     2370 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/plone5/00_install_addon.js
--rw-r--r--  2.0 unx     2478 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/plone4/00_install_addon.js
--rw-r--r--  2.0 unx     2475 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/ftests/eea/00_install_addon.js
--rw-r--r--  2.0 unx      451 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/cache/nocache.py
--rw-r--r--  2.0 unx      421 b- defN 22-Feb-17 13:58 eea.sentry-2.4/eea/sentry/cache/__init__.py
-200 files, 179650 bytes uncompressed, 59882 bytes compressed:  66.7%
+Zip file size: 101049 bytes, number of entries: 250
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/
+-rw-r--r--  2.0 unx       38 b- defN 23-May-24 11:52 eea.sentry-3.0/setup.cfg
+-rw-r--r--  2.0 unx     2280 b- defN 23-May-24 11:51 eea.sentry-3.0/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     7079 b- defN 23-May-24 11:52 eea.sentry-3.0/PKG-INFO
+-rw-r--r--  2.0 unx     4338 b- defN 23-May-24 11:51 eea.sentry-3.0/README.rst
+-rw-r--r--  2.0 unx     1841 b- defN 23-May-24 11:51 eea.sentry-3.0/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 23-May-24 11:51 eea.sentry-3.0/MANIFEST.in
+-rw-r--r--  2.0 unx       59 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     7079 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        4 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       66 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     6599 b- defN 23-May-24 11:52 eea.sentry-3.0/eea.sentry.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     1750 b- defN 23-May-24 11:51 eea.sentry-3.0/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      909 b- defN 23-May-24 11:51 eea.sentry-3.0/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 23-May-24 11:51 eea.sentry-3.0/docs/LICENSE.GPL
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/
+-rw-r--r--  2.0 unx       80 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/profiles/
+-rw-r--r--  2.0 unx        4 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/version.txt
+-rw-r--r--  2.0 unx      605 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/configure.zcml
+-rw-r--r--  2.0 unx      850 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/setuphandlers.py
+-rw-r--r--  2.0 unx      235 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/interfaces.py
+-rw-r--r--  2.0 unx      832 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/processors.py
+-rw-r--r--  2.0 unx      328 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/README.txt
+-rw-r--r--  2.0 unx     1539 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles.zcml
+-rw-r--r--  2.0 unx     6540 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 11:52 eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/plone.po
+-rw-r--r--  2.0 unx      715 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/upgrades/configure.zcml
+-rw-r--r--  2.0 unx       17 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/upgrades/__init__.py
+-rw-r--r--  2.0 unx     1539 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/tests/base.py
+-rw-r--r--  2.0 unx      660 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/browser/js/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/browser/zpt/
+-rw-r--r--  2.0 unx      831 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/browser/configure.zcml
+-rw-r--r--  2.0 unx     3755 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/browser/sentry.py
+-rw-r--r--  2.0 unx       16 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/browser/__init__.py
+-rw-r--r--  2.0 unx     1446 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/browser/js/sentry.js
+-rw-r--r--  2.0 unx    99019 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/browser/js/bundle.tracing.min.js
+-rw-r--r--  2.0 unx      304 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/browser/zpt/sentry.pt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/profiles/common/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/profiles/plone5/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 11:52 eea.sentry-3.0/eea/sentry/profiles/plone4/
+-rw-r--r--  2.0 unx      120 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/uninstall/browserlayer.xml
+-rw-r--r--  2.0 unx       87 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/common/metadata.xml
+-rw-r--r--  2.0 unx      138 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/common/browserlayer.xml
+-rw-r--r--  2.0 unx      158 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/plone5/metadata.xml
+-rw-r--r--  2.0 unx      819 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/plone5/registry.xml
+-rw-r--r--  2.0 unx      158 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/plone4/metadata.xml
+-rw-r--r--  2.0 unx      279 b- defN 23-May-24 11:51 eea.sentry-3.0/eea/sentry/profiles/plone4/jsregistry.xml
+250 files, 173321 bytes uncompressed, 57555 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,601 +1,751 @@
-Filename: eea.sentry-2.4/
+Filename: eea.sentry-3.0/
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/
+Filename: eea.sentry-3.0/eea.sentry.egg-info/
 Comment: 
 
-Filename: eea.sentry-2.4/docs/
+Filename: eea.sentry-3.0/docs/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/
+Filename: eea.sentry-3.0/eea/
 Comment: 
 
-Filename: eea.sentry-2.4/setup.cfg
+Filename: eea.sentry-3.0/setup.cfg
 Comment: 
 
-Filename: eea.sentry-2.4/CONTRIBUTING.md
+Filename: eea.sentry-3.0/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.sentry-2.4/PKG-INFO
+Filename: eea.sentry-3.0/PKG-INFO
 Comment: 
 
-Filename: eea.sentry-2.4/README.rst
+Filename: eea.sentry-3.0/README.rst
 Comment: 
 
-Filename: eea.sentry-2.4/setup.py
+Filename: eea.sentry-3.0/setup.py
 Comment: 
 
-Filename: eea.sentry-2.4/MANIFEST.in
+Filename: eea.sentry-3.0/MANIFEST.in
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/entry_points.txt
+Filename: eea.sentry-3.0/eea.sentry.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/dependency_links.txt
+Filename: eea.sentry-3.0/eea.sentry.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/PKG-INFO
+Filename: eea.sentry-3.0/eea.sentry.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/namespace_packages.txt
+Filename: eea.sentry-3.0/eea.sentry.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/not-zip-safe
+Filename: eea.sentry-3.0/eea.sentry.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/requires.txt
+Filename: eea.sentry-3.0/eea.sentry.egg-info/requires.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/top_level.txt
+Filename: eea.sentry-3.0/eea.sentry.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea.sentry.egg-info/SOURCES.txt
+Filename: eea.sentry-3.0/eea.sentry.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.sentry-2.4/docs/HISTORY.txt
+Filename: eea.sentry-3.0/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.sentry-2.4/docs/LICENSE.txt
+Filename: eea.sentry-3.0/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.sentry-2.4/docs/LICENSE.GPL
+Filename: eea.sentry-3.0/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/
+Filename: eea.sentry-3.0/eea/sentry/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/__init__.py
+Filename: eea.sentry-3.0/eea/__init__.py
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/
+Filename: eea.sentry-3.0/eea/sentry/locales/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/upgrades/
+Filename: eea.sentry-3.0/eea/sentry/upgrades/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/tests/
+Filename: eea.sentry-3.0/eea/sentry/tests/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/
+Filename: eea.sentry-3.0/eea/sentry/browser/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/
+Filename: eea.sentry-3.0/eea/sentry/profiles/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/
+Filename: eea.sentry-3.0/eea/sentry/version.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/cache/
+Filename: eea.sentry-3.0/eea/sentry/configure.zcml
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/version.txt
+Filename: eea.sentry-3.0/eea/sentry/setuphandlers.py
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/configure.zcml
+Filename: eea.sentry-3.0/eea/sentry/interfaces.py
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/setuphandlers.py
+Filename: eea.sentry-3.0/eea/sentry/processors.py
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/interfaces.py
+Filename: eea.sentry-3.0/eea/sentry/README.txt
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/processors.py
+Filename: eea.sentry-3.0/eea/sentry/profiles.zcml
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/README.txt
+Filename: eea.sentry-3.0/eea/sentry/__init__.py
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles.zcml
+Filename: eea.sentry-3.0/eea/sentry/locales/zh_TW/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/__init__.py
+Filename: eea.sentry-3.0/eea/sentry/locales/en/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/zh_TW/
+Filename: eea.sentry-3.0/eea/sentry/locales/hr/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/en/
+Filename: eea.sentry-3.0/eea/sentry/locales/es/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hr/
+Filename: eea.sentry-3.0/eea/sentry/locales/pt_BR/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/es/
+Filename: eea.sentry-3.0/eea/sentry/locales/ro/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt_BR/
+Filename: eea.sentry-3.0/eea/sentry/locales/eu/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ro/
+Filename: eea.sentry-3.0/eea/sentry/locales/el/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/eu/
+Filename: eea.sentry-3.0/eea/sentry/locales/it/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/el/
+Filename: eea.sentry-3.0/eea/sentry/locales/ru/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/it/
+Filename: eea.sentry-3.0/eea/sentry/locales/is/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ru/
+Filename: eea.sentry-3.0/eea/sentry/locales/lt/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/is/
+Filename: eea.sentry-3.0/eea/sentry/locales/hu/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lt/
+Filename: eea.sentry-3.0/eea/sentry/locales/nl/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hu/
+Filename: eea.sentry-3.0/eea/sentry/locales/pt/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/nl/
+Filename: eea.sentry-3.0/eea/sentry/locales/fi/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt/
+Filename: eea.sentry-3.0/eea/sentry/locales/lv/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fi/
+Filename: eea.sentry-3.0/eea/sentry/locales/sl/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lv/
+Filename: eea.sentry-3.0/eea/sentry/locales/mt/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sl/
+Filename: eea.sentry-3.0/eea/sentry/locales/tr/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/mt/
+Filename: eea.sentry-3.0/eea/sentry/locales/no/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/tr/
+Filename: eea.sentry-3.0/eea/sentry/locales/sv/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/no/
+Filename: eea.sentry-3.0/eea/sentry/locales/bg/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sv/
+Filename: eea.sentry-3.0/eea/sentry/locales/kl/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/bg/
+Filename: eea.sentry-3.0/eea/sentry/locales/et/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/kl/
+Filename: eea.sentry-3.0/eea/sentry/locales/sk/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/et/
+Filename: eea.sentry-3.0/eea/sentry/locales/pl/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sk/
+Filename: eea.sentry-3.0/eea/sentry/locales/cs/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pl/
+Filename: eea.sentry-3.0/eea/sentry/locales/da/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/cs/
+Filename: eea.sentry-3.0/eea/sentry/locales/fr/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/da/
+Filename: eea.sentry-3.0/eea/sentry/locales/de/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fr/
+Filename: eea.sentry-3.0/eea/sentry/locales/eea.pot
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/de/
+Filename: eea.sentry-3.0/eea/sentry/locales/update.sh
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/eea.pot
+Filename: eea.sentry-3.0/eea/sentry/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/update.sh
+Filename: eea.sentry-3.0/eea/sentry/locales/__init__.py
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/plone-manual.pot
+Filename: eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/__init__.py
+Filename: eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/zh_TW/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/en/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/en/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/en/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hr/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/es/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/es/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/es/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt_BR/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ro/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/eu/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/el/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/el/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/el/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/it/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/it/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/it/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ru/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/is/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/is/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/is/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lt/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hu/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/nl/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fi/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lv/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sl/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/mt/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/tr/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/no/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/no/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/no/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sv/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/bg/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/kl/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/et/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/et/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/et/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sk/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pl/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/cs/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/da/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/da/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/da/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fr/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/de/LC_MESSAGES/
+Filename: eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/de/LC_MESSAGES/eea.po
+Filename: eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/locales/de/LC_MESSAGES/plone.po
+Filename: eea.sentry-3.0/eea/sentry/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/upgrades/configure.zcml
+Filename: eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/upgrades/__init__.py
+Filename: eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/tests/base.py
+Filename: eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/tests/test_doctests.py
+Filename: eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/tests/__init__.py
+Filename: eea.sentry-3.0/eea/sentry/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/js/
+Filename: eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/zpt/
+Filename: eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/configure.zcml
+Filename: eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/sentry.py
+Filename: eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/__init__.py
+Filename: eea.sentry-3.0/eea/sentry/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/js/sentry.js
+Filename: eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/js/bundle.tracing.min.js
+Filename: eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/browser/zpt/sentry.pt
+Filename: eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/uninstall/
+Filename: eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/common/
+Filename: eea.sentry-3.0/eea/sentry/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/plone5/
+Filename: eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/plone4/
+Filename: eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/uninstall/browserlayer.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/common/metadata.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/common/browserlayer.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/plone5/metadata.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/plone5/registry.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/plone4/metadata.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/profiles/plone4/jsregistry.xml
+Filename: eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/kgs/
+Filename: eea.sentry-3.0/eea/sentry/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/plone5/
+Filename: eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/plone4/
+Filename: eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/eea/
+Filename: eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/kgs/00_install_addon.js
+Filename: eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/plone5/00_install_addon.js
+Filename: eea.sentry-3.0/eea/sentry/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/plone4/00_install_addon.js
+Filename: eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/ftests/eea/00_install_addon.js
+Filename: eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/cache/nocache.py
+Filename: eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.sentry-2.4/eea/sentry/cache/__init__.py
+Filename: eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/eea.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/sk/LC_MESSAGES/plone.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/plone.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/eea.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/eea.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/pl/LC_MESSAGES/plone.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/plone.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/eea.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/eea.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/cs/LC_MESSAGES/plone.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/plone.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/eea.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/eea.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/da/LC_MESSAGES/plone.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/plone.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/eea.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/eea.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/fr/LC_MESSAGES/plone.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/plone.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/eea.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/eea.mo
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/locales/de/LC_MESSAGES/plone.po
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/upgrades/configure.zcml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/upgrades/__init__.py
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/tests/base.py
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/tests/test_doctests.py
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/tests/__init__.py
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/js/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/zpt/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/configure.zcml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/sentry.py
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/__init__.py
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/js/sentry.js
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/js/bundle.tracing.min.js
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/browser/zpt/sentry.pt
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/uninstall/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/common/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/plone5/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/plone4/
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/uninstall/browserlayer.xml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/common/metadata.xml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/common/browserlayer.xml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/plone5/metadata.xml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/plone5/registry.xml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/plone4/metadata.xml
+Comment: 
+
+Filename: eea.sentry-3.0/eea/sentry/profiles/plone4/jsregistry.xml
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.sentry-2.4/CONTRIBUTING.md` & `eea.sentry-3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/PKG-INFO` & `eea.sentry-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.sentry
-Version: 2.4
+Version: 3.0
 Summary: Zope/Plone Sentry integration
 Home-page: https://github.com/eea/eea.sentry
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Platform: UNKNOWN
@@ -157,14 +157,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.0 - (2023-05-05)
+---------------------------
+* Refactor: Drop eea.cache dependency in favor of plone.memoize
+  [avoinea]
+
 2.4 - (2022-01-13)
 ---------------------------
 * Bug fix: AttributeError PARENTS
   [avoinea]
 
 2.3 - (2021-10-11)
 ---------------------------
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eea.sentry Version: 2.4 Summary: Zope/Plone Sentry
+Metadata-Version: 2.1 Name: eea.sentry Version: 3.0 Summary: Zope/Plone Sentry
 integration Home-page: https://github.com/eea/eea.sentry Author: European
 Environment Agency: IDM2 A-Team Author-email: eea-edw-a-team-
 alerts@googlegroups.com License: GPL version 2 Keywords: EEA Add-ons Plone Zope
 Platform: UNKNOWN Classifier: Environment :: Web Environment Classifier:
 Framework :: Plone Classifier: Framework :: Plone :: Addon Classifier:
 Framework :: Plone :: 4.3 Classifier: Framework :: Plone :: 5.2 Classifier:
 Framework :: Plone :: 6.0 Classifier: Programming Language :: Python
@@ -61,28 +61,29 @@
 copy of the GNU General Public License along with this program; if not, write
 to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 02111-1307 USA. The Initial Owner of the Original Code is European Environment
 Agency (EEA). Portions created by Eau de Web are Copyright (C) 2009 by European
 Environment Agency. All Rights Reserved. Funding ======= EEA_ - European
 Environment Agency (EU) .. _EEA: https://www.eea.europa.eu/ .. _`EEA Web
 Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1 Changelog
-========= 2.4 - (2022-01-13) --------------------------- * Bug fix:
-AttributeError PARENTS [avoinea] 2.3 - (2021-10-11) --------------------------
-- * Bug fix: KeyError HTTP_USER_AGENT [avoinea] * Bug fix:
-FilesystemResourceDirectory object has no attribute getId [avoinea] 2.2 -
-(2021-10-03) --------------------------- * Fix python version in setup.py
-[avoinea] 2.1 - (2021-09-28) --------------------------- * add upgrade step for
-the new javascript [valipod] 2.0 - (2021-09-28) --------------------------- *
-Change: major version bump for the new sentry SDK 1.5 - (2021-09-24) ----------
------------------ * Change: Migrate to the new sentry SDK [valipod] 1.4 -
-(2019-12-02) --------------------------- * Bug fix: Fix JS integration [avoinea
-refs #110157] 1.3 - (2019-11-15) -------------------------- * Feature: Python3
-support [alecghica, iulianpetcheshi, avoinea refs #110155] 1.2 - (2019-07-30) -
-------------------------- * maintain backwards compatibility with non-plone
-systems when checking for anonymous [valipod refs #102005] 1.0 - (2019-06-01) -
------------------ * Upgrade step: Within "Plone > Site setup > Add-ons"
-install/reinstall eea.sentry [avoinea refs #104872] * Feature: Add JS
-integration [avoinea refs #104872] 0.2 - (2019-05-16) ------------------ *
-Feature: Setup Sentry logger via environment variables [avoinea refs #104872]
-0.1 - (2019-05-16) ------------------ * Feature: Add custom raven processors to
-cleanup Zope REQUEST [avoinea refs #104872] * Upgrade step: Within "Plone >
-Site setup > Add-ons" install eea.sentry [avoinea refs #104872]
+========= 3.0 - (2023-05-05) --------------------------- * Refactor: Drop
+eea.cache dependency in favor of plone.memoize [avoinea] 2.4 - (2022-01-13) ---
+------------------------ * Bug fix: AttributeError PARENTS [avoinea] 2.3 -
+(2021-10-11) --------------------------- * Bug fix: KeyError HTTP_USER_AGENT
+[avoinea] * Bug fix: FilesystemResourceDirectory object has no attribute getId
+[avoinea] 2.2 - (2021-10-03) --------------------------- * Fix python version
+in setup.py [avoinea] 2.1 - (2021-09-28) --------------------------- * add
+upgrade step for the new javascript [valipod] 2.0 - (2021-09-28) --------------
+------------- * Change: major version bump for the new sentry SDK 1.5 - (2021-
+09-24) --------------------------- * Change: Migrate to the new sentry SDK
+[valipod] 1.4 - (2019-12-02) --------------------------- * Bug fix: Fix JS
+integration [avoinea refs #110157] 1.3 - (2019-11-15) -------------------------
+- * Feature: Python3 support [alecghica, iulianpetcheshi, avoinea refs #110155]
+1.2 - (2019-07-30) -------------------------- * maintain backwards
+compatibility with non-plone systems when checking for anonymous [valipod refs
+#102005] 1.0 - (2019-06-01) ------------------ * Upgrade step: Within "Plone >
+Site setup > Add-ons" install/reinstall eea.sentry [avoinea refs #104872] *
+Feature: Add JS integration [avoinea refs #104872] 0.2 - (2019-05-16) ---------
+--------- * Feature: Setup Sentry logger via environment variables [avoinea
+refs #104872] 0.1 - (2019-05-16) ------------------ * Feature: Add custom raven
+processors to cleanup Zope REQUEST [avoinea refs #104872] * Upgrade step:
+Within "Plone > Site setup > Add-ons" install eea.sentry [avoinea refs #104872]
```

## Comparing `eea.sentry-2.4/README.rst` & `eea.sentry-3.0/README.rst`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/setup.py` & `eea.sentry-3.0/setup.py`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea.sentry.egg-info/PKG-INFO` & `eea.sentry-3.0/eea.sentry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.sentry
-Version: 2.4
+Version: 3.0
 Summary: Zope/Plone Sentry integration
 Home-page: https://github.com/eea/eea.sentry
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Platform: UNKNOWN
@@ -157,14 +157,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.0 - (2023-05-05)
+---------------------------
+* Refactor: Drop eea.cache dependency in favor of plone.memoize
+  [avoinea]
+
 2.4 - (2022-01-13)
 ---------------------------
 * Bug fix: AttributeError PARENTS
   [avoinea]
 
 2.3 - (2021-10-11)
 ---------------------------
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eea.sentry Version: 2.4 Summary: Zope/Plone Sentry
+Metadata-Version: 2.1 Name: eea.sentry Version: 3.0 Summary: Zope/Plone Sentry
 integration Home-page: https://github.com/eea/eea.sentry Author: European
 Environment Agency: IDM2 A-Team Author-email: eea-edw-a-team-
 alerts@googlegroups.com License: GPL version 2 Keywords: EEA Add-ons Plone Zope
 Platform: UNKNOWN Classifier: Environment :: Web Environment Classifier:
 Framework :: Plone Classifier: Framework :: Plone :: Addon Classifier:
 Framework :: Plone :: 4.3 Classifier: Framework :: Plone :: 5.2 Classifier:
 Framework :: Plone :: 6.0 Classifier: Programming Language :: Python
@@ -61,28 +61,29 @@
 copy of the GNU General Public License along with this program; if not, write
 to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 02111-1307 USA. The Initial Owner of the Original Code is European Environment
 Agency (EEA). Portions created by Eau de Web are Copyright (C) 2009 by European
 Environment Agency. All Rights Reserved. Funding ======= EEA_ - European
 Environment Agency (EU) .. _EEA: https://www.eea.europa.eu/ .. _`EEA Web
 Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1 Changelog
-========= 2.4 - (2022-01-13) --------------------------- * Bug fix:
-AttributeError PARENTS [avoinea] 2.3 - (2021-10-11) --------------------------
-- * Bug fix: KeyError HTTP_USER_AGENT [avoinea] * Bug fix:
-FilesystemResourceDirectory object has no attribute getId [avoinea] 2.2 -
-(2021-10-03) --------------------------- * Fix python version in setup.py
-[avoinea] 2.1 - (2021-09-28) --------------------------- * add upgrade step for
-the new javascript [valipod] 2.0 - (2021-09-28) --------------------------- *
-Change: major version bump for the new sentry SDK 1.5 - (2021-09-24) ----------
------------------ * Change: Migrate to the new sentry SDK [valipod] 1.4 -
-(2019-12-02) --------------------------- * Bug fix: Fix JS integration [avoinea
-refs #110157] 1.3 - (2019-11-15) -------------------------- * Feature: Python3
-support [alecghica, iulianpetcheshi, avoinea refs #110155] 1.2 - (2019-07-30) -
-------------------------- * maintain backwards compatibility with non-plone
-systems when checking for anonymous [valipod refs #102005] 1.0 - (2019-06-01) -
------------------ * Upgrade step: Within "Plone > Site setup > Add-ons"
-install/reinstall eea.sentry [avoinea refs #104872] * Feature: Add JS
-integration [avoinea refs #104872] 0.2 - (2019-05-16) ------------------ *
-Feature: Setup Sentry logger via environment variables [avoinea refs #104872]
-0.1 - (2019-05-16) ------------------ * Feature: Add custom raven processors to
-cleanup Zope REQUEST [avoinea refs #104872] * Upgrade step: Within "Plone >
-Site setup > Add-ons" install eea.sentry [avoinea refs #104872]
+========= 3.0 - (2023-05-05) --------------------------- * Refactor: Drop
+eea.cache dependency in favor of plone.memoize [avoinea] 2.4 - (2022-01-13) ---
+------------------------ * Bug fix: AttributeError PARENTS [avoinea] 2.3 -
+(2021-10-11) --------------------------- * Bug fix: KeyError HTTP_USER_AGENT
+[avoinea] * Bug fix: FilesystemResourceDirectory object has no attribute getId
+[avoinea] 2.2 - (2021-10-03) --------------------------- * Fix python version
+in setup.py [avoinea] 2.1 - (2021-09-28) --------------------------- * add
+upgrade step for the new javascript [valipod] 2.0 - (2021-09-28) --------------
+------------- * Change: major version bump for the new sentry SDK 1.5 - (2021-
+09-24) --------------------------- * Change: Migrate to the new sentry SDK
+[valipod] 1.4 - (2019-12-02) --------------------------- * Bug fix: Fix JS
+integration [avoinea refs #110157] 1.3 - (2019-11-15) -------------------------
+- * Feature: Python3 support [alecghica, iulianpetcheshi, avoinea refs #110155]
+1.2 - (2019-07-30) -------------------------- * maintain backwards
+compatibility with non-plone systems when checking for anonymous [valipod refs
+#102005] 1.0 - (2019-06-01) ------------------ * Upgrade step: Within "Plone >
+Site setup > Add-ons" install/reinstall eea.sentry [avoinea refs #104872] *
+Feature: Add JS integration [avoinea refs #104872] 0.2 - (2019-05-16) ---------
+--------- * Feature: Setup Sentry logger via environment variables [avoinea
+refs #104872] 0.1 - (2019-05-16) ------------------ * Feature: Add custom raven
+processors to cleanup Zope REQUEST [avoinea refs #104872] * Upgrade step:
+Within "Plone > Site setup > Add-ons" install eea.sentry [avoinea refs #104872]
```

## Comparing `eea.sentry-2.4/docs/HISTORY.txt` & `eea.sentry-3.0/docs/HISTORY.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+3.0 - (2023-05-05)
+---------------------------
+* Refactor: Drop eea.cache dependency in favor of plone.memoize
+  [avoinea]
+
 2.4 - (2022-01-13)
 ---------------------------
 * Bug fix: AttributeError PARENTS
   [avoinea]
 
 2.3 - (2021-10-11)
 ---------------------------
```

## Comparing `eea.sentry-2.4/docs/LICENSE.txt` & `eea.sentry-3.0/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/docs/LICENSE.GPL` & `eea.sentry-3.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/configure.zcml` & `eea.sentry-3.0/eea/sentry/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/setuphandlers.py` & `eea.sentry-3.0/eea/sentry/setuphandlers.py`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/processors.py` & `eea.sentry-3.0/eea/sentry/processors.py`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/profiles.zcml` & `eea.sentry-3.0/eea/sentry/profiles.zcml`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/__init__.py` & `eea.sentry-3.0/eea/sentry/__init__.py`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/upgrades/configure.zcml` & `eea.sentry-3.0/eea/sentry/upgrades/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/tests/base.py` & `eea.sentry-3.0/eea/sentry/tests/base.py`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/tests/test_doctests.py` & `eea.sentry-3.0/eea/sentry/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/browser/configure.zcml` & `eea.sentry-3.0/eea/sentry/browser/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/browser/sentry.py` & `eea.sentry-3.0/eea/sentry/browser/sentry.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import json
 import six
 import logging
 import socket
 from contextlib import closing
 from Products.Five.browser import BrowserView
-from eea.sentry.cache import ramcache
+from plone.memoize import view
 from six.moves.urllib.parse import urlparse
 if six.PY2:
     from eventlet.green import urllib2 as request
 else:
     from eventlet.green.urllib import request
 
 try:
@@ -34,15 +34,15 @@
     _environment = os.environ.get("SENTRY_ENVIRONMENT", None)
 
     def __init__(self, context, request, view=None, manager=None):
         super(Sentry, self).__init__(context, request)
         self.view = view
         self.manager = manager
 
-    @ramcache(lambda *args: "environment", lifetime=86400)
+    @view.memoize
     def environment(self):
         """ Sentry environment
         """
         if not self._environment:
             self._environment = os.environ.get(
                 'ENVIRONMENT', os.environ.get('SENTRY_ENVIRONMENT', ''))
             if not self._environment:
@@ -54,36 +54,36 @@
                     logger.warning(
                         "Please provide SENTRY_ENVIRONMENT env as we "
                         "could not get it automatically from %s due to: %s",
                         url, err)
                     self._environment = 'devel'
         return self._environment
 
-    @ramcache(lambda *args: "version", lifetime=86400)
+    @view.memoize
     def version(self):
         """ KGS version
         """
         return os.environ.get(
             "SENTRY_RELEASE", os.environ.get("EEA_KGS_VERSION", ""))
 
-    @ramcache(lambda *args: "dsn", lifetime=86400)
+    @view.memoize
     def dsn(self):
         """ Public Sentry DSN
         """
         dsn = os.environ.get("SENTRY_DSN", "")
         if "@" not in dsn:
             return dsn
 
         # Remove password from SENTRY_DSN, if provided (old format)
         url = urlparse(dsn)
         public = url._replace(netloc="{}@{}".format(
             url.username, url.hostname))
         return public.geturl()
 
-    @ramcache(lambda *args: "site", lifetime=86400)
+    @view.memoize
     def site(self):
         """ return site id
         """
         site = get_site(self.request)
         if site:
             return site.getId()
         return os.environ.get(
```

## Comparing `eea.sentry-2.4/eea/sentry/browser/js/sentry.js` & `eea.sentry-3.0/eea/sentry/browser/js/sentry.js`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/browser/js/bundle.tracing.min.js` & `eea.sentry-3.0/eea/sentry/browser/js/bundle.tracing.min.js`

 * *Files identical despite different names*

## Comparing `eea.sentry-2.4/eea/sentry/profiles/plone5/registry.xml` & `eea.sentry-3.0/eea/sentry/profiles/plone5/registry.xml`

 * *Files identical despite different names*

