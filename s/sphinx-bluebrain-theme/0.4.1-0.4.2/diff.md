# Comparing `tmp/sphinx-bluebrain-theme-0.4.1.tar.gz` & `tmp/sphinx-bluebrain-theme-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-bluebrain-theme-0.4.1.tar", last modified: Fri Feb 17 08:22:46 2023, max compression
+gzip compressed data, was "sphinx-bluebrain-theme-0.4.2.tar", last modified: Fri Aug  4 13:34:45 2023, max compression
```

## Comparing `sphinx-bluebrain-theme-0.4.1.tar` & `sphinx-bluebrain-theme-0.4.2.tar`

### file list

```diff
@@ -1,197 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.868912 sphinx-bluebrain-theme-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.840911 sphinx-bluebrain-theme-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.840911 sphinx-bluebrain-theme-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/.github/workflows/publish-pkg.yml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-17 08:22:46.868912 sphinx-bluebrain-theme-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-17 08:22:46.868912 sphinx-bluebrain-theme-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.844911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.844911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/iframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.844911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/hero.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.848911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/af.html
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ca.html
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/cs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/da.html
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/de.html
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/en.html
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/es.html
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/fa.html
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/fi.html
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/fr.html
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/gl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/gr.html
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/he.html
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/hi.html
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/hr.html
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/hu.html
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/id.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/it.html
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ja.html
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/kr.html
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/nl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/nn.html
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/no.html
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/pl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/pt.html
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ru.html
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sh.html
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/si.html
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sr.html
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sv.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/tr.html
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/uk.html
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/vi.html
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/zh-Hant.html
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/zh-TW.html
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/zh.html
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language.html
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/nav-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/palette.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/social.html
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/source.html
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/tabs-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/toc-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/toc.html
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.848911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.852911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/material-icons.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.852911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11560 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.eot
--rw-r--r--   0 runner    (1001) docker     (123)    55181 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.eot
--rw-r--r--   0 runner    (1001) docker     (123)    55652 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28192 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    59362 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.856911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   128180 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44300 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.860911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4523 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.eot
--rw-r--r--   0 runner    (1001) docker     (123)    43644 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29988 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.eot
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28508 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16539 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    43156 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.860911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/epfl-logo-new.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.860911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/bitbucket.1b09e088.svg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/github.f0b8504a.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-17 08:22:33.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/gitlab.6dd19c00.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.860911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)    80116 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/application.718059d6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.864911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.da.js
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.de.js
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.du.js
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.es.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fi.js
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fr.js
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.hu.js
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.it.js
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.jp.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.multi.js
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.nl.js
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.no.js
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.pt.js
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ro.js
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.stemmer.support.js
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.sv.js
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.th.js
--rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.tr.js
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/tinyseg.js
--rw-r--r--   0 runner    (1001) docker     (123)   556464 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/wordcut.js
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/modernizr.74668098.js
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/theme.js_t
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/utils.js
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/jquery-3.2.1.js
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.864911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/search/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/search/search_index.json_t
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/searchtools.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.864911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/application-palette.3e3d1dff.css
--rw-r--r--   0 runner    (1001) docker     (123)    75449 2023-02-17 08:22:43.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/application.4031d38b.css
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/theme.css_t
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/underscore-1.3.1.js
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.868912 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/autodoc_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/inject_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/navutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/search_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-02-17 08:22:21.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/toc_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 08:22:46.844911 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-17 08:22:46.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-02-17 08:22:46.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 08:22:46.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-17 08:22:46.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 08:22:46.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-17 08:22:46.000000 sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.032455 sphinx-bluebrain-theme-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.008454 sphinx-bluebrain-theme-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.012454 sphinx-bluebrain-theme-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/.github/workflows/publish-pkg.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-04 13:34:45.032455 sphinx-bluebrain-theme-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.012454 sphinx-bluebrain-theme-0.4.2/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1738 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/ci/check-regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 13:34:45.036455 sphinx-bluebrain-theme-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.012454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.012454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.012454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/hero.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.020454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/af.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ca.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/cs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/da.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/de.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/en.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/es.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/fa.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/fi.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/fr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/gl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/gr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/he.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/hi.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/hr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/hu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/id.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/it.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ja.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/kr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/nl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/nn.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/no.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/pl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/pt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ru.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sh.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/si.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sv.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/tr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/uk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/vi.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/zh-Hant.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/zh-TW.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/zh.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/nav-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/palette.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/social.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/source.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/tabs-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/toc-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/toc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.020454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.020454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/material-icons.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.024454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11560 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    55181 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    55652 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28192 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    59362 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.024454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   128180 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44300 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.028454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4523 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    43644 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29988 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28508 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16539 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    43156 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.028454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/epfl-logo-new.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.028454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/bitbucket.1b09e088.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/github.f0b8504a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-04 13:34:37.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/gitlab.6dd19c00.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.028454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    80116 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/application.718059d6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.032455 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.da.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.de.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.du.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.es.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.it.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.jp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.multi.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.no.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.stemmer.support.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.th.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/tinyseg.js
+-rw-r--r--   0 runner    (1001) docker     (123)   556464 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/wordcut.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/modernizr.74668098.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/theme.js_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/jquery-3.2.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.032455 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/search/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/search/search_index.json_t
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/searchtools.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.032455 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/application-palette.3e3d1dff.css
+-rw-r--r--   0 runner    (1001) docker     (123)    75449 2023-08-04 13:34:42.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/application.4031d38b.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/theme.css_t
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/underscore-1.3.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.032455 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/autodoc_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/inject_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/navutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/search_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-08-04 13:34:21.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/toc_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:34:45.012454 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-04 13:34:44.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-08-04 13:34:45.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:34:44.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 13:34:44.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-04 13:34:44.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 13:34:44.000000 sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/top_level.txt
```

### Comparing `sphinx-bluebrain-theme-0.4.1/.github/workflows/publish-pkg.yml` & `sphinx-bluebrain-theme-0.4.2/.github/workflows/publish-pkg.yml`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           submodules: true
-      - name: Set up Python 3.8
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: 3.11
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip setuptools
           pip install tox tox-gh-actions
       - name: Build
         run: |
             python translate_templates.py
```

