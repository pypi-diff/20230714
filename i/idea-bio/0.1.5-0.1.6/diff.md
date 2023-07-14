# Comparing `tmp/idea_bio-0.1.5.tar.gz` & `tmp/idea_bio-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idea_bio-0.1.5.tar", max compression
+gzip compressed data, was "idea_bio-0.1.6.tar", max compression
```

## Comparing `idea_bio-0.1.5.tar` & `idea_bio-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-14 03:15:58.372612 idea_bio-0.1.5/LICENSE
--rw-r--r--   0        0        0     2069 2023-07-14 03:15:58.375945 idea_bio-0.1.5/README.md
--rw-r--r--   0        0        0      201 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/__init__.py
--rw-r--r--   0        0        0     1561 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/_go.py
--rw-r--r--   0        0        0    10142 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/_idea.py
--rw-r--r--   0        0        0      438 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/_utils.py
--rw-r--r--   0        0        0      691 2023-07-14 15:12:08.109779 idea_bio-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 idea_bio-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 03:15:58.372612 idea_bio-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2069 2023-07-14 03:15:58.375945 idea_bio-0.1.6/README.md
+-rw-r--r--   0        0        0      201 2023-07-14 03:15:58.392612 idea_bio-0.1.6/idea/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-14 03:15:58.392612 idea_bio-0.1.6/idea/_go.py
+-rw-r--r--   0        0        0    13085 2023-07-14 17:32:15.663859 idea_bio-0.1.6/idea/_idea.py
+-rw-r--r--   0        0        0      597 2023-07-14 17:32:15.663859 idea_bio-0.1.6/idea/_utils.py
+-rw-r--r--   0        0        0      691 2023-07-14 17:32:15.663859 idea_bio-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 idea_bio-0.1.6/PKG-INFO
```

### Comparing `idea_bio-0.1.5/LICENSE` & `idea_bio-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.5/README.md` & `idea_bio-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.5/idea/_go.py` & `idea_bio-0.1.6/idea/_go.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.5/idea/_idea.py` & `idea_bio-0.1.6/idea/_idea.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,41 +9,53 @@
 
 class IDEA:
     def __init__(
         self,
         degs: pd.DataFrame,
         go: pd.DataFrame,
         deg_size_name: str = "padj",
+        deg_color_name: str = "padj",
         deg_gene_name: str = "gene",
         go_size_name: str = "adj_pvalue",
         go_term_name: str = "term_name",
         go_overlap_name: str = "overlapping_genes",
-        neg_log_xform_degs: bool = True,
+        neg_log_xform_degs_size: bool = True,
+        neg_log_xform_degs_color: bool = True,
+        absolute_degs_color: bool = True,
         neg_log_xform_go: bool = True,
         set_deg_mass: bool = True,
         set_go_mass: bool = True,
         edge_color: str = "grey",
+        edge_width: float = 1.0,
         gene_palette: str = "Reds",
         term_palette: str = "Blues",
         gene_color: Optional[str] = None,
         term_color: Optional[str] = None,
+        center: Optional[float] = None,
+        fontsize: int = 14,
+        fontface: str = "arial",
+        fontcolor: str = "black",
     ):
         """
         Initialize the IDEA class.
 
         Parameters
         ----------
         degs : pd.DataFrame
             A dataframe of differentially expressed genes.
         go : pd.DataFrame
             A dataframe of gene ontology terms.
         deg_size_name : str, optional
             The name of the column in `degs` that should be used for
             the size of the differentially expressed genes. By default,
             this is `"padj"`.
+        deg_color_name : str, optional
+            The name of the column in `degs` that should be used for
+            the color of the differentially expressed genes. By default,
+            this is `"padj"`.
         deg_gene_name : str, optional
             The name of the column in `degs` that should be used for
             the gene names of the differentially expressed genes. By
             default, this is `"gene"`.
         go_size_name : str, optional
             The name of the column in `go` that should be used for
             the size of the gene ontology terms. By default, this is
@@ -51,17 +63,23 @@
         go_term_name : str, optional
             The name of the column in `go` that should be used for
             the gene ontology terms. By default, this is `"term_name"`.
         go_overlap_name : str, optional
             The name of the column in `go` that should be used for
             the overlapping genes of the gene ontology terms. By
             default, this is `"overlapping_genes"`.
-        neg_log_xform_degs : bool, optional
+        neg_log_xform_degs_size : bool, optional
+            Whether or not to invert the attributes of the differentially
+            expressed genes. By default, this is `True`.
+        neg_log_xform_degs_color : bool, optional
             Whether or not to invert the attributes of the differentially
             expressed genes. By default, this is `True`.
+        absolute_degs_color: bool, optional
+            Whether or not to take the absolute value of the color attribute
+            for the differentially expressed genes. By default, this is `True`.
         neg_log_xform_go : bool, optional
             Whether or not to invert the attributes of the gene ontology
             terms. By default, this is `True`.
         set_deg_mass : bool, optional
             Whether or not to set the mass of the differentially expressed
             genes with the deg size. By default, this is `True`.
         set_go_mass : bool, optional
@@ -85,54 +103,82 @@
             this is `None`. If `None`, the color will be set to the
             `gene_palette`. Otherwise, the color will be set to the
             `gene_color`.
         term_color : str, optional
             The color of the gene ontology terms. By default, this is
             `None`. If `None`, the color will be set to the `term_palette`.
             Otherwise, the color will be set to the `term_color`.
+        center : float, optional
+            The center of the DEG color scale. Set to zero for diverging
+            color scales. By default, this is `None`.
+        fontsize : int, optional
+            The fontsize of the labels. By default, this is `14`.
+        edge_width : float, optional
+            The width of the edges. By default, this is `1.0`.
+        fontface : str, optional
+            The fontface of the labels. By default, this is `"arial"`.
+        fontcolor : str, optional
+            The fontcolor of the labels. By default, this is `"black"`.
         """
         self._degs = degs
         self._go = go
         self._deg_size_name = deg_size_name
