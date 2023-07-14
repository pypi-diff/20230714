# Comparing `tmp/django-beam-1.4.2.tar.gz` & `tmp/django-beam-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-beam-1.4.2.tar", last modified: Thu Jul 13 12:43:43 2023, max compression
+gzip compressed data, was "django-beam-1.5.0.tar", last modified: Fri Jul 14 09:28:14 2023, max compression
```

## Comparing `django-beam-1.4.2.tar` & `django-beam-1.5.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.255217 django-beam-1.4.2/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.4.2/LICENSE
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.4.2/MANIFEST.in
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-07-13 12:43:43.255291 django-beam-1.4.2/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.4.2/README.md
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-07-13 12:43:43.255835 django-beam-1.4.2/setup.cfg
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.4.2/setup.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231379 django-beam-1.4.2/src/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.237210 django-beam-1.4.2/src/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/components.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.237488 django-beam-1.4.2/src/beam/contrib/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.238153 django-beam-1.4.2/src/beam/contrib/auth/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/apps.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/forms.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230107 django-beam-1.4.2/src/beam/contrib/auth/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.239867 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/logged_out.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/login.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_change_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_change_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_complete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_email.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/views.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.240018 django-beam-1.4.2/src/beam/contrib/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/autocomplete_light/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230305 django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.240166 django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.240756 django-beam-1.4.2/src/beam/contrib/reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/apps.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230492 django-beam-1.4.2/src/beam/contrib/reversion/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241049 django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/viewsets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/layouts.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230620 django-beam-1.4.2/src/beam/locale/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230674 django-beam-1.4.2/src/beam/locale/de/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241197 django-beam-1.4.2/src/beam/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/registry.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241438 django-beam-1.4.2/src/beam/templatetags/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/templatetags/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10854 2023-07-13 12:40:44.000000 django-beam-1.4.2/src/beam/templatetags/beam_tags.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241696 django-beam-1.4.2/src/beam/themes/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241888 django-beam-1.4.2/src/beam/themes/bootstrap4/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231001 django-beam-1.4.2/src/beam/themes/bootstrap4/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231118 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.242033 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/css/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.243094 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/actions.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/add_related.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/inlines.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231238 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.245522 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/base.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/create.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1537 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/dashboard.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2265 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/delete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-07-13 12:40:03.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8143 2023-07-13 12:40:44.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/list.html
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.249422 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1750 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2168 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4596 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3298 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1516 2023-07-13 12:40:44.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      843 2023-07-13 12:39:52.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6373 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3075 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4856 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2094 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5068 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/update.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/widgets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/types.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-05-31 11:33:31.000000 django-beam-1.4.2/src/beam/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/viewsets.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.250053 django-beam-1.4.2/src/django_beam.egg-info/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/requires.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/top_level.txt
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.255066 django-beam-1.4.2/tests/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.4.2/tests/test_components.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.4.2/tests/test_contrib_auth.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_contrib_autocomplete.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.4.2/tests/test_contrib_reversion.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_layouts.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_registry.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.4.2/tests/test_tags.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.4.2/tests/test_urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.4.2/tests/test_utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.4.2/tests/test_views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.472109 django-beam-1.5.0/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.5.0/LICENSE
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.5.0/MANIFEST.in
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3717 2023-07-14 09:28:14.472229 django-beam-1.5.0/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3268 2023-07-14 09:27:11.000000 django-beam-1.5.0/README.md
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-07-14 09:28:14.472638 django-beam-1.5.0/setup.cfg
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.5.0/setup.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.439407 django-beam-1.5.0/src/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.442768 django-beam-1.5.0/src/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/components.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.443052 django-beam-1.5.0/src/beam/contrib/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.443687 django-beam-1.5.0/src/beam/contrib/auth/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/apps.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/forms.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.438111 django-beam-1.5.0/src/beam/contrib/auth/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.445046 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/logged_out.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/login.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_change_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_change_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_complete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_email.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/auth/views.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.445184 django-beam-1.5.0/src/beam/contrib/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/autocomplete_light/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.438304 django-beam-1.5.0/src/beam/contrib/autocomplete_light/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.445384 django-beam-1.5.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.447685 django-beam-1.5.0/src/beam/contrib/reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/reversion/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/reversion/apps.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.438491 django-beam-1.5.0/src/beam/contrib/reversion/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.448060 django-beam-1.5.0/src/beam/contrib/reversion/templates/beam_reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/reversion/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/contrib/reversion/viewsets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/layouts.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.438611 django-beam-1.5.0/src/beam/locale/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.438662 django-beam-1.5.0/src/beam/locale/de/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.448235 django-beam-1.5.0/src/beam/locale/de/LC_MESSAGES/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/registry.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.449021 django-beam-1.5.0/src/beam/templatetags/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/templatetags/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10854 2023-07-13 12:40:44.000000 django-beam-1.5.0/src/beam/templatetags/beam_tags.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.449301 django-beam-1.5.0/src/beam/themes/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.449490 django-beam-1.5.0/src/beam/themes/bootstrap4/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.438978 django-beam-1.5.0/src/beam/themes/bootstrap4/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.439109 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.450036 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/css/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.453921 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/actions.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/add_related.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/inlines.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.439256 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.456625 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/base.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/create.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1537 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/dashboard.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2265 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/delete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-07-13 12:40:03.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8143 2023-07-13 12:40:44.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/list.html
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.459894 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1750 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2168 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4596 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3298 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1516 2023-07-13 12:40:44.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      843 2023-07-13 12:39:52.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6373 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3075 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4856 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2094 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5407 2023-07-14 09:27:11.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/update.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/themes/bootstrap4/widgets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/types.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21972 2023-07-14 09:27:11.000000 django-beam-1.5.0/src/beam/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-05-30 12:51:34.000000 django-beam-1.5.0/src/beam/viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.460636 django-beam-1.5.0/src/django_beam.egg-info/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3717 2023-07-14 09:28:14.000000 django-beam-1.5.0/src/django_beam.egg-info/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-07-14 09:28:14.000000 django-beam-1.5.0/src/django_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-07-14 09:28:14.000000 django-beam-1.5.0/src/django_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-07-14 09:28:14.000000 django-beam-1.5.0/src/django_beam.egg-info/requires.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-07-14 09:28:14.000000 django-beam-1.5.0/src/django_beam.egg-info/top_level.txt
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-14 09:28:14.471880 django-beam-1.5.0/tests/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.5.0/tests/test_actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.5.0/tests/test_components.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.5.0/tests/test_contrib_auth.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.5.0/tests/test_contrib_autocomplete.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.5.0/tests/test_contrib_reversion.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.5.0/tests/test_inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.5.0/tests/test_layouts.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.5.0/tests/test_registry.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.5.0/tests/test_tags.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.5.0/tests/test_urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.5.0/tests/test_utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    37640 2023-07-14 09:27:11.000000 django-beam-1.5.0/tests/test_views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.5.0/tests/test_viewsets.py
```

### Comparing `django-beam-1.4.2/LICENSE` & `django-beam-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/PKG-INFO` & `django-beam-1.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: django-beam
-Version: 1.4.2
-Summary: A crud library for python
-Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.4.2.tar.gz
-Author: Raphael Kimmig
-Author-email: raphael@ampad.de
-License: BSD 3-Clause License
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # django-beam [![CI](https://github.com/django-beam/django-beam/actions/workflows/tox.yml/badge.svg)](https://github.com/django-beam/django-beam/actions/workflows/tox.yml) [![ReadTheDocs](https://readthedocs.org/projects/django-beam/badge/)](https://django-beam.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/django-beam/django-beam/branch/master/graph/badge.svg?token=U0C27SY9XM)](https://codecov.io/gh/django-beam/django-beam)
 
 django-beam provides you with a set of views, templates, and integrations for the most common CRUD applications. It aims to offer the functionality of Django's own admin but in a way that integrates seamlessly with your frontend code.
 
 ## Features
 
 - CRUD operations based on class-based views
