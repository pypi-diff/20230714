# Comparing `tmp/clinker-0.0.8.tar.gz` & `tmp/clinker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clinker-0.0.8.tar", last modified: Wed Dec  2 07:46:33 2020, max compression
+gzip compressed data, was "dist/clinker-0.0.9.tar", last modified: Fri Dec  4 05:31:55 2020, max compression
```

## Comparing `clinker-0.0.8.tar` & `clinker-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 07:46:33.971684 clinker-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-12-02 07:46:21.000000 clinker-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4501 2020-12-02 07:46:33.971684 clinker-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3320 2020-12-02 07:46:21.000000 clinker-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 07:46:33.967684 clinker-0.0.8/clinker/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20079 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/align.py
--rw-r--r--   0 runner    (1001) docker     (116)     8067 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/classes.py
--rw-r--r--   0 runner    (1001) docker     (116)     2722 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/formatters.py
--rw-r--r--   0 runner    (1001) docker     (116)     6402 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 07:46:33.967684 clinker-0.0.8/clinker/plot/
--rw-r--r--   0 runner    (1001) docker     (116)     7037 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot/clinker.js
--rw-r--r--   0 runner    (1001) docker     (116)    26841 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot/clustermap.min.js
--rw-r--r--   0 runner    (1001) docker     (116)   267786 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     9097 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot/index.html
--rw-r--r--   0 runner    (1001) docker     (116)     2623 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot/mock.json
--rw-r--r--   0 runner    (1001) docker     (116)     2016 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot/style.css
--rw-r--r--   0 runner    (1001) docker     (116)     3923 2020-12-02 07:46:21.000000 clinker-0.0.8/clinker/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 07:46:33.967684 clinker-0.0.8/clinker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4501 2020-12-02 07:46:33.000000 clinker-0.0.8/clinker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      476 2020-12-02 07:46:33.000000 clinker-0.0.8/clinker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 07:46:33.000000 clinker-0.0.8/clinker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-12-02 07:46:33.000000 clinker-0.0.8/clinker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-02 07:46:33.000000 clinker-0.0.8/clinker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-02 07:46:33.000000 clinker-0.0.8/clinker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-02 07:46:33.971684 clinker-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2020-12-02 07:46:21.000000 clinker-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 05:31:55.062927 clinker-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2020-12-04 05:31:41.000000 clinker-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     4501 2020-12-04 05:31:55.062927 clinker-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3320 2020-12-04 05:31:41.000000 clinker-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 05:31:55.054927 clinker-0.0.9/clinker/
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20079 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/align.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8067 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/classes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2722 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6402 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 05:31:55.062927 clinker-0.0.9/clinker/plot/
+-rw-r--r--   0 runner    (1001) docker     (116)     7037 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot/clinker.js
+-rw-r--r--   0 runner    (1001) docker     (116)    26562 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot/clustermap.min.js
+-rw-r--r--   0 runner    (1001) docker     (116)   267786 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (116)     9097 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot/index.html
+-rw-r--r--   0 runner    (1001) docker     (116)     2623 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot/mock.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2016 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot/style.css
+-rw-r--r--   0 runner    (1001) docker     (116)     3923 2020-12-04 05:31:41.000000 clinker-0.0.9/clinker/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-04 05:31:55.058927 clinker-0.0.9/clinker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4501 2020-12-04 05:31:54.000000 clinker-0.0.9/clinker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      476 2020-12-04 05:31:54.000000 clinker-0.0.9/clinker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-04 05:31:54.000000 clinker-0.0.9/clinker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-12-04 05:31:54.000000 clinker-0.0.9/clinker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-04 05:31:54.000000 clinker-0.0.9/clinker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-04 05:31:54.000000 clinker-0.0.9/clinker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-04 05:31:55.062927 clinker-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1155 2020-12-04 05:31:41.000000 clinker-0.0.9/setup.py
```

### Comparing `clinker-0.0.8/PKG-INFO` & `clinker-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinker
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/gamcil/clinker
 Author: Cameron Gilchrist
 License: UNKNOWN
 Description: # clinker
         [![DOI](https://zenodo.org/badge/193022148.svg)](https://zenodo.org/badge/latestdoi/193022148)
```

### Comparing `clinker-0.0.8/README.md` & `clinker-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/align.py` & `clinker-0.0.9/clinker/align.py`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/classes.py` & `clinker-0.0.9/clinker/classes.py`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/formatters.py` & `clinker-0.0.9/clinker/formatters.py`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/main.py` & `clinker-0.0.9/clinker/main.py`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/plot/clinker.js` & `clinker-0.0.9/clinker/plot/clinker.js`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/plot/clustermap.min.js` & `clinker-0.0.9/clinker/plot/clustermap.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -424,15 +424,16 @@
                     [p, h, f] = u(a, o),
                     [x, y, m] = u(l, c);
                 return f > m ? [x, y, m, p, h, f] : [p, h, f, x, y, m]
             },
             getGroups: (t, e) => t.map(t => [t.query.uid, t.target.uid]).map((t, e, a) => a.slice(e).reduce((e, a) => t.some(t => a.includes(t)) ? [...new Set([...e, ...a])] : e, [])).map((t, e) => ({
                 label: "Group " + e,
                 genes: t,
-                hidden: !1
+                hidden: !1,
+                colour: null
             })).reduce((t, e) => {
                 let a = !1;
                 return t = t.map(t => (t.genes.some(t => e.genes.includes(t)) && (a = !0, t.genes = [...new Set([...t.genes, ...e.genes])]), t)), !a && t.push({
                     ...e,
                     uid: t.length
                 }), t
             }, e || []),
@@ -447,36 +448,28 @@
                 }), e
             },
             updateGroups: t => {
                 let {
                     domain: e,
                     range: a
                 } = p.getGroupDomainAndRange(t), l = t.map(t => t.uid);
-                d.group.domain(e).range(a), d.name.domain(l).range(t.map(t => t.label)), d.colour.domain(l).range(d3.quantize(d3.interpolateRainbow, t.length + 1))
+                d.group.domain(e).range(a), d.name.domain(l).range(t.map(t => t.label));
+                let n = d3.quantize(d3.interpolateRainbow, t.length + 1);
+                t.forEach((t, e) => {
+                    t.colour && (n[e] = t.colour)
+                }), d.colour.domain(l).range(n)
             },
             hide: (t, e) => {
                 t.preventDefault(), e.hidden = !0, c.update()
             },
             rename: (t, e) => {
                 if (t.defaultPrevented) return;
                 let a = d3.select(t.target),
                     l = prompt("Enter new value:", a.text());
                 l && (e.label = l, a.text(l), c.update())
-            },
-            hideGroup: t => {
-                let e = d.group.domain(),
-                    a = d.group.range(),
-                    l = [],
-                    n = [];
-                for (let [r, s] of a.entries()) s !== t && (n.push(s), l.push(e[r]));
-                d.group.domain(l), d.group.range(n);
-                let r = d.colour.domain(),
-                    s = d.colour.range(),
-                    o = r.indexOf(t);
-                r.splice(o, 1), s.splice(o, 1), d.colour.domain(r).range(s)
             }
         },
         h = {
             getId: t => "locus_" + t.uid,
             realLength: t => d.x(t._end - t._start),
             updateTrackBar: t => {
                 let e = r.gene.shape.tipHeight + r.gene.shape.bodyHeight / 2;
@@ -737,17 +730,15 @@
                 })
             })
         }
 
         function i(t, e) {
             let a = d3.select("input.colourPicker");
             a.on("change", () => {
-                let t = a.node().value,
-                    l = d.colour.range();
-                l[e] = t, d.colour.range(l), d3.selectAll(".group-" + e).attr("fill", t)
+                e.colour = a.node().value, c.update()
             }), a.node().click()
         }
 
         function m() {
             let t = prompt("Enter new length (bp):", r.scaleBar.basePair);
             t && (r.scaleBar.basePair = t, c.update())
         }
```

### Comparing `clinker-0.0.8/clinker/plot/d3.min.js` & `clinker-0.0.9/clinker/plot/d3.min.js`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/plot/index.html` & `clinker-0.0.9/clinker/plot/index.html`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/plot/mock.json` & `clinker-0.0.9/clinker/plot/mock.json`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/plot/style.css` & `clinker-0.0.9/clinker/plot/style.css`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker/plot.py` & `clinker-0.0.9/clinker/plot.py`

 * *Files identical despite different names*

### Comparing `clinker-0.0.8/clinker.egg-info/PKG-INFO` & `clinker-0.0.9/clinker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinker
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/gamcil/clinker
 Author: Cameron Gilchrist
 License: UNKNOWN
 Description: # clinker
         [![DOI](https://zenodo.org/badge/193022148.svg)](https://zenodo.org/badge/latestdoi/193022148)
```

### Comparing `clinker-0.0.8/setup.py` & `clinker-0.0.9/setup.py`

 * *Files identical despite different names*

