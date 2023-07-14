# Comparing `tmp/plone.app.discussion-4.0.1.tar.gz` & `tmp/plone.app.discussion-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.discussion-4.0.1.tar", last modified: Thu Apr 13 23:08:24 2023, max compression
+gzip compressed data, was "plone.app.discussion-4.0.2.tar", last modified: Fri Jul 14 10:06:50 2023, max compression
```

## Comparing `plone.app.discussion-4.0.1.tar` & `plone.app.discussion-4.0.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.104374 plone.app.discussion-4.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    44676 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    47374 2023-04-13 23:08:24.104516 plone.app.discussion-4.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1736 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.074598 plone.app.discussion-4.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      726 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.076502 plone.app.discussion-4.0.1/docs/source/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.077516 plone.app.discussion-4.0.1/docs/source/api/
--rw-r--r--   0 maurits    (501) staff       (20)       54 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/api/comment.txt
--rw-r--r--   0 maurits    (501) staff       (20)       59 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/api/conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)      599 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/api/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/architecture.txt
--rw-r--r--   0 maurits    (501) staff       (20)       59 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/captcha.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6706 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       50 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/design.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2148 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/email-notification.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.080272 plone.app.discussion-4.0.1/docs/source/howtos/
--rw-r--r--   0 maurits    (501) staff       (20)     5493 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_extend_the_comment_form.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1242 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5116 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_override_comments_viewlet.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2526 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_override_enable_conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5038 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt
--rw-r--r--   0 maurits    (501) staff       (20)      301 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_write_a_custom_email_notification.txt
--rw-r--r--   0 maurits    (501) staff       (20)      330 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)      629 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3670 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/workflow.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.080580 plone.app.discussion-4.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.082947 plone.app.discussion-4.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.089297 plone.app.discussion-4.0.1/plone/app/discussion/
--rw-r--r--   0 maurits    (501) staff       (20)     3064 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2563 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/architecture.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.093698 plone.app.discussion-4.0.1/plone/app/discussion/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2592 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.py
--rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1216 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4035 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/comment.py
--rw-r--r--   0 maurits    (501) staff       (20)    12326 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21248 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.py
--rw-r--r--   0 maurits    (501) staff       (20)     4789 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      892 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9705 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2407 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)    15336 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15100 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1420 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     2025 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/validator.py
--rw-r--r--   0 maurits    (501) staff       (20)     3786 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    15442 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/comment.py
--rw-r--r--   0 maurits    (501) staff       (20)      394 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/comment.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4253 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2310 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/contentrules.py
--rw-r--r--   0 maurits    (501) staff       (20)     3554 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/contentrules.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    13839 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6886 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/design.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2452 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/events.py
--rw-r--r--   0 maurits    (501) staff       (20)    13956 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      501 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/notifications.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      651 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.070852 plone.app.discussion-4.0.1/plone/app/discussion/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.096599 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      170 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      504 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      621 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      247 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1104 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/portal_atct.xml
--rw-r--r--   0 maurits    (501) staff       (20)      261 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1189 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.096833 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1182 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      205 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.071342 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.097075 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     3068 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.097350 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     7060 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)      421 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows.xml
--rw-r--r--   0 maurits    (501) staff       (20)      255 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/subscribers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4037 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.103505 plone.app.discussion-4.0.1/plone/app/discussion/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3965 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/collection-integration-test.txt
--rw-r--r--   0 maurits    (501) staff       (20)     8931 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comment_review_workflow.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17844 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comments.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.104058 plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     2490 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_discussion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2580 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_moderation.robot
--rw-r--r--   0 maurits    (501) staff       (20)    20481 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    19247 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comment.py
--rw-r--r--   0 maurits    (501) staff       (20)    28444 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comments_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     5457 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_contentrules.py
--rw-r--r--   0 maurits    (501) staff       (20)     8117 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    34617 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7051 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_events.py
--rw-r--r--   0 maurits    (501) staff       (20)      985 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     8558 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     4544 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_multiple_state_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     7620 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_view.py
--rw-r--r--   0 maurits    (501) staff       (20)    12004 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_notifications.py
--rw-r--r--   0 maurits    (501) staff       (20)      879 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)    12733 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2597 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tool.py
--rw-r--r--   0 maurits    (501) staff       (20)     3909 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     3685 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.082475 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    47374 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4351 2023-04-13 23:08:24.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      535 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1965 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:08:24.104990 plone.app.discussion-4.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2256 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.724647 plone.app.discussion-4.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    44785 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    47520 2023-07-14 10:06:50.724362 plone.app.discussion-4.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1736 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.693816 plone.app.discussion-4.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.696092 plone.app.discussion-4.0.2/docs/source/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.697071 plone.app.discussion-4.0.2/docs/source/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       54 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/api/comment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/api/conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/api/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/architecture.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/captcha.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6706 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       50 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/design.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2148 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/email-notification.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.699633 plone.app.discussion-4.0.2/docs/source/howtos/
+-rw-r--r--   0 maurits    (501) staff       (20)     5493 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/howto_extend_the_comment_form.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1242 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5116 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/howto_override_comments_viewlet.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2526 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/howto_override_enable_conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5038 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/howto_write_a_custom_email_notification.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      330 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/howtos/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      629 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3670 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/docs/source/workflow.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.699931 plone.app.discussion-4.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.702454 plone.app.discussion-4.0.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.709632 plone.app.discussion-4.0.2/plone/app/discussion/
+-rw-r--r--   0 maurits    (501) staff       (20)     3064 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2563 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/architecture.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.713821 plone.app.discussion-4.0.2/plone/app/discussion/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2592 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/captcha.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/captcha.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1216 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/captcha.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4035 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11136 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/comments.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    21248 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/comments.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4789 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      892 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9705 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2407 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15354 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/moderation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    15100 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/moderation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1420 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2025 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/browser/validator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3786 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15442 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)      394 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/comment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4253 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2310 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/contentrules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3554 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/contentrules.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    13839 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6886 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/design.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2452 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13956 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/notifications.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      651 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.689874 plone.app.discussion-4.0.2/plone/app/discussion/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.716426 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      504 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      621 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      247 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1104 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/portal_atct.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      261 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1189 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.716681 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1182 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/types/Discussion_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.690436 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.716944 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     3068 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.717206 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/comment_review_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     7060 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      421 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      255 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/subscribers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4037 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.723306 plone.app.discussion-4.0.2/plone/app/discussion/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3965 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/collection-integration-test.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     8931 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/functional_test_comment_review_workflow.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17844 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/functional_test_comments.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.724010 plone.app.discussion-4.0.2/plone/app/discussion/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     2490 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/robot/test_discussion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2580 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/robot/test_moderation.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    20481 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19247 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28444 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_comments_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5457 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_contentrules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8117 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34617 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7051 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)      985 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8558 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4544 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_moderation_multiple_state_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7620 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_moderation_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12004 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_notifications.py
+-rw-r--r--   0 maurits    (501) staff       (20)      879 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12733 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tests/test_workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2597 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/tool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3909 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3685 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone/app/discussion/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:06:50.702206 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    47520 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4341 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/plone.app.discussion.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4464 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-14 10:06:50.724714 plone.app.discussion-4.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2455 2023-07-14 10:06:50.000000 plone.app.discussion-4.0.2/setup.py
```

### Comparing `plone.app.discussion-4.0.1/CHANGES.rst` & `plone.app.discussion-4.0.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-07-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.0.1 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Remove translations folder,
```

### Comparing `plone.app.discussion-4.0.1/PKG-INFO` & `plone.app.discussion-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.discussion
-Version: 4.0.1
+Version: 4.0.2
 Summary: Enhanced discussion support for Plone
 Home-page: https://pypi.org/project/plone.app.discussion
 Author: Timo Stollenwerk - Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone discussion
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Introduction
 ============
 
 
 plone.app.discussion is the commenting system used since Plone 4.1.