@@ -90,10 +76,30 @@
 
 - `beam.contrib.auth`: Viewsets for editing users and groups, and optional templates for default Django registration views.
 - `beam.contrib.autocomplete_light`: Integration with `django-autocomplete-light`.
 - `beam.contrib.reversion`: Experimental integration with `django-reversion`.
 
 Refer to the documentation for usage instructions on each of the contrib packages.
 
+## Testing
+
+You can use the [tox](https://tox.readthedocs.io/en/latest/) testing tool to run the tests:
+
+```bash
+tox -e py38-djangolatest
+```
+
+Run the tests of a specific test file only:
+
+```bash
+tox -e py38-djangolatest -- test_tags
+```
+
+Run against all supported versions of Python and Django:
+
+```bash
+tox
+```
+
 ## Support
 
 If you encounter any issues or have questions, please refer to the [django-beam documentation](https://django-beam.readthedocs.io/en/latest/) or raise an issue on the [GitHub repository](https://github.com/yourgithubuser/django-beam/issues).
```

### Comparing `django-beam-1.4.2/README.md` & `django-beam-1.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: django-beam
+Version: 1.5.0
+Summary: A crud library for python
+Home-page: https://github.com/django-beam/django-beam
+Download-URL: https://github.com/django-beam/django-beam/archive/1.5.0.tar.gz
+Author: Raphael Kimmig
+Author-email: raphael@ampad.de
+License: BSD 3-Clause License
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # django-beam [![CI](https://github.com/django-beam/django-beam/actions/workflows/tox.yml/badge.svg)](https://github.com/django-beam/django-beam/actions/workflows/tox.yml) [![ReadTheDocs](https://readthedocs.org/projects/django-beam/badge/)](https://django-beam.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/django-beam/django-beam/branch/master/graph/badge.svg?token=U0C27SY9XM)](https://codecov.io/gh/django-beam/django-beam)
 
 django-beam provides you with a set of views, templates, and integrations for the most common CRUD applications. It aims to offer the functionality of Django's own admin but in a way that integrates seamlessly with your frontend code.
 
 ## Features
 
 - CRUD operations based on class-based views
@@ -76,10 +90,30 @@
 
 - `beam.contrib.auth`: Viewsets for editing users and groups, and optional templates for default Django registration views.
 - `beam.contrib.autocomplete_light`: Integration with `django-autocomplete-light`.
 - `beam.contrib.reversion`: Experimental integration with `django-reversion`.
 
 Refer to the documentation for usage instructions on each of the contrib packages.
 
+## Testing
+
+You can use the [tox](https://tox.readthedocs.io/en/latest/) testing tool to run the tests:
+
+```bash
+tox -e py38-djangolatest
+```
+
+Run the tests of a specific test file only:
+
+```bash
+tox -e py38-djangolatest -- test_tags
+```
+
+Run against all supported versions of Python and Django:
+
+```bash
+tox
+```
+
 ## Support
 
 If you encounter any issues or have questions, please refer to the [django-beam documentation](https://django-beam.readthedocs.io/en/latest/) or raise an issue on the [GitHub repository](https://github.com/yourgithubuser/django-beam/issues).
```

### Comparing `django-beam-1.4.2/setup.cfg` & `django-beam-1.5.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = django-beam
-version = 1.4.2
+version = 1.5.0
 description = A crud library for python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/django-beam/django-beam
-download_url = https://github.com/django-beam/django-beam/archive/1.4.2.tar.gz
+download_url = https://github.com/django-beam/django-beam/archive/1.5.0.tar.gz
 author = Raphael Kimmig
 author_email = raphael@ampad.de
 keywords = 
 license = BSD 3-Clause License
 classifiers = 
 	Framework :: Django
 	Programming Language :: Python :: 3
```

### Comparing `django-beam-1.4.2/src/beam/actions.py` & `django-beam-1.5.0/src/beam/actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/components.py` & `django-beam-1.5.0/src/beam/components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/forms.py` & `django-beam-1.5.0/src/beam/contrib/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/login.html` & `django-beam-1.5.0/src/beam/contrib/auth/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_change_form.html` & `django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_confirm.html` & `django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_done.html` & `django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_email.html` & `django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_form.html` & `django-beam-1.5.0/src/beam/contrib/auth/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/auth/views.py` & `django-beam-1.5.0/src/beam/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/autocomplete_light/__init__.py` & `django-beam-1.5.0/src/beam/contrib/autocomplete_light/__init__.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css` & `django-beam-1.5.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html` & `django-beam-1.5.0/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_list.html` & `django-beam-1.5.0/src/beam/contrib/reversion/templates/beam_reversion/version_list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/reversion/views.py` & `django-beam-1.5.0/src/beam/contrib/reversion/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/contrib/reversion/viewsets.py` & `django-beam-1.5.0/src/beam/contrib/reversion/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/inlines.py` & `django-beam-1.5.0/src/beam/inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/layouts.py` & `django-beam-1.5.0/src/beam/layouts.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/locale/de/LC_MESSAGES/django.mo` & `django-beam-1.5.0/src/beam/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/registry.py` & `django-beam-1.5.0/src/beam/registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/templatetags/beam_tags.py` & `django-beam-1.5.0/src/beam/templatetags/beam_tags.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css` & `django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/actions.js` & `django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/add_related.js` & `django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/add_related.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js` & `django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/inlines.js` & `django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/inlines.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js` & `django-beam-1.5.0/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/base.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/base.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/dashboard.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/delete.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/delete.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/detail.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/form.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/list.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/actions.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/actions.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/filters.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/filters.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/layout.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/links.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/messages.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/messages.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 <div class="row align-items-center" data-object-count="{% if is_paginated %}{{ page_obj.paginator.count }}{% else %}{{ object_list.count }}{% endif %}">
     <div class="{% if is_paginated %}col-sm-4{% else %}col-12{% endif %}">
         <div class="object-count">
             {% if object_list %}
                 {% if is_paginated %}
                     {% blocktrans with total=page_obj.paginator.count start=page_obj.start_index end=page_obj.end_index name=options.verbose_name_plural %}Showing {{ start }} to {{ end }} of {{ total }} {{ name }}{% endblocktrans %}
+                    {% if page_obj.paginator.count <= paginate_max_show_all %}
+                        <a class="ml-2"
+                           href="{% preserve_query_string ignore_params=page_param show_all=1 %}">
+                            {% trans "Show all"|capfirst %}
+                        </a>
+                    {% endif %}
                 {% elif page_obj.paginator.count == 1 %}
                     {% blocktrans with total=page_obj.paginator.count name_singular=options.verbose_name %}Showing {{ total }} {{ name_singular }}{% endblocktrans %}
                 {% else %}
                     {% blocktrans with total=object_list.count name_plural=options.verbose_name_plural %}Showing {{ total }} {{ name_plural }}{% endblocktrans %}
                 {% endif %}
             {% endif %}
         </div>
```

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/update.html` & `django-beam-1.5.0/src/beam/themes/bootstrap4/templates/beam/update.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/themes/bootstrap4/widgets.py` & `django-beam-1.5.0/src/beam/themes/bootstrap4/widgets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/urls.py` & `django-beam-1.5.0/src/beam/urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/utils.py` & `django-beam-1.5.0/src/beam/utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/beam/views.py` & `django-beam-1.5.0/src/beam/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,33 +532,44 @@
     ListActionsMixin,
     FiltersetMixin,
     SearchableListMixin,
     SortableListMixin,
     ComponentMixin,
     generic.ListView,
 ):
+    paginate_max_show_all = 250
+
     @property
     def search_fields(self):
         return self.component.list_search_fields
 
     def get_paginate_by(self, queryset):
-        return self.component.list_paginate_by
+        paginate_by = self.paginate_by or self.component.list_paginate_by
+
+        show_all = self.request.GET.get("show_all", False)
+
+        if show_all and queryset.count() <= self.paginate_max_show_all:
+            # ensure the queryset will not be paginated
+            return None
+
+        return paginate_by
 
     def get_search_query(self):
         if not self.search_fields:
             return ""
         return super().get_search_query()
 
     def get_template_names(self):
         return super().get_template_names() + ["beam/list.html"]
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["search_query"] = self.get_search_query()
         context["list_item_link_layout"] = self.component.list_item_link_layout
+        context["paginate_max_show_all"] = self.paginate_max_show_all
         return context
 
 
 class DetailView(InlineActionMixin, ComponentMixin, InlinesMixin, generic.DetailView):
     def get_template_names(self):
         return super().get_template_names() + ["beam/detail.html"]
```

### Comparing `django-beam-1.4.2/src/beam/viewsets.py` & `django-beam-1.5.0/src/beam/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/src/django_beam.egg-info/PKG-INFO` & `django-beam-1.5.0/src/django_beam.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.4.2
+Version: 1.5.0
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.4.2.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.5.0.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -90,10 +90,30 @@
 
 - `beam.contrib.auth`: Viewsets for editing users and groups, and optional templates for default Django registration views.
 - `beam.contrib.autocomplete_light`: Integration with `django-autocomplete-light`.
 - `beam.contrib.reversion`: Experimental integration with `django-reversion`.
 
 Refer to the documentation for usage instructions on each of the contrib packages.
 
+## Testing
+
+You can use the [tox](https://tox.readthedocs.io/en/latest/) testing tool to run the tests:
+
+```bash
+tox -e py38-djangolatest
+```
+
+Run the tests of a specific test file only:
+
+```bash
+tox -e py38-djangolatest -- test_tags
+```
+
+Run against all supported versions of Python and Django:
+
+```bash
+tox
+```
+
 ## Support
 
 If you encounter any issues or have questions, please refer to the [django-beam documentation](https://django-beam.readthedocs.io/en/latest/) or raise an issue on the [GitHub repository](https://github.com/yourgithubuser/django-beam/issues).
```

### Comparing `django-beam-1.4.2/src/django_beam.egg-info/SOURCES.txt` & `django-beam-1.5.0/src/django_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_actions.py` & `django-beam-1.5.0/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_components.py` & `django-beam-1.5.0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_contrib_auth.py` & `django-beam-1.5.0/tests/test_contrib_auth.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_contrib_autocomplete.py` & `django-beam-1.5.0/tests/test_contrib_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_contrib_reversion.py` & `django-beam-1.5.0/tests/test_contrib_reversion.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_inlines.py` & `django-beam-1.5.0/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_registry.py` & `django-beam-1.5.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_tags.py` & `django-beam-1.5.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_urls.py` & `django-beam-1.5.0/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_utils.py` & `django-beam-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.2/tests/test_views.py` & `django-beam-1.5.0/tests/test_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import TestCase, mock
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Permission
 from django.urls import reverse
+from django.utils.translation import gettext as _
 from django_webtest import WebTest
 from testapp.models import (
     CascadingSighting,
     Dragonfly,
     ProtectedSighting,
     Sighting,
     SightingReference,
@@ -159,14 +160,35 @@
         self.assertContains(response, "page=4")
         self.assertContains(response, "page=6")
 
         self.assertNotContains(response, "page=8")
         self.assertContains(response, "page=9")
         self.assertContains(response, "page=10")
 
+    def test_list_pagination_show_all(self):
+        for i in range(DragonflyViewSet.list_paginate_by * 2):
+            Dragonfly.objects.create(name="dragonfly-{:02}".format(i), age=100)
+
+        first_page = self.app.get(
+            DragonflyViewSet().links["list"].reverse(),
+            user=user_with_perms(["testapp.view_dragonfly"]),
+        )
+
+        show_all_page = first_page.click(_("Show all"))
+        self.assertContains(show_all_page, "dragonfly-00")
+        self.assertContains(show_all_page, "dragonfly-01")
+        self.assertContains(show_all_page, "dragonfly-02")
+        self.assertContains(show_all_page, "dragonfly-03")
+        self.assertContains(show_all_page, "dragonfly-04")
+        self.assertContains(show_all_page, "dragonfly-05")
+        self.assertContains(show_all_page, "dragonfly-06")
+        self.assertContains(show_all_page, "dragonfly-07")
+        self.assertContains(show_all_page, "dragonfly-08")
+        self.assertContains(show_all_page, "dragonfly-09")
+
     def test_list_requires_permission(self):
         Dragonfly.objects.create(name="alpha", age=12)
         self.app.get(
             DragonflyViewSet().links["list"].reverse(),
             user=user_with_perms([]),
             status=403,
         )
@@ -187,14 +209,53 @@
         response = self.app.get(
             DragonflyViewSet().links["list"].reverse() + "?q=alpha",
             user=user_with_perms(["testapp.view_dragonfly"]),
         )
         self.assertContains(response, "alpha")
         self.assertNotContains(response, "omega")
 
+    def test_list_clear_search(self):
+        Dragonfly.objects.create(name="alpha", age=12)
+        Dragonfly.objects.create(name="omega", age=99)
+        result_page = self.app.get(
+            DragonflyViewSet().links["list"].reverse() + "?q=alpha",
+            user=user_with_perms(["testapp.view_dragonfly"]),
+        )
+        response = result_page.click(_("Clear"), index=0)
+
+        self.assertContains(response, "alpha")
+        self.assertContains(response, "omega")
+
+    def test_list_search_and_pagination(self):
+        for i in range(DragonflyViewSet.list_paginate_by * 5):
+            Dragonfly.objects.create(name="dragonfly-{:02}".format(i), age=100)
+
+        first_page = self.app.get(
+            DragonflyViewSet().links["list"].reverse() + "?q=dragonfly-1",
+            user=user_with_perms(["testapp.view_dragonfly"]),
+        )
+        self.assertContains(first_page, "dragonfly-10")
+        self.assertContains(first_page, "dragonfly-11")
+        self.assertContains(first_page, "dragonfly-12")
+        self.assertContains(first_page, "dragonfly-13")
+        self.assertContains(first_page, "dragonfly-14")
+        self.assertNotContains(first_page, "dragonfly-15")
+
+        second_page = first_page.click("2")
+        self.assertNotContains(second_page, "dragonfly-14")
+        self.assertContains(second_page, "dragonfly-15")
+        self.assertContains(second_page, "dragonfly-16")
+        self.assertContains(second_page, "dragonfly-17")
+        self.assertContains(second_page, "dragonfly-18")
+        self.assertContains(second_page, "dragonfly-19")
+        self.assertNotContains(second_page, "dragonfly-20")
+
+        search_form = second_page.forms["search-form"]
+        self.assertEqual(search_form["q"].value, "dragonfly-1")
+
     def test_list_filter_with_class(self):
         Dragonfly.objects.create(name="alpha", age=12)
         Dragonfly.objects.create(name="omega", age=99)
         response = self.app.get(
             DragonflyViewSet().links["list"].reverse(),
             user=user_with_perms(["testapp.view_dragonfly"]),
         )
@@ -230,23 +291,110 @@
         filter_form = response.forms["filter-form"]
 
         filter_form["filter-name"] = "Tokyo"
         tokyo_response = filter_form.submit()
         self.assertNotContains(tokyo_response, "alpha")
         self.assertContains(tokyo_response, "omega")
 
+    def test_list_filter_empty(self):
+        alpha = Dragonfly.objects.create(name="alpha", age=12)
+        omega = Dragonfly.objects.create(name="omega", age=99)
+        Sighting.objects.create(name="Berlin", dragonfly=alpha)
+        Sighting.objects.create(name="Tokyo", dragonfly=omega)
+
+        response = self.app.get(
+            SightingViewSet().links["list"].reverse(),
+            user=user_with_perms(["testapp.view_sighting"]),
+        )
+
+        filter_form = response.forms["filter-form"]
+
         filter_form["filter-name"] = "nothing"
         empty_response = filter_form.submit()
         self.assertNotContains(empty_response, "alpha")
         self.assertNotContains(empty_response, "omega")
         self.assertContains(
             empty_response,
             "Could not find any sightings that match the current filters",
         )
 
+    def test_list_clear_filter(self):
+        Dragonfly.objects.create(name="alpha", age=12)
+        response = self.app.get(
+            DragonflyViewSet().links["list"].reverse(),
+            user=user_with_perms(["testapp.view_dragonfly"]),
+        )
+
+        filter_form = response.forms["filter-form"]
+
+        filter_form["filter-max_age"] = "0"
+        max_0 = filter_form.submit()
+        self.assertNotContains(max_0, "alpha")
+
+        cleared = max_0.click(_("Clear filters"))
+        self.assertContains(cleared, "alpha")
+
+    def test_list_search_and_filter(self):
+        Dragonfly.objects.create(name="alpha", age=12)
+        Dragonfly.objects.create(name="beta", age=23)
+        Dragonfly.objects.create(name="alvin", age=52)
+        Dragonfly.objects.create(name="omega", age=99)
+        searched = self.app.get(
+            DragonflyViewSet().links["list"].reverse() + "?q=al",
+            user=user_with_perms(["testapp.view_dragonfly"]),
+        )
+        self.assertContains(searched, "alpha")
+        self.assertNotContains(searched, "beta")
+        self.assertContains(searched, "alvin")
+        self.assertNotContains(searched, "omega")
+
+        filter_form = searched.forms["filter-form"]
+
+        filter_form["filter-max_age"] = "50"
+        max_50_and_searched = filter_form.submit()
+        self.assertContains(max_50_and_searched, "alpha")
+        self.assertNotContains(max_50_and_searched, "beta")
+        self.assertNotContains(max_50_and_searched, "alvin")
+        self.assertNotContains(max_50_and_searched, "omega")
+
+        max_50 = max_50_and_searched.click(_("Clear"), index=0)
+        self.assertContains(max_50, "alpha")
+        self.assertContains(max_50, "beta")
+        self.assertNotContains(max_50, "alvin")
+        self.assertNotContains(max_50, "omega")
+
+    def test_list_filter_and_search(self):
+        Dragonfly.objects.create(name="alpha", age=12)
+        Dragonfly.objects.create(name="beta", age=23)
+        Dragonfly.objects.create(name="alvin", age=52)
+        Dragonfly.objects.create(name="omega", age=99)
+
+        max_50 = self.app.get(
+            DragonflyViewSet().links["list"].reverse() + "?filter-max_age=50",
+            user=user_with_perms(["testapp.view_dragonfly"]),
+        )
+        self.assertContains(max_50, "alpha")
+        self.assertContains(max_50, "beta")
+        self.assertNotContains(max_50, "alvin")
+        self.assertNotContains(max_50, "omega")
+
+        search_form = max_50.forms["search-form"]
+        search_form["q"] = "al"
+        max_50_and_searched = search_form.submit()
+        self.assertContains(max_50_and_searched, "alpha")
+        self.assertNotContains(max_50_and_searched, "beta")
+        self.assertNotContains(max_50_and_searched, "alvin")
+        self.assertNotContains(max_50_and_searched, "omega")
+
+        searched = max_50_and_searched.click(_("Clear filters"))
+        self.assertContains(searched, "alpha")
+        self.assertNotContains(searched, "beta")
+        self.assertContains(searched, "alvin")
+        self.assertNotContains(searched, "omega")
+
     def test_list_sort(self):
         user = user_with_perms(["testapp.view_dragonfly"])
 
         Dragonfly.objects.create(name="alpha", age=12)
         Dragonfly.objects.create(name="omega", age=99)
 
         response = self.app.get(
```

### Comparing `django-beam-1.4.2/tests/test_viewsets.py` & `django-beam-1.5.0/tests/test_viewsets.py`

 * *Files identical despite different names*

