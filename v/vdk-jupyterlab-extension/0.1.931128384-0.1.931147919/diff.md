# Comparing `tmp/vdk_jupyterlab_extension-0.1.931128384.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.931147919.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.931128384.tar` & `vdk_jupyterlab_extension-0.1.931147919.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/install.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/jest.config.js
--rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/package-lock.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/tsconfig.json
--rw-r--r--   0        0        0   421787 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/schema/plugin.json
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/handler.ts
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/index.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/jobData.ts
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/vdkTags.ts
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/delete-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/DeleteJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/800.4263948a6ec2f7571262.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/remoteEntry.46042e96ac50df945c8f.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/LICENSE
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/pyproject.toml
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/install.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/jest.config.js
+-rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/package-lock.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/tsconfig.json
+-rw-r--r--   0        0        0   421787 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/schema/plugin.json
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/handler.ts
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/index.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/jobData.ts
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/vdkTags.ts
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/delete-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/DeleteJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/remoteEntry.b6f98de260318ecd5e13.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.931147919/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/jest.config.js` & `vdk_jupyterlab_extension-0.1.931147919/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/package-lock.json` & `vdk_jupyterlab_extension-0.1.931147919/package-lock.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/package.json` & `vdk_jupyterlab_extension-0.1.931147919/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.931147919'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.931128384"
+    "version": "0.1.931147919"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/tsconfig.json` & `vdk_jupyterlab_extension-0.1.931147919/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/yarn.lock` & `vdk_jupyterlab_extension-0.1.931147919/yarn.lock`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.931147919/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/handler.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/index.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/delete-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/delete-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/DeleteJob.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/DeleteJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.931147919/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.931147919/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/style/base.css` & `vdk_jupyterlab_extension-0.1.931147919/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.931147919/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.931147919/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.931147919/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.931147919/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.931147919/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b6f98de260318ecd5e13.js'}}",*

 * * "'version'": "'0.1.931147919'"}*

```diff
@@ -77,15 +77,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.46042e96ac50df945c8f.js",
+            "load": "static/remoteEntry.b6f98de260318ecd5e13.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -150,9 +150,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.931128384"
+    "version": "0.1.931147919"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.931147919'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.931128384"
+    "version": "0.1.931147919"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/800.4263948a6ec2f7571262.js` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -58,15 +58,15 @@
                         className: "jp-vdk-input",
                         placeholder: d(this.props.value),
                         onChange: this.onInputChange
                     })))
                 }
             }
             var h = a(142),
-                g = a(165);
+                g = a(820);
             async function b(e = "", t = {}) {
                 const a = g.ServerConnection.makeSettings(),
                     n = h.URLExt.join(a.baseUrl, "vdk-jupyterlab-extension", e);
                 let o;
                 try {
                     o = await g.ServerConnection.makeRequest(n, t, a)
                 } catch (e) {
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/remoteEntry.46042e96ac50df945c8f.js` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/remoteEntry.b6f98de260318ecd5e13.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -44,18 +44,18 @@
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
         747: "e678254df7945f8ed34d",
-        800: "4263948a6ec2f7571262"
+        800: "8ed62c07893a05a3a69b"
     } [e] + ".js?v=" + {
         747: "e678254df7945f8ed34d",
-        800: "4263948a6ec2f7571262"
+        800: "8ed62c07893a05a3a69b"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => y.e(800).then((() => () => y(800))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.931128384"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.931147919"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -212,20 +212,20 @@
         var a = y.I(r);
         return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        165: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         271: () => p("default", "react", [1, 17, 0, 1]),
         280: () => p("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        820: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         986: () => p("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
     }, v = {
-        800: [33, 38, 123, 142, 165, 271, 280, 986]
+        800: [33, 38, 123, 142, 271, 280, 820, 986]
     }, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
                     }
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/.gitignore` & `vdk_jupyterlab_extension-0.1.931147919/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/README.md` & `vdk_jupyterlab_extension-0.1.931147919/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,20 @@
 If the server extension is installed and enabled, but you are not seeing
 the frontend extension, check the frontend extension is installed:
 
 ```bash
 jupyter labextension list
 ```
 
+If you are struggling with a particular aspect of the JupyterLab API,
+you can contact the Jupyter team in the following way: go to their repo
+(https://github.com/jupyterlab/jupyterlab), go to Issues, go to New issue,
+then click on Open in the "Chat with the devs" section, which will send you
+to a Gitter channel where you can ask your question.
+
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
```

### Comparing `vdk_jupyterlab_extension-0.1.931128384/pyproject.toml` & `vdk_jupyterlab_extension-0.1.931147919/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931128384/PKG-INFO` & `vdk_jupyterlab_extension-0.1.931147919/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.931128384
+Version: 0.1.931147919
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
@@ -79,14 +79,20 @@
 If the server extension is installed and enabled, but you are not seeing
 the frontend extension, check the frontend extension is installed:
 
 ```bash
 jupyter labextension list
 ```
 
+If you are struggling with a particular aspect of the JupyterLab API,
+you can contact the Jupyter team in the following way: go to their repo
+(https://github.com/jupyterlab/jupyterlab), go to Issues, go to New issue,
+then click on Open in the "Chat with the devs" section, which will send you
+to a Gitter channel where you can ask your question.
+
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
```