@@ -88,14 +89,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-07-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.0.1 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Remove translations folder,
```

### Comparing `plone.app.discussion-4.0.1/README.rst` & `plone.app.discussion-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/LICENSE.GPL` & `plone.app.discussion-4.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/LICENSE.txt` & `plone.app.discussion-4.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/api/index.txt` & `plone.app.discussion-4.0.2/docs/source/api/index.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/conf.py` & `plone.app.discussion-4.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/email-notification.txt` & `plone.app.discussion-4.0.2/docs/source/email-notification.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/howtos/howto_extend_the_comment_form.txt` & `plone.app.discussion-4.0.2/docs/source/howtos/howto_extend_the_comment_form.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt` & `plone.app.discussion-4.0.2/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/howtos/howto_override_comments_viewlet.txt` & `plone.app.discussion-4.0.2/docs/source/howtos/howto_override_comments_viewlet.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/howtos/howto_override_enable_conversation.txt` & `plone.app.discussion-4.0.2/docs/source/howtos/howto_override_enable_conversation.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt` & `plone.app.discussion-4.0.2/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/index.txt` & `plone.app.discussion-4.0.2/docs/source/index.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/docs/source/workflow.txt` & `plone.app.discussion-4.0.2/docs/source/workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/TODO.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/architecture.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/architecture.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/captcha.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/captcha.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/captcha.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/comment.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/comment.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.pt` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/comments.pt`

 * *Files 4% similar despite different names*

