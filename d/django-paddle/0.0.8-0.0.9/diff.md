# Comparing `tmp/django-paddle-0.0.8.tar.gz` & `tmp/django-paddle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-paddle-0.0.8.tar", last modified: Sun May 10 13:19:24 2020, max compression
+gzip compressed data, was "django-paddle-0.0.9.tar", last modified: Sun Nov 28 15:56:57 2021, max compression
```

## Comparing `django-paddle-0.0.8.tar` & `django-paddle-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 k         (1000) k         (1000)        0 2020-05-10 13:19:24.495575 django-paddle-0.0.8/
--rw-r--r--   0 k         (1000) k         (1000)      302 2020-05-10 13:19:24.495575 django-paddle-0.0.8/PKG-INFO
--rw-r--r--   0 k         (1000) k         (1000)      312 2020-05-02 18:47:30.000000 django-paddle-0.0.8/README.md
-drwxr-xr-x   0 k         (1000) k         (1000)        0 2020-05-10 13:19:24.493575 django-paddle-0.0.8/django_paddle/
--rw-r--r--   0 k         (1000) k         (1000)        0 2020-04-29 19:32:36.000000 django-paddle-0.0.8/django_paddle/__init__.py
--rw-r--r--   0 k         (1000) k         (1000)      586 2020-05-02 18:47:30.000000 django-paddle-0.0.8/django_paddle/admin.py
--rw-r--r--   0 k         (1000) k         (1000)      135 2020-04-29 19:32:36.000000 django-paddle-0.0.8/django_paddle/apps.py
--rw-r--r--   0 k         (1000) k         (1000)     3481 2020-05-02 18:47:30.000000 django-paddle-0.0.8/django_paddle/client.py
-drwxr-xr-x   0 k         (1000) k         (1000)        0 2020-05-10 13:19:24.494575 django-paddle-0.0.8/django_paddle/management/
--rw-r--r--   0 k         (1000) k         (1000)        0 2020-05-06 21:38:15.000000 django-paddle-0.0.8/django_paddle/management/__init__.py
-drwxr-xr-x   0 k         (1000) k         (1000)        0 2020-05-10 13:19:24.494575 django-paddle-0.0.8/django_paddle/management/commands/
--rw-r--r--   0 k         (1000) k         (1000)        0 2020-05-06 21:38:20.000000 django-paddle-0.0.8/django_paddle/management/commands/__init__.py
--rw-r--r--   0 k         (1000) k         (1000)      320 2020-05-09 22:31:54.000000 django-paddle-0.0.8/django_paddle/management/commands/paddle_sync_payments.py
--rw-r--r--   0 k         (1000) k         (1000)      217 2020-05-02 18:47:30.000000 django-paddle-0.0.8/django_paddle/management/commands/paddle_sync_plans.py
--rw-r--r--   0 k         (1000) k         (1000)      241 2020-05-02 18:47:30.000000 django-paddle-0.0.8/django_paddle/management/commands/paddle_sync_subscriptions.py
-drwxr-xr-x   0 k         (1000) k         (1000)        0 2020-05-10 13:19:24.495575 django-paddle-0.0.8/django_paddle/migrations/
--rw-r--r--   0 k         (1000) k         (1000)     3768 2020-05-09 22:04:12.000000 django-paddle-0.0.8/django_paddle/migrations/0001_initial.py
--rw-r--r--   0 k         (1000) k         (1000)        0 2020-04-29 19:32:36.000000 django-paddle-0.0.8/django_paddle/migrations/__init__.py
--rw-r--r--   0 k         (1000) k         (1000)     5869 2020-05-10 13:16:03.000000 django-paddle-0.0.8/django_paddle/models.py
--rw-r--r--   0 k         (1000) k         (1000)     1045 2020-05-03 16:00:42.000000 django-paddle-0.0.8/django_paddle/receivers.py
--rw-r--r--   0 k         (1000) k         (1000)     1052 2020-04-29 19:32:36.000000 django-paddle-0.0.8/django_paddle/signals.py
--rw-r--r--   0 k         (1000) k         (1000)      148 2020-04-29 19:32:36.000000 django-paddle-0.0.8/django_paddle/urls.py
--rw-r--r--   0 k         (1000) k         (1000)     1687 2020-05-03 19:17:50.000000 django-paddle-0.0.8/django_paddle/utils.py
--rw-r--r--   0 k         (1000) k         (1000)      559 2020-05-03 16:12:05.000000 django-paddle-0.0.8/django_paddle/views.py
-drwxr-xr-x   0 k         (1000) k         (1000)        0 2020-05-10 13:19:24.494575 django-paddle-0.0.8/django_paddle.egg-info/
--rw-r--r--   0 k         (1000) k         (1000)      302 2020-05-10 13:19:24.000000 django-paddle-0.0.8/django_paddle.egg-info/PKG-INFO
--rw-r--r--   0 k         (1000) k         (1000)      778 2020-05-10 13:19:24.000000 django-paddle-0.0.8/django_paddle.egg-info/SOURCES.txt
--rw-r--r--   0 k         (1000) k         (1000)        1 2020-05-10 13:19:24.000000 django-paddle-0.0.8/django_paddle.egg-info/dependency_links.txt
--rw-r--r--   0 k         (1000) k         (1000)       59 2020-05-10 13:19:24.000000 django-paddle-0.0.8/django_paddle.egg-info/requires.txt
--rw-r--r--   0 k         (1000) k         (1000)       14 2020-05-10 13:19:24.000000 django-paddle-0.0.8/django_paddle.egg-info/top_level.txt
--rw-r--r--   0 k         (1000) k         (1000)       38 2020-05-10 13:19:24.495575 django-paddle-0.0.8/setup.cfg
--rw-r--r--   0 k         (1000) k         (1000)      517 2020-05-10 13:19:10.000000 django-paddle-0.0.8/setup.py
+drwxrwxr-x   0 k         (1000) k         (1000)        0 2021-11-28 15:56:57.646519 django-paddle-0.0.9/
+-rw-rw-r--   0 k         (1000) k         (1000)      302 2021-11-28 15:56:57.646519 django-paddle-0.0.9/PKG-INFO
+-rw-rw-r--   0 k         (1000) k         (1000)     3320 2021-11-28 13:34:18.000000 django-paddle-0.0.9/README.md
+drwxrwxr-x   0 k         (1000) k         (1000)        0 2021-11-28 15:56:57.646519 django-paddle-0.0.9/django_paddle/
+-rw-rw-r--   0 k         (1000) k         (1000)        0 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/__init__.py
+-rw-rw-r--   0 k         (1000) k         (1000)      586 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/admin.py
+-rw-rw-r--   0 k         (1000) k         (1000)      135 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/apps.py
+-rw-rw-r--   0 k         (1000) k         (1000)     3793 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/client.py
+drwxrwxr-x   0 k         (1000) k         (1000)        0 2021-11-28 15:56:57.646519 django-paddle-0.0.9/django_paddle/management/
+-rw-rw-r--   0 k         (1000) k         (1000)        0 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/management/__init__.py
+drwxrwxr-x   0 k         (1000) k         (1000)        0 2021-11-28 15:56:57.646519 django-paddle-0.0.9/django_paddle/management/commands/
+-rw-rw-r--   0 k         (1000) k         (1000)        0 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/management/commands/__init__.py
+-rw-rw-r--   0 k         (1000) k         (1000)      320 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/management/commands/paddle_sync_payments.py
+-rw-rw-r--   0 k         (1000) k         (1000)      217 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/management/commands/paddle_sync_plans.py
+-rw-rw-r--   0 k         (1000) k         (1000)      327 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/management/commands/paddle_sync_subscriptions.py
+drwxrwxr-x   0 k         (1000) k         (1000)        0 2021-11-28 15:56:57.646519 django-paddle-0.0.9/django_paddle/migrations/
+-rw-rw-r--   0 k         (1000) k         (1000)     3768 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/migrations/0001_initial.py
+-rw-rw-r--   0 k         (1000) k         (1000)      426 2021-11-28 15:32:51.000000 django-paddle-0.0.9/django_paddle/migrations/0002_paddlesubscription_cancellation_effective_date.py
+-rw-rw-r--   0 k         (1000) k         (1000)        0 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/migrations/__init__.py
+-rw-rw-r--   0 k         (1000) k         (1000)     6477 2021-11-28 15:43:51.000000 django-paddle-0.0.9/django_paddle/models.py
+-rw-rw-r--   0 k         (1000) k         (1000)     1605 2021-11-28 15:48:11.000000 django-paddle-0.0.9/django_paddle/receivers.py
+-rw-rw-r--   0 k         (1000) k         (1000)     1052 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/signals.py
+-rw-rw-r--   0 k         (1000) k         (1000)      148 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/urls.py
+-rw-rw-r--   0 k         (1000) k         (1000)     1687 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/utils.py
+-rw-rw-r--   0 k         (1000) k         (1000)      716 2021-11-28 13:34:18.000000 django-paddle-0.0.9/django_paddle/views.py
+drwxrwxr-x   0 k         (1000) k         (1000)        0 2021-11-28 15:56:57.646519 django-paddle-0.0.9/django_paddle.egg-info/
+-rw-rw-r--   0 k         (1000) k         (1000)      302 2021-11-28 15:56:57.000000 django-paddle-0.0.9/django_paddle.egg-info/PKG-INFO
+-rw-rw-r--   0 k         (1000) k         (1000)      858 2021-11-28 15:56:57.000000 django-paddle-0.0.9/django_paddle.egg-info/SOURCES.txt
+-rw-rw-r--   0 k         (1000) k         (1000)        1 2021-11-28 15:56:57.000000 django-paddle-0.0.9/django_paddle.egg-info/dependency_links.txt
+-rw-rw-r--   0 k         (1000) k         (1000)       59 2021-11-28 15:56:57.000000 django-paddle-0.0.9/django_paddle.egg-info/requires.txt
+-rw-rw-r--   0 k         (1000) k         (1000)       14 2021-11-28 15:56:57.000000 django-paddle-0.0.9/django_paddle.egg-info/top_level.txt
+-rw-rw-r--   0 k         (1000) k         (1000)       38 2021-11-28 15:56:57.646519 django-paddle-0.0.9/setup.cfg
+-rw-rw-r--   0 k         (1000) k         (1000)      517 2021-11-28 15:56:37.000000 django-paddle-0.0.9/setup.py
```

### Comparing `django-paddle-0.0.8/django_paddle/admin.py` & `django-paddle-0.0.9/django_paddle/admin.py`

 * *Files identical despite different names*

### Comparing `django-paddle-0.0.8/django_paddle/client.py` & `django-paddle-0.0.9/django_paddle/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,22 +30,30 @@
             url=self.base_url + 'subscription/plans',
             json=payload
         )
         return rsp.json()['response'][0]
 
     # Subscriptions
 
