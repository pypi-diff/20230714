# Comparing `tmp/django-appmail-4.0.tar.gz` & `tmp/django-appmail-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appmail-4.0.tar", max compression
+gzip compressed data, was "django-appmail-5.0.0.tar", max compression
```

## Comparing `django-appmail-4.0.tar` & `django-appmail-5.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1075 2022-12-16 10:44:39.973222 django-appmail-4.0/LICENSE
--rw-r--r--   0        0        0     4653 2022-12-22 11:24:22.745771 django-appmail-4.0/README.md
--rw-r--r--   0        0        0      234 2022-12-16 10:44:39.973950 django-appmail-4.0/appmail/CHANGELOG.md
--rwxr-xr-x   0        0        0       73 2022-12-22 11:25:15.212615 django-appmail-4.0/appmail/__init__.py
--rwxr-xr-x   0        0        0     9296 2022-12-22 10:55:59.157475 django-appmail-4.0/appmail/admin.py
--rw-r--r--   0        0        0       90 2022-12-16 10:44:39.974695 django-appmail-4.0/appmail/apps.py
--rw-r--r--   0        0        0     5243 2022-12-22 10:55:59.158792 django-appmail-4.0/appmail/forms.py
--rw-r--r--   0        0        0     2879 2022-12-22 10:55:59.163444 django-appmail-4.0/appmail/helpers.py
--rw-r--r--   0        0        0        0 2022-12-16 10:44:39.975402 django-appmail-4.0/appmail/management/__init__.py
--rw-r--r--   0        0        0        0 2022-12-16 10:44:39.975624 django-appmail-4.0/appmail/management/commands/__init__.py
--rw-r--r--   0        0        0     1963 2022-12-16 10:44:39.975845 django-appmail-4.0/appmail/management/commands/truncate_logged_messages.py
--rw-r--r--   0        0        0     3165 2022-12-16 10:44:39.976154 django-appmail-4.0/appmail/migrations/0001_initial.py
--rw-r--r--   0        0        0     1245 2022-12-16 10:44:39.976379 django-appmail-4.0/appmail/migrations/0002_add_template_description.py
--rw-r--r--   0        0        0      672 2022-12-16 10:44:39.976677 django-appmail-4.0/appmail/migrations/0003_emailtemplate_test_context.py
--rw-r--r--   0        0        0      607 2022-12-16 10:44:39.977159 django-appmail-4.0/appmail/migrations/0004_emailtemplate_is_active.py
--rw-r--r--   0        0        0     1560 2022-12-16 10:44:39.977517 django-appmail-4.0/appmail/migrations/0005_emailtemplate_from_email__reply_to.py
--rw-r--r--   0        0        0      566 2022-12-16 10:44:39.977836 django-appmail-4.0/appmail/migrations/0006_emailtemplate_supports_attachments.py
--rw-r--r--   0        0        0     3342 2022-12-16 10:44:39.978192 django-appmail-4.0/appmail/migrations/0007_loggedemailmessage.py
--rw-r--r--   0        0        0      595 2022-12-22 10:55:59.182237 django-appmail-4.0/appmail/migrations/0008_add_logged_message_indexes.py
--rw-r--r--   0        0        0        0 2022-12-16 10:44:39.978622 django-appmail-4.0/appmail/migrations/__init__.py
--rwxr-xr-x   0        0        0    16231 2022-12-22 10:55:59.190086 django-appmail-4.0/appmail/models.py
--rw-r--r--   0        0        0      805 2022-12-16 10:44:39.979937 django-appmail-4.0/appmail/settings.py
--rw-r--r--   0        0        0      769 2022-12-16 10:44:39.981706 django-appmail-4.0/appmail/templates/admin/appmail/emailtemplate/change_form.html
--rw-r--r--   0        0        0      842 2022-12-16 10:44:39.982204 django-appmail-4.0/appmail/templates/admin/appmail/loggedmessage/change_form.html
--rw-r--r--   0        0        0     1930 2022-12-16 10:44:39.982634 django-appmail-4.0/appmail/templates/appmail/send_test_email.html
--rw-r--r--   0        0        0      105 2022-12-16 10:44:39.982995 django-appmail-4.0/appmail/templates/base.html
--rw-r--r--   0        0        0       42 2022-12-16 10:44:39.983277 django-appmail-4.0/appmail/templates/base.txt
--rw-r--r--   0        0        0      585 2022-12-16 10:44:39.983789 django-appmail-4.0/appmail/tests/fixtures/templates.json
--rw-r--r--   0        0        0     1352 2022-12-16 10:44:39.984038 django-appmail-4.0/appmail/urls.py
--rw-r--r--   0        0        0     4977 2022-12-16 10:44:39.984304 django-appmail-4.0/appmail/views.py
--rw-r--r--   0        0        0     1239 2022-12-22 11:25:31.384064 django-appmail-4.0/pyproject.toml
--rw-r--r--   0        0        0     5756 2022-12-22 11:26:03.694949 django-appmail-4.0/setup.py
--rw-r--r--   0        0        0     5622 2022-12-22 11:26:03.695245 django-appmail-4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-12-16 10:44:39.973222 django-appmail-5.0.0/LICENSE
+-rw-r--r--   0        0        0     4653 2023-07-14 14:42:19.962376 django-appmail-5.0.0/README.md
+-rw-r--r--   0        0        0      234 2022-12-16 10:44:39.973950 django-appmail-5.0.0/appmail/CHANGELOG.md
+-rwxr-xr-x   0        0        0       73 2023-07-14 14:39:50.022409 django-appmail-5.0.0/appmail/__init__.py
+-rwxr-xr-x   0        0        0    11914 2023-07-14 14:37:37.680621 django-appmail-5.0.0/appmail/admin.py
+-rw-r--r--   0        0        0       89 2023-07-14 14:37:37.680981 django-appmail-5.0.0/appmail/apps.py
+-rw-r--r--   0        0        0     5243 2022-12-22 10:55:59.158792 django-appmail-5.0.0/appmail/forms.py
+-rw-r--r--   0        0        0     2879 2022-12-22 10:55:59.163444 django-appmail-5.0.0/appmail/helpers.py
+-rw-r--r--   0        0        0        0 2022-12-16 10:44:39.975402 django-appmail-5.0.0/appmail/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-16 10:44:39.975624 django-appmail-5.0.0/appmail/management/commands/__init__.py
+-rw-r--r--   0        0        0     1962 2023-07-14 14:37:37.681340 django-appmail-5.0.0/appmail/management/commands/truncate_logged_messages.py
+-rw-r--r--   0        0        0     3164 2023-07-14 14:37:37.681674 django-appmail-5.0.0/appmail/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1244 2023-07-14 14:37:37.681966 django-appmail-5.0.0/appmail/migrations/0002_add_template_description.py
+-rw-r--r--   0        0        0      671 2023-07-14 14:37:37.682232 django-appmail-5.0.0/appmail/migrations/0003_emailtemplate_test_context.py
+-rw-r--r--   0        0        0      606 2023-07-14 14:37:37.682477 django-appmail-5.0.0/appmail/migrations/0004_emailtemplate_is_active.py
+-rw-r--r--   0        0        0     1559 2023-07-14 14:37:37.682706 django-appmail-5.0.0/appmail/migrations/0005_emailtemplate_from_email__reply_to.py
+-rw-r--r--   0        0        0      565 2023-07-14 14:37:37.682968 django-appmail-5.0.0/appmail/migrations/0006_emailtemplate_supports_attachments.py
+-rw-r--r--   0        0        0     3341 2023-07-14 14:37:37.683249 django-appmail-5.0.0/appmail/migrations/0007_loggedemailmessage.py
+-rw-r--r--   0        0        0      594 2023-07-14 14:37:37.683519 django-appmail-5.0.0/appmail/migrations/0008_add_logged_message_indexes.py
+-rw-r--r--   0        0        0        0 2022-12-16 10:44:39.978622 django-appmail-5.0.0/appmail/migrations/__init__.py
+-rwxr-xr-x   0        0        0    16231 2023-07-14 14:37:37.683921 django-appmail-5.0.0/appmail/models.py
+-rw-r--r--   0        0        0      805 2022-12-16 10:44:39.979937 django-appmail-5.0.0/appmail/settings.py
+-rw-r--r--   0        0        0      769 2022-12-16 10:44:39.981706 django-appmail-5.0.0/appmail/templates/admin/appmail/emailtemplate/change_form.html
+-rw-r--r--   0        0        0      842 2022-12-16 10:44:39.982204 django-appmail-5.0.0/appmail/templates/admin/appmail/loggedmessage/change_form.html
+-rw-r--r--   0        0        0      926 2023-07-14 14:37:37.684251 django-appmail-5.0.0/appmail/templates/admin/appmail/loggedmessage/template_name_filter.html
+-rw-r--r--   0        0        0     1930 2022-12-16 10:44:39.982634 django-appmail-5.0.0/appmail/templates/appmail/send_test_email.html
+-rw-r--r--   0        0        0      105 2022-12-16 10:44:39.982995 django-appmail-5.0.0/appmail/templates/base.html
+-rw-r--r--   0        0        0       42 2022-12-16 10:44:39.983277 django-appmail-5.0.0/appmail/templates/base.txt
+-rw-r--r--   0        0        0      585 2022-12-16 10:44:39.983789 django-appmail-5.0.0/appmail/tests/fixtures/templates.json
+-rw-r--r--   0        0        0     1352 2022-12-16 10:44:39.984038 django-appmail-5.0.0/appmail/urls.py
+-rw-r--r--   0        0        0     4977 2022-12-16 10:44:39.984304 django-appmail-5.0.0/appmail/views.py
+-rw-r--r--   0        0        0     1241 2023-07-14 14:39:56.852321 django-appmail-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5758 2023-07-14 14:44:24.767022 django-appmail-5.0.0/setup.py
+-rw-r--r--   0        0        0     5624 2023-07-14 14:44:24.767346 django-appmail-5.0.0/PKG-INFO
```

### Comparing `django-appmail-4.0/LICENSE` & `django-appmail-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/README.md` & `django-appmail-5.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/django-appmail.svg)](https://pypi.org/project/django-appmail/)
 
 Django app for managing transactional email templates.
 
 ## Compatibility
 
-This project now requires Django 3.2+ and Python 3.8+. If you require a previous
+This project now requires Django 4.0+ and Python 3.9+. If you require a previous
 version you will have to refer to the relevant branch or tag.
 
 ## Background
 
 This project arose out of a project to integrate a large transactional Django
 application with Mandrill, and the lessons learned. It also owes a minor h/t to
 this project from 2011 (https://github.com/hugorodgerbrown/AppMail).
```

### Comparing `django-appmail-4.0/appmail/admin.py` & `django-appmail-5.0.0/appmail/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         pretty = json.dumps(data, sort_keys=True, indent=4, separators=(",", ": "))
         html = pretty.replace(" ", "&nbsp;").replace("\n", "<br>")
         return mark_safe("<pre><code>%s</code></pre>" % html)  # noqa: S703,S308
 
 
 @admin.register(EmailTemplate)
 class EmailTemplateAdmin(AdminBase):
-
     formfield_overrides = {JSONField: {"widget": JSONWidget}}
 
     list_display = (
         "name",
         "subject",
         "language",
         "version",
@@ -233,26 +232,102 @@
         return HttpResponseRedirect(request.path)
 
     deactivate_templates.short_description = _lazy(  # type: ignore
         "Deactivate selected email templates"
     )
 
 
+class TemplateNameListFilter(admin.SimpleListFilter):
+    """
+    Provide a list of template names to filter by.
+
+    This is more efficient than providing `template__name` to list_filter
+    because that would ask the question "which templates are in use for
+    this set of logged messages" which requires a join and is thus slower
+    over a large result set. This instead asks the question "which templates
+    are even available" which is much faster.
+    """
+
+    title = _lazy("Template name")
+    parameter_name = "template_name"
+    template = "admin/appmail/loggedmessage/template_name_filter.html"
+
+    def lookups(
+        self, request: HttpRequest, model_admin: admin.ModelAdmin
+    ) -> tuple[tuple[str, str], ...]:
+        templates = (
+            EmailTemplate.objects.values_list("name", flat=True)
+            .distinct()
+            .order_by("name")
+        )
+        return tuple((name, name) for name in templates)
+
+    def queryset(self, request: HttpRequest, queryset: QuerySet) -> QuerySet:
+        """
+        Return the filtered queryset.
+
+        Filter based on the value provided in the query string and
+        retrievable via `self.value()`.
+
+        """
+        if value := self.value():
+            return queryset.filter(template__name__exact=value)
+
+        return queryset
+
+
+class TemplateLanguageListFilter(admin.SimpleListFilter):
+    """
+    Provide a list of template languages to filter by.
+
+    This is more efficient than providing `template__language` to list_filter
+    because that would ask the question "which template languages are in use
+    for this set of logged messages" which requires a join and is thus slower
+    over a large result set. This instead asks the question "which templates
+    languages are even available" which is much faster.
+    """
+
+    title = _lazy("Template language")
+    parameter_name = "template_language"
+
+    def lookups(
+        self, request: HttpRequest, model_admin: admin.ModelAdmin
+    ) -> tuple[tuple[str, str], ...]:
+        templates = (
+            EmailTemplate.objects.values_list("language", flat=True)
+            .distinct()
+            .order_by("language")
+        )
+        return tuple((lang, lang) for lang in templates)
+
+    def queryset(self, request: HttpRequest, queryset: QuerySet) -> QuerySet:
+        """
+        Return the filtered queryset.
+
+        Filter based on the value provided in the query string and
+        retrievable via `self.value()`.
+
+        """
+        if value := self.value():
+            return queryset.filter(template__language__exact=value)
+
+        return queryset
+
+
 @admin.register(LoggedMessage)
 class LoggedMessageAdmin(AdminBase):
-
     exclude = ("html", "context")
 
     formfield_overrides = {JSONField: {"widget": JSONWidget}}
 
     list_display = ("to", "template_name", "_subject", "timestamp")
 
     list_select_related = ("template",)
 
-    list_filter = ("timestamp", "template__name", "template__language")
+    list_filter = ("timestamp", TemplateNameListFilter, TemplateLanguageListFilter)
 
     raw_id_fields = ("user", "template")
 
     readonly_fields = (
         "to",
         "user",
         "template",
```

### Comparing `django-appmail-4.0/appmail/forms.py` & `django-appmail-5.0.0/appmail/forms.py`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/helpers.py` & `django-appmail-5.0.0/appmail/helpers.py`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/management/commands/truncate_logged_messages.py` & `django-appmail-5.0.0/appmail/management/commands/truncate_logged_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from django.utils.translation import gettext_lazy as _lazy
 
 from appmail.models import LoggedMessage
 from appmail.settings import LOG_RETENTION_PERIOD
 
 
 class Command(BaseCommand):
-
     help = _lazy("Truncate all log records that have passed the LOG_RETENTION_PERIOD.")
 
     def add_arguments(self, parser: CommandParser) -> None:
         super().add_arguments(parser)
         parser.add_argument(
             "-r",
             "--retention",
```

### Comparing `django-appmail-4.0/appmail/migrations/0001_initial.py` & `django-appmail-5.0.0/appmail/migrations/0001_initial.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.10 on 2017-03-11 11:36
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="EmailTemplate",
```

### Comparing `django-appmail-4.0/appmail/migrations/0002_add_template_description.py` & `django-appmail-5.0.0/appmail/migrations/0002_add_template_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("appmail", "0001_initial")]
 
     operations = [
         migrations.AddField(
             model_name="emailtemplate",
             name="description",
             field=models.CharField(
```

### Comparing `django-appmail-4.0/appmail/migrations/0003_emailtemplate_test_context.py` & `django-appmail-5.0.0/appmail/migrations/0003_emailtemplate_test_context.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.10.6 on 2017-05-06 08:15
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("appmail", "0002_add_template_description")]
 
     operations = [
         migrations.AddField(
             model_name="emailtemplate",
             name="test_context",
             field=models.JSONField(
```

### Comparing `django-appmail-4.0/appmail/migrations/0004_emailtemplate_is_active.py` & `django-appmail-5.0.0/appmail/migrations/0004_emailtemplate_is_active.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.10.6 on 2017-08-07 06:10
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("appmail", "0003_emailtemplate_test_context")]
 
     operations = [
         migrations.AddField(
             model_name="emailtemplate",
             name="is_active",
             field=models.BooleanField(
```

### Comparing `django-appmail-4.0/appmail/migrations/0005_emailtemplate_from_email__reply_to.py` & `django-appmail-5.0.0/appmail/migrations/0005_emailtemplate_from_email__reply_to.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("appmail", "0004_emailtemplate_is_active")]
 
     operations = [
         migrations.AddField(
             model_name="emailtemplate",
             name="from_email",
             field=models.CharField(
```

### Comparing `django-appmail-4.0/appmail/migrations/0006_emailtemplate_supports_attachments.py` & `django-appmail-5.0.0/appmail/migrations/0006_emailtemplate_supports_attachments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.7 on 2019-11-12 07:35
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("appmail", "0005_emailtemplate_from_email__reply_to")]
 
     operations = [
         migrations.AddField(
             model_name="emailtemplate",
             name="supports_attachments",
             field=models.BooleanField(
```

### Comparing `django-appmail-4.0/appmail/migrations/0007_loggedemailmessage.py` & `django-appmail-5.0.0/appmail/migrations/0007_loggedemailmessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import django.db.models.deletion
 import django.utils.timezone
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("appmail", "0006_emailtemplate_supports_attachments"),
     ]
 
     operations = [
         migrations.CreateModel(
```

### Comparing `django-appmail-4.0/appmail/migrations/0008_add_logged_message_indexes.py` & `django-appmail-5.0.0/appmail/migrations/0008_add_logged_message_indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.4 on 2022-12-21 11:52
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("appmail", "0007_loggedemailmessage"),
     ]
 
     operations = [
         migrations.AddIndex(
             model_name="loggedmessage",
```

### Comparing `django-appmail-4.0/appmail/models.py` & `django-appmail-5.0.0/appmail/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,16 +424,16 @@
 
     class Meta:
         get_latest_by = "timestamp"
         verbose_name = "Email message"
         verbose_name_plural = "Email messages sent"
         indexes = (
             # Indexes to help the admin search.
-            models.Index(fields=['to']),
-            models.Index(fields=['subject']),
+            models.Index(fields=["to"]),
+            models.Index(fields=["subject"]),
         )
 
     def __repr__(self) -> str:
         return (
             f"<LoggedMessage id:{self.id} template='{self.template_name}' "
             f"to='{self.to}'>"
         )
```

### Comparing `django-appmail-4.0/appmail/settings.py` & `django-appmail-5.0.0/appmail/settings.py`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/templates/admin/appmail/emailtemplate/change_form.html` & `django-appmail-5.0.0/appmail/templates/admin/appmail/emailtemplate/change_form.html`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/templates/admin/appmail/loggedmessage/change_form.html` & `django-appmail-5.0.0/appmail/templates/admin/appmail/loggedmessage/change_form.html`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/templates/appmail/send_test_email.html` & `django-appmail-5.0.0/appmail/templates/appmail/send_test_email.html`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/tests/fixtures/templates.json` & `django-appmail-5.0.0/appmail/tests/fixtures/templates.json`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/urls.py` & `django-appmail-5.0.0/appmail/urls.py`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/appmail/views.py` & `django-appmail-5.0.0/appmail/views.py`

 * *Files identical despite different names*

### Comparing `django-appmail-4.0/pyproject.toml` & `django-appmail-5.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-appmail"
-version = "4.0"
+version = "5.0.0"
 description = "Django app for managing localised email templates."
 authors = ["YunoJuno <code@yunojuno.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/yunojuno/django-appmail"
 repository = "https://github.com/yunojuno/django-appmail"
 classifiers = [
```

### Comparing `django-appmail-4.0/setup.py` & `django-appmail-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
              'tests/fixtures/*']}
 
 install_requires = \
 ['django>=3.2,<5.0']
 
 setup_kwargs = {
     'name': 'django-appmail',
-    'version': '4.0',
+    'version': '5.0.0',
     'description': 'Django app for managing localised email templates.',
-    'long_description': '# Django-AppMail\n\n[![PyPI](https://img.shields.io/pypi/v/django-appmail.svg)](https://pypi.org/project/django-appmail/)\n\nDjango app for managing transactional email templates.\n\n## Compatibility\n\nThis project now requires Django 3.2+ and Python 3.8+. If you require a previous\nversion you will have to refer to the relevant branch or tag.\n\n## Background\n\nThis project arose out of a project to integrate a large transactional Django\napplication with Mandrill, and the lessons learned. It also owes a minor h/t to\nthis project from 2011 (https://github.com/hugorodgerbrown/AppMail).\n\nThe core requirement is to provide an easy way to add / edit email templates to\na Django project, in such a way that it doesn\'t require a developer to make\nchanges. The easiest way to use templated emails in Django is to rely on the\nin-built template structure, but that means that the templates are held in\nfiles, under version control, which makes it very hard for non-developers to\nedit.\n\nThis is **not** a WYSIWYG HTML editor, and it doesn\'t do anything clever. It\ndoesn\'t handle the sending of the emails - it simply provides a convenient\nmechanism for storing and rendering email content.\n\n```python\nfrom appmail.models import EmailTemplate, AppmailMessage\n\ndef send_order_confirmation(order_id):\n    order = Orders.objects.get(id=order_id)\n    template = EmailTemplate.objects.current(\'order_confirmation\')\n    context = { "order": order }\n    message = AppmailMessage(\n        template=template,\n        context=context,\n        to=[order.recipient.email]\n    )\n    message.send()\n```\n\nThe core requirements are:\n\n1. List / preview existing templates\n2. Edit subject line, plain text and HTML content\n3. Use standard Django template syntax\n4. Support base templates\n5. Template versioning\n6. Language support\n7. Send test emails\n8. Log emails sent (if desired)\n\n### Email logging (v2)\n\nFrom v2 on, it is possible to log all emails that are sent via\n`AppmailMessage.send`. It records the template, context and the rendered output,\nso that the email can be views as sent, and resent. It will attempt to record\nthe User to whom the email was sent, as well as the email address. This is\ndependent on there being a unique 1:1 match from email to User object, but can\nprove useful in tracking emails sent to users when they change their email\naddress.\n\n### Template properties\n\nIndividual templates are stored as model objects in the database. The standard\nDjango admin site is used to view / filter templates. The templates are ordered\nby name, language and version. This combination is unique. The language and\nversion properties have sensible defaults (`version=settings.LANGUAGE_CODE` and\n`version=0`) so don\'t need to set if you don\'t require it. There is no\ninheritance or relationship between different languages and versions - they are\nstored as independent objects.\n\n```python\n# get the default order_summary email (language = settings.LANGUAGE_CODE)\ntemplate = EmailTemplate.objects.current(\'order_summary\')\n# get the french version\ntemplate = EmailTemplate.objects.current(\'order_summary\', language=\'fr\')\n# get a specific version\ntemplate = EmailTemplate.objects.version(\'order_summary\', 1)\n```\n\n**Template syntax**\n\nThe templates themselves use standard Django template syntax, including the use\nof tags, filters. There is nothing special about them, however there is one\ncaveat - template inheritance.\n\n**Template inheritance**\n\nAlthough the template content is not stored on disk, without re-engineering the\ntemplate rendering methods any parent templates must be. This is annoying, but\nthere is a valid assumption behind it - if you are changing your base templates\nyou are probably involving designers and developers already, so having to rely\non a developer to make the changes is acceptable.\n\n**Sending test emails**\n\nYou can send test emails to an email address through the admin list view.\n\n<img src="screenshots/appmail-test-email-action.png" alt="EmailTemplate admin\nchange form" />\n\nThe custom admin action \'Send test emails\' will redirect to an intermediate page\nwhere you can enter the recipient email address and send the email:\n\n<img src="screenshots/appmail-test-email-send.png"/>\n\nThere is also a linkon individual template admin pages (top-right, next to the\nhistory link):\n\n<img src="screenshots/appmail-template-change-form.png" alt="EmailTemplate admin\nchange form" />\n\n## Tests\n\nThere is a test suite for the app, which is best run through `tox`.\n\n## License\n\nMIT\n\n## Contributing\n\nUsual rules apply:\n\n1. Fork to your own account\n2. Fix the issue / add the feature\n3. Submit PR\n\nPlease take care to follow the coding style - and PEP8.\n',
+    'long_description': '# Django-AppMail\n\n[![PyPI](https://img.shields.io/pypi/v/django-appmail.svg)](https://pypi.org/project/django-appmail/)\n\nDjango app for managing transactional email templates.\n\n## Compatibility\n\nThis project now requires Django 4.0+ and Python 3.9+. If you require a previous\nversion you will have to refer to the relevant branch or tag.\n\n## Background\n\nThis project arose out of a project to integrate a large transactional Django\napplication with Mandrill, and the lessons learned. It also owes a minor h/t to\nthis project from 2011 (https://github.com/hugorodgerbrown/AppMail).\n\nThe core requirement is to provide an easy way to add / edit email templates to\na Django project, in such a way that it doesn\'t require a developer to make\nchanges. The easiest way to use templated emails in Django is to rely on the\nin-built template structure, but that means that the templates are held in\nfiles, under version control, which makes it very hard for non-developers to\nedit.\n\nThis is **not** a WYSIWYG HTML editor, and it doesn\'t do anything clever. It\ndoesn\'t handle the sending of the emails - it simply provides a convenient\nmechanism for storing and rendering email content.\n\n```python\nfrom appmail.models import EmailTemplate, AppmailMessage\n\ndef send_order_confirmation(order_id):\n    order = Orders.objects.get(id=order_id)\n    template = EmailTemplate.objects.current(\'order_confirmation\')\n    context = { "order": order }\n    message = AppmailMessage(\n        template=template,\n        context=context,\n        to=[order.recipient.email]\n    )\n    message.send()\n```\n\nThe core requirements are:\n\n1. List / preview existing templates\n2. Edit subject line, plain text and HTML content\n3. Use standard Django template syntax\n4. Support base templates\n5. Template versioning\n6. Language support\n7. Send test emails\n8. Log emails sent (if desired)\n\n### Email logging (v2)\n\nFrom v2 on, it is possible to log all emails that are sent via\n`AppmailMessage.send`. It records the template, context and the rendered output,\nso that the email can be views as sent, and resent. It will attempt to record\nthe User to whom the email was sent, as well as the email address. This is\ndependent on there being a unique 1:1 match from email to User object, but can\nprove useful in tracking emails sent to users when they change their email\naddress.\n\n### Template properties\n\nIndividual templates are stored as model objects in the database. The standard\nDjango admin site is used to view / filter templates. The templates are ordered\nby name, language and version. This combination is unique. The language and\nversion properties have sensible defaults (`version=settings.LANGUAGE_CODE` and\n`version=0`) so don\'t need to set if you don\'t require it. There is no\ninheritance or relationship between different languages and versions - they are\nstored as independent objects.\n\n```python\n# get the default order_summary email (language = settings.LANGUAGE_CODE)\ntemplate = EmailTemplate.objects.current(\'order_summary\')\n# get the french version\ntemplate = EmailTemplate.objects.current(\'order_summary\', language=\'fr\')\n# get a specific version\ntemplate = EmailTemplate.objects.version(\'order_summary\', 1)\n```\n\n**Template syntax**\n\nThe templates themselves use standard Django template syntax, including the use\nof tags, filters. There is nothing special about them, however there is one\ncaveat - template inheritance.\n\n**Template inheritance**\n\nAlthough the template content is not stored on disk, without re-engineering the\ntemplate rendering methods any parent templates must be. This is annoying, but\nthere is a valid assumption behind it - if you are changing your base templates\nyou are probably involving designers and developers already, so having to rely\non a developer to make the changes is acceptable.\n\n**Sending test emails**\n\nYou can send test emails to an email address through the admin list view.\n\n<img src="screenshots/appmail-test-email-action.png" alt="EmailTemplate admin\nchange form" />\n\nThe custom admin action \'Send test emails\' will redirect to an intermediate page\nwhere you can enter the recipient email address and send the email:\n\n<img src="screenshots/appmail-test-email-send.png"/>\n\nThere is also a linkon individual template admin pages (top-right, next to the\nhistory link):\n\n<img src="screenshots/appmail-template-change-form.png" alt="EmailTemplate admin\nchange form" />\n\n## Tests\n\nThere is a test suite for the app, which is best run through `tox`.\n\n## License\n\nMIT\n\n## Contributing\n\nUsual rules apply:\n\n1. Fork to your own account\n2. Fix the issue / add the feature\n3. Submit PR\n\nPlease take care to follow the coding style - and PEP8.\n',
     'author': 'YunoJuno',
     'author_email': 'code@yunojuno.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/yunojuno/django-appmail',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `django-appmail-4.0/PKG-INFO` & `django-appmail-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appmail
-Version: 4.0
+Version: 5.0.0
 Summary: Django app for managing localised email templates.
 Home-page: https://github.com/yunojuno/django-appmail
 License: MIT
 Author: YunoJuno
 Author-email: code@yunojuno.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
@@ -27,15 +27,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/django-appmail.svg)](https://pypi.org/project/django-appmail/)
 
 Django app for managing transactional email templates.
 
 ## Compatibility
 
-This project now requires Django 3.2+ and Python 3.8+. If you require a previous
+This project now requires Django 4.0+ and Python 3.9+. If you require a previous
 version you will have to refer to the relevant branch or tag.
 
 ## Background
 
 This project arose out of a project to integrate a large transactional Django
 application with Mandrill, and the lessons learned. It also owes a minor h/t to
 this project from 2011 (https://github.com/hugorodgerbrown/AppMail).
```

