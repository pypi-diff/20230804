# Comparing `tmp/wagtail-mailchimp-integration-0.0.7.tar.gz` & `tmp/wagtail-mailchimp-integration-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-mailchimp-integration-0.0.7.tar", last modified: Mon Jun 12 13:10:52 2023, max compression
+gzip compressed data, was "wagtail-mailchimp-integration-0.0.8.tar", last modified: Fri Aug  4 14:45:52 2023, max compression
```

## Comparing `wagtail-mailchimp-integration-0.0.7.tar` & `wagtail-mailchimp-integration-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.224516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-08-04 14:45:52.000000 wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-04 14:45:52.000000 wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:45:52.000000 wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 14:45:52.000000 wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 14:45:52.000000 wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.478398 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:45:52.482398 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/wagtailmailchimp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-04 14:45:37.000000 wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/widgets.py
```

### Comparing `wagtail-mailchimp-integration-0.0.7/LICENSE` & `wagtail-mailchimp-integration-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/PKG-INFO` & `wagtail-mailchimp-integration-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.7
+Version: 0.0.8
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-mailchimp-integration-0.0.7/README.md` & `wagtail-mailchimp-integration-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/setup.cfg` & `wagtail-mailchimp-integration-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-mailchimp-integration
-version = 0.0.7
+version = 0.0.8
 description = Integration of Mailchimp Email Marketing in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-mailchimp-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/PKG-INFO` & `wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.7
+Version: 0.0.8
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/SOURCES.txt` & `wagtail-mailchimp-integration-0.0.8/wagtail_mailchimp_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/api.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/api.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/forms.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/0001_initial.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/models.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import json
 
 from django.contrib import messages
 from django.db import models
 from django.forms import BooleanField
 from django.template import Context, Template
-from django.template.response import TemplateResponse
-from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
-from django.views.decorators.csrf import csrf_exempt
 from mailchimp3.mailchimpclient import MailChimpError
 from wagtail.admin.panels import FieldPanel, FieldRowPanel, MultiFieldPanel
 from wagtail.contrib.forms.models import AbstractForm
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 
 from .api import MailchimpApi
@@ -108,103 +105,67 @@
 
     is_mailchimp_integration = True
 
     def remove_mailchimp_field(self, form):
         form.fields.pop(self.mailchimp_field_name, None)
         return form.cleaned_data.pop(self.mailchimp_field_name, None)
 
-    def process_form_submission(self, form, request=None):
+    def serve(self, request, *args, **kwargs):
+        # We need to access the request later on in integration operation
+        self.request = request
+
+        return super(AbstractMailchimpIntegrationForm, self).serve(request, *args, **kwargs)
 
+    def process_form_submission(self, form):
         self.remove_mailchimp_field(form)
 
         form_submission = super(AbstractMailchimpIntegrationForm, self).process_form_submission(form)
 
-        try:
-            self.post_process_submission(form, form_submission)
-        except Exception as e:
-            pass
-
-        return form_submission
-
-    def post_process_submission(self, form, form_submission):
-        pass
-
-    def should_process_form(self, request, form_data):
-        return True
-
-    def render_landing_page(self, request, form_submission=None, *args, form_context=None, **kwargs):
-        context = self.get_context(request)
-        context['form_submission'] = form_submission
-        if form_context:
-            context.update(form_context)
-
-        return TemplateResponse(
-            request,
-            self.get_landing_page_template(request),
-            context
-        )
+        if self.request:
+            try:
 
-    @method_decorator(csrf_exempt)
-    def serve(self, request, *args, **kwargs):
-        if request.method == 'POST':
-            form = self.get_form(request.POST, request.FILES, page=self, user=request.user)
+                form_data = dict(form.data)
+                user_checked_sub = bool(form_data.get(self.mailchimp_field_name, False))
+                user_selected_interests = form_data.get(self.mailchimp_interests_field_name, None)
+
+                if user_checked_sub:
+                    self.mailchimp_integration_operation(self, form=form, request=self.request,
+                                                         user_selected_interests=user_selected_interests)
+            except Exception as e:
+                pass
 
-            if form.is_valid():
-                form_submission = None
-                hide_thank_you_text = False
-                if self.should_process_form(request, form.cleaned_data):
-                    form_submission = self.process_form_submission(form)
-                    form_data = dict(form.data)
-                    user_checked_sub = bool(form_data.get(self.mailchimp_field_name, False))
-                    user_selected_interests = form_data.get(self.mailchimp_interests_field_name, None)
-
-                    if user_checked_sub:
-                        self.integration_operation(self, form=form, request=request,
-                                                   user_selected_interests=user_selected_interests)
-                else:
-                    # we have an issue with the form submission.Don't show thank you text
-                    hide_thank_you_text = True
-
-                return self.render_landing_page(request, form_submission,
-                                                *args,
-                                                form_context={'hide_thank_you_text': hide_thank_you_text},
-                                                **kwargs)
+        return form_submission
 