-    def subscriptions_list(self, include_deleted=None):
+    def subscriptions_list(self, state=None):
+
+        """
+        :param state:   filter by state, returns all active, past_due, trialing
+                        and paused subscription plans if not specified.
+                        Will NOT return deleted subscriptions
+                See https://developer.paddle.com/api-reference/subscription-api/users/listusers
+        """
 
         subscriptions = []
         max_results = 200
         payload = copy(self.base_payload)
         payload.update(page=1, results_per_page=max_results)
-        if include_deleted:
-            payload.update(state='deleted')
+
+        if state:
+            payload.update(state=state)
 
         while True:
             data = requests.post(
                 url=self.base_url + 'subscription/users',
                 json=payload
             ).json()['response']
             subscriptions += data
```

### Comparing `django-paddle-0.0.8/django_paddle/migrations/0001_initial.py` & `django-paddle-0.0.9/django_paddle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-paddle-0.0.8/django_paddle/models.py` & `django-paddle-0.0.9/django_paddle/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 
 from django.db import models
-from django.utils.timezone import make_aware
+from django.utils import timezone
 from django_paddle.client import PaddleClient
 from django_paddle.utils import get_account_model, get_account_by_passthrough
 
 
 pc = PaddleClient()
 
 
@@ -74,14 +74,18 @@
 class PaddleRecurringPrice(PaddlePrice):
 
     class Meta:
         default_related_name = 'recurring_prices'
 
 
 class PaddleSubscription(models.Model):