+        self._deg_color_name = deg_color_name
         self._deg_gene_name = deg_gene_name
         self._go_size_name = go_size_name
         self._go_term_name = go_term_name
         self._go_overlap_name = go_overlap_name
-        self._neg_log_xform_degs = neg_log_xform_degs
+        self._neg_log_xform_degs_size = neg_log_xform_degs_size
+        self._neg_log_xform_degs_color = neg_log_xform_degs_color
+        self._absolute_degs_color = absolute_degs_color
         self._neg_log_xform_go = neg_log_xform_go
         self._set_deg_mass = set_deg_mass
         self._set_go_mass = set_go_mass
         self._edge_color = edge_color
+        self._edge_width = edge_width
         self._gene_palette = gene_palette
         self._term_palette = term_palette
         self._gene_color = gene_color
         self._term_color = term_color
+        self._center = center
+        self._fontsize = fontsize
+        self._fontface = fontface
+        self._fontcolor = fontcolor
+        self._font_shorthand = f"{self._fontsize}px {self._fontface} {self._fontcolor}"
 
         self._validate_degs()
         self._validate_go()
         self._build_bipartite_graph()
 
     def _validate_degs(self):
-        for col in [self._deg_size_name, self._deg_gene_name]:
+        for col in [self._deg_size_name, self._deg_color_name, self._deg_gene_name]:
             if col not in self._degs.columns:
                 raise ValueError(f"Column '{col}' not found in DEGs.")
         logging.info(f"Found {self._degs.shape[0]} differentially expressed genes.")
 
     def _validate_go(self):
         for col in [self._go_size_name, self._go_term_name, self._go_overlap_name]:
             if col not in self._go.columns:
                 raise ValueError(f"Column '{col}' not found in GO terms.")
         logging.info(f"Found {self._go.shape[0]} gene ontology terms.")
 
     def _build_deg_attributes(self):
         genes = self._degs[self._deg_gene_name].values
-        attributes = self._degs[self._deg_size_name].values
-        if self._neg_log_xform_degs:
-            attributes = -np.log10(attributes)
-        self._gene_attributes = dict(zip(genes, attributes))
+        sizes = self._degs[self._deg_size_name].values
+        colors = self._degs[self._deg_color_name].values
+        if self._neg_log_xform_degs_size:
+            sizes = -np.log10(sizes)
+        if self._absolute_degs_color:
+            colors = np.abs(colors)
+        if self._neg_log_xform_degs_color:
+            colors = -np.log10(colors)
+        self._gene_attributes = {
+            gene: {"attr_size": size, "attr_color": color}
+            for gene, size, color in zip(genes, sizes, colors)
+        }
 
     def _build_go_attributes(self):
         terms = self._go[self._go_term_name].values
         overlaps = self._go[self._go_overlap_name].values
         attributes = self._go[self._go_size_name].values
 
         if self._neg_log_xform_go:
@@ -147,52 +193,74 @@
         """
         Inserts a GO term into the graph.
         """
         self.graph.add_node(
             term,
             cond="term",
             shape="square",
+            title=term,
             attr=self._term_attributes[term]["attribute"],
             size=self._term_attributes[term]["attribute"],
             mass=self._term_attributes[term]["attribute"] if self._set_go_mass else 1.0,
             color=self._term_color
             if self._term_color is not None
             else self._edge_color,
             color_border="black",
+            font=self._font_shorthand,
         )
 
     def _insert_deg_gene(self, gene: str):
         """
         Inserts a DEG gene into the graph.
         """
         self.graph.add_node(
             gene,
             cond="gene",
             shape="circle",
-            attr=self._gene_attributes[gene],
-            size=self._gene_attributes[gene],
-            mass=self._gene_attributes[gene] if self._set_deg_mass else 1.0,
+            title=gene,
+            color_border="black",
+            attr=self._gene_attributes[gene]["attr_color"],
+            size=self._gene_attributes[gene]["attr_size"],
+            mass=self._gene_attributes[gene]["attr_size"]
+            if self._set_deg_mass
+            else 1.0,
+            font=self._font_shorthand,
         )
 
     def _insert_edge(self, term: str, gene: str):
         """
         Inserts an edge between a GO term and a DEG gene into the graph.
         """
-        self.graph.add_edge(term, gene, color=self._edge_color)
+        self.graph.add_edge(
+            term,
+            gene,
+            color=self._edge_color,
+            weight=self._edge_width,
+        )
+
+    def _valid_gene(self, gene: str) -> bool:
+        """
+        Validates that a gene is in the DEGs.
+        """
+        return gene in self._gene_attributes
 
     def _set_color(self, cond: str):
         distribution = []
 
         for node in self.graph.nodes(data=True):
             if node[1]["cond"] == cond:
                 distribution.append(node[1]["attr"])
         distribution = np.array(distribution)
 
         palette = self._term_palette if cond == "term" else self._gene_palette
-        hex_colors = _array_to_hex(distribution, palette)
+
+        if cond == "term":
+            hex_colors = _array_to_hex(distribution, palette)
+        else:
+            hex_colors = _array_to_hex(distribution, palette, self._center)
 
         idx = 0
         for node in self.graph.nodes(data=True):
             if node[1]["cond"] == cond:
                 node[1]["color"] = hex_colors[idx]
                 idx += 1
 
@@ -200,14 +268,16 @@
         self._build_deg_attributes()
         self._build_go_attributes()
 
         self.graph = nx.Graph()
         for term in self._term_attributes:
             self._insert_go_term(term)
             for gene in self._term_attributes[term]["overlap"]:
+                if not self._valid_gene(gene):
+                    continue
                 self._insert_deg_gene(gene)
                 self._insert_edge(term, gene)
 
         if self._term_palette is not None and self._term_color is None:
             self._set_color("term")
         if self._gene_palette is not None and self._gene_color is None:
             self._set_color("gene")
@@ -229,17 +299,16 @@
         )
 
     def visualize(
         self,
         filepath: str = "network.html",
         height: str = "1000px",
         width: str = "100%",
-        physics_toggle: bool = True,
-        physics: bool = True,
         notebook: bool = False,
+        show_physics_options: bool = False,
         **kwargs,
     ):
         """
         Creates the pyvis visualization. For more information on the
         additional keyword arguments, see `pyvis.network.Network`.
 
         Parameters
@@ -249,12 +318,14 @@
         width : str, optional
             The width of the visualization. By default, this is `"100%"`.
         kwargs
             Additional keyword arguments to pass to `pyvis.network.Network`.
         """
         net = Network(height=height, width=width, notebook=notebook, **kwargs)
         net.from_nx(self.graph)
-        net.toggle_physics(physics_toggle)
-        if physics_toggle:
-            net.show_buttons(filter_=["physics"])
+        if show_physics_options:
+            buttons = []
+            if show_physics_options:
+                buttons.append("physics")
+            net.show_buttons(filter_=buttons)
         net.write_html(filepath)
         logging.info(f"Visualization saved to {filepath}.")
```

### Comparing `idea_bio-0.1.5/pyproject.toml` & `idea_bio-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idea-bio"
-version = "0.1.5"
+version = "0.1.6"
 description = "Integrated Differential Expression and Annotation"
 authors = ["Noam Teyssier"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "idea" }
 ]
```

### Comparing `idea_bio-0.1.5/PKG-INFO` & `idea_bio-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idea-bio
-Version: 0.1.5
+Version: 0.1.6
 Summary: Integrated Differential Expression and Annotation
 Home-page: https://github.com/noamteyssier/idea
 License: MIT
 Keywords: bioinformatics,differential expression,annotation,networks
 Author: Noam Teyssier
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