-        form = self.get_form(page=self, user=request.user)
-        context = self.get_context(request)
+    def get_form(self, *args, **kwargs):
+        form = super(AbstractMailchimpIntegrationForm, self).get_form(*args, **kwargs)
 
         if self.has_list_id_and_email:
             form.fields[self.mailchimp_field_name] = BooleanField(
                 label='',
                 required=False,
                 widget=MailchimpSubscriberOptinWidget(
-                    interest_categories=self.get_data().get("interest_categories", []),
+                    interest_categories=self.get_mc_data().get("interest_categories", []),
                     label=self.mailing_list_checkbox_label or self.default_mailing_list_checkbox_label,
                     interests_field_name=self.mailchimp_interests_field_name
                 )
             )
 
-        context['form'] = form
-        return TemplateResponse(
-            request,
-            self.get_template(request),
-            context
-        )
+        return form
 
-    def integration_operation(self, instance, **kwargs):
+    def mailchimp_integration_operation(self, instance, **kwargs):
         request = kwargs.get('request', None)
 
         mc_settings = MailchimpSettings.for_request(request)
 
         mailchimp = MailchimpApi(api_key=mc_settings.api_key)
 
         user_selected_interests = kwargs.get('user_selected_interests', None)
 
-        rendered_dictionary = self.render_dictionary(
-            self.format_form_submission(kwargs['form']),
+        rendered_dictionary = self.render_mc_dictionary(
+            self.format_mc_form_submission(kwargs['form']),
             user_selected_interests=user_selected_interests
         )
 
         try:
             dict_data = json.loads(rendered_dictionary)
             list_id = self.audience_list_id
             mailchimp.add_user_to_list(list_id=list_id, data=dict_data)
@@ -226,22 +187,22 @@
                             " adding you to our mailing list. We will try to add you later")
         except Exception as e:
             if request:
                 messages.add_message(
                     request, messages.ERROR,
                     "We are having issues adding you to our mailing list. We will try to add you later")
 
-    def format_form_submission(self, form):
+    def format_mc_form_submission(self, form):
         formatted_form_data = {}
 
         for k, v in form.cleaned_data.items():
             formatted_form_data[k.replace('-', '_')] = v
         return formatted_form_data
 
-    def get_data(self):
+    def get_mc_data(self):
         data = {
             "email_field": None,
             "merge_fields": {},
             "interest_categories": {}
         }
 
         merge_fields_mapping = {}
@@ -264,57 +225,59 @@
             else:
                 data["merge_fields"].update({key: value})
 
         data.update({"interest_categories": interest_categories})
 
         return data
 
-    def get_merge_fields(self):
-        if 'merge_fields' in self.get_data():
-            return self.get_data()['merge_fields']
+    def get_mc_merge_fields(self):
+        data = self.get_mc_data()
+        if 'merge_fields' in data:
+            return data.get('merge_fields')
         return {}
 
-    def get_email_field_template(self):
-        return "{}{}{}".format("{{", self.get_data()['email_field'], "}}")
+    def get_mc_email_field_template(self):
+        return "{}{}{}".format("{{", self.get_mc_data()['email_field'], "}}")
 
-    def get_merge_fields_template(self):
-        fields = self.get_merge_fields()
+    def get_mc_merge_fields_template(self):
+        fields = self.get_mc_merge_fields()
         for key, value in fields.items():
             if value:
                 fields[key] = "{}{}{}".format("{{", value, "}}")
         return fields
 
     @property
     def has_list_id_and_email(self):
-        return self.audience_list_id and self.get_email_address()
+        return bool(self.audience_list_id and self.get_mc_email_address())
 
-    def get_email_address(self):
-        if "email_field" in self.get_data():
-            return self.get_data().get("email_field")
+    def get_mc_email_address(self):
+        data = self.get_mc_data()
+        if "email_field" in data:
+            return data.get("email_field")
         return None
 
-    def combine_interest_categories(self):
+    def combine_mc_interest_categories(self):
         interest_dict = {}
-        for interest_category in self.get_data().get('interest_categories', []):
+        for interest_category in self.get_mc_data().get('interest_categories', []):
             for interest in interest_category.get("interests", []):
                 interest_dict.update({interest.get("id"): interest.get("id")})
 
         return interest_dict
 
-    def render_dictionary(self, form_submission, user_selected_interests=None):
+    def render_mc_dictionary(self, form_submission, user_selected_interests=None):
 
-        interests = self.combine_interest_categories(),
+        interests = self.combine_mc_interest_categories(),
 
         if user_selected_interests:
             interests = {}
             for interest in user_selected_interests:
                 interests[interest] = True
 
         rendered_dictionary_template = json.dumps({
-            'email_address': self.get_email_field_template(),
-            'merge_fields': self.get_merge_fields_template(),
+            'email_address': self.get_mc_email_field_template(),
+            'merge_fields': self.get_mc_merge_fields_template(),
             'interests': interests,
             'status': 'subscribed',
         })
 
         rendered_dictionary = Template(rendered_dictionary_template).render(Context(form_submission))
         return rendered_dictionary
```

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/views.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/wagtail_hooks.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/widgets.py` & `wagtail-mailchimp-integration-0.0.8/wagtailmailchimp/widgets.py`

 * *Files identical despite different names*