### Comparing `sphinx-bluebrain-theme-0.4.1/.github/workflows/run-tox.yml` & `sphinx-bluebrain-theme-0.4.2/.github/workflows/run-tox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 jobs:
   check:
     name: Run checks
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           submodules: true
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
```

### Comparing `sphinx-bluebrain-theme-0.4.1/CHANGELOG.rst` & `sphinx-bluebrain-theme-0.4.2/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+0.4.2
+-----
+- |fixed| Fix creation of empty search_index.json
+
 0.3.0
 -----
 
 - |changed| bump python version in tox
 - |fixed| show or hide home button depending on context
 - |fixed| move classifier in metadata section in setup.cfg
```

### Comparing `sphinx-bluebrain-theme-0.4.1/CONTRIBUTING.rst` & `sphinx-bluebrain-theme-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/LICENSE.txt` & `sphinx-bluebrain-theme-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/PKG-INFO` & `sphinx-bluebrain-theme-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: sphinx-bluebrain-theme
-Version: 0.4.1
+Version: 0.4.2
 Summary: Blue Brain Project theme for Sphinx
 Home-page: https://github.com/BlueBrain/sphinx-bluebrain-theme
 Author: Blue Brain Project, EPFL
 License: MIT License
 Project-URL: Tracker, https://github.com/BlueBrain/sphinx-bluebrain-theme/issues
 Project-URL: Source, https://github.com/BlueBrain/sphinx-bluebrain-theme
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Sphinx BlueBrain Theme
 ======================
 
 |build_status| |license| |black| |docs|