+
+    # TODO: use enum types for state field instead of plain varchar strings
+    # https://docs.djangoproject.com/en/3.0/ref/models/fields/#enumeration-types
+
     id = models.PositiveIntegerField(
         primary_key=True,
         unique=True
     )
     account = models.ForeignKey(
         to=get_account_model(),
         null=True,
@@ -97,14 +101,29 @@
     user_id = models.PositiveIntegerField()
     user_email = models.EmailField()
     marketing_consent = models.BooleanField()
     update_url = models.CharField(max_length=255)
     cancel_url = models.CharField(max_length=255)
     state = models.CharField(max_length=255)
     signup_date = models.DateTimeField()
+    cancellation_effective_date = models.DateTimeField(null=True, default=None)
+
+    @property
+    def is_active(self):
+        if self.state == 'active':
+            return True
+
+        if timezone.now() < self.cancellation_effective_date:
+            return True
+
+        return False
+
+    @property
+    def is_canceled(self):
+        return bool(self.cancellation_effective_date)
 
     def cancel(self):
         pc.subscriptions_cancel(self.id)
         self.state = 'deleted'
         self.save()
 
     def pause(self):
@@ -118,29 +137,29 @@
         self.save()
 
     def sync_payments(self):
         for payment in pc.payments_list(subscription_id=self.id):
             defaults = {
                 'amount': payment['amount'],
                 'currency': payment['currency'],
-                'payout_date': make_aware(datetime.strptime(payment['payout_date'], '%Y-%m-%d')),
+                'payout_date': timezone.make_aware(datetime.strptime(payment['payout_date'], '%Y-%m-%d')),
                 'is_paid': payment['is_paid'],
                 'is_one_off_charge': payment['is_one_off_charge'],
             }
             if 'receipt_url' in payment:
                 defaults['receipt_url'] = payment['receipt_url']
             PaddlePayment.objects.update_or_create(
                 id=payment['id'],
-                subscription=self,
+                subscription_id=PaddleSubscription.objects.get(self.id),
                 defaults=defaults
             )
 
     @staticmethod
-    def sync():
-        for sub in pc.subscriptions_list():
+    def sync(state=None):
+        for sub in pc.subscriptions_list(state=state):
             transaction = pc.transactions_list(entity='subscription', id=sub['subscription_id'])[0]
             account = get_account_by_passthrough(transaction['passthrough'])
 
             try:
                 plan = PaddlePlan.objects.get(id=sub['plan_id'])
             except PaddlePlan.DoesNotExist:
                 plan = None
@@ -148,15 +167,15 @@
             defaults = {
                     'user_id': sub['user_id'],
                     'user_email': sub['user_email'],
                     'marketing_consent': sub['marketing_consent'],
                     'update_url': sub['update_url'],
                     'cancel_url': sub['cancel_url'],
                     'state': sub['state'],
-                    'signup_date': make_aware(datetime.strptime(sub['signup_date'], '%Y-%m-%d %H:%M:%S'))
+                    'signup_date': timezone.make_aware(datetime.strptime(sub['signup_date'], '%Y-%m-%d %H:%M:%S'))
             }
 
             if plan:
                 defaults['plan'] = plan
 
             if account:
                 defaults['account'] = account
@@ -180,8 +199,7 @@
     amount = models.PositiveIntegerField()
     currency = models.CharField(max_length=255)
     payout_date = models.DateField(max_length=255)
     is_paid = models.BooleanField()
     is_one_off_charge = models.BooleanField()
     receipt_url = models.CharField(max_length=255, null=True)
 
-
```

### Comparing `django-paddle-0.0.8/django_paddle/signals.py` & `django-paddle-0.0.9/django_paddle/signals.py`

 * *Files identical despite different names*

### Comparing `django-paddle-0.0.8/django_paddle/utils.py` & `django-paddle-0.0.9/django_paddle/utils.py`

 * *Files identical despite different names*

### Comparing `django-paddle-0.0.8/django_paddle/views.py` & `django-paddle-0.0.9/django_paddle/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,13 +12,18 @@
 @csrf_exempt
 @require_POST
 def webhook(request):
     payload = request.POST.dict()
 
     if webhook_signature_is_valid(payload):
         alert_name = payload['alert_name']
-        getattr(signals, alert_name).send(
-            sender=Webhook,
-            payload=payload
-        )
+        signal = getattr(signals, alert_name)
+        if signal:
+            signal.send(
+                sender=Webhook,
+                payload=payload
+            )
+        else:
+            # Log warning if alert_name does not match any signal?
+            pass
 
     return HttpResponse()
```

### Comparing `django-paddle-0.0.8/django_paddle.egg-info/SOURCES.txt` & `django-paddle-0.0.9/django_paddle.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 django_paddle.egg-info/top_level.txt
 django_paddle/management/__init__.py
 django_paddle/management/commands/__init__.py
 django_paddle/management/commands/paddle_sync_payments.py
 django_paddle/management/commands/paddle_sync_plans.py
 django_paddle/management/commands/paddle_sync_subscriptions.py
 django_paddle/migrations/0001_initial.py
+django_paddle/migrations/0002_paddlesubscription_cancellation_effective_date.py
 django_paddle/migrations/__init__.py
```

### Comparing `django-paddle-0.0.8/setup.py` & `django-paddle-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='django-paddle',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     description='Django models for integrating Paddle.com subscriptions',
     url='https://github.com/kennell/django-paddle',
     author='Kevin Kennell',
     author_email='kevin@kennell.de',
     install_requires=[
         'django',
```

