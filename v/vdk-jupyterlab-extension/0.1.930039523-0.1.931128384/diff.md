# Comparing `tmp/vdk_jupyterlab_extension-0.1.930039523.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.931128384.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.930039523.tar` & `vdk_jupyterlab_extension-0.1.931128384.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/install.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/jest.config.js
--rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/package-lock.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/tsconfig.json
--rw-r--r--   0        0        0   421787 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/schema/plugin.json
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/handler.ts
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/index.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/jobData.ts
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/vdkTags.ts
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/delete-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/DeleteJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/remoteEntry.29e2672ca61716c7c15c.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/LICENSE
--rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/pyproject.toml
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.930039523/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/install.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/jest.config.js
+-rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/package-lock.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/tsconfig.json
+-rw-r--r--   0        0        0   421787 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/schema/plugin.json
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/handler.ts
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/index.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/jobData.ts
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/vdkTags.ts
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/delete-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/DeleteJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/800.4263948a6ec2f7571262.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/remoteEntry.46042e96ac50df945c8f.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/LICENSE
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/pyproject.toml
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931128384/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.931128384/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/jest.config.js` & `vdk_jupyterlab_extension-0.1.931128384/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/package-lock.json` & `vdk_jupyterlab_extension-0.1.931128384/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998313000709117%*

 * *Differences: {"'dependencies'": "{'@babel/helper-compilation-targets': {'dependencies': {'semver': {'version': "*

 * *                   "'6.3.1', 'resolved': 'https://registry.npmjs.org/semver/-/semver-6.3.1.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA=='}}}, "*

 * *                   "'@babel/helper-create-regexp-features-plugin': {'dependencies': {'semver': "*

 * *                   "{'version': '6.3.1', 'resolved': "*

 * *   […]*

```diff
@@ -72,17 +72,17 @@
             },
             "resolved": "https://registry.npmjs.org/@babel/helper-builder-binary-assignment-operator-visitor/-/helper-builder-binary-assignment-operator-visitor-7.22.3.tgz",
             "version": "7.22.3"
         },
         "@babel/helper-compilation-targets": {
             "dependencies": {
                 "semver": {
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "integrity": "sha512-Ji+ywpHeuqxB8WDxraCiqR0xfhYjiDE/e6k7FuIaANnoOFxAHskHChz4vA1mJC9Lbm01s1PVAGhQY4FUKSkGZw==",
             "requires": {
                 "@babel/compat-data": "^7.22.5",
                 "@babel/helper-validator-option": "^7.22.5",
                 "browserslist": "^4.21.3",
@@ -92,17 +92,17 @@
             "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.5.tgz",
             "version": "7.22.5"
         },
         "@babel/helper-create-regexp-features-plugin": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-1VpEFOIbMRaXyDeUwUfmTIxExLwQ+zkW+Bh5zXpApA3oQedBx9v/updixWxnx/bZpKw7u8VxWjb/qWpIcmPq8A==",
             "requires": {
                 "@babel/helper-annotate-as-pure": "^7.22.5",
                 "regexpu-core": "^5.3.1",
@@ -3082,20 +3082,20 @@
                     },
                     "resolved": "https://registry.npmjs.org/jest-serializer/-/jest-serializer-26.6.2.tgz",
                     "version": "26.6.2"
                 },
                 "jest-snapshot": {
                     "dependencies": {
                         "semver": {
-                            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                             "requires": {
                                 "lru-cache": "^6.0.0"
                             },
-                            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                            "version": "7.5.3"
+                            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                            "version": "7.5.4"
                         }
                     },
                     "integrity": "sha512-OLhxz05EzUtsAmOMzuupt1lHYXCNib0ECyuZ/PZOx9TrZcC8vL0x+DUG3TL+GLX3yHG45e6YGjIm0XwDc3q3og==",
                     "requires": {
                         "@babel/types": "^7.0.0",
                         "@jest/types": "^26.6.2",
                         "@types/babel__traverse": "^7.0.4",
@@ -3187,37 +3187,37 @@
                 },
                 "react-is": {
                     "integrity": "sha512-w2GsyukL62IJnlaff/nRegPQR94C/XXamvMWmSHRJ4y7Ts/4ocGRmTHvOs8PSE6pB3dWOrD/nueuU5sduBsQ4w==",
                     "resolved": "https://registry.npmjs.org/react-is/-/react-is-17.0.2.tgz",
                     "version": "17.0.2"
                 },
                 "semver": {
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 },
                 "source-map": {
                     "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
                     "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
                     "version": "0.6.1"
                 },
                 "throat": {
                     "integrity": "sha512-fcwX4mndzpLQKBS1DVYhGAcYaYt7vsHNIvQV+WXMvnow5cgjPphq5CaayLaGsjRdSCKZFNGt7/GYAuXaNOiYCA==",
                     "resolved": "https://registry.npmjs.org/throat/-/throat-5.0.0.tgz",
                     "version": "5.0.0"
                 },
                 "ts-jest": {
                     "dependencies": {
                         "semver": {
-                            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                             "requires": {
                                 "lru-cache": "^6.0.0"
                             },
-                            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                            "version": "7.5.3"
+                            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                            "version": "7.5.4"
                         }
                     },
                     "integrity": "sha512-rua+rCP8DxpA8b4DQD/6X2HQS8Zy/xzViVYfEs2OQu68tkCuKLV0Md8pmX55+W24uRIyAsf/BajRfxOs+R2MKA==",
                     "requires": {
                         "bs-logger": "0.x",
                         "buffer-from": "1.x",
                         "fast-json-stable-stringify": "2.x",
@@ -3603,20 +3603,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -3985,20 +3985,20 @@
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "yallist": {
                     "dev": true,
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
@@ -4068,20 +4068,20 @@
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "yallist": {
                     "dev": true,
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
@@ -5147,20 +5147,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -5746,20 +5746,20 @@
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "type-fest": {
                     "dev": true,
                     "integrity": "sha512-4dbzIzqvjtgiM5rw1k5rEHtBANKmdudhGyBEajN01fEyhaAIhsoKNy6y7+IN93IfpFtwY9iqi7kD+xwKhQsNJA==",
                     "resolved": "https://registry.npmjs.org/type-fest/-/type-fest-0.8.1.tgz",
                     "version": "0.8.1"
                 },
@@ -7269,17 +7269,17 @@
                         "json5": "^2.2.2",
                         "semver": "^6.3.0"
                     },
                     "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.22.5.tgz",
                     "version": "7.22.5"
                 },
                 "semver": {
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "integrity": "sha512-pzqtp31nLv/XFOzXGuvhCb8qhjmTVo5vjVk19XE4CRlSWz0KoeJ3bw9XsA7nOp9YBf4qHjwBxkDzKcME/J29Yg==",
             "requires": {
                 "@babel/core": "^7.12.3",
                 "@babel/parser": "^7.14.7",
                 "@istanbuljs/schema": "^0.1.2",
@@ -8175,20 +8175,20 @@
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "yallist": {
                     "dev": true,
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
@@ -8803,17 +8803,17 @@
             "integrity": "sha512-h5bgJWpxJNswbU7qCrV0tIKQCaS3blPDrqKWx+QxzuzL1zGUzij9XCWLrSLsJPu5t+eWA/ycetzYAO5IOMcWAQ==",
             "resolved": "https://registry.npmjs.org/lz-string/-/lz-string-1.5.0.tgz",
             "version": "1.5.0"
         },
         "make-dir": {
             "dependencies": {
                 "semver": {
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "integrity": "sha512-g3FeP20LNwhALb/6Cz6Dd4F2ngze0jz7tbzrD2wAV+o9FeNHe4rL+yK2md0J/fiSf1sa1ADhXqi5+oVwOM/eGw==",
             "requires": {
                 "semver": "^6.0.0"
             },
             "resolved": "https://registry.npmjs.org/make-dir/-/make-dir-3.1.0.tgz",
@@ -8941,20 +8941,20 @@
                         "validate-npm-package-license": "^3.0.1"
                     },
                     "resolved": "https://registry.npmjs.org/normalize-package-data/-/normalize-package-data-3.0.3.tgz",
                     "version": "3.0.3"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "type-fest": {
                     "dev": true,
                     "integrity": "sha512-OIAYXk8+ISY+qTOwkHtKqzAuxchoMiD9Udx+FSGQDuiRR+PJKJHc2NJAXlbhkGwTt/4/nKZxELY1w3ReWOL8mw==",
                     "resolved": "https://registry.npmjs.org/type-fest/-/type-fest-0.18.1.tgz",
                     "version": "0.18.1"
                 },
@@ -9241,21 +9241,21 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "optional": true,
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "uuid": {
                     "integrity": "sha512-+NYs2QeMWy+GWFOEm9xnn6HCDp0l7QBD7ml8zLUmJ+93Q5NF0NocErnwkTkXVFNiX3/fpC6afS8Dhb/gz7R7eg==",
                     "optional": true,
                     "resolved": "https://registry.npmjs.org/uuid/-/uuid-8.3.2.tgz",
                     "version": "8.3.2"
                 },
@@ -10565,17 +10565,17 @@
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
             "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.3.0.tgz",
             "version": "3.3.0"
         },
         "semver": {
-            "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz",
-            "version": "5.7.1"
+            "integrity": "sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.2.tgz",
+            "version": "5.7.2"
         },
         "serialize-javascript": {
             "integrity": "sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==",
             "requires": {
                 "randombytes": "^2.1.0"
             },
             "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-5.0.1.tgz",
@@ -11744,20 +11744,20 @@
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+                    "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-                    "version": "7.5.3"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+                    "version": "7.5.4"
                 },
                 "yallist": {
                     "dev": true,
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
@@ -12787,17 +12787,17 @@
             "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.5.tgz",
             "version": "7.22.5"
         },
         "node_modules/@babel/helper-compilation-targets/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/helper-create-regexp-features-plugin": {
             "dependencies": {
                 "@babel/helper-annotate-as-pure": "^7.22.5",
                 "regexpu-core": "^5.3.1",
                 "semver": "^6.3.0"
             },
@@ -12813,17 +12813,17 @@
             "version": "7.22.5"
         },
         "node_modules/@babel/helper-create-regexp-features-plugin/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/helper-environment-visitor": {
             "engines": {
                 "node": ">=6.9.0"
             },
             "integrity": "sha512-XGmhECfVA/5sAt+H+xpSg0mfrHq6FzNr9Oxh7PSEBBRUb/mL7Kz3NICXb194rCqAEdxkhPT1a88teizAFyvk8Q==",
             "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.22.5.tgz",
@@ -16530,17 +16530,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/@jupyterlab/testutils/node_modules/jest-util": {
             "dependencies": {
                 "@jest/types": "^26.6.2",
                 "@types/node": "*",
                 "chalk": "^4.0.0",
                 "graceful-fs": "^4.2.4",
@@ -16630,17 +16630,17 @@
             "resolved": "https://registry.npmjs.org/react-is/-/react-is-17.0.2.tgz",
             "version": "17.0.2"
         },
         "node_modules/@jupyterlab/testutils/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@jupyterlab/testutils/node_modules/source-map": {
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
             "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
@@ -16684,17 +16684,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/@jupyterlab/testutils/node_modules/v8-to-istanbul": {
             "dependencies": {
                 "@types/istanbul-lib-coverage": "^2.0.1",
                 "convert-source-map": "^1.6.0",
                 "source-map": "^0.7.3"
             },
@@ -17070,17 +17070,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/@npmcli/fs/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/@npmcli/move-file": {
@@ -17522,17 +17522,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/@typescript-eslint/eslint-plugin/node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
@@ -17664,17 +17664,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/@typescript-eslint/typescript-estree/node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
@@ -19089,17 +19089,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/css-loader/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/cssesc": {
@@ -19994,17 +19994,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/eslint/node_modules/type-fest": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-4dbzIzqvjtgiM5rw1k5rEHtBANKmdudhGyBEajN01fEyhaAIhsoKNy6y7+IN93IfpFtwY9iqi7kD+xwKhQsNJA==",
@@ -21956,17 +21956,17 @@
             "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.22.5.tgz",
             "version": "7.22.5"
         },
         "node_modules/istanbul-lib-instrument/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/istanbul-lib-report": {
             "dependencies": {
                 "istanbul-lib-coverage": "^3.0.0",
                 "make-dir": "^3.0.0",
                 "supports-color": "^7.1.0"
             },
@@ -23185,17 +23185,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/jest-snapshot/node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
@@ -23976,17 +23976,17 @@
             "resolved": "https://registry.npmjs.org/make-dir/-/make-dir-3.1.0.tgz",
             "version": "3.1.0"
         },
         "node_modules/make-dir/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/make-error": {
             "integrity": "sha512-s8UhlNe7vPKomQhC1qFelMokr/Sc3AgNbso3n74mVPA5LTZwkB9NlXf4XPamLxJE8h0gh73rM94xvwRT2CVInw==",
             "resolved": "https://registry.npmjs.org/make-error/-/make-error-1.3.6.tgz",
             "version": "1.3.6"
         },
         "node_modules/makeerror": {
@@ -24183,17 +24183,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/meow/node_modules/type-fest": {
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "funding": {
@@ -24579,18 +24579,18 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/node-notifier/node_modules/uuid": {
             "bin": {
                 "uuid": "dist/bin/uuid"
             },
             "integrity": "sha512-+NYs2QeMWy+GWFOEm9xnn6HCDp0l7QBD7ml8zLUmJ+93Q5NF0NocErnwkTkXVFNiX3/fpC6afS8Dhb/gz7R7eg==",
             "optional": true,
@@ -26388,17 +26388,17 @@
             "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.3.0.tgz",
             "version": "3.3.0"
         },
         "node_modules/semver": {
             "bin": {
                 "semver": "bin/semver"
             },
-            "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz",
-            "version": "5.7.1"
+            "integrity": "sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.2.tgz",
+            "version": "5.7.2"
         },
         "node_modules/serialize-javascript": {
             "dependencies": {
                 "randombytes": "^2.1.0"
             },
             "integrity": "sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==",
             "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-5.0.1.tgz",
@@ -27973,17 +27973,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/ts-jest/node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/package.json` & `vdk_jupyterlab_extension-0.1.931128384/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.931128384'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.930039523"
+    "version": "0.1.931128384"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/tsconfig.json` & `vdk_jupyterlab_extension-0.1.931128384/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/yarn.lock` & `vdk_jupyterlab_extension-0.1.931128384/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3877,17 +3877,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.459"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.459.tgz#25a23370f4ae8aaa8f77aaf00133aa4994f4148e"
-  integrity sha512-XXRS5NFv8nCrBL74Rm3qhJjA2VCsRFx0OjHKBMPI0otij56aun8UWiKTDABmd5/7GTR021pA4wivs+Ri6XCElg==
+  version "1.4.460"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.460.tgz#f360a5059c039c4a5fb4dfa99680ad8129dd9f84"
+  integrity sha512-kKiHnbrHME7z8E6AYaw0ehyxY5+hdaRmeUbjBO22LZMdqTYCO29EvF0T1cQ3pJ1RN5fyMcHl1Lmcsdt9WWJpJQ==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -7352,17 +7352,17 @@
 
 postcss-value-parser@^4.1.0, postcss-value-parser@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11, postcss@^8.4.5:
-  version "8.4.25"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.25.tgz#4a133f5e379eda7f61e906c3b1aaa9b81292726f"
-  integrity sha512-7taJ/8t2av0Z+sQEvNzCkpDynl0tX3uJMCODi6nT3PfASC7dYCWV9aQ+uiCf+KBD4SEFcu+GvJdGdwzQ6OSjCw==
+  version "8.4.26"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.26.tgz#1bc62ab19f8e1e5463d98cf74af39702a00a9e94"
+  integrity sha512-jrXHFF8iTloAenySjM/ob3gSj7pCu0Ji49hnjqzsgSRa50hkWCKD0HQ+gMNJkW38jBI68MpAAg7ZWwHwX8NMMw==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.931128384/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/handler.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/index.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/delete-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/delete-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/DeleteJob.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/DeleteJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.931128384/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.931128384/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/style/base.css` & `vdk_jupyterlab_extension-0.1.931128384/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.931128384/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.931128384/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.931128384/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.931128384/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.931128384/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.46042e96ac50df945c8f.js'}}",*

 * * "'version'": "'0.1.931128384'"}*

```diff
@@ -77,15 +77,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.29e2672ca61716c7c15c.js",
+            "load": "static/remoteEntry.46042e96ac50df945c8f.js",
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
-    "version": "0.1.930039523"
+    "version": "0.1.931128384"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.931128384'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.930039523"
+    "version": "0.1.931128384"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/800.4263948a6ec2f7571262.js`

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
-                g = a(820);
+                g = a(165);
             async function b(e = "", t = {}) {
                 const a = g.ServerConnection.makeSettings(),
                     n = h.URLExt.join(a.baseUrl, "vdk-jupyterlab-extension", e);
                 let o;
                 try {
                     o = await g.ServerConnection.makeRequest(n, t, a)
                 } catch (e) {
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/remoteEntry.29e2672ca61716c7c15c.js` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/remoteEntry.46042e96ac50df945c8f.js`

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
-        800: "8ed62c07893a05a3a69b"
+        800: "4263948a6ec2f7571262"
     } [e] + ".js?v=" + {
         747: "e678254df7945f8ed34d",
-        800: "8ed62c07893a05a3a69b"
+        800: "4263948a6ec2f7571262"
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
-                })("vdk-jupyterlab-extension", "0.1.930039523"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.931128384"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
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
+        165: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         271: () => p("default", "react", [1, 17, 0, 1]),
         280: () => p("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
-        820: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         986: () => p("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
     }, v = {
-        800: [33, 38, 123, 142, 271, 280, 820, 986]
+        800: [33, 38, 123, 142, 165, 271, 280, 986]
     }, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
                     }
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.931128384/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/.gitignore` & `vdk_jupyterlab_extension-0.1.931128384/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/README.md` & `vdk_jupyterlab_extension-0.1.931128384/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,21 @@
 ## Requirements
 
 - JupyterLab >= 3.0
 - python ~=3.7
 - Versatile Data Kit
 - npm
 
-## Install
-
-To install the extension,first navigate to the project directory and then execute:
+## Install and run
 
 ```bash
-# Once in the project directory, use the npm ci command to install
-# the exact versions of the dependencies specified in the package-lock.json
-npm ci
-# Install the extension
+# install the extension
 pip install vdk-jupyterlab-extension
+# run jupyterlab
+jupyter lab
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
```

### Comparing `vdk_jupyterlab_extension-0.1.930039523/pyproject.toml` & `vdk_jupyterlab_extension-0.1.931128384/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.930039523/PKG-INFO` & `vdk_jupyterlab_extension-0.1.931128384/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.930039523
+Version: 0.1.931128384
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
@@ -46,24 +46,21 @@
 ## Requirements
 
 - JupyterLab >= 3.0
 - python ~=3.7
 - Versatile Data Kit
 - npm
 
-## Install
-
-To install the extension,first navigate to the project directory and then execute:
+## Install and run
 
 ```bash
-# Once in the project directory, use the npm ci command to install
-# the exact versions of the dependencies specified in the package-lock.json
-npm ci
-# Install the extension
+# install the extension
 pip install vdk-jupyterlab-extension
+# run jupyterlab
+jupyter lab
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
```