```

### Comparing `sphinx-bluebrain-theme-0.4.1/README.rst` & `sphinx-bluebrain-theme-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/setup.cfg` & `sphinx-bluebrain-theme-0.4.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -15,27 +15,30 @@
 license_file = LICENSE.txt
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Sphinx :: Theme
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Documentation :: Sphinx
 	Topic :: Software Development :: Documentation
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.8
 setup_requires = 
 	setuptools
 	setuptools_scm
 install_requires = 
 	sphinx>=v3.4.0
 	Jinja2~=3.0.0
+	importlib-resources; python_version == "3.8"
 packages = find:
 include_package_data = True
 
 [options.packages.find]
 exclude = 
 	mkdocs2sphinx
 	mkdocs-material
```

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/__init__.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """sphinx_bluebrain_theme package."""
-
 from os import path
 
 from sphinx_bluebrain_theme import utils
 
 
 def setup(app):
     """Initialise the theme and connect theme specific functions to events."""
@@ -12,7 +11,8 @@
     app.setup_extension("sphinx_bluebrain_theme.ext.details")
     app.setup_extension("sphinx_bluebrain_theme.ext.iframe")
     app.connect("builder-inited", utils.add_filters)
     app.connect("builder-inited", utils.add_autodoc_override)
     app.connect("env-updated", utils.write_metadata_sphinx)
     app.connect("html-page-context", utils.build_tocs)
     app.connect("html-page-context", utils.inject_context_variables)
+    app.connect("build-finished", utils.copy_search_index_json)
```

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/base.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/base.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/details.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/details.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/iframe.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/iframe.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/ext/tabs.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/ext/tabs.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/layout.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/footer.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/header.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/header.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/hero.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/hero.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/af.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/af.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ar.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ar.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ca.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ca.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/cs.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/cs.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/da.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/da.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/de.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/de.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/en.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/en.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/es.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/es.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/fa.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/fa.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/fi.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/fi.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/fr.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/fr.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/gl.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/gl.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/gr.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/gr.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/he.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/he.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/hi.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/hi.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/hr.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/hr.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/hu.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/hu.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/id.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/id.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/it.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/it.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ja.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ja.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/kr.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/kr.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/nl.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/nl.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/nn.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/nn.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/no.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/no.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/pl.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/pl.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/pt.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/pt.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/ru.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/ru.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sh.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sh.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/si.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/si.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sk.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sk.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sr.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sr.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/sv.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/sv.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/tr.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/tr.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/uk.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/uk.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/vi.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/vi.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/zh-Hant.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/zh-Hant.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/zh-TW.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/zh-TW.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language/zh.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language/zh.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/language.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/language.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/nav-item.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/nav-item.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/nav.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/nav.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/palette.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/palette.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/search.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/social.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/social.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/source.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/source.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/tabs-item.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/tabs-item.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/tabs.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/tabs.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/toc-item.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/toc-item.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/partials/toc.html` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/partials/toc.html`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/font-awesome.css` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/material-icons.css` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/material-icons.css`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/LICENSE.txt` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans/open-sans-v15-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/open-sans.css` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/open-sans.css`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/FontAwesome.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/specimen/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/OFL.txt` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.eot` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.ttf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff2` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web/titillium-web-v6-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/fonts/titillium-web.css` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/fonts/titillium-web.css`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/epfl-logo-new.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/epfl-logo-new.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/bitbucket.1b09e088.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/bitbucket.1b09e088.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/github.f0b8504a.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/github.f0b8504a.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/images/icons/gitlab.6dd19c00.svg` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/images/icons/gitlab.6dd19c00.svg`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/application.718059d6.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/application.718059d6.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.da.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.da.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.de.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.de.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.du.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.du.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.es.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.es.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fi.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fr.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.hu.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.it.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.it.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ja.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.jp.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.jp.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.multi.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.nl.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.no.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.no.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.pt.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ro.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ru.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.stemmer.support.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.sv.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.th.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.th.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.tr.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/tinyseg.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/lunr/wordcut.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/modernizr.74668098.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/modernizr.74668098.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/theme.js_t` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/theme.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/javascripts/utils.js` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/javascripts/utils.js`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/application-palette.3e3d1dff.css` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/application-palette.3e3d1dff.css`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/application.4031d38b.css` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/application.4031d38b.css`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/static/stylesheets/theme.css_t` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/static/stylesheets/theme.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/theme.conf` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/autodoc_override.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/autodoc_override.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/filters.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/filters.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/inject_context.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/inject_context.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/metadata.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/navutils.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/navutils.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/search_builder.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/search_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """This module contains the classes used to build the search_index.json file for lunr search.
 
 See https://github.com/mkdocs/mkdocs/blob/master/mkdocs/contrib/search/search_index.py
 which shows the expected structure of the JSON search index and the
 approach used by mkdocs to generate it
 """
 
