# Comparing `tmp/anywidget-0.6.1.tar.gz` & `tmp/anywidget-0.6.2.tar.gz`

## Comparing `anywidget-0.6.1.tar` & `anywidget-0.6.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.6.1/.pre-commit-config.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.1/CHANGELOG.md -> packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.6.1/CITATION.cff
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 anywidget-0.6.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget.json
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 anywidget-0.6.1/package.json
--rw-r--r--   0        0        0   273627 2020-02-02 00:00:00.000000 anywidget-0.6.1/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.6.1/pnpm-workspace.yaml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 anywidget-0.6.1/tsconfig.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.6.1/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/widget.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/138.6d69013365e0a65d34c8.js
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/326.44c2db4e788cbf8b5f08.js
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/remoteEntry.2cf77409ad03a77cbd09.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 anywidget-0.6.1/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.6.1/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.6.1/examples/Counter.ipynb
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.6.1/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/tsconfig.json
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/__tests__/widget.test.ts
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 anywidget-0.6.1/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_descriptor.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_utils.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.6.1/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.6.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.6.1/LICENSE
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 anywidget-0.6.1/README.md
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 anywidget-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 anywidget-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.6.2/.pre-commit-config.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.2/CHANGELOG.md -> packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.6.2/CITATION.cff
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 anywidget-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget.json
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 anywidget-0.6.2/package.json
+-rw-r--r--   0        0        0   272029 2020-02-02 00:00:00.000000 anywidget-0.6.2/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.6.2/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 anywidget-0.6.2/tsconfig.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.6.2/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/__init__.py
+-rw-r--r--   0        0        0    25347 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/widget.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/labextension/static/138.842852ea2bafcf459e69.js
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/labextension/static/326.8293ec79dbdf802e77d1.js
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/labextension/static/remoteEntry.cc3d041878be8537a74e.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 anywidget-0.6.2/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.6.2/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.6.2/examples/Counter.ipynb
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.6.2/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     8347 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/tsconfig.json
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/__tests__/widget.test.ts
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 anywidget-0.6.2/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.6.2/tests/test_descriptor.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.6.2/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.6.2/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.6.2/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.6.2/tests/test_utils.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.6.2/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 anywidget-0.6.2/README.md
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 anywidget-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 anywidget-0.6.2/PKG-INFO
```

### Comparing `anywidget-0.6.1/.pre-commit-config.yaml` & `anywidget-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/CITATION.cff` & `anywidget-0.6.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/CONTRIBUTING.md` & `anywidget-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/package.json` & `anywidget-0.6.2/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9479166666666667%*

 * *Differences: {"'devDependencies'": "{'@changesets/cli': '^2.26.2', 'esbuild': '^0.18.11', 'happy-dom': "*

 * *                      "'^10.0.7', 'typescript': '^5.1.6', 'vitest': '^0.32.4'}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "devDependencies": {
-        "@changesets/cli": "^2.26.1",
+        "@changesets/cli": "^2.26.2",
         "@svitejs/changesets-changelog-github-compact": "^1.1.0",
-        "esbuild": "^0.18.10",
-        "happy-dom": "^9.20.3",
-        "typescript": "^5.1.3",
-        "vitest": "^0.32.2"
+        "esbuild": "^0.18.11",
+        "happy-dom": "^10.0.7",
+        "typescript": "^5.1.6",
+        "vitest": "^0.32.4"
     },
     "name": "@anywidget/monorepo",
     "packageManager": "pnpm@8.6.1",
     "scripts": {
         "build": "pnpm build:nb && pnpm build:lab",
         "build:lab": "jupyter labextension build packages/anywidget",
         "build:nb": "pnpm --filter=!docs build && cp packages/anywidget/dist/index.js anywidget/nbextension/index.js",
```

### Comparing `anywidget-0.6.1/pnpm-lock.yaml` & `anywidget-0.6.2/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,31 @@
   excludeLinksFromLockfile: false
 
 importers:
 
   .:
     devDependencies:
       '@changesets/cli':
-        specifier: ^2.26.1
-        version: 2.26.1
+        specifier: ^2.26.2
+        version: 2.26.2
       '@svitejs/changesets-changelog-github-compact':
         specifier: ^1.1.0
         version: 1.1.0
       esbuild:
-        specifier: ^0.18.10
-        version: 0.18.10
+        specifier: ^0.18.11
+        version: 0.18.11
       happy-dom:
-        specifier: ^9.20.3
-        version: 9.20.3
+        specifier: ^10.0.7
+        version: 10.0.7
       typescript:
-        specifier: ^5.1.3
-        version: 5.1.3
+        specifier: ^5.1.6
+        version: 5.1.6
       vitest:
-        specifier: ^0.32.2
-        version: 0.32.2(happy-dom@9.20.3)
+        specifier: ^0.32.4
+        version: 0.32.4(happy-dom@10.0.7)
 
   docs:
     dependencies:
       '@algolia/client-search':
         specifier: ^4.13.1
         version: 4.13.1
       '@astrojs/markdown-remark':
@@ -109,19 +109,19 @@
         specifier: workspace:~
         version: link:../vite
       '@jupyter-widgets/base':
         specifier: ^2 || ^3 || ^4 || ^5 || ^6
         version: 2.0.0
     devDependencies:
       '@jupyter-widgets/base-manager':
-        specifier: ^1.0.5
-        version: 1.0.5(crypto@1.0.1)
+        specifier: ^1.0.6
+        version: 1.0.6(crypto@1.0.1)
       '@jupyterlab/builder':
         specifier: ^3.6.5
-        version: 3.6.5(crypto@1.0.1)(esbuild@0.18.10)
+        version: 3.6.5(crypto@1.0.1)(esbuild@0.18.11)
 
   packages/types: {}
 
   packages/vite:
     devDependencies:
       vite:
         specifier: ^4.3.9
@@ -636,131 +636,131 @@
     resolution: {integrity: sha512-zo3MIHGOkPOfoRXitsgHLjEXmlDaD/5KU1Uzuc9GNiZPhSqVxVRtxuPaSBZDsYZ9qV88AjtMtWW7ww98loJ9KA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/helper-string-parser': 7.22.5
       '@babel/helper-validator-identifier': 7.22.5
       to-fast-properties: 2.0.0
 
-  /@changesets/apply-release-plan@6.1.3:
-    resolution: {integrity: sha512-ECDNeoc3nfeAe1jqJb5aFQX7CqzQhD2klXRez2JDb/aVpGUbX673HgKrnrgJRuQR/9f2TtLoYIzrGB9qwD77mg==}
+  /@changesets/apply-release-plan@6.1.4:
+    resolution: {integrity: sha512-FMpKF1fRlJyCZVYHr3CbinpZZ+6MwvOtWUuO8uo+svcATEoc1zRDcj23pAurJ2TZ/uVz1wFHH6K3NlACy0PLew==}
     dependencies:
       '@babel/runtime': 7.22.5
-      '@changesets/config': 2.3.0
+      '@changesets/config': 2.3.1
       '@changesets/get-version-range-type': 0.3.2
       '@changesets/git': 2.0.0
       '@changesets/types': 5.2.1
       '@manypkg/get-packages': 1.1.3
       detect-indent: 6.1.0
       fs-extra: 7.0.1
       lodash.startcase: 4.4.0
       outdent: 0.5.0
-      prettier: 2.8.2
+      prettier: 2.8.8
       resolve-from: 5.0.0
-      semver: 5.7.1
+      semver: 7.5.3
     dev: true
 
-  /@changesets/assemble-release-plan@5.2.3:
-    resolution: {integrity: sha512-g7EVZCmnWz3zMBAdrcKhid4hkHT+Ft1n0mLussFMcB1dE2zCuwcvGoy9ec3yOgPGF4hoMtgHaMIk3T3TBdvU9g==}
+  /@changesets/assemble-release-plan@5.2.4:
+    resolution: {integrity: sha512-xJkWX+1/CUaOUWTguXEbCDTyWJFECEhmdtbkjhn5GVBGxdP/JwaHBIU9sW3FR6gD07UwZ7ovpiPclQZs+j+mvg==}
     dependencies:
       '@babel/runtime': 7.22.5
       '@changesets/errors': 0.1.4
-      '@changesets/get-dependents-graph': 1.3.5
+      '@changesets/get-dependents-graph': 1.3.6
       '@changesets/types': 5.2.1
       '@manypkg/get-packages': 1.1.3
-      semver: 5.7.1
+      semver: 7.5.3
     dev: true
 
   /@changesets/changelog-git@0.1.14:
     resolution: {integrity: sha512-+vRfnKtXVWsDDxGctOfzJsPhaCdXRYoe+KyWYoq5X/GqoISREiat0l3L8B0a453B2B4dfHGcZaGyowHbp9BSaA==}
     dependencies:
       '@changesets/types': 5.2.1
     dev: true
 
-  /@changesets/cli@2.26.1:
-    resolution: {integrity: sha512-XnTa+b51vt057fyAudvDKGB0Sh72xutQZNAdXkCqPBKO2zvs2yYZx5hFZj1u9cbtpwM6Sxtcr02/FQJfZOzemQ==}
+  /@changesets/cli@2.26.2:
+    resolution: {integrity: sha512-dnWrJTmRR8bCHikJHl9b9HW3gXACCehz4OasrXpMp7sx97ECuBGGNjJhjPhdZNCvMy9mn4BWdplI323IbqsRig==}
     hasBin: true
     dependencies:
       '@babel/runtime': 7.22.5
-      '@changesets/apply-release-plan': 6.1.3
-      '@changesets/assemble-release-plan': 5.2.3
+      '@changesets/apply-release-plan': 6.1.4
+      '@changesets/assemble-release-plan': 5.2.4
       '@changesets/changelog-git': 0.1.14
-      '@changesets/config': 2.3.0
+      '@changesets/config': 2.3.1
       '@changesets/errors': 0.1.4
-      '@changesets/get-dependents-graph': 1.3.5
-      '@changesets/get-release-plan': 3.0.16
+      '@changesets/get-dependents-graph': 1.3.6
+      '@changesets/get-release-plan': 3.0.17
       '@changesets/git': 2.0.0
       '@changesets/logger': 0.0.5
       '@changesets/pre': 1.0.14
       '@changesets/read': 0.5.9
       '@changesets/types': 5.2.1
       '@changesets/write': 0.2.3
       '@manypkg/get-packages': 1.1.3
       '@types/is-ci': 3.0.0
-      '@types/semver': 6.2.3
+      '@types/semver': 7.5.0
       ansi-colors: 4.1.3
       chalk: 2.4.2
       enquirer: 2.3.6
       external-editor: 3.1.0
       fs-extra: 7.0.1
       human-id: 1.0.2
       is-ci: 3.0.1
       meow: 6.1.1
       outdent: 0.5.0
       p-limit: 2.3.0
       preferred-pm: 3.0.3
       resolve-from: 5.0.0
-      semver: 5.7.1
+      semver: 7.5.3
       spawndamnit: 2.0.0
       term-size: 2.2.1
       tty-table: 4.2.1
     dev: true
 
-  /@changesets/config@2.3.0:
-    resolution: {integrity: sha512-EgP/px6mhCx8QeaMAvWtRrgyxW08k/Bx2tpGT+M84jEdX37v3VKfh4Cz1BkwrYKuMV2HZKeHOh8sHvja/HcXfQ==}
+  /@changesets/config@2.3.1:
+    resolution: {integrity: sha512-PQXaJl82CfIXddUOppj4zWu+987GCw2M+eQcOepxN5s+kvnsZOwjEJO3DH9eVy+OP6Pg/KFEWdsECFEYTtbg6w==}
     dependencies:
       '@changesets/errors': 0.1.4
-      '@changesets/get-dependents-graph': 1.3.5
+      '@changesets/get-dependents-graph': 1.3.6
       '@changesets/logger': 0.0.5
       '@changesets/types': 5.2.1
       '@manypkg/get-packages': 1.1.3
       fs-extra: 7.0.1
       micromatch: 4.0.5
     dev: true
 
   /@changesets/errors@0.1.4:
     resolution: {integrity: sha512-HAcqPF7snsUJ/QzkWoKfRfXushHTu+K5KZLJWPb34s4eCZShIf8BFO3fwq6KU8+G7L5KdtN2BzQAXOSXEyiY9Q==}
     dependencies:
       extendable-error: 0.1.7
     dev: true
 
-  /@changesets/get-dependents-graph@1.3.5:
-    resolution: {integrity: sha512-w1eEvnWlbVDIY8mWXqWuYE9oKhvIaBhzqzo4ITSJY9hgoqQ3RoBqwlcAzg11qHxv/b8ReDWnMrpjpKrW6m1ZTA==}
+  /@changesets/get-dependents-graph@1.3.6:
+    resolution: {integrity: sha512-Q/sLgBANmkvUm09GgRsAvEtY3p1/5OCzgBE5vX3vgb5CvW0j7CEljocx5oPXeQSNph6FXulJlXV3Re/v3K3P3Q==}
     dependencies:
       '@changesets/types': 5.2.1
       '@manypkg/get-packages': 1.1.3
       chalk: 2.4.2
       fs-extra: 7.0.1
-      semver: 5.7.1
+      semver: 7.5.3
     dev: true
 
   /@changesets/get-github-info@0.5.2:
     resolution: {integrity: sha512-JppheLu7S114aEs157fOZDjFqUDpm7eHdq5E8SSR0gUBTEK0cNSHsrSR5a66xs0z3RWuo46QvA3vawp8BxDHvg==}
     dependencies:
       dataloader: 1.4.0
       node-fetch: 2.6.11
     transitivePeerDependencies:
       - encoding
     dev: true
 
-  /@changesets/get-release-plan@3.0.16:
-    resolution: {integrity: sha512-OpP9QILpBp1bY2YNIKFzwigKh7Qe9KizRsZomzLe6pK8IUo8onkAAVUD8+JRKSr8R7d4+JRuQrfSSNlEwKyPYg==}
+  /@changesets/get-release-plan@3.0.17:
+    resolution: {integrity: sha512-6IwKTubNEgoOZwDontYc2x2cWXfr6IKxP3IhKeK+WjyD6y3M4Gl/jdQvBw+m/5zWILSOCAaGLu2ZF6Q+WiPniw==}
     dependencies:
       '@babel/runtime': 7.22.5
-      '@changesets/assemble-release-plan': 5.2.3
-      '@changesets/config': 2.3.0
+      '@changesets/assemble-release-plan': 5.2.4
+      '@changesets/config': 2.3.1
       '@changesets/pre': 1.0.14
       '@changesets/read': 0.5.9
       '@changesets/types': 5.2.1
       '@manypkg/get-packages': 1.1.3
     dev: true
 
   /@changesets/get-version-range-type@0.3.2:
@@ -826,15 +826,15 @@
   /@changesets/write@0.2.3:
     resolution: {integrity: sha512-Dbamr7AIMvslKnNYsLFafaVORx4H0pvCA2MHqgtNCySMe1blImEyAEOzDmcgKAkgz4+uwoLz7demIrX+JBr/Xw==}
     dependencies:
       '@babel/runtime': 7.22.5
       '@changesets/types': 5.2.1
       fs-extra: 7.0.1
       human-id: 1.0.2
-      prettier: 2.8.2
+      prettier: 2.8.8
     dev: true
 
   /@discoveryjs/json-ext@0.5.7:
     resolution: {integrity: sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==}
     engines: {node: '>=10.0.0'}
     dev: true
 
@@ -874,16 +874,16 @@
     resolution: {integrity: sha512-KBMWvEZooR7+kzY0BtbTQn0OAYY7CsiydT63pVEaPtVYF0hXbUaOyZog37DKxK7NF3XacBJOpYT4adIJh+avxA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     optional: true
 
-  /@esbuild/android-arm64@0.18.10:
-    resolution: {integrity: sha512-ynm4naLbNbK0ajf9LUWtQB+6Vfg1Z/AplArqr4tGebC00Z6m9Y91OVIcjDa461wGcZwcaHYaZAab4yJxfhisTQ==}
+  /@esbuild/android-arm64@0.18.11:
+    resolution: {integrity: sha512-snieiq75Z1z5LJX9cduSAjUr7vEI1OdlzFPMw0HH5YI7qQHDd3qs+WZoMrWYDsfRJSq36lIA6mfZBkvL46KoIw==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -891,16 +891,16 @@
     resolution: {integrity: sha512-rIKddzqhmav7MSmoFCmDIb6e2W57geRsM94gV2l38fzhXMwq7hZoClug9USI2pFRGL06f4IOPHHpFNOkWieR8A==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     optional: true
 
-  /@esbuild/android-arm@0.18.10:
-    resolution: {integrity: sha512-3KClmVNd+Fku82uZJz5C4Rx8m1PPmWUFz5Zkw8jkpZPOmsq+EG1TTOtw1OXkHuX3WczOFQigrtf60B1ijKwNsg==}
+  /@esbuild/android-arm@0.18.11:
+    resolution: {integrity: sha512-q4qlUf5ucwbUJZXF5tEQ8LF7y0Nk4P58hOsGk3ucY0oCwgQqAnqXVbUuahCddVHfrxmpyewRpiTHwVHIETYu7Q==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -908,16 +908,16 @@
     resolution: {integrity: sha512-uUTTc4xGNDT7YSArp/zbtmbhO0uEEK9/ETW29Wk1thYUJBz3IVnvgEiEwEa9IeLyvnpKrWK64Utw2bgUmDveww==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     optional: true
 
-  /@esbuild/android-x64@0.18.10:
-    resolution: {integrity: sha512-vFfXj8P9Yfjh54yqUDEHKzqzYuEfPyAOl3z7R9hjkwt+NCvbn9VMxX+IILnAfdImRBfYVItgSUsqGKhJFnBwZw==}
+  /@esbuild/android-x64@0.18.11:
+    resolution: {integrity: sha512-iPuoxQEV34+hTF6FT7om+Qwziv1U519lEOvekXO9zaMMlT9+XneAhKL32DW3H7okrCOBQ44BMihE8dclbZtTuw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -925,16 +925,16 @@
     resolution: {integrity: sha512-80wEoCfF/hFKM6WE1FyBHc9SfUblloAWx6FJkFWTWiCoht9Mc0ARGEM47e67W9rI09YoUxJL68WHfDRYEAvOhg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     optional: true
 
-  /@esbuild/darwin-arm64@0.18.10:
-    resolution: {integrity: sha512-k2OJQ7ZxE6sVc91+MQeZH9gFeDAH2uIYALPAwTjTCvcPy9Dzrf7V7gFUQPYkn09zloWhQ+nvxWHia2x2ZLR0sQ==}
+  /@esbuild/darwin-arm64@0.18.11:
+    resolution: {integrity: sha512-Gm0QkI3k402OpfMKyQEEMG0RuW2LQsSmI6OeO4El2ojJMoF5NLYb3qMIjvbG/lbMeLOGiW6ooU8xqc+S0fgz2w==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -942,16 +942,16 @@
     resolution: {integrity: sha512-IJM4JJsLhRYr9xdtLytPLSH9k/oxR3boaUIYiHkAawtwNOXKE8KoU8tMvryogdcT8AU+Bflmh81Xn6Q0vTZbQw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     optional: true
 
-  /@esbuild/darwin-x64@0.18.10:
-    resolution: {integrity: sha512-tnz/mdZk1L1Z3WpGjin/L2bKTe8/AKZpI8fcCLtH+gq8WXWsCNJSxlesAObV4qbtTl6pG5vmqFXfWUQ5hV8PAQ==}
+  /@esbuild/darwin-x64@0.18.11:
+    resolution: {integrity: sha512-N15Vzy0YNHu6cfyDOjiyfJlRJCB/ngKOAvoBf1qybG3eOq0SL2Lutzz9N7DYUbb7Q23XtHPn6lMDF6uWbGv9Fw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -959,16 +959,16 @@
     resolution: {integrity: sha512-pBwbc7DufluUeGdjSU5Si+P3SoMF5DQ/F/UmTSb8HXO80ZEAJmrykPyzo1IfNbAoaqw48YRpv8shwd1NoI0jcQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/freebsd-arm64@0.18.10:
-    resolution: {integrity: sha512-QJluV0LwBrbHnYYwSKC+K8RGz0g/EyhpQH1IxdoFT0nM7PfgjE+aS8wxq/KFEsU0JkL7U/EEKd3O8xVBxXb2aA==}
+  /@esbuild/freebsd-arm64@0.18.11:
+    resolution: {integrity: sha512-atEyuq6a3omEY5qAh5jIORWk8MzFnCpSTUruBgeyN9jZq1K/QI9uke0ATi3MHu4L8c59CnIi4+1jDKMuqmR71A==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -976,16 +976,16 @@
     resolution: {integrity: sha512-4lu+n8Wk0XlajEhbEffdy2xy53dpR06SlzvhGByyg36qJw6Kpfk7cp45DR/62aPH9mtJRmIyrXAS5UWBrJT6TQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/freebsd-x64@0.18.10:
-    resolution: {integrity: sha512-Hi/ycUkS6KTw+U9G5PK5NoK7CZboicaKUSVs0FSiPNtuCTzK6HNM4DIgniH7hFaeuszDS9T4dhAHWiLSt/Y5Ng==}
+  /@esbuild/freebsd-x64@0.18.11:
+    resolution: {integrity: sha512-XtuPrEfBj/YYYnAAB7KcorzzpGTvOr/dTtXPGesRfmflqhA4LMF0Gh/n5+a9JBzPuJ+CGk17CA++Hmr1F/gI0Q==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -993,16 +993,16 @@
     resolution: {integrity: sha512-ct1Tg3WGwd3P+oZYqic+YZF4snNl2bsnMKRkb3ozHmnM0dGWuxcPTTntAF6bOP0Sp4x0PjSF+4uHQ1xvxfRKqg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-arm64@0.18.10:
-    resolution: {integrity: sha512-Nz6XcfRBOO7jSrVpKAyEyFOPGhySPNlgumSDhWAspdQQ11ub/7/NZDMhWDFReE9QH/SsCOCLQbdj0atAk/HMOQ==}
+  /@esbuild/linux-arm64@0.18.11:
+    resolution: {integrity: sha512-c6Vh2WS9VFKxKZ2TvJdA7gdy0n6eSy+yunBvv4aqNCEhSWVor1TU43wNRp2YLO9Vng2G+W94aRz+ILDSwAiYog==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1010,16 +1010,16 @@
     resolution: {integrity: sha512-cdmT3KxjlOQ/gZ2cjfrQOtmhG4HJs6hhvm3mWSRDPtZ/lP5oe8FWceS10JaSJC13GBd4eH/haHnqf7hhGNLerA==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-arm@0.18.10:
-    resolution: {integrity: sha512-HfFoxY172tVHPIvJy+FHxzB4l8xU7e5cxmNS11cQ2jt4JWAukn/7LXaPdZid41UyTweqa4P/1zs201gRGCTwHw==}
+  /@esbuild/linux-arm@0.18.11:
+    resolution: {integrity: sha512-Idipz+Taso/toi2ETugShXjQ3S59b6m62KmLHkJlSq/cBejixmIydqrtM2XTvNCywFl3VC7SreSf6NV0i6sRyg==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1027,16 +1027,16 @@
     resolution: {integrity: sha512-w4IRhSy1VbsNxHRQpeGCHEmibqdTUx61Vc38APcsRbuVgK0OPEnQ0YD39Brymn96mOx48Y2laBQGqgZ0j9w6SQ==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-ia32@0.18.10:
-    resolution: {integrity: sha512-otMdmSmkMe+pmiP/bZBjfphyAsTsngyT9RCYwoFzqrveAbux9nYitDTpdgToG0Z0U55+PnH654gCH2GQ1aB6Yw==}
+  /@esbuild/linux-ia32@0.18.11:
+    resolution: {integrity: sha512-S3hkIF6KUqRh9n1Q0dSyYcWmcVa9Cg+mSoZEfFuzoYXXsk6196qndrM+ZiHNwpZKi3XOXpShZZ+9dfN5ykqjjw==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1044,16 +1044,16 @@
     resolution: {integrity: sha512-2iAngUbBPMq439a+z//gE+9WBldoMp1s5GWsUSgqHLzLJ9WoZLZhpwWuym0u0u/4XmZ3gpHmzV84PonE+9IIdQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-loong64@0.18.10:
-    resolution: {integrity: sha512-t8tjFuON1koxskzQ4VFoh0T5UDUMiLYjwf9Wktd0tx8AoK6xgU+5ubKOpWpcnhEQ2tESS5u0v6QuN8PX/ftwcQ==}
+  /@esbuild/linux-loong64@0.18.11:
+    resolution: {integrity: sha512-MRESANOoObQINBA+RMZW+Z0TJWpibtE7cPFnahzyQHDCA9X9LOmGh68MVimZlM9J8n5Ia8lU773te6O3ILW8kw==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1061,16 +1061,16 @@
     resolution: {integrity: sha512-LKJltc4LVdMKHsrFe4MGNPp0hqDFA1Wpt3jE1gEyM3nKUvOiO//9PheZZHfYRfYl6AwdTH4aTcXSqBerX0ml4A==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-mips64el@0.18.10:
-    resolution: {integrity: sha512-+dUkcVzcfEJHz3HEnVpIJu8z8Wdn2n/nWMWdl6FVPFGJAVySO4g3+XPzNKFytVFwf8hPVDwYXzVcu8GMFqsqZw==}
+  /@esbuild/linux-mips64el@0.18.11:
+    resolution: {integrity: sha512-qVyPIZrXNMOLYegtD1u8EBccCrBVshxMrn5MkuFc3mEVsw7CCQHaqZ4jm9hbn4gWY95XFnb7i4SsT3eflxZsUg==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1078,16 +1078,16 @@
     resolution: {integrity: sha512-/c/DGybs95WXNS8y3Ti/ytqETiW7EU44MEKuCAcpPto3YjQbyK3IQVKfF6nbghD7EcLUGl0NbiL5Rt5DMhn5tg==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-ppc64@0.18.10:
-    resolution: {integrity: sha512-sO3PjjxEGy+PY2qkGe2gwJbXdZN9wAYpVBZWFD0AwAoKuXRkWK0/zaMQ5ekUFJDRDCRm8x5U0Axaub7ynH/wVg==}
+  /@esbuild/linux-ppc64@0.18.11:
+    resolution: {integrity: sha512-T3yd8vJXfPirZaUOoA9D2ZjxZX4Gr3QuC3GztBJA6PklLotc/7sXTOuuRkhE9W/5JvJP/K9b99ayPNAD+R+4qQ==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1095,16 +1095,16 @@
     resolution: {integrity: sha512-FC3nUAWhvFoutlhAkgHf8f5HwFWUL6bYdvLc/TTuxKlvLi3+pPzdZiFKSWz/PF30TB1K19SuCxDTI5KcqASJqA==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-riscv64@0.18.10:
-    resolution: {integrity: sha512-JDtdbJg3yjDeXLv4lZYE1kiTnxv73/8cbPHY9T/dUKi8rYOM/k5b3W4UJLMUksuQ6nTm5c89W1nADsql6FW75A==}
+  /@esbuild/linux-riscv64@0.18.11:
+    resolution: {integrity: sha512-evUoRPWiwuFk++snjH9e2cAjF5VVSTj+Dnf+rkO/Q20tRqv+644279TZlPK8nUGunjPAtQRCj1jQkDAvL6rm2w==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1112,16 +1112,16 @@
     resolution: {integrity: sha512-IbFsFbxMWLuKEbH+7sTkKzL6NJmG2vRyy6K7JJo55w+8xDk7RElYn6xvXtDW8HCfoKBFK69f3pgBJSUSQPr+4Q==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-s390x@0.18.10:
-    resolution: {integrity: sha512-NLuSKcp8WckjD2a7z5kzLiCywFwBTMlIxDNuud1AUGVuwBBJSkuubp6cNjJ0p5c6CZaA3QqUGwjHJBiG1SoOFw==}
+  /@esbuild/linux-s390x@0.18.11:
+    resolution: {integrity: sha512-/SlRJ15XR6i93gRWquRxYCfhTeC5PdqEapKoLbX63PLCmAkXZHY2uQm2l9bN0oPHBsOw2IswRZctMYS0MijFcg==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1129,16 +1129,16 @@
     resolution: {integrity: sha512-68ngA9lg2H6zkZcyp22tsVt38mlhWde8l3eJLWkyLrp4HwMUr3c1s/M2t7+kHIhvMjglIBrFpncX1SzMckomGw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     optional: true
 
-  /@esbuild/linux-x64@0.18.10:
-    resolution: {integrity: sha512-wj2KRsCsFusli+6yFgNO/zmmLslislAWryJnodteRmGej7ZzinIbMdsyp13rVGde88zxJd5vercNYK9kuvlZaQ==}
+  /@esbuild/linux-x64@0.18.11:
+    resolution: {integrity: sha512-xcncej+wF16WEmIwPtCHi0qmx1FweBqgsRtEL1mSHLFR6/mb3GEZfLQnx+pUDfRDEM4DQF8dpXIW7eDOZl1IbA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1146,16 +1146,16 @@
     resolution: {integrity: sha512-CwFq42rXCR8TYIjIfpXCbRX0rp1jo6cPIUPSaWwzbVI4aOfX96OXY8M6KNmtPcg7QjYeDmN+DD0Wp3LaBOLf4Q==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/netbsd-x64@0.18.10:
-    resolution: {integrity: sha512-pQ9QqxEPI3cVRZyUtCoZxhZK3If+7RzR8L2yz2+TDzdygofIPOJFaAPkEJ5rYIbUO101RaiYxfdOBahYexLk5A==}
+  /@esbuild/netbsd-x64@0.18.11:
+    resolution: {integrity: sha512-aSjMHj/F7BuS1CptSXNg6S3M4F3bLp5wfFPIJM+Km2NfIVfFKhdmfHF9frhiCLIGVzDziggqWll0B+9AUbud/Q==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1163,16 +1163,16 @@
     resolution: {integrity: sha512-cnq5brJYrSZ2CF6c35eCmviIN3k3RczmHz8eYaVlNasVqsNY+JKohZU5MKmaOI+KkllCdzOKKdPs762VCPC20g==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     optional: true
 
-  /@esbuild/openbsd-x64@0.18.10:
-    resolution: {integrity: sha512-k8GTIIW9I8pEEfoOUm32TpPMgSg06JhL5DO+ql66aLTkOQUs0TxCA67Wi7pv6z8iF8STCGcNbm3UWFHLuci+ag==}
+  /@esbuild/openbsd-x64@0.18.11:
+    resolution: {integrity: sha512-tNBq+6XIBZtht0xJGv7IBB5XaSyvYPCm1PxJ33zLQONdZoLVM0bgGqUrXnJyiEguD9LU4AHiu+GCXy/Hm9LsdQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1180,16 +1180,16 @@
     resolution: {integrity: sha512-vCRT7yP3zX+bKWFeP/zdS6SqdWB8OIpaRq/mbXQxTGHnIxspRtigpkUcDMlSCOejlHowLqII7K2JKevwyRP2rg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     optional: true
 
-  /@esbuild/sunos-x64@0.18.10:
-    resolution: {integrity: sha512-vIGYJIdEI6d4JBucAx8py792G8J0GP40qSH+EvSt80A4zvGd6jph+5t1g+eEXcS2aRpgZw6CrssNCFZxTdEsxw==}
+  /@esbuild/sunos-x64@0.18.11:
+    resolution: {integrity: sha512-kxfbDOrH4dHuAAOhr7D7EqaYf+W45LsAOOhAet99EyuxxQmjbk8M9N4ezHcEiCYPaiW8Dj3K26Z2V17Gt6p3ng==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1197,16 +1197,16 @@
     resolution: {integrity: sha512-yYx+8jwowUstVdorcMdNlzklLYhPxjniHWFKgRqH7IFlUEa0Umu3KuYplf1HUZZ422e3NU9F4LGb+4O0Kdcaag==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     optional: true
 
-  /@esbuild/win32-arm64@0.18.10:
-    resolution: {integrity: sha512-kRhNcMZFGMW+ZHCarAM1ypr8OZs0k688ViUCetVCef9p3enFxzWeBg9h/575Y0nsFu0ZItluCVF5gMR2pwOEpA==}
+  /@esbuild/win32-arm64@0.18.11:
+    resolution: {integrity: sha512-Sh0dDRyk1Xi348idbal7lZyfSkjhJsdFeuC13zqdipsvMetlGiFQNdO+Yfp6f6B4FbyQm7qsk16yaZk25LChzg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1214,16 +1214,16 @@
     resolution: {integrity: sha512-eggDKanJszUtCdlVs0RB+h35wNlb5v4TWEkq4vZcmVt5u/HiDZrTXe2bWFQUez3RgNHwx/x4sk5++4NSSicKkw==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     optional: true
 
-  /@esbuild/win32-ia32@0.18.10:
-    resolution: {integrity: sha512-AR9PX1whYaYh9p0EOaKna0h48F/A101Mt/ag72+kMkkBZXPQ7cjbz2syXI/HI3OlBdUytSdHneljfjvUoqwqiQ==}
+  /@esbuild/win32-ia32@0.18.11:
+    resolution: {integrity: sha512-o9JUIKF1j0rqJTFbIoF4bXj6rvrTZYOrfRcGyL0Vm5uJ/j5CkBD/51tpdxe9lXEDouhRgdr/BYzUrDOvrWwJpg==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
@@ -1231,27 +1231,34 @@
     resolution: {integrity: sha512-lAhycmKnVOuRYNtRtatQR1LPQf2oYCkRGkSFnseDAKPl8lu5SOsK/e1sXe5a0Pc5kHIHe6P2I/ilntNv2xf3cA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     optional: true
 
-  /@esbuild/win32-x64@0.18.10:
-    resolution: {integrity: sha512-5sTkYhAGHNRr6bVf4RM0PsscqVr6/DBYdrlMh168oph3usid3lKHcHEEHmr34iZ9GHeeg2juFOxtpl6XyC3tpw==}
+  /@esbuild/win32-x64@0.18.11:
+    resolution: {integrity: sha512-rQI4cjLHd2hGsM1LqgDI7oOCYbQ6IBOVsX9ejuRMSze0GqXUG2ekwiKkiBU1pRGSeCqFFHxTrcEydB2Hyoz9CA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
   /@gar/promisify@1.1.3:
     resolution: {integrity: sha512-k2Ty1JcVojjJFwrg/ThKi2ujJ7XNLYaFGNB/bWT9wGR+oSMJHMa5w+CUq6p/pVrKeNNgA7pCqEcjSnHVoqJQFw==}
     dev: true
 
+  /@jest/schemas@29.4.3:
+    resolution: {integrity: sha512-VLYKXQmtmuEz6IxJsrZwzG9NvtkQsWNnWMsKxqWNu3+CnfzJQhp0WDDKWLVV9hLKr0l3SLLFRqcYHjhtyuDVxg==}
+    engines: {node: ^14.15.0 || ^16.10.0 || >=18.0.0}
+    dependencies:
+      '@sinclair/typebox': 0.25.24
+    dev: true
+
   /@jridgewell/gen-mapping@0.3.3:
     resolution: {integrity: sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.15
       '@jridgewell/trace-mapping': 0.3.18
@@ -1279,18 +1286,18 @@
 
   /@jridgewell/trace-mapping@0.3.18:
     resolution: {integrity: sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==}
     dependencies:
       '@jridgewell/resolve-uri': 3.1.0
       '@jridgewell/sourcemap-codec': 1.4.14
 
-  /@jupyter-widgets/base-manager@1.0.5(crypto@1.0.1):
-    resolution: {integrity: sha512-+pagXIXBbSq1NdqaJ8xJj52SF3t0zyUofDHVZ1bFrfWIhl5qZuLxtD16PvnqO+n1gIPLlW238Og6QuIGKOKkZQ==}
+  /@jupyter-widgets/base-manager@1.0.6(crypto@1.0.1):
+    resolution: {integrity: sha512-CZmDBbImzK3tUuGLmZDRXqPyLxwzZHuHOD/reYr87A4kbBrREe7xFxWqr+v0iLcadxwtzNdP+H+bQUF+S76NXw==}
     dependencies:
-      '@jupyter-widgets/base': 6.0.4(crypto@1.0.1)
+      '@jupyter-widgets/base': 6.0.5(crypto@1.0.1)
       '@jupyterlab/services': 6.6.4(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       base64-js: 1.5.1
       sanitize-html: 2.11.0
     transitivePeerDependencies:
       - bufferutil
       - crypto
@@ -1313,16 +1320,16 @@
       lodash: 4.17.21
     transitivePeerDependencies:
       - bufferutil
       - encoding
       - utf-8-validate
     dev: false
 
-  /@jupyter-widgets/base@6.0.4(crypto@1.0.1):
-    resolution: {integrity: sha512-w5KUL8q44Isp0N/ElOAJbPSgWBdeGZO5EYEcz50rfqYAUMSh2Qx0oQJYMddbRgi8b5CajGHFvcHTfvwaNDLSmA==}
+  /@jupyter-widgets/base@6.0.5(crypto@1.0.1):
+    resolution: {integrity: sha512-33LXLYKHOJSinTcmFF7ScNtVU8RMo/8HRknyLKauB5t99cuov3ULpL0fTiV272EAWYrGVZ6eGrNUyJY3kbqCqg==}
     dependencies:
       '@jupyterlab/services': 6.6.4(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/messaging': 1.10.3
       '@lumino/widgets': 1.37.2(crypto@1.0.1)
       '@types/backbone': 1.4.14
       '@types/lodash': 4.14.195
@@ -1332,15 +1339,15 @@
     transitivePeerDependencies:
       - bufferutil
       - crypto
       - encoding
       - utf-8-validate
     dev: true
 
-  /@jupyterlab/builder@3.6.5(crypto@1.0.1)(esbuild@0.18.10):
+  /@jupyterlab/builder@3.6.5(crypto@1.0.1)(esbuild@0.18.11):
     resolution: {integrity: sha512-J9WO50gxjJ1bUo7BCix0fSxpRySCwaR8AaWNQ5QdYT1ARSGuSnfM9ZyeUOS61DvL3+h7IqsPTQQr5tbhIWv91Q==}
     hasBin: true
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/application': 1.31.4(crypto@1.0.1)
       '@lumino/commands': 1.21.1(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
@@ -1367,15 +1374,15 @@
       source-map-loader: 1.0.2(webpack@5.88.0)
       style-loader: 2.0.0(webpack@5.88.0)
       supports-color: 7.2.0
       svg-url-loader: 6.0.0(webpack@5.88.0)
       terser-webpack-plugin: 4.2.3(webpack@5.88.0)
       to-string-loader: 1.2.0
       url-loader: 4.1.1(file-loader@6.0.0)(webpack@5.88.0)
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
       webpack-cli: 4.10.0(webpack@5.88.0)
       webpack-merge: 5.9.0
       worker-loader: 3.0.8(webpack@5.88.0)
     transitivePeerDependencies:
       - '@swc/core'
       - '@webpack-cli/generators'
       - '@webpack-cli/migrate'
@@ -1824,14 +1831,18 @@
   /@proload/core@0.3.3:
     resolution: {integrity: sha512-7dAFWsIK84C90AMl24+N/ProHKm4iw0akcnoKjRvbfHifJZBLhaDsDus1QJmhG12lXj4e/uB/8mB/0aduCW+NQ==}
     dependencies:
       deepmerge: 4.3.1
       escalade: 3.1.1
     dev: false
 
+  /@sinclair/typebox@0.25.24:
+    resolution: {integrity: sha512-XJfwUVUKDHF5ugKwIcxEgc9k8b7HbznCp6eUfWgu710hMPNIO4aw4/zB5RogDQz8nd6gyCDpU9O/m6qYEWY6yQ==}
+    dev: true
+
   /@svitejs/changesets-changelog-github-compact@1.1.0:
     resolution: {integrity: sha512-qhUGGDHcpbY2zpjW3SwqchuW8J/5EzlPFud7xNntHKA7f3a/mx5+g+ruJKFHSAiVZYo30PALt+AyhmPUNKH/Og==}
     engines: {node: ^14.13.1 || ^16.0.0 || >=18}
     dependencies:
       '@changesets/get-github-info': 0.5.2
       dotenv: 16.3.1
     transitivePeerDependencies:
@@ -2007,16 +2018,16 @@
   /@types/resolve@1.20.2:
     resolution: {integrity: sha512-60BCwRFOZCQhDncwQdxxeOEEkbc5dIMccYLwbxsS4TUNeVECQ/pBJ0j09mrHOl/JJvpRPGwO9SvE4nR2Nb/a4Q==}
 
   /@types/scheduler@0.16.3:
     resolution: {integrity: sha512-5cJ8CB4yAx7BH1oMvdU0Jh9lrEXyPkar6F9G/ERswkCuvP4KQZfZkSjcMbAICCpQTN4OuZn8tz0HiKv9TGZgrQ==}
     dev: false
 
-  /@types/semver@6.2.3:
-    resolution: {integrity: sha512-KQf+QAMWKMrtBMsB8/24w53tEsxllMj6TuA80TT/5igJalLI/zm0L3oXRbIAl4Ohfc85gyHX/jhMwsVkmhLU4A==}
+  /@types/semver@7.5.0:
+    resolution: {integrity: sha512-G8hZ6XJiHnuhQKR7ZmysCeJWE08o8T0AXtk5darsCaTVsYZhhgUrq53jizaR2FvsoeCwJhlmwTjkXBY5Pn/ZHw==}
     dev: true
 
   /@types/sizzle@2.3.3:
     resolution: {integrity: sha512-JYM8x9EGF163bEyhdJBpR2QX1R5naCJHC8ucJylJ3w9/CVBaskdQ8WqBf8MmQrd1kRvp/a4TS8HJ+bxzR7ZJYQ==}
 
   /@types/source-list-map@0.1.2:
     resolution: {integrity: sha512-K5K+yml8LTo9bWJI/rECfIPrGgxdpeNbj+d53lwN4QjW1MCwlkhUms+gtdzigTeUyBr09+u8BwOIY3MXvHdcsA==}
@@ -2035,51 +2046,50 @@
       '@types/source-list-map': 0.1.2
       source-map: 0.6.1
     dev: true
 
   /@types/yargs-parser@21.0.0:
     resolution: {integrity: sha512-iO9ZQHkZxHn4mSakYV0vFHAVDyEOIJQrV2uZ06HxEPcx+mt8swXoZHIbaaJ2crJYFfErySgktuTZ3BeLz+XmFA==}
 
-  /@vitest/expect@0.32.2:
-    resolution: {integrity: sha512-6q5yzweLnyEv5Zz1fqK5u5E83LU+gOMVBDuxBl2d2Jfx1BAp5M+rZgc5mlyqdnxquyoiOXpXmFNkcGcfFnFH3Q==}
+  /@vitest/expect@0.32.4:
+    resolution: {integrity: sha512-m7EPUqmGIwIeoU763N+ivkFjTzbaBn0n9evsTOcde03ugy2avPs3kZbYmw3DkcH1j5mxhMhdamJkLQ6dM1bk/A==}
     dependencies:
-      '@vitest/spy': 0.32.2
-      '@vitest/utils': 0.32.2
+      '@vitest/spy': 0.32.4
+      '@vitest/utils': 0.32.4
       chai: 4.3.7
     dev: true
 
-  /@vitest/runner@0.32.2:
-    resolution: {integrity: sha512-06vEL0C1pomOEktGoLjzZw+1Fb+7RBRhmw/06WkDrd1akkT9i12su0ku+R/0QM69dfkIL/rAIDTG+CSuQVDcKw==}
+  /@vitest/runner@0.32.4:
+    resolution: {integrity: sha512-cHOVCkiRazobgdKLnczmz2oaKK9GJOw6ZyRcaPdssO1ej+wzHVIkWiCiNacb3TTYPdzMddYkCgMjZ4r8C0JFCw==}
     dependencies:
-      '@vitest/utils': 0.32.2
-      concordance: 5.0.4
+      '@vitest/utils': 0.32.4
       p-limit: 4.0.0
       pathe: 1.1.1
     dev: true
 
-  /@vitest/snapshot@0.32.2:
-    resolution: {integrity: sha512-JwhpeH/PPc7GJX38vEfCy9LtRzf9F4er7i4OsAJyV7sjPwjj+AIR8cUgpMTWK4S3TiamzopcTyLsZDMuldoi5A==}
+  /@vitest/snapshot@0.32.4:
+    resolution: {integrity: sha512-IRpyqn9t14uqsFlVI2d7DFMImGMs1Q9218of40bdQQgMePwVdmix33yMNnebXcTzDU5eiV3eUsoxxH5v0x/IQA==}
     dependencies:
       magic-string: 0.30.0
       pathe: 1.1.1
-      pretty-format: 27.5.1
+      pretty-format: 29.5.0
     dev: true
 
-  /@vitest/spy@0.32.2:
-    resolution: {integrity: sha512-Q/ZNILJ4ca/VzQbRM8ur3Si5Sardsh1HofatG9wsJY1RfEaw0XKP8IVax2lI1qnrk9YPuG9LA2LkZ0EI/3d4ug==}
+  /@vitest/spy@0.32.4:
+    resolution: {integrity: sha512-oA7rCOqVOOpE6rEoXuCOADX7Lla1LIa4hljI2MSccbpec54q+oifhziZIJXxlE/CvI2E+ElhBHzVu0VEvJGQKQ==}
     dependencies:
       tinyspy: 2.1.1
     dev: true
 
-  /@vitest/utils@0.32.2:
-    resolution: {integrity: sha512-lnJ0T5i03j0IJaeW73hxe2AuVnZ/y1BhhCOuIcl9LIzXnbpXJT9Lrt6brwKHXLOiA7MZ6N5hSJjt0xE1dGNCzQ==}
+  /@vitest/utils@0.32.4:
+    resolution: {integrity: sha512-Gwnl8dhd1uJ+HXrYyV0eRqfmk9ek1ASE/LWfTCuWMw+d07ogHqp4hEAV28NiecimK6UY9DpSEPh+pXBA5gtTBg==}
     dependencies:
       diff-sequences: 29.4.3
       loupe: 2.3.6
-      pretty-format: 27.5.1
+      pretty-format: 29.5.0
     dev: true
 
   /@vscode/emmet-helper@2.9.1:
     resolution: {integrity: sha512-+cdkHZ/QlvSXXsA/fstnyl1EwIFJyKA9Mw4Yz4oC6gXTTewfViYWOddtDPVYKGtda/vA0rcnHTAF/Xl7+QGKgQ==}
     dependencies:
       emmet: 2.4.4
       jsonc-parser: 2.3.1
@@ -2198,15 +2208,15 @@
 
   /@webpack-cli/configtest@1.2.0(webpack-cli@4.10.0)(webpack@5.88.0):
     resolution: {integrity: sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==}
     peerDependencies:
       webpack: 4.x.x || 5.x.x
       webpack-cli: 4.x.x
     dependencies:
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
       webpack-cli: 4.10.0(webpack@5.88.0)
     dev: true
 
   /@webpack-cli/info@1.5.0(webpack-cli@4.10.0):
     resolution: {integrity: sha512-e8tSXZpw2hPl2uMJY6fsMswaok5FdlGNRTktvFk2sD8RjH0hE2+XistawJx1vmKteh4NmGmNUrp+Tb2w+udPcQ==}
     peerDependencies:
       webpack-cli: 4.x.x
@@ -2467,15 +2477,15 @@
       server-destroy: 1.0.1
       shiki: 0.14.1
       slash: 4.0.0
       string-width: 5.1.2
       strip-ansi: 7.1.0
       supports-esm: 1.0.0
       tsconfig-resolver: 3.0.1
-      typescript: 5.1.3
+      typescript: 5.1.6
       unist-util-visit: 4.1.2
       vfile: 5.3.7
       vite: 4.3.9(@types/node@18.0.0)
       vitefu: 0.2.4(vite@4.3.9)
       yargs-parser: 21.1.1
       zod: 3.21.4
     transitivePeerDependencies:
@@ -2567,18 +2577,14 @@
   /bl@5.1.0:
     resolution: {integrity: sha512-tv1ZJHLfTDnXE6tMHv73YgSJaWR2AFuPwMntBe7XL/GBFHnT0CLnsHMogfk5+GzCDC5ZWarSCYaIGATZt9dNsQ==}
     dependencies:
       buffer: 6.0.3
       inherits: 2.0.4
       readable-stream: 3.6.2
 
-  /blueimp-md5@2.19.0:
-    resolution: {integrity: sha512-DRQrD6gJyy8FbiE4s+bDoXS9hiW3Vbx5uCdwvcCf3zLHL+Iv7LtGHLpr+GZV8rHG8tK766FGYBwRbu8pELTt+w==}
-    dev: true
-
   /boxen@6.2.1:
     resolution: {integrity: sha512-H4PEsJXfFI/Pt8sjDWbHlQPx4zL/bvSQjcilJmaulGt5mLDorHOHpmdXAJcBcmru7PhYSp/cDMWRko4ZUMFkSw==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dependencies:
       ansi-align: 3.0.1
       camelcase: 6.3.0
       chalk: 4.1.2
@@ -2896,28 +2902,14 @@
   /commondir@1.0.1:
     resolution: {integrity: sha512-W9pAhw0ja1Edb5GVdIF1mjZw/ASI0AlShXM83UUGe2DVr5TdAPEA1OA8m/g8zWp9x6On7gqufY+FatDbC3MDQg==}
     dev: true
 
   /concat-map@0.0.1:
     resolution: {integrity: sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==}
 
-  /concordance@5.0.4:
-    resolution: {integrity: sha512-OAcsnTEYu1ARJqWVGwf4zh4JDfHZEaSNlNccFmt8YjB2l/n19/PF2viLINHc57vO4FKIAFl2FWASIGZZWZ2Kxw==}
-    engines: {node: '>=10.18.0 <11 || >=12.14.0 <13 || >=14'}
-    dependencies:
-      date-time: 3.1.0
-      esutils: 2.0.3
-      fast-diff: 1.3.0
-      js-string-escape: 1.0.1
-      lodash: 4.17.21
-      md5-hex: 3.0.1
-      semver: 7.5.3
-      well-known-symbols: 2.0.0
-    dev: true
-
   /convert-source-map@1.9.0:
     resolution: {integrity: sha512-ASFBup0Mz1uyiIjANan1jzLQami9z1PoYSZCiiYW2FczPbenXc45FZdBZLzOT+r6+iciuEModtmCti+hjaAk0A==}
 
   /cookie@0.5.0:
     resolution: {integrity: sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==}
     engines: {node: '>= 0.6'}
 
@@ -2954,15 +2946,15 @@
       postcss-modules-extract-imports: 3.0.0(postcss@8.4.24)
       postcss-modules-local-by-default: 4.0.3(postcss@8.4.24)
       postcss-modules-scope: 3.0.0(postcss@8.4.24)
       postcss-modules-values: 4.0.0(postcss@8.4.24)
       postcss-value-parser: 4.2.0
       schema-utils: 3.3.0
       semver: 7.5.3
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /css.escape@1.5.1:
     resolution: {integrity: sha512-YUifsXXuknHlUsmlgyY0PKzgPOr7/FjCePfHNt0jxm83wHZi44VDMQ7/fGNkjY3/jV1MC+1CmZbaHzugyeRtpg==}
     dev: true
 
   /cssesc@3.0.0:
@@ -3005,21 +2997,14 @@
       whatwg-url: 8.7.0
     dev: true
 
   /dataloader@1.4.0:
     resolution: {integrity: sha512-68s5jYdlvasItOJnCuI2Q9s4q98g0pCyL3HrcKJu8KNugUl8ahgmZYg38ysLTgQjjXX3H8CJLkAvWrclWfcalw==}
     dev: true
 
-  /date-time@3.1.0:
-    resolution: {integrity: sha512-uqCUKXE5q1PNBXjPqvwhwJf9SwMoAHBgWJ6DcrnS5o+W2JOiIILl0JEdVD8SGujrNS02GGxgwAg2PN2zONgtjg==}
-    engines: {node: '>=6'}
-    dependencies:
-      time-zone: 1.0.0
-    dev: true
-
   /debug@4.3.4:
     resolution: {integrity: sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==}
     engines: {node: '>=6.0'}
     peerDependencies:
       supports-color: '*'
     peerDependenciesMeta:
       supports-color:
@@ -3320,42 +3305,42 @@
       '@esbuild/netbsd-x64': 0.17.19
       '@esbuild/openbsd-x64': 0.17.19
       '@esbuild/sunos-x64': 0.17.19
       '@esbuild/win32-arm64': 0.17.19
       '@esbuild/win32-ia32': 0.17.19
       '@esbuild/win32-x64': 0.17.19
 
-  /esbuild@0.18.10:
-    resolution: {integrity: sha512-33WKo67auOXzZHBY/9DTJRo7kIvfU12S+D4sp2wIz39N88MDIaCGyCwbW01RR70pK6Iya0I74lHEpyLfFqOHPA==}
+  /esbuild@0.18.11:
+    resolution: {integrity: sha512-i8u6mQF0JKJUlGR3OdFLKldJQMMs8OqM9Cc3UCi9XXziJ9WERM5bfkHaEAy0YAvPRMgqSW55W7xYn84XtEFTtA==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
     optionalDependencies:
-      '@esbuild/android-arm': 0.18.10
-      '@esbuild/android-arm64': 0.18.10
-      '@esbuild/android-x64': 0.18.10
-      '@esbuild/darwin-arm64': 0.18.10
-      '@esbuild/darwin-x64': 0.18.10
-      '@esbuild/freebsd-arm64': 0.18.10
-      '@esbuild/freebsd-x64': 0.18.10
-      '@esbuild/linux-arm': 0.18.10
-      '@esbuild/linux-arm64': 0.18.10
-      '@esbuild/linux-ia32': 0.18.10
-      '@esbuild/linux-loong64': 0.18.10
-      '@esbuild/linux-mips64el': 0.18.10
-      '@esbuild/linux-ppc64': 0.18.10
-      '@esbuild/linux-riscv64': 0.18.10
-      '@esbuild/linux-s390x': 0.18.10
-      '@esbuild/linux-x64': 0.18.10
-      '@esbuild/netbsd-x64': 0.18.10
-      '@esbuild/openbsd-x64': 0.18.10
-      '@esbuild/sunos-x64': 0.18.10
-      '@esbuild/win32-arm64': 0.18.10
-      '@esbuild/win32-ia32': 0.18.10
-      '@esbuild/win32-x64': 0.18.10
+      '@esbuild/android-arm': 0.18.11
+      '@esbuild/android-arm64': 0.18.11
+      '@esbuild/android-x64': 0.18.11
+      '@esbuild/darwin-arm64': 0.18.11
+      '@esbuild/darwin-x64': 0.18.11
+      '@esbuild/freebsd-arm64': 0.18.11
+      '@esbuild/freebsd-x64': 0.18.11
+      '@esbuild/linux-arm': 0.18.11
+      '@esbuild/linux-arm64': 0.18.11
+      '@esbuild/linux-ia32': 0.18.11
+      '@esbuild/linux-loong64': 0.18.11
+      '@esbuild/linux-mips64el': 0.18.11
+      '@esbuild/linux-ppc64': 0.18.11
+      '@esbuild/linux-riscv64': 0.18.11
+      '@esbuild/linux-s390x': 0.18.11
+      '@esbuild/linux-x64': 0.18.11
+      '@esbuild/netbsd-x64': 0.18.11
+      '@esbuild/openbsd-x64': 0.18.11
+      '@esbuild/sunos-x64': 0.18.11
+      '@esbuild/win32-arm64': 0.18.11
+      '@esbuild/win32-ia32': 0.18.11
+      '@esbuild/win32-x64': 0.18.11
     dev: true
 
   /escalade@3.1.1:
     resolution: {integrity: sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==}
     engines: {node: '>=6'}
 
   /escape-string-regexp@1.0.5:
@@ -3439,19 +3424,14 @@
 
   /estree-walker@3.0.3:
     resolution: {integrity: sha512-7RUKfXgSMMkzt6ZuXmqapOurLGPPfgj6l9uRZ7lRGolvk0y2yocc35LdcxKC5PQZdn2DMqioAQ2NoWcrTKmm6g==}
     dependencies:
       '@types/estree': 1.0.1
     dev: false
 
-  /esutils@2.0.3:
-    resolution: {integrity: sha512-kVscqXk4OCp68SZ0dkgEKVi6/8ij300KBWTJq32P/dYeWTSwK41WyTxalN1eRmA5Z9UU/LX9D7FWSmV9SAYx6g==}
-    engines: {node: '>=0.10.0'}
-    dev: true
-
   /events@3.3.0:
     resolution: {integrity: sha512-mQw+2fkQbALzQ7V0MY0IqdnXNOeTtP4r0lN9z7AAawCXgqea7bDii20AYrIBrFd/Hx0M2Ocz6S111CaFkUcb0Q==}
     engines: {node: '>=0.8.x'}
 
   /execa@5.1.1:
     resolution: {integrity: sha512-8uSpZZocAZRBAPIEINJj3Lo9HyGitllczc27Eh5YYojjMFMn8yHMDMaUHE2Jqfq05D/wucwI4JGURyXt1vchyg==}
     engines: {node: '>=10'}
@@ -3515,18 +3495,14 @@
       iconv-lite: 0.4.24
       tmp: 0.0.33
     dev: true
 
   /fast-deep-equal@3.1.3:
     resolution: {integrity: sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==}
 
-  /fast-diff@1.3.0:
-    resolution: {integrity: sha512-VxPP4NqbUjj6MaAOafWeUn2cXWLcCtljklUtZf0Ind4XQ+QPtmA0b18zZy0jIQx+ExRVCR/ZQpBmik5lXshNsw==}
-    dev: true
-
   /fast-glob@3.2.12:
     resolution: {integrity: sha512-DVj4CQIYYow0BlaelwK1pHl5n5cRSJfM60UA0zK891sVInoPri2Ekj7+e1CT3/3qxXenpI+nBBmQAcJPJgaj4w==}
     engines: {node: '>=8.6.0'}
     dependencies:
       '@nodelib/fs.stat': 2.0.5
       '@nodelib/fs.walk': 1.2.8
       glob-parent: 5.1.2
@@ -3556,15 +3532,15 @@
     resolution: {integrity: sha512-/aMOAYEFXDdjG0wytpTL5YQLfZnnTmLNjn+AIrJ/6HVnTfDqLsVKUUwkDf4I4kgex36BvjuXEn/TX9B/1ESyqQ==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 2.7.1
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /fill-range@7.0.1:
     resolution: {integrity: sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==}
     engines: {node: '>=8'}
     dependencies:
       to-regex-range: 5.0.1
@@ -3825,16 +3801,16 @@
     engines: {node: '>=6.0'}
     dependencies:
       js-yaml: 3.14.1
       kind-of: 6.0.3
       section-matter: 1.0.0
       strip-bom-string: 1.0.0
 
-  /happy-dom@9.20.3:
-    resolution: {integrity: sha512-eBsgauT435fXFvQDNcmm5QbGtYzxEzOaX35Ia+h6yP/wwa4xSWZh1CfP+mGby8Hk6Xu59mTkpyf72rUXHNxY7A==}
+  /happy-dom@10.0.7:
+    resolution: {integrity: sha512-NRMRGQcJ3BuIikmzXjrVJdV72ZbEeljE0cES2zQ2NomUFytsMGJCKZ2o3TjMwoCMh5yWY93DUMjR9PYr5WW0ug==}
     dependencies:
       css.escape: 1.5.1
       entities: 4.5.0
       iconv-lite: 0.6.3
       webidl-conversions: 7.0.0
       whatwg-encoding: 2.0.0
       whatwg-mimetype: 3.0.0
@@ -4366,19 +4342,14 @@
     resolution: {integrity: sha512-QAdOptna2NYiSSpv0O/BwoHBSmz4YhpzJHyi+fnMRTXFjp7B8i/YG5Z8IfusxB1ufjcD2Sre1F3R+nX3fvy7gg==}
     hasBin: true
     dev: false
 
   /jquery@3.7.0:
     resolution: {integrity: sha512-umpJ0/k8X0MvD1ds0P9SfowREz2LenHsQaxSohMZ5OMNEU2r0tf8pdeEFTHMFxWVxKNyU9rTtK3CWzUCTKJUeQ==}
 
-  /js-string-escape@1.0.1:
-    resolution: {integrity: sha512-Smw4xcfIQ5LVjAOuJCvN/zIodzA/BBSsluuoSykP+lUvScIi4U6RJLfwHet5cxFnCswUjISV8oAXaqaJDY3chg==}
-    engines: {node: '>= 0.8'}
-    dev: true
-
   /js-tokens@4.0.0:
     resolution: {integrity: sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==}
 
   /js-yaml@3.14.1:
     resolution: {integrity: sha512-okMH7OXXJ7YrN9Ok3/SXrnu4iX9yOk+25nqX4imS2npuvTYDmo/QEZoqwZkYaIDk3jVvBOTOIEgEhaLOynBS9g==}
     hasBin: true
     dependencies:
@@ -4452,15 +4423,15 @@
     peerDependencies:
       webpack: '*'
     peerDependenciesMeta:
       webpack:
         optional: true
     dependencies:
       '@types/webpack-sources': 0.1.9
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
       webpack-sources: 1.4.3
     dev: true
 
   /lilconfig@2.1.0:
     resolution: {integrity: sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==}
     engines: {node: '>=10'}
     dev: false
@@ -4607,21 +4578,14 @@
     resolution: {integrity: sha512-WWC0ZuMzCyDHYCasEGs4IPvLyTGftYwh6wIEOULOF0HXcqZlhwRzrK0w2VUlxWA98xnvb/jszw4ZSkJ6ADpM6Q==}
     engines: {node: '>=0.10.0'}
     dev: false
 
   /markdown-table@3.0.3:
     resolution: {integrity: sha512-Z1NL3Tb1M9wH4XESsCDEksWoKTdlUafKc4pt0GRwjUyXaCFZ+dc3g2erqB6zm3szA2IUSi7VnPI+o/9jnxh9hw==}
 
-  /md5-hex@3.0.1:
-    resolution: {integrity: sha512-BUiRtTtV39LIJwinWBjqVsU9xhdnz7/i889V859IBFpuqGAj6LuOvHv5XLbgZ2R7ptJoJaEcxkv88/h25T7Ciw==}
-    engines: {node: '>=8'}
-    dependencies:
-      blueimp-md5: 2.19.0
-    dev: true
-
   /mdast-util-definitions@5.1.2:
     resolution: {integrity: sha512-8SVPMuHqlPME/z3gqVwWY4zVXn8lqKv/pAhC57FuJ40ImXyBpmO5ukh98zB2v7Blql2FiHjHv9LVztSIqjY+MA==}
     dependencies:
       '@types/mdast': 3.0.11
       '@types/unist': 2.0.6
       unist-util-visit: 4.1.2
 
@@ -5179,15 +5143,15 @@
     resolution: {integrity: sha512-Ac4s+xhVbqlyhXS5J/Vh/QXUz3ycXlCqoCPpg0vdfhsIBH9eg/It/9L1r1XhSCH737M1lqcWnMuWL13zcygn5A==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.4.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
       webpack-sources: 1.4.3
     dev: true
 
   /minimatch@3.1.2:
     resolution: {integrity: sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==}
     dependencies:
       brace-expansion: 1.1.11
@@ -5777,21 +5741,21 @@
     dev: true
 
   /prettier@2.8.8:
     resolution: {integrity: sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==}
     engines: {node: '>=10.13.0'}
     hasBin: true
 
-  /pretty-format@27.5.1:
-    resolution: {integrity: sha512-Qb1gy5OrP5+zDf2Bvnzdl3jsTf1qXVMazbvCoKhtKqVs4/YK4ozX4gKQJJVyNe+cajNPn0KoC0MC3FUmaHWEmQ==}
-    engines: {node: ^10.13.0 || ^12.13.0 || ^14.15.0 || >=15.0.0}
+  /pretty-format@29.5.0:
+    resolution: {integrity: sha512-V2mGkI31qdttvTFX7Mt4efOqHXqJWMu4/r66Xh3Z3BwZaPfPJgp6/gbwoujRpPUtfEF6AUUWx3Jim3GCw5g/Qw==}
+    engines: {node: ^14.15.0 || ^16.10.0 || >=18.0.0}
     dependencies:
-      ansi-regex: 5.0.1
+      '@jest/schemas': 29.4.3
       ansi-styles: 5.2.0
-      react-is: 17.0.2
+      react-is: 18.2.0
     dev: true
 
   /pretty-format@3.8.0:
     resolution: {integrity: sha512-WuxUnVtlWL1OfZFQFuqvnvs6MiAGk9UNsBostyBOB0Is9wb5uRESevA6rnl/rkksXaGX3GzZhPup5d6Vp1nFew==}
     dev: false
 
   /prismjs@1.29.0:
@@ -5851,29 +5815,29 @@
     resolution: {integrity: sha512-ZnScIV3ag9A4wPX/ZayxL/jZH+euYb6FcUinPcgiQW0+UBtEv0O6Q3lGd3cqJ+GHH+rksEv3Pj99oxJ3u3VIKA==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /react-dom@18.2.0(react@18.2.0):
     resolution: {integrity: sha512-6IMTriUmvsjHUjNtEDudZfuDQUoWXVxKHhlEGSk81n4YFS+r/Kl99wXiwlVXtPBtJenozv2P+hxDsw9eA7Xo6g==}
     peerDependencies:
       react: ^18.2.0
     dependencies:
       loose-envify: 1.4.0
       react: 18.2.0
       scheduler: 0.23.0
     dev: false
 
-  /react-is@17.0.2:
-    resolution: {integrity: sha512-w2GsyukL62IJnlaff/nRegPQR94C/XXamvMWmSHRJ4y7Ts/4ocGRmTHvOs8PSE6pB3dWOrD/nueuU5sduBsQ4w==}
+  /react-is@18.2.0:
+    resolution: {integrity: sha512-xWGDIW6x921xtzPkhiULtthJHoJvBbF3q26fzloPCK0hsvxtPVelvftw3zjbHWSkR2km9Z+4uxbDDK/6Zw9B8w==}
     dev: true
 
   /react@18.2.0:
     resolution: {integrity: sha512-/3IjMdb2L9QbBdWiW5e3P2/npwMBaU9mHCSCUzNln0ZCYbcfTsGbTJrU/kGemdH2IWmB2ioZ+zkxtmq6g09fGQ==}
     engines: {node: '>=0.10.0'}
     dependencies:
       loose-envify: 1.4.0
@@ -6340,15 +6304,15 @@
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       data-urls: 2.0.0
       iconv-lite: 0.6.3
       loader-utils: 2.0.4
       schema-utils: 2.7.1
       source-map: 0.6.1
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /source-map-support@0.5.21:
     resolution: {integrity: sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==}
     dependencies:
       buffer-from: 1.1.2
       source-map: 0.6.1
@@ -6531,15 +6495,15 @@
     resolution: {integrity: sha512-Z0gYUJmzZ6ZdRUqpg1r8GsaFKypE+3xAzuFeMuoHgjc9KZv3wMyCRjQIWEbhoFSq7+7yoHXySDJyyWQaPajeiQ==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /style-to-object@0.4.1:
     resolution: {integrity: sha512-HFpbb5gr2ypci7Qw+IOhnP2zOU7e77b+rzM+wTzXzfi1PrtBCX0E7Pk4wL4iTLnhzZ+JgEGAhX81ebTg/aYjQw==}
     dependencies:
       inline-style-parser: 0.1.1
     dev: false
@@ -6594,15 +6558,15 @@
   /svg-url-loader@6.0.0(webpack@5.88.0):
     resolution: {integrity: sha512-Qr5SCKxyxKcRnvnVrO3iQj9EX/v40UiGEMshgegzV7vpo3yc+HexELOdtWcA3MKjL8IyZZ1zOdcILmDEa/8JJQ==}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       file-loader: 6.0.0(webpack@5.88.0)
       loader-utils: 2.0.4
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /synckit@0.8.5:
     resolution: {integrity: sha512-L1dapNV6vu2s/4Sputv8xGsCdAVlb5nRDMFU/E27D44l5U6cw1g0dGd45uLc+OXjNMmF4ntiMdCimzcjFKQI8Q==}
     engines: {node: ^14.18.0 || >=16.0.0}
     dependencies:
       '@pkgr/utils': 2.4.1
@@ -6672,21 +6636,21 @@
       find-cache-dir: 3.3.2
       jest-worker: 26.6.2
       p-limit: 3.1.0
       schema-utils: 3.3.0
       serialize-javascript: 5.0.1
       source-map: 0.6.1
       terser: 5.18.1
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
       webpack-sources: 1.4.3
     transitivePeerDependencies:
       - bluebird
     dev: true
 
-  /terser-webpack-plugin@5.3.9(esbuild@0.18.10)(webpack@5.88.0):
+  /terser-webpack-plugin@5.3.9(esbuild@0.18.11)(webpack@5.88.0):
     resolution: {integrity: sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       '@swc/core': '*'
       esbuild: '*'
       uglify-js: '*'
       webpack: ^5.1.0
@@ -6695,20 +6659,20 @@
         optional: true
       esbuild:
         optional: true
       uglify-js:
         optional: true
     dependencies:
       '@jridgewell/trace-mapping': 0.3.18
-      esbuild: 0.18.10
+      esbuild: 0.18.11
       jest-worker: 27.5.1
       schema-utils: 3.3.0
       serialize-javascript: 6.0.1
       terser: 5.18.1
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /terser@5.18.1:
     resolution: {integrity: sha512-j1n0Ao919h/Ai5r43VAnfV/7azUYW43GPxK7qSATzrsERfW7+y2QW9Cp9ufnRF5CQUWbnLSo7UJokSWCqg4tsQ==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
@@ -6727,19 +6691,14 @@
 
   /thenify@3.3.1:
     resolution: {integrity: sha512-RVZSIV5IG10Hk3enotrhvz0T9em6cyHBLkH/YAZuKqd8hRkKhSfCGIcP2KUY0EPxndzANBmNllzWPwak+bheSw==}
     dependencies:
       any-promise: 1.3.0
     dev: false
 
-  /time-zone@1.0.0:
-    resolution: {integrity: sha512-TIsDdtKo6+XrPtiTm1ssmMngN1sAhyKnTO2kunQWqNPWIVvCm15Wmw4SWInwTVgJ5u/Tr04+8Ei9TNcw4x4ONA==}
-    engines: {node: '>=4'}
-    dev: true
-
   /tinybench@2.5.0:
     resolution: {integrity: sha512-kRwSG8Zx4tjF9ZiyH4bhaebu+EDz1BOx9hOigYHlUW4xxI/wKIUQUqo018UlU4ar6ATPBsaMrdbKZ+tmPdohFA==}
     dev: true
 
   /tinypool@0.5.0:
     resolution: {integrity: sha512-paHQtnrlS1QZYKF/GnLoOM/DN9fqaGOFbCbxzAhwniySnzl9Ebk8w73/dd34DAhe/obUbPAOldTyYXQZxnPBPQ==}
     engines: {node: '>=14.0.0'}
@@ -6856,16 +6815,16 @@
     resolution: {integrity: sha512-KjZypGq+I/H7HI5HlOoGHkWUUGq+Q0TPhQurLbyrVrvnKTBgzLhIJ7j6J/XTQOi0d1RjyZ0wdas8bKs2p0x3Ng==}
     dependencies:
       call-bind: 1.0.2
       for-each: 0.3.3
       is-typed-array: 1.1.10
     dev: true
 
-  /typescript@5.1.3:
-    resolution: {integrity: sha512-XH627E9vkeqhlZFQuL+UsyAXEnibT0kWR2FWONlr4sTjvxyJYnyefgrkyECLzM5NenmKzRAy2rR/OlYLA1HkZw==}
+  /typescript@5.1.6:
+    resolution: {integrity: sha512-zaWCozRZ6DLEWAWFrVDz1H6FVXzUSfTy5FUMWsQlU8Ym5JP9eO4xkTIROFCQvhQf61z6O/G6ugw3SgAnvvm+HA==}
     engines: {node: '>=14.17'}
     hasBin: true
 
   /ufo@1.1.2:
     resolution: {integrity: sha512-TrY6DsjTQQgyS3E3dBaOXf0TpPD8u9FVrVYmKVegJuFw51n/YB9XPt+U6ydzFG5ZIN7+DIjPbNmXoBj9esYhgQ==}
     dev: true
 
@@ -7007,15 +6966,15 @@
       file-loader:
         optional: true
     dependencies:
       file-loader: 6.0.0(webpack@5.88.0)
       loader-utils: 2.0.4
       mime-types: 2.1.35
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /url-parse@1.4.7:
     resolution: {integrity: sha512-d3uaVyzDB9tQoSXFvuSUNFibTd9zxd2bkVrDRvF5TmvWWQwqE4lgYJ5m+x1DbecWkw+LK4RNl2CU1hHuOKPVlg==}
     dependencies:
       querystringify: 2.2.0
       requires-port: 1.0.0
@@ -7064,16 +7023,16 @@
     resolution: {integrity: sha512-r7qlzkgErKjobAmyNIkkSpizsFPYiUPuJb5pNW1RB4JcYVZhs4lIbVqk8XPk033CV/1z8ss5pkax8SuhGpcG8g==}
     dependencies:
       '@types/unist': 2.0.6
       is-buffer: 2.0.5
       unist-util-stringify-position: 3.0.3
       vfile-message: 3.1.4
 
-  /vite-node@0.32.2(@types/node@18.0.0):
-    resolution: {integrity: sha512-dTQ1DCLwl2aEseov7cfQ+kDMNJpM1ebpyMMMwWzBvLbis8Nla/6c9WQcqpPssTwS6Rp/+U6KwlIj8Eapw4bLdA==}
+  /vite-node@0.32.4(@types/node@18.0.0):
+    resolution: {integrity: sha512-L2gIw+dCxO0LK14QnUMoqSYpa9XRGnTTTDjW2h19Mr+GR0EFj4vx52W41gFXfMLqpA00eK4ZjOVYo1Xk//LFEw==}
     engines: {node: '>=v14.18.0'}
     hasBin: true
     dependencies:
       cac: 6.7.14
       debug: 4.3.4
       mlly: 1.4.0
       pathe: 1.1.1
@@ -7127,16 +7086,16 @@
       vite: ^3.0.0 || ^4.0.0
     peerDependenciesMeta:
       vite:
         optional: true
     dependencies:
       vite: 4.3.9(@types/node@18.0.0)
 
-  /vitest@0.32.2(happy-dom@9.20.3):
-    resolution: {integrity: sha512-hU8GNNuQfwuQmqTLfiKcqEhZY72Zxb7nnN07koCUNmntNxbKQnVbeIS6sqUgR3eXSlbOpit8+/gr1KpqoMgWCQ==}
+  /vitest@0.32.4(happy-dom@10.0.7):
+    resolution: {integrity: sha512-3czFm8RnrsWwIzVDu/Ca48Y/M+qh3vOnF16czJm98Q/AN1y3B6PBsyV8Re91Ty5s7txKNjEhpgtGPcfdbh2MZg==}
     engines: {node: '>=v14.18.0'}
     hasBin: true
     peerDependencies:
       '@edge-runtime/vm': '*'
       '@vitest/browser': '*'
       '@vitest/ui': '*'
       happy-dom: '*'
@@ -7161,36 +7120,35 @@
         optional: true
       webdriverio:
         optional: true
     dependencies:
       '@types/chai': 4.3.5
       '@types/chai-subset': 1.3.3
       '@types/node': 18.0.0
-      '@vitest/expect': 0.32.2
-      '@vitest/runner': 0.32.2
-      '@vitest/snapshot': 0.32.2
-      '@vitest/spy': 0.32.2
-      '@vitest/utils': 0.32.2
+      '@vitest/expect': 0.32.4
+      '@vitest/runner': 0.32.4
+      '@vitest/snapshot': 0.32.4
+      '@vitest/spy': 0.32.4
+      '@vitest/utils': 0.32.4
       acorn: 8.9.0
       acorn-walk: 8.2.0
       cac: 6.7.14
       chai: 4.3.7
-      concordance: 5.0.4
       debug: 4.3.4
-      happy-dom: 9.20.3
+      happy-dom: 10.0.7
       local-pkg: 0.4.3
       magic-string: 0.30.0
       pathe: 1.1.1
       picocolors: 1.0.0
       std-env: 3.3.3
       strip-literal: 1.0.1
       tinybench: 2.5.0
       tinypool: 0.5.0
       vite: 4.3.9(@types/node@18.0.0)
-      vite-node: 0.32.2(@types/node@18.0.0)
+      vite-node: 0.32.4(@types/node@18.0.0)
       why-is-node-running: 2.2.2
     transitivePeerDependencies:
       - less
       - sass
       - stylus
       - sugarss
       - supports-color
@@ -7303,15 +7261,15 @@
       colorette: 2.0.20
       commander: 7.2.0
       cross-spawn: 7.0.3
       fastest-levenshtein: 1.0.16
       import-local: 3.1.0
       interpret: 2.2.0
       rechoir: 0.7.1
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
       webpack-merge: 5.9.0
     dev: true
 
   /webpack-merge@5.9.0:
     resolution: {integrity: sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==}
     engines: {node: '>=10.0.0'}
     dependencies:
@@ -7327,15 +7285,15 @@
     dev: true
 
   /webpack-sources@3.2.3:
     resolution: {integrity: sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==}
     engines: {node: '>=10.13.0'}
     dev: true
 
-  /webpack@5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0):
+  /webpack@5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0):
     resolution: {integrity: sha512-O3jDhG5e44qIBSi/P6KpcCcH7HD+nYIHVBhdWFxcLOcIGN8zGo5nqF3BjyNCxIh4p1vFdNnreZv2h2KkoAw3lw==}
     engines: {node: '>=10.13.0'}
     hasBin: true
     peerDependencies:
       webpack-cli: '*'
     peerDependenciesMeta:
       webpack-cli:
@@ -7358,29 +7316,24 @@
       graceful-fs: 4.2.11
       json-parse-even-better-errors: 2.3.1
       loader-runner: 4.3.0
       mime-types: 2.1.35
       neo-async: 2.6.2
       schema-utils: 3.3.0
       tapable: 2.2.1
-      terser-webpack-plugin: 5.3.9(esbuild@0.18.10)(webpack@5.88.0)
+      terser-webpack-plugin: 5.3.9(esbuild@0.18.11)(webpack@5.88.0)
       watchpack: 2.4.0
       webpack-cli: 4.10.0(webpack@5.88.0)
       webpack-sources: 3.2.3
     transitivePeerDependencies:
       - '@swc/core'
       - esbuild
       - uglify-js
     dev: true
 
-  /well-known-symbols@2.0.0:
-    resolution: {integrity: sha512-ZMjC3ho+KXo0BfJb7JgtQ5IBuvnShdlACNkKkdsqBmYw3bPAaJfPeYUo6tLUaT5tG/Gkh7xkpBhKRQ9e7pyg9Q==}
-    engines: {node: '>=6'}
-    dev: true
-
   /whatwg-encoding@2.0.0:
     resolution: {integrity: sha512-p41ogyeMUrw3jWclHWTQg1k05DSVXPLcVxRTYsXUk+ZooOCZLcoYgPZ/HL/D/N+uQPOtcp1me1WhBEaX02mhWg==}
     engines: {node: '>=12'}
     dependencies:
       iconv-lite: 0.6.3
     dev: true
 
@@ -7482,15 +7435,15 @@
     resolution: {integrity: sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.10)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.11)(webpack-cli@4.10.0)
     dev: true
 
   /wrap-ansi@6.2.0:
     resolution: {integrity: sha512-r6lPcBGxZXlIcymEu7InxDMhdW0KDxpLgoFLcguasxCaJ/SOIZwINatK9KY/tf+ZrlywOKU0UDj3ATXUBfxJXA==}
     engines: {node: '>=8'}
     dependencies:
       ansi-styles: 4.3.0
```

### Comparing `anywidget-0.6.1/anywidget/_descriptor.py` & `anywidget-0.6.2/anywidget/_descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -480,15 +480,17 @@
         # provide an API for the user to customize serialization
         return asdict
 
     if _is_traitlets_object(obj):
         return _get_traitlets_state
 
     if _is_pydantic_model(obj):
-        return _get_pydantic_state
+        if hasattr(obj, "model_dump"):
+            return _get_pydantic_state_v2
+        return _get_pydantic_state_v1
 
     if _is_msgspec_struct(obj):
         return _get_msgspec_state
 
     # pickle protocol ... probably not type-safe enough for our purposes
     # https://docs.python.org/3/library/pickle.html#object.__getstate__
     # if hasattr(type(obj), "__getstate__"):
@@ -634,24 +636,29 @@
 
 def _is_pydantic_model(obj: Any) -> TypeGuard[pydantic.BaseModel]:
     """Return `True` if an object is an instance of pydantic.BaseModel."""
     pydantic = sys.modules.get("pydantic")
     return isinstance(obj, pydantic.BaseModel) if pydantic is not None else False
 
 
-def _get_pydantic_state(obj: pydantic.BaseModel) -> Serializable:
+def _get_pydantic_state_v1(obj: pydantic.BaseModel) -> Serializable:
     """Get the state of a pydantic BaseModel instance.
 
     To take advantage of pydantic's support for custom encoders (with json_encoders)
-    we call obj.json() here, and then cast back to a dict (which is what the comm
-    expects.)
+    we call obj.json() here, and then cast back to a dict (which is what
+    the comm expects).
     """
     return json.loads(obj.json())
 
 
+def _get_pydantic_state_v2(obj: pydantic.BaseModel) -> Serializable:
+    """Get the state of a pydantic (v2) BaseModel instance."""
+    return obj.model_dump(mode="json")
+
+
 # ------------- msgspec support --------------
 
 
 def _is_msgspec_struct(obj: Any) -> TypeGuard[msgspec.Struct]:
     """Return `True` if an object is an instance of msgspec.Struct."""
     msgspec = sys.modules.get("msgspec")
     return isinstance(obj, msgspec.Struct) if msgspec is not None else False
```

### Comparing `anywidget-0.6.1/anywidget/_file_contents.py` & `anywidget-0.6.2/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/anywidget/_protocols.py` & `anywidget-0.6.2/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/anywidget/_util.py` & `anywidget-0.6.2/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/anywidget/experimental.py` & `anywidget-0.6.2/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/anywidget/widget.py` & `anywidget-0.6.2/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/anywidget/labextension/package.json` & `anywidget-0.6.2/anywidget/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9507211538461539%*

 * *Differences: {"'devDependencies'": "{'@jupyter-widgets/base-manager': '^1.0.6'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.cc3d041878be8537a74e.js'}}",*

 * * "'version'": "'0.6.2'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "Trevor Manz",
     "dependencies": {
         "@anywidget/types": "workspace:~",
         "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
-        "@jupyter-widgets/base-manager": "^1.0.5",
+        "@jupyter-widgets/base-manager": "^1.0.6",
         "@jupyterlab/builder": "^3.6.5"
     },
     "exports": {
         ".": "./dist/index.js",
         "./types": {
             "import": "./dist/types.mjs",
             "require": "./dist/types.cjs",
@@ -23,15 +23,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2cf77409ad03a77cbd09.js"
+            "load": "static/remoteEntry.cc3d041878be8537a74e.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -45,9 +45,9 @@
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs",
         "typecheck": "tsc --noEmit"
     },
     "type": "module",
-    "version": "0.6.1"
+    "version": "0.6.2"
 }
```

### Comparing `anywidget-0.6.1/anywidget/labextension/static/138.6d69013365e0a65d34c8.js` & `anywidget-0.6.2/anywidget/labextension/static/138.842852ea2bafcf459e69.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -117,11 +117,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.6.1/anywidget/labextension/static/326.44c2db4e788cbf8b5f08.js` & `anywidget-0.6.2/anywidget/labextension/static/326.8293ec79dbdf802e77d1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -135,11 +135,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.6.1/anywidget/labextension/static/remoteEntry.2cf77409ad03a77cbd09.js` & `anywidget-0.6.2/anywidget/labextension/static/remoteEntry.cc3d041878be8537a74e.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, g = {
+    var e, r, t, n, o, a, i, u, f, l, s, d, p, c, h, v, g = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,112 +20,112 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        m = {};
+        b = {};
 
-    function y(e) {
-        var r = m[e];
+    function m(e) {
+        var r = b[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = b[e] = {
             exports: {}
         };
-        return g[e](t, t.exports, y), t.exports
+        return g[e](t, t.exports, m), t.exports
     }
-    y.m = g, y.c = m, y.n = e => {
+    m.m = g, m.c = b, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return y.d(r, {
+        return m.d(r, {
             a: r
         }), r
-    }, y.d = (e, r) => {
-        for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
+    }, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        138: "6d69013365e0a65d34c8",
-        326: "44c2db4e788cbf8b5f08"
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
+        138: "842852ea2bafcf459e69",
+        326: "8293ec79dbdf802e77d1"
     } [e] + ".js?v=" + {
-        138: "6d69013365e0a65d34c8",
-        326: "44c2db4e788cbf8b5f08"
-    } [e], y.g = function() {
+        138: "842852ea2bafcf459e69",
+        326: "8293ec79dbdf802e77d1"
+    } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", y.l = (t, n, o, a) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var s = f[l];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, y.r = e => {
+    }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        y.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        y.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                y.o(y.S, t) || (y.S[t] = {});
-                var a = y.S[t],
+                m.o(m.S, t) || (m.S[t] = {});
+                var a = m.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => y.e(138).then((() => () => y(138))),
+                        get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.6.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.6.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        y.g.importScripts && (e = y.g.location + "");
-        var r = y.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), y.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -148,130 +148,130 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
-                } else if (l)
-                    if (d == f)
+            for (var i = 0, u = 1, f = !0;; u++, i++) {
+                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
+                    if (!f || "u" != d) return !1
+                } else if (f)
+                    if (d == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (f = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    f = !1, u--
                 } else {
-                    if (u <= n || f < d != o) return !1;
-                    l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                    if (u <= n || s < d != o) return !1;
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = y.S[e];
-        if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(l(e, t, o, n)), d(e[t][o])
-    }, f = e => {
+        return a(n, o) || s(f(e, t, o, n)), d(e[t][o])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
-        var a = y.I(r);
-        return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
+        var a = m.I(r);
+        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, h = {
         395: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, v = {
         326: [395]
-    }, y.f.consumes = (e, r) => {
-        y.o(v, e) && v[e].forEach((e => {
-            if (y.o(c, e)) return r.push(c[e]);
+    }, m.f.consumes = (e, r) => {
+        m.o(v, e) && v[e].forEach((e => {
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    c[e] = 0, y.m[e] = t => {
-                        delete y.c[e], t.exports = r()
+                    c[e] = 0, m.m[e] = t => {
+                        delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], y.m[e] = t => {
-                        throw delete y.c[e], r
+                    delete c[e], m.m[e] = t => {
+                        throw delete m.c[e], r
                     }
                 };
             try {
                 var o = h[e]();
                 o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        y.f.j = (r, t) => {
-            var n = y.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = y.p + y.u(r),
+                    var a = m.p + m.u(r),
                         i = new Error;
-                    y.l(a, (t => {
-                        if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    m.l(a, (t => {
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) y.o(i, n) && (y.m[n] = i[n]);
-                    u && u(y)
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                    u && u(m)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var b = y(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
+    var y = m(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
 })();
```

### Comparing `anywidget-0.6.1/anywidget/nbextension/index.js` & `anywidget-0.6.2/anywidget/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.6.1";
+var version = "0.6.2";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.6.1/docs/README.md` & `anywidget-0.6.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/astro.config.js` & `anywidget-0.6.2/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/package.json` & `anywidget-0.6.2/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/anywidget-overview.png` & `anywidget-0.6.2/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/banner-dark.png` & `anywidget-0.6.2/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/banner-light.png` & `anywidget-0.6.2/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/banner-minimal.png` & `anywidget-0.6.2/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/client-js-diagram.png` & `anywidget-0.6.2/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/default-og-image.png` & `anywidget-0.6.2/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/favicon.svg` & `anywidget-0.6.2/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/public/widget-overview.png` & `anywidget-0.6.2/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/scripts/ipynb.mjs` & `anywidget-0.6.2/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/scripts/utils.mjs` & `anywidget-0.6.2/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/consts.ts` & `anywidget-0.6.2/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/CodeHero.astro` & `anywidget-0.6.2/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/CounterButton.astro` & `anywidget-0.6.2/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/HeadCommon.astro` & `anywidget-0.6.2/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/HeadSEO.astro` & `anywidget-0.6.2/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Hero.astro` & `anywidget-0.6.2/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.6.2/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.6.2/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.6.2/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/Header.astro` & `anywidget-0.6.2/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/HeaderButton.css` & `anywidget-0.6.2/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.6.2/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.6.2/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/Search.css` & `anywidget-0.6.2/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/Search.tsx` & `anywidget-0.6.2/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.6.2/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.6.2/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.6.2/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.6.2/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.6.2/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.6.2/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.6.2/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.6.2/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/components/examples/Counter.astro` & `anywidget-0.6.2/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/layouts/MainLayout.astro` & `anywidget-0.6.2/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/layouts/SplashLayout.astro` & `anywidget-0.6.2/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.6.2/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.6.2/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/pages/en/bundling.md` & `anywidget-0.6.2/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/pages/en/experimental.md` & `anywidget-0.6.2/docs/src/pages/en/experimental.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/pages/en/getting-started.mdx` & `anywidget-0.6.2/docs/src/pages/en/getting-started.mdx`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 	let selection = d3.select(el);
 	/* ... */
 }
 ```
 
 The `render` function can also (optionally) return a callback that is executed any time the view is
 removed from the DOM. This feature is useful when dealing with complex event listeners, subscriptions,
-or third-party libraries that require proper teardwon.
+or third-party libraries that require proper teardown.
 
 ```javascript
 /** @param {{ model: DOMWidgetModel, el: HTMLElement }} context */
 export function render({ model, el }) {
 	// Create DOM elements and set up subscribers
 	return () => {
 		// Optionally cleanup
```

### Comparing `anywidget-0.6.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.6.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.6.2/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/styles/index.css` & `anywidget-0.6.2/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/docs/src/styles/theme.css` & `anywidget-0.6.2/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/examples/Counter.ipynb` & `anywidget-0.6.2/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/examples/minimal_example.ipynb` & `anywidget-0.6.2/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/packages/anywidget/CHANGELOG.md` & `anywidget-0.6.2/packages/anywidget/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # anywidget
 
+## 0.6.2
+
+### Patch Changes
+
+- feat(descriptor): Auto-detect and serialize `pydantic` v1 and v2 models ([`518ced9`](https://github.com/manzt/anywidget/commit/518ced9ffae209c06d85d2f0de2ed37d51d67edb))
+
 ## 0.6.1
 
 ### Patch Changes
 
 - feat: Bring back support for Python 3.7 ([#167](https://github.com/manzt/anywidget/pull/167))
 
 ## 0.6.0
```

### Comparing `anywidget-0.6.1/packages/anywidget/build.mjs` & `anywidget-0.6.2/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/packages/anywidget/package.json` & `anywidget-0.6.2/packages/anywidget/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'devDependencies'": "{'@jupyter-widgets/base-manager': '^1.0.6'}", "'version'": "'0.6.2'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "Trevor Manz",
     "dependencies": {
         "@anywidget/types": "workspace:~",
         "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
-        "@jupyter-widgets/base-manager": "^1.0.5",
+        "@jupyter-widgets/base-manager": "^1.0.6",
         "@jupyterlab/builder": "^3.6.5"
     },
     "exports": {
         ".": "./dist/index.js",
         "./types": {
             "import": "./dist/types.mjs",
             "require": "./dist/types.cjs",
@@ -41,9 +41,9 @@
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs",
         "typecheck": "tsc --noEmit"
     },
     "type": "module",
-    "version": "0.6.1"
+    "version": "0.6.2"
 }
```

### Comparing `anywidget-0.6.1/packages/anywidget/__tests__/widget.test.ts` & `anywidget-0.6.2/packages/anywidget/__tests__/widget.test.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/packages/anywidget/src/plugin.js` & `anywidget-0.6.2/packages/anywidget/src/plugin.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/packages/anywidget/src/widget.js` & `anywidget-0.6.2/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/tests/test_descriptor.py` & `anywidget-0.6.2/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/tests/test_experimental.py` & `anywidget-0.6.2/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/tests/test_file_contents.py` & `anywidget-0.6.2/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/tests/test_utils.py` & `anywidget-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/tests/test_widget.py` & `anywidget-0.6.2/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/LICENSE` & `anywidget-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/README.md` & `anywidget-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/pyproject.toml` & `anywidget-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.6.1/PKG-INFO` & `anywidget-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.6.1
+Version: 0.6.2
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```