```diff
@@ -1,241 +1,303 @@
-<tal:block tal:define="userHasReplyPermission view/can_reply;
-                       isDiscussionAllowed view/is_discussion_allowed;
-                       isAnonymousDiscussionAllowed view/anonymous_discussion_allowed;
-                       isEditCommentAllowed view/edit_comment_allowed;
-                       isDeleteOwnCommentAllowed view/delete_own_comment_allowed;
-                       isAnon view/is_anonymous;
-                       canReview view/can_review;
-                       replies python:view.get_replies(canReview);
-                       has_replies python:view.has_replies(canReview);
-                       showCommenterImage view/show_commenter_image;
-                       errors options/state/getErrors|nothing;
-                       wtool context/@@plone_tools/workflow;
-                       auth_token context/@@authenticator/token|nothing"
-    tal:condition="python:isDiscussionAllowed or has_replies"
-    i18n:domain="plone">
-    <div class="pat-discussion">
-        <div class="reply"
-            tal:condition="python:isAnon and not isAnonymousDiscussionAllowed">
-            <form tal:attributes="action view/login_action">
-                <button class="btn btn-primary mb-3"
-                    type="submit"
-                    value="Log in to add comments"
-                    i18n:attributes="value label_login_to_add_comments;"
-                    i18n:translate="label_login_to_add_comments">Log in to add comments</button>
-            </form>
-        </div>
-
-        <div class="discussion"
-            tal:condition="has_replies">
-            <tal:getreplies repeat="reply_dict replies">
-
-                <div class="comment"
-                    tal:define="reply reply_dict/comment;
-                             comment_id reply/getId;
-                             depth reply_dict/depth|python:0;
-                             depth python: depth > 10 and '10' or depth;
-                             author_home_url python:view.get_commenter_home_url(username=reply.author_username);
-                             has_author_link python:author_home_url and not isAnon;
-                             portrait_url python:view.get_commenter_portrait(reply.author_username);
-                             review_state python:wtool.getInfoFor(reply, 'review_state', 'none');
-                             canEdit python:view.can_edit(reply);
-                             canDelete python:view.can_delete(reply);
-                             colorclass python:lambda x: 'state-private' if x=='rejected' else ('state-internal' if x=='spam' else 'state-'+x);"
-                    tal:attributes="class python:'comment level-{depth} {state}'.format(depth= depth, state=colorclass(review_state));
-                                 id comment_id"
-                    tal:condition="python:canReview or review_state == 'published'">
-
-                    <div class="d-flex flex-row align-items-center mb-3">
-
-                        <!-- commenter image -->
-                        <div class="comment-image me-3"
-                            tal:condition="showCommenterImage">
-                            <a href=""
-                                tal:condition="has_author_link"
-                                tal:attributes="href author_home_url">
-                                <img src="defaultUser.png"
-                                    alt=""
-                                    tal:attributes="src portrait_url; alt reply/author_name" />
-                            </a>
-                            <img src="defaultUser.png"
-                                alt=""
-                                tal:condition="not: has_author_link"
-                                tal:attributes="src portrait_url; alt reply/author_name" />
-                        </div>
-
-                        <!-- commenter name and date -->
-                        <div class="comment-author">
-
-                            <a href=""
-                                tal:condition="has_author_link"
-                                tal:attributes="href author_home_url">${reply/author_name}</a>
-
-                            <span tal:condition="not: has_author_link">${reply/author_name}</span>
+<tal:block tal:define="
+             userHasReplyPermission view/can_reply;
+             isDiscussionAllowed view/is_discussion_allowed;
+             isAnonymousDiscussionAllowed view/anonymous_discussion_allowed;
+             isEditCommentAllowed view/edit_comment_allowed;
+             isDeleteOwnCommentAllowed view/delete_own_comment_allowed;
+             isAnon view/is_anonymous;
+             canReview view/can_review;
+             replies python:view.get_replies(canReview);
+             has_replies python:view.has_replies(canReview);
+             showCommenterImage view/show_commenter_image;
+             errors options/state/getErrors|nothing;
+             wtool context/@@plone_tools/workflow;
+             auth_token context/@@authenticator/token|nothing;
+           "
+           tal:condition="python:isDiscussionAllowed or has_replies"
+           i18n:domain="plone"
+>
+  <div class="pat-discussion">
+    <div class="reply"
+         tal:condition="python:isAnon and not isAnonymousDiscussionAllowed"
+    >
+      <form tal:attributes="
+              action view/login_action;
+            ">
+        <button class="btn btn-primary mb-3"
+                type="submit"
+                value="Log in to add comments"
+                i18n:attributes="value label_login_to_add_comments;"
+                i18n:translate="label_login_to_add_comments"
+        >Log in to add comments</button>
+      </form>
+    </div>
 
-                            <span tal:condition="not: reply/author_name"
-                                i18n:translate="label_anonymous">Anonymous</span>
+    <div class="discussion"
+         tal:condition="has_replies"
+    >
+      <tal:getreplies repeat="reply_dict replies">
+
+        <div class="comment"
+             tal:define="
+               reply reply_dict/comment;
+               comment_id reply/getId;
+               depth reply_dict/depth|python:0;
+               depth python: depth > 10 and '10' or depth;
+               author_home_url python:view.get_commenter_home_url(username=reply.author_username);
+               has_author_link python:author_home_url and not isAnon;
+               portrait_url python:view.get_commenter_portrait(reply.author_username);
+               review_state python:wtool.getInfoFor(reply, 'review_state', 'none');
+               canEdit python:view.can_edit(reply);
+               canDelete python:view.can_delete(reply);
+               colorclass python:lambda x: 'state-private' if x=='rejected' else ('state-internal' if x=='spam' else 'state-'+x);
+             "
+             tal:condition="python:canReview or review_state == 'published'"
+             tal:attributes="
+               class python:'comment level-{depth} {state}'.format(depth= depth, state=colorclass(review_state));
+               id comment_id;
+             "
+        >
+
+          <div class="d-flex flex-row align-items-center mb-3">
+
+            <!-- commenter image -->
+            <div class="comment-image me-3"
+                 tal:condition="showCommenterImage"
+            >
+              <a href=""
+                 tal:condition="has_author_link"
+                 tal:attributes="
+                   href author_home_url;
+                 "
+              >
+                <img alt=""
+                     src="defaultUser.png"
+                     tal:attributes="
+                       src portrait_url;
+                       alt reply/author_name;
+                     "
+                />
+              </a>
+              <img alt=""
+                   src="defaultUser.png"
+                   tal:condition="not: has_author_link"
+                   tal:attributes="
+                     src portrait_url;
+                     alt reply/author_name;
+                   "
+              />
+            </div>
 
-                            <br />
+            <!-- commenter name and date -->
+            <div class="comment-author">
 
-                            <small class="text-muted"
-                                tal:content="python:view.format_time(reply.modification_date)">
+              <a href=""
+                 tal:condition="has_author_link"
+                 tal:attributes="
+                   href author_home_url;
+                 "
+              >${reply/author_name}</a>
+
+              <span tal:condition="not: has_author_link">${reply/author_name}</span>
+
+              <span tal:condition="not: reply/author_name"
+                    i18n:translate="label_anonymous"
+              >Anonymous</span>
+
+              <br />
+
+              <small class="text-muted"
+                     tal:content="python:view.format_time(reply.modification_date)"
+              >
                       8/23/2001 12:40:44 PM
-                            </small>
+              </small>
+
+            </div>
+          </div>
 
-                        </div>
-                    </div>
 
 
+          <!-- comment body -->
+          <div class="comment-body">
 
-                    <!-- comment body -->
-                    <div class="comment-body">
-
-                        <span tal:replace="structure reply/getText" />
-
-                        <!-- comment actions -->
-                        <div class="d-flex flex-row justify-content-end mb-3">
-
-                            <div class="comment-actions actions-edit"
-                                tal:condition="python:isEditCommentAllowed and canEdit">
-
-                                <!-- edit -->
-                                <a class="pat-plone-modal context comment-action action-edit btn btn-primary btn-sm"
-                                    tal:condition="auth_token"
-                                    tal:attributes="href string:${reply/absolute_url}/@@edit-comment?_authenticator=${auth_token}"
-                                    i18n:translate="Edit">Edit</a>
-
-                                <form name="edit"
-                                    action=""
-                                    method="get"
-                                    class="comment-action action-edit"
-                                    tal:condition="not: auth_token"
-                                    tal:attributes="action string:${reply/absolute_url}/@@edit-comment;
-                                                id string:edit-${comment_id}">
-
-                                    <button name="form.button.EditComment"
-                                        class="context btn btn-primary btn-sm"
-                                        type="submit"
-                                        value="Edit"
-                                        i18n:attributes="value label_edit;"
-                                        i18n:translate="label_edit">Edit</button>
-
-                                </form>
-
-                            </div>
-
-                            <div class="comment-actions actions-delete"
-                                tal:condition="python:canDelete">
-
-                                <!-- delete own comment -->
-                                <form name="delete"
-                                    action=""
-                                    method="post"
-                                    class="comment-action action-delete"
-                                    tal:condition="python:not canDelete and isDeleteOwnCommentAllowed and view.could_delete_own(reply)"
-                                    tal:attributes="action string:${reply/absolute_url}/@@delete-own-comment;
-                                                style python:view.can_delete_own(reply) and 'display: inline' or 'display: none';
-                                                id string:delete-${comment_id}">
-                                    <button name="form.button.DeleteComment"
-                                        class="destructive btn btn-danger btn-sm"
-                                        type="submit"
-                                        value="Delete"
-                                        i18n:attributes="value label_delete;"
-                                        i18n:translate="label_delete">Delete</button>
-                                </form>
-
-                                <!-- delete -->
-                                <form name="delete"
-                                    action=""
-                                    method="post"
-                                    class="comment-action action-delete"
-                                    tal:condition="python:canDelete"
-                                    tal:attributes="action string:${reply/absolute_url}/@@moderate-delete-comment;
-                                                id string:delete-${comment_id}">
-                                    <button name="form.button.DeleteComment"
-                                        class="destructive btn btn-danger btn-sm"
-                                        type="submit"
-                                        value="Delete"
-                                        i18n:attributes="value label_delete;"
-                                        i18n:translate="label_delete">Delete</button>
-                                </form>
-
-                            </div>
-
-                            <div class="comment-actions actions-workflow d-flex flex-row"
-                                tal:condition="reply_dict/actions|nothing">
-
-                                <form name=""
-                                    action=""
-                                    method="get"
-                                    class="comment-action action-${action/id}"
-                                    tal:condition="canReview"
-                                    tal:repeat="action reply_dict/actions|nothing"
-                                    tal:attributes="action string:${reply/absolute_url}/@@transmit-comment;
-                                                name action/id;
-                                                id string:${action/id}-${comment_id};
-                                                ">
-                                    <input type="hidden"
-                                        name="workflow_action"
-                                        tal:attributes="value action/id" />
-                                    <button name="form.button.TransmitComment"
-                                        class="context btn btn-primary btn-sm"
-                                        type="submit"
-                                        i18n:translate="">${action/title}</button>
-                                </form>
-
-                            </div>
-
-                        </div>
-                        <!-- end comment actions -->
-
-
-                    </div>
-                    <button class="context reply-to-comment-button hide allowMultiSubmit btn btn-primary btn-sm"
-                        tal:condition="python:isDiscussionAllowed and (isAnon and isAnonymousDiscussionAllowed or userHasReplyPermission)"
-                        i18n:translate="label_reply">
-                    Reply
-                    </button>
+            <span tal:replace="structure reply/getText"></span>
 
-                </div>
+            <!-- comment actions -->
+            <div class="d-flex flex-row justify-content-end mb-3">
+
+              <div class="comment-actions actions-edit"
+                   tal:condition="python:isEditCommentAllowed and canEdit"
+              >
+
+                <!-- edit -->
+                <a class="pat-plone-modal context comment-action action-edit btn btn-primary btn-sm"
+                   tal:condition="auth_token"
+                   tal:attributes="
+                     href string:${reply/absolute_url}/@@edit-comment?_authenticator=${auth_token};
+                   "
+                   i18n:translate="Edit"
+                >Edit</a>
+
+                <form class="comment-action action-edit"
+                      action=""
+                      method="get"
+                      name="edit"
+                      tal:condition="not: auth_token"
+                      tal:attributes="
+                        action string:${reply/absolute_url}/@@edit-comment;
+                        id string:edit-${comment_id};
+                      "
+                >
+
+                  <button class="context btn btn-primary btn-sm"
+                          name="form.button.EditComment"
+                          type="submit"
+                          value="Edit"
+                          i18n:attributes="value label_edit;"
+                          i18n:translate="label_edit"
+                  >Edit</button>
+
+                </form>
+
+              </div>
+
+              <div class="comment-actions actions-delete"
+                   tal:condition="python:canDelete"
+              >
+
+                <!-- delete own comment -->
+                <form class="comment-action action-delete"
+                      action=""
+                      method="post"
+                      name="delete"
+                      tal:condition="python:not canDelete and isDeleteOwnCommentAllowed and view.could_delete_own(reply)"
+                      tal:attributes="
+                        action string:${reply/absolute_url}/@@delete-own-comment;
+                        style python:view.can_delete_own(reply) and 'display: inline' or 'display: none';
+                        id string:delete-${comment_id};
+                      "
+                >
+                  <button class="destructive btn btn-danger btn-sm"
+                          name="form.button.DeleteComment"
+                          type="submit"
+                          value="Delete"
+                          i18n:attributes="value label_delete;"
+                          i18n:translate="label_delete"
+                  >Delete</button>
+                </form>
+
+                <!-- delete -->
+                <form class="comment-action action-delete"
+                      action=""
+                      method="post"
+                      name="delete"
+                      tal:condition="python:canDelete"
+                      tal:attributes="
+                        action string:${reply/absolute_url}/@@moderate-delete-comment;
+                        id string:delete-${comment_id};
+                      "
+                >
+                  <button class="destructive btn btn-danger btn-sm"
+                          name="form.button.DeleteComment"
+                          type="submit"
+                          value="Delete"
+                          i18n:attributes="value label_delete;"
+                          i18n:translate="label_delete"
+                  >Delete</button>
+                </form>
+
+              </div>
+
+              <div class="comment-actions actions-workflow d-flex flex-row"
+                   tal:condition="reply_dict/actions|nothing"
+              >
+
+                <form class="comment-action action-${action/id}"
+                      action=""
+                      method="get"
+                      name=""
+                      tal:condition="canReview"
+                      tal:repeat="action reply_dict/actions|nothing"
+                      tal:attributes="
+                        action string:${reply/absolute_url}/@@transmit-comment;
+                        name action/id;
+                        id string:${action/id}-${comment_id};
+                      "
+                >
+                  <input name="workflow_action"
+                         type="hidden"
+                         tal:attributes="
+                           value action/id;
+                         "
+                  />
+                  <button class="context btn btn-primary btn-sm"
+                          name="form.button.TransmitComment"
+                          type="submit"
+                          i18n:translate=""
+                  >${action/title}</button>
+                </form>
 
-            </tal:getreplies>
+              </div>
 
-            <div tal:condition="python: has_replies and not isDiscussionAllowed"
-                class="discreet"
-                i18n:translate="label_commenting_disabled">
-            Commenting has been disabled.
             </div>
+            <!-- end comment actions -->
 
-        </div>
 
-        <div class="reply"
-            tal:condition="python:has_replies and (isAnon and not isAnonymousDiscussionAllowed)">
-            <form tal:attributes="action view/login_action"
-                class="mb-3">
-                <button class="standalone loginbutton btn btn-primary"
-                    type="submit"
-                    value="Log in to add comments"
-                    i18n:attributes="value label_login_to_add_comments;"
-                    i18n:translate="label_login_to_add_comments">Log in to add comments</button>
-            </form>
+          </div>
+          <button class="context reply-to-comment-button hide allowMultiSubmit btn btn-primary btn-sm"
+                  tal:condition="python:isDiscussionAllowed and (isAnon and isAnonymousDiscussionAllowed or userHasReplyPermission)"
+                  i18n:translate="label_reply"
+          >
+                    Reply
+          </button>
+
         </div>
 
-        <div id="commenting"
-            class="reply border p-3"
-            tal:condition="python:isDiscussionAllowed and (isAnon and isAnonymousDiscussionAllowed or userHasReplyPermission)">
+      </tal:getreplies>
 
-            <fieldset>
+      <div class="discreet"
+           tal:condition="python: has_replies and not isDiscussionAllowed"
+           i18n:translate="label_commenting_disabled"
+      >
+            Commenting has been disabled.
+      </div>
 
-                <legend i18n:translate="label_add_comment">Add comment</legend>
+    </div>
+
+    <div class="reply"
+         tal:condition="python:has_replies and (isAnon and not isAnonymousDiscussionAllowed)"
+    >
+      <form class="mb-3"
+            tal:attributes="
+              action view/login_action;
+            "
+      >
+        <button class="standalone loginbutton btn btn-primary"
+                type="submit"
+                value="Log in to add comments"
+                i18n:attributes="value label_login_to_add_comments;"
+                i18n:translate="label_login_to_add_comments"
+        >Log in to add comments</button>
+      </form>
+    </div>
 
-                <p tal:content="view/comment_transform_message">
+    <div class="reply border p-3"
+         id="commenting"
+         tal:condition="python:isDiscussionAllowed and (isAnon and isAnonymousDiscussionAllowed or userHasReplyPermission)"
+    >
+
+      <fieldset>
+
+        <legend i18n:translate="label_add_comment">Add comment</legend>
+
+        <p tal:content="view/comment_transform_message">
                 You can add a comment by filling out the form below. Plain text
                 formatting.
-                </p>
+        </p>
 
-                <div tal:replace="structure view/form/render" />
+        <div tal:replace="structure view/form/render"></div>
 
-            </fieldset>
-        </div>
+      </fieldset>
     </div>
+  </div>
 </tal:block>
```

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/comments.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/configure.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.pt` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/conversation.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/conversation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.pt` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/moderation.pt`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         <h1 i18n:translate="heading_moderate_comments">
             Moderate comments
         </h1>
         <div class="alert alert-info"
              role="status"
              tal:condition="python: not moderation_enabled"
         >
-          <strong>Info</strong>
+          <strong i18n:translate="">Info</strong>
           <div i18n:translate="message_moderation_disabled">Moderation workflow is disabled. You have to
             <a href=""
                tal:attributes="
                  href string:${context/portal_url}/@@content-controlpanel?type_id=Discussion Item;
                "
                i18n:name="enable_comment_workflow"
                i18n:translate="message_enable_comment_workflow"
```

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/moderation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/traversal.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/browser/validator.py` & `plone.app.discussion-4.0.2/plone/app/discussion/browser/validator.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/catalog.py` & `plone.app.discussion-4.0.2/plone/app/discussion/catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/comment.py` & `plone.app.discussion-4.0.2/plone/app/discussion/comment.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/configure.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/contentrules.py` & `plone.app.discussion-4.0.2/plone/app/discussion/contentrules.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/contentrules.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/contentrules.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/conversation.py` & `plone.app.discussion-4.0.2/plone/app/discussion/conversation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/design.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/design.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/events.py` & `plone.app.discussion-4.0.2/plone/app/discussion/events.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/interfaces.py` & `plone.app.discussion-4.0.2/plone/app/discussion/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/permissions.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/permissions.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/actions.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/controlpanel.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/portal_atct.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/portal_atct.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/rolemap.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/types/Discussion_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml` & `plone.app.discussion-4.0.2/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/subscribers.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/testing.py` & `plone.app.discussion-4.0.2/plone/app/discussion/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/collection-integration-test.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/collection-integration-test.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comment_review_workflow.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/functional_test_comment_review_workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comments.txt` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/functional_test_comments.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_discussion.robot` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/robot/test_discussion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_moderation.robot` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/robot/test_moderation.robot`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_catalog.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comment.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comments_viewlet.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_comments_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_contentrules.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_contentrules.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_controlpanel.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_conversation.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_events.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_functional.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_indexers.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_multiple_state_view.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_moderation_multiple_state_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_view.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_moderation_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_notifications.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_robot.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_workflow.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/tool.py` & `plone.app.discussion-4.0.2/plone/app/discussion/tool.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/upgrades.py` & `plone.app.discussion-4.0.2/plone/app/discussion/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/upgrades.zcml` & `plone.app.discussion-4.0.2/plone/app/discussion/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone/app/discussion/vocabularies.py` & `plone.app.discussion-4.0.2/plone/app/discussion/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.1/plone.app.discussion.egg-info/PKG-INFO` & `plone.app.discussion-4.0.2/plone.app.discussion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.discussion
-Version: 4.0.1
+Version: 4.0.2
 Summary: Enhanced discussion support for Plone
 Home-page: https://pypi.org/project/plone.app.discussion
 Author: Timo Stollenwerk - Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone discussion
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Introduction
 ============
 
 
 plone.app.discussion is the commenting system used since Plone 4.1.