+import json
+import os
 import re
-from json import dumps
 
 try:
-    from html.parser import HTMLParser
+    from importlib.resources import files, as_file
 except ImportError:
-    from HTMLParser import HTMLParser
+    # backport for python 3.8
+    from importlib_resources import files, as_file
+
+from html.parser import HTMLParser
+from sphinx.util.fileutil import copy_asset_file
 
 
 class IndexEntry:
     """Holds the data for each entry in the search index."""
 
     MULTI_SPACE_REGEX = re.compile(r"\s+")
 
@@ -78,15 +83,15 @@
         self.feed(contents)
 
     def __repr__(self):
         """Returns the dumped json as the repr for the entry.
 
         The dumped json is used for the search index build.
         """
-        return dumps(
+        return json.dumps(
             {"docs": [e.as_dict() for e in self._entries], "config": {}}, sort_keys=True
         )
 
     def handle_starttag(self, tag, attrs):
         """Handles the possible HTML tags as required for building the index."""
         attrsdict = dict(attrs)
 
@@ -121,7 +126,16 @@
         # always add the data to the complete page entry
         self._current_page.text_list.append(data)
 
         if self._is_heading:
             self._current_section.title = data
         elif self._current_section is not None:
             self._current_section.text_list.append(data)
+
+
+def copy_search_index_json(app, exc):
+    """Create and copy the search_index.json file."""
+    if app.builder.format == "html" and not exc:
+        output = os.path.join(app.builder.outdir, "_static/search")
+        path = files("sphinx_bluebrain_theme")
+        with as_file(path / "static/search/search_index.json_t") as file_:
+            copy_asset_file(str(file_), output, context=app.builder.globalcontext)
```

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme/utils/toc_builder.py` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme/utils/toc_builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/PKG-INFO` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: sphinx-bluebrain-theme
-Version: 0.4.1
+Version: 0.4.2
 Summary: Blue Brain Project theme for Sphinx
 Home-page: https://github.com/BlueBrain/sphinx-bluebrain-theme
 Author: Blue Brain Project, EPFL
 License: MIT License
 Project-URL: Tracker, https://github.com/BlueBrain/sphinx-bluebrain-theme/issues
 Project-URL: Source, https://github.com/BlueBrain/sphinx-bluebrain-theme
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Sphinx BlueBrain Theme
 ======================
 
 |build_status| |license| |black| |docs|
```

### Comparing `sphinx-bluebrain-theme-0.4.1/sphinx_bluebrain_theme.egg-info/SOURCES.txt` & `sphinx-bluebrain-theme-0.4.2/sphinx_bluebrain_theme.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/publish-pkg.yml
 .github/workflows/run-tox.yml
+ci/check-regressions.py
 sphinx_bluebrain_theme/__init__.py
 sphinx_bluebrain_theme/base.html
 sphinx_bluebrain_theme/layout.html
 sphinx_bluebrain_theme/search.html
 sphinx_bluebrain_theme/theme.conf
 sphinx_bluebrain_theme.egg-info/PKG-INFO
 sphinx_bluebrain_theme.egg-info/SOURCES.txt
```