@@ -88,14 +89,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-07-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.0.1 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Remove translations folder,
```

### Comparing `plone.app.discussion-4.0.1/plone.app.discussion.egg-info/SOURCES.txt` & `plone.app.discussion-4.0.2/plone.app.discussion.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 docs/README.txt
 docs/source/architecture.txt
 docs/source/captcha.txt
 docs/source/conf.py
```

### Comparing `plone.app.discussion-4.0.1/plone.app.discussion.egg-info/requires.txt` & `plone.app.discussion-4.0.2/plone.app.discussion.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 BTrees
 Products.GenericSetup
 Products.ZCatalog
 Products.statusmessages
 persistent
 plone.api
 plone.app.event
-plone.dexterity
 plone.registry
 plone.resource
 plone.uuid
 zope.annotation
 setuptools
 plone.app.layout
 plone.app.registry
@@ -27,8 +26,9 @@
 plone.app.contenttypes[test]
 plone.app.robotframework
 plone.app.vocabularies
 plone.testing
 plone.protect
 Products.MailHost
 robotsuite
+plone.dexterity
 python-dateutil
```

### Comparing `plone.app.discussion-4.0.1/setup.py` & `plone.app.discussion-4.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.1"
+version = "4.0.2"
+
+long_description = (
+    f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
+)
 
 install_requires = [
     "BTrees",
     "Products.GenericSetup",
     "Products.ZCatalog",
     "Products.statusmessages",
     "persistent",
     "plone.api",
     "plone.app.event",
-    "plone.dexterity",
     "plone.registry",
     "plone.resource",
     "plone.uuid",
     "zope.annotation",
     "setuptools",
     "plone.app.layout",
     "plone.app.registry",
@@ -27,15 +31,18 @@
     "z3c.form>=2.3.3",
 ]
 
 setup(
     name="plone.app.discussion",
     version=version,
     description="Enhanced discussion support for Plone",
-    long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
@@ -67,11 +74,12 @@
             "plone.app.contenttypes[test]",
             "plone.app.robotframework",
             "plone.app.vocabularies",
             "plone.testing",
             "plone.protect",
             "Products.MailHost",
             "robotsuite",
+            "plone.dexterity",
             "python-dateutil",
         ],
     },
 )
```

