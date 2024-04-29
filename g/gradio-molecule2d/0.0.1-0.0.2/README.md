# Comparing `tmp/gradio_molecule2d-0.0.1.tar.gz` & `tmp/gradio_molecule2d-0.0.2.tar.gz`

## Comparing `gradio_molecule2d-0.0.1.tar` & `gradio_molecule2d-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,25 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/__init__.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/molecule2d.py
--rw-r--r--   0        0        0    19535 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/molecule2d.pyi
--rw-r--r--   0        0        0   403242 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/component/index.js
--rw-r--r--   0        0        0    33310 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/demo/__init__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/demo/css.css
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/demo/requirements.txt
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/demo/space.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/ClearButton.svelte
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/Editor.svelte
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/Example.svelte
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/Index.svelte
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/Viewer.svelte
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/gradio.config.js
--rw-r--r--   0        0        0   292374 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/package-lock.json
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/style.css
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/test.html
--rwxr-xr-x   0        0        0   140439 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/utils/RDKit_minimal.js
--rwxr-xr-x   0        0        0  5860641 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/utils/RDKit_minimal.wasm
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/utils/initRDKit.ts
--rw-r--r--   0        0        0 12442162 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/frontend/utils/ketcher.js
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/.gitignore
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/README.md
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/__init__.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/molecule2d.py
+-rw-r--r--   0        0        0    19535 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/molecule2d.pyi
+-rw-r--r--   0        0        0   403788 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/component/index.js
+-rw-r--r--   0        0        0    33310 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/demo/__init__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/demo/css.css
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/demo/requirements.txt
+-rw-r--r--   0        0        0     7382 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/demo/space.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/ClearButton.svelte
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/Editor.svelte
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/Example.svelte
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/Index.svelte
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/Viewer.svelte
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/gradio.config.js
+-rw-r--r--   0        0        0   292374 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/frontend/style.css
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/.gitignore
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/README.md
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 gradio_molecule2d-0.0.2/PKG-INFO
```

### Comparing `gradio_molecule2d-0.0.1/backend/gradio_molecule2d/molecule2d.py` & `gradio_molecule2d-0.0.2/backend/gradio_molecule2d/molecule2d.py`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/backend/gradio_molecule2d/molecule2d.pyi` & `gradio_molecule2d-0.0.2/backend/gradio_molecule2d/molecule2d.pyi`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/component/index.js` & `gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 const {
-    SvelteComponent: zf,
-    assign: Hf,
-    create_slot: Wf,
-    detach: qf,
-    element: Vf,
-    get_all_dirty_from_scope: Xf,
-    get_slot_changes: Yf,
-    get_spread_update: Gf,
-    init: Uf,
-    insert: Zf,
-    safe_not_equal: Kf,
-    set_dynamic_element_data: ta,
-    set_style: ot,
-    toggle_class: Mt,
-    transition_in: ja,
-    transition_out: Ja,
-    update_slot_base: jf
+    SvelteComponent: Wf,
+    assign: qf,
+    create_slot: Vf,
+    detach: Xf,
+    element: Yf,
+    get_all_dirty_from_scope: Gf,
+    get_slot_changes: Uf,
+    get_spread_update: Zf,
+    init: Kf,
+    insert: jf,
+    safe_not_equal: Jf,
+    set_dynamic_element_data: ia,
+    set_style: ht,
+    toggle_class: Bt,
+    transition_in: Ja,
+    transition_out: Qa,
+    update_slot_base: Qf
 } = window.__gradio__svelte__internal;
 
-function Jf(d) {
+function eu(d) {
     let e, t, r;
     const i = (
             /*#slots*/
             d[18].default
         ),
-        s = Wf(
+        s = Vf(
             i,
             d,
             /*$$scope*/
             d[17],
             null
         );
     let a = [{
@@ -43,104 +43,104 @@
             )
         }, {
             class: t = "block " + /*elem_classes*/
                 d[3].join(" ") + " svelte-nl1om8"
         }],
         n = {};
     for (let h = 0; h < a.length; h += 1)
-        n = Hf(n, a[h]);
+        n = qf(n, a[h]);
     return {
         c() {
-            e = Vf(
+            e = Yf(
                 /*tag*/
                 d[14]
-            ), s && s.c(), ta(
+            ), s && s.c(), ia(
                 /*tag*/
                 d[14]
-            )(e, n), Mt(
+            )(e, n), Bt(
                 e,
                 "hidden",
                 /*visible*/
                 d[10] === !1
-            ), Mt(
+            ), Bt(
                 e,
                 "padded",
                 /*padding*/
                 d[6]
-            ), Mt(
+            ), Bt(
                 e,
                 "border_focus",
                 /*border_mode*/
                 d[5] === "focus"
-            ), Mt(
+            ), Bt(
                 e,
                 "border_contrast",
                 /*border_mode*/
                 d[5] === "contrast"
-            ), Mt(e, "hide-container", ! /*explicit_call*/
+            ), Bt(e, "hide-container", ! /*explicit_call*/
                 d[8] && ! /*container*/
-                d[9]), ot(
+                d[9]), ht(
                 e,
                 "height",
                 /*get_dimension*/
                 d[15](
                     /*height*/
                     d[0]
                 )
-            ), ot(e, "width", typeof /*width*/ d[1] == "number" ? `calc(min(${/*width*/
+            ), ht(e, "width", typeof /*width*/ d[1] == "number" ? `calc(min(${/*width*/
       d[1]}px, 100%))` : (
                 /*get_dimension*/
                 d[15](
                     /*width*/
                     d[1]
                 )
-            )), ot(
+            )), ht(
                 e,
                 "border-style",
                 /*variant*/
                 d[4]
-            ), ot(
+            ), ht(
                 e,
                 "overflow",
                 /*allow_overflow*/
                 d[11] ? "visible" : "hidden"
-            ), ot(
+            ), ht(
                 e,
                 "flex-grow",
                 /*scale*/
                 d[12]
-            ), ot(e, "min-width", `calc(min(${/*min_width*/
-      d[13]}px, 100%))`), ot(e, "border-width", "var(--block-border-width)");
+            ), ht(e, "min-width", `calc(min(${/*min_width*/
+      d[13]}px, 100%))`), ht(e, "border-width", "var(--block-border-width)");
         },
         m(h, l) {
-            Zf(h, e, l), s && s.m(e, null), r = !0;
+            jf(h, e, l), s && s.m(e, null), r = !0;
         },
         p(h, l) {
             s && s.p && (!r || l & /*$$scope*/
-                    131072) && jf(
+                    131072) && Qf(
                     s,
                     i,
                     h,
                     /*$$scope*/
                     h[17],
-                    r ? Yf(
+                    r ? Uf(
                         i,
                         /*$$scope*/
                         h[17],
                         l,
                         null
-                    ) : Xf(
+                    ) : Gf(
                         /*$$scope*/
                         h[17]
                     ),
                     null
-                ), ta(
+                ), ia(
                     /*tag*/
                     h[14]
-                )(e, n = Gf(a, [
+                )(e, n = Zf(a, [
                     (!r || l & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
                             h[7]
                         )
                     },
@@ -152,116 +152,116 @@
                         )
                     },
                     (!r || l & /*elem_classes*/
                         8 && t !== (t = "block " + /*elem_classes*/
                             h[3].join(" ") + " svelte-nl1om8")) && {
                         class: t
                     }
-                ])), Mt(
+                ])), Bt(
                     e,
                     "hidden",
                     /*visible*/
                     h[10] === !1
-                ), Mt(
+                ), Bt(
                     e,
                     "padded",
                     /*padding*/
                     h[6]
-                ), Mt(
+                ), Bt(
                     e,
                     "border_focus",
                     /*border_mode*/
                     h[5] === "focus"
-                ), Mt(
+                ), Bt(
                     e,
                     "border_contrast",
                     /*border_mode*/
                     h[5] === "contrast"
-                ), Mt(e, "hide-container", ! /*explicit_call*/
+                ), Bt(e, "hide-container", ! /*explicit_call*/
                     h[8] && ! /*container*/
                     h[9]), l & /*height*/
-                1 && ot(
+                1 && ht(
                     e,
                     "height",
                     /*get_dimension*/
                     h[15](
                         /*height*/
                         h[0]
                     )
                 ), l & /*width*/
-                2 && ot(e, "width", typeof /*width*/ h[1] == "number" ? `calc(min(${/*width*/
+                2 && ht(e, "width", typeof /*width*/ h[1] == "number" ? `calc(min(${/*width*/
       h[1]}px, 100%))` : (
                     /*get_dimension*/
                     h[15](
                         /*width*/
                         h[1]
                     )
                 )), l & /*variant*/
-                16 && ot(
+                16 && ht(
                     e,
                     "border-style",
                     /*variant*/
                     h[4]
                 ), l & /*allow_overflow*/
-                2048 && ot(
+                2048 && ht(
                     e,
                     "overflow",
                     /*allow_overflow*/
                     h[11] ? "visible" : "hidden"
                 ), l & /*scale*/
-                4096 && ot(
+                4096 && ht(
                     e,
                     "flex-grow",
                     /*scale*/
                     h[12]
                 ), l & /*min_width*/
-                8192 && ot(e, "min-width", `calc(min(${/*min_width*/
+                8192 && ht(e, "min-width", `calc(min(${/*min_width*/
       h[13]}px, 100%))`);
         },
         i(h) {
-            r || (ja(s, h), r = !0);
+            r || (Ja(s, h), r = !0);
         },
         o(h) {
-            Ja(s, h), r = !1;
+            Qa(s, h), r = !1;
         },
         d(h) {
-            h && qf(e), s && s.d(h);
+            h && Xf(e), s && s.d(h);
         }
     };
 }
 
-function Qf(d) {
+function tu(d) {
     let e, t = (
         /*tag*/
-        d[14] && Jf(d)
+        d[14] && eu(d)
     );
     return {
         c() {
             t && t.c();
         },
         m(r, i) {
             t && t.m(r, i), e = !0;
         },
         p(r, [i]) {
             /*tag*/
             r[14] && t.p(r, i);
         },
         i(r) {
-            e || (ja(t, r), e = !0);
+            e || (Ja(t, r), e = !0);
         },
         o(r) {
-            Ja(t, r), e = !1;
+            Qa(t, r), e = !1;
         },
         d(r) {
             t && t.d(r);
         }
     };
 }
 
-function eu(d, e, t) {
+function ru(d, e, t) {
     let {
         $$slots: r = {},
         $$scope: i
     } = e, {
         height: s = void 0
     } = e, {
         width: a = void 0
@@ -280,57 +280,57 @@
     } = e, {
         test_id: m = void 0
     } = e, {
         explicit_call: _ = !1
     } = e, {
         container: v = !0
     } = e, {
-        visible: N = !0
+        visible: A = !0
     } = e, {
-        allow_overflow: B = !0
+        allow_overflow: T = !0
     } = e, {
-        scale: x = null
+        scale: k = null
     } = e, {
-        min_width: L = 0
-    } = e, k = g === "fieldset" ? "fieldset" : "div";
-    const z = (D) => {
+        min_width: x = 0
+    } = e, R = g === "fieldset" ? "fieldset" : "div";
+    const O = (D) => {
         if (D !== void 0) {
             if (typeof D == "number")
                 return D + "px";
             if (typeof D == "string")
                 return D;
         }
     };
     return d.$$set = (D) => {
-        "height" in D && t(0, s = D.height), "width" in D && t(1, a = D.width), "elem_id" in D && t(2, n = D.elem_id), "elem_classes" in D && t(3, h = D.elem_classes), "variant" in D && t(4, l = D.variant), "border_mode" in D && t(5, c = D.border_mode), "padding" in D && t(6, u = D.padding), "type" in D && t(16, g = D.type), "test_id" in D && t(7, m = D.test_id), "explicit_call" in D && t(8, _ = D.explicit_call), "container" in D && t(9, v = D.container), "visible" in D && t(10, N = D.visible), "allow_overflow" in D && t(11, B = D.allow_overflow), "scale" in D && t(12, x = D.scale), "min_width" in D && t(13, L = D.min_width), "$$scope" in D && t(17, i = D.$$scope);
+        "height" in D && t(0, s = D.height), "width" in D && t(1, a = D.width), "elem_id" in D && t(2, n = D.elem_id), "elem_classes" in D && t(3, h = D.elem_classes), "variant" in D && t(4, l = D.variant), "border_mode" in D && t(5, c = D.border_mode), "padding" in D && t(6, u = D.padding), "type" in D && t(16, g = D.type), "test_id" in D && t(7, m = D.test_id), "explicit_call" in D && t(8, _ = D.explicit_call), "container" in D && t(9, v = D.container), "visible" in D && t(10, A = D.visible), "allow_overflow" in D && t(11, T = D.allow_overflow), "scale" in D && t(12, k = D.scale), "min_width" in D && t(13, x = D.min_width), "$$scope" in D && t(17, i = D.$$scope);
     }, [
         s,
         a,
         n,
         h,
         l,
         c,
         u,
         m,
         _,
         v,
-        N,
-        B,
-        x,
-        L,
+        A,
+        T,
         k,
-        z,
+        x,
+        R,
+        O,
         g,
         i,
         r
     ];
 }
-class tu extends zf {
+class iu extends Wf {
     constructor(e) {
-        super(), Uf(this, e, eu, Qf, Kf, {
+        super(), Kf(this, e, ru, tu, Jf, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -342,139 +342,139 @@
             allow_overflow: 11,
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
-    SvelteComponent: ru,
-    attr: iu,
-    create_slot: nu,
-    detach: su,
-    element: au,
-    get_all_dirty_from_scope: lu,
-    get_slot_changes: ou,
-    init: hu,
-    insert: fu,
-    safe_not_equal: uu,
-    transition_in: cu,
-    transition_out: gu,
-    update_slot_base: du
+    SvelteComponent: nu,
+    attr: su,
+    create_slot: au,
+    detach: lu,
+    element: ou,
+    get_all_dirty_from_scope: hu,
+    get_slot_changes: fu,
+    init: uu,
+    insert: cu,
+    safe_not_equal: gu,
+    transition_in: du,
+    transition_out: pu,
+    update_slot_base: vu
 } = window.__gradio__svelte__internal;
 
-function pu(d) {
+function mu(d) {
     let e, t;
     const r = (
             /*#slots*/
             d[1].default
         ),
-        i = nu(
+        i = au(
             r,
             d,
             /*$$scope*/
             d[0],
             null
         );
     return {
         c() {
-            e = au("div"), i && i.c(), iu(e, "class", "svelte-1hnfib2");
+            e = ou("div"), i && i.c(), su(e, "class", "svelte-1hnfib2");
         },
         m(s, a) {
-            fu(s, e, a), i && i.m(e, null), t = !0;
+            cu(s, e, a), i && i.m(e, null), t = !0;
         },
         p(s, [a]) {
             i && i.p && (!t || a & /*$$scope*/
-                1) && du(
+                1) && vu(
                 i,
                 r,
                 s,
                 /*$$scope*/
                 s[0],
-                t ? ou(
+                t ? fu(
                     r,
                     /*$$scope*/
                     s[0],
                     a,
                     null
-                ) : lu(
+                ) : hu(
                     /*$$scope*/
                     s[0]
                 ),
                 null
             );
         },
         i(s) {
-            t || (cu(i, s), t = !0);
+            t || (du(i, s), t = !0);
         },
         o(s) {
-            gu(i, s), t = !1;
+            pu(i, s), t = !1;
         },
         d(s) {
-            s && su(e), i && i.d(s);
+            s && lu(e), i && i.d(s);
         }
     };
 }
 
-function vu(d, e, t) {
+function bu(d, e, t) {
     let {
         $$slots: r = {},
         $$scope: i
     } = e;
     return d.$$set = (s) => {
         "$$scope" in s && t(0, i = s.$$scope);
     }, [i, r];
 }
-class mu extends ru {
+class wu extends nu {
     constructor(e) {
-        super(), hu(this, e, vu, pu, uu, {});
+        super(), uu(this, e, bu, mu, gu, {});
     }
 }
 const {
-    SvelteComponent: bu,
-    attr: ra,
-    check_outros: wu,
-    create_component: yu,
-    create_slot: _u,
-    destroy_component: Su,
+    SvelteComponent: yu,
+    attr: na,
+    check_outros: _u,
+    create_component: Su,
+    create_slot: Cu,
+    destroy_component: Au,
     detach: Ni,
-    element: Cu,
-    empty: Au,
-    get_all_dirty_from_scope: Nu,
-    get_slot_changes: ku,
-    group_outros: Ru,
-    init: xu,
+    element: Nu,
+    empty: ku,
+    get_all_dirty_from_scope: Ru,
+    get_slot_changes: xu,
+    group_outros: Tu,
+    init: Eu,
     insert: ki,
-    mount_component: Tu,
-    safe_not_equal: Eu,
-    set_data: Lu,
-    space: Mu,
-    text: Bu,
+    mount_component: Lu,
+    safe_not_equal: Mu,
+    set_data: Bu,
+    space: Du,
+    text: Pu,
     toggle_class: kr,
     transition_in: Gr,
     transition_out: Ri,
-    update_slot_base: Du
+    update_slot_base: $u
 } = window.__gradio__svelte__internal;
 
-function ia(d) {
+function sa(d) {
     let e, t;
-    return e = new mu({
+    return e = new wu({
         props: {
             $$slots: {
-                default: [Pu]
+                default: [Iu]
             },
             $$scope: {
                 ctx: d
             }
         }
     }), {
         c() {
-            yu(e.$$.fragment);
+            Su(e.$$.fragment);
         },
         m(r, i) {
-            Tu(e, r, i), t = !0;
+            Lu(e, r, i), t = !0;
         },
         p(r, i) {
             const s = {};
             i & /*$$scope, info*/
                 10 && (s.$$scope = {
                     dirty: i,
                     ctx: r
@@ -483,91 +483,91 @@
         i(r) {
             t || (Gr(e.$$.fragment, r), t = !0);
         },
         o(r) {
             Ri(e.$$.fragment, r), t = !1;
         },
         d(r) {
-            Su(e, r);
+            Au(e, r);
         }
     };
 }
 
-function Pu(d) {
+function Iu(d) {
     let e;
     return {
         c() {
-            e = Bu(
+            e = Pu(
                 /*info*/
                 d[1]
             );
         },
         m(t, r) {
             ki(t, e, r);
         },
         p(t, r) {
             r & /*info*/
-                2 && Lu(
+                2 && Bu(
                     e,
                     /*info*/
                     t[1]
                 );
         },
         d(t) {
             t && Ni(e);
         }
     };
 }
 
-function $u(d) {
+function Ou(d) {
     let e, t, r, i;
     const s = (
             /*#slots*/
             d[2].default
         ),
-        a = _u(
+        a = Cu(
             s,
             d,
             /*$$scope*/
             d[3],
             null
         );
     let n = (
         /*info*/
-        d[1] && ia(d)
+        d[1] && sa(d)
     );
     return {
         c() {
-            e = Cu("span"), a && a.c(), t = Mu(), n && n.c(), r = Au(), ra(e, "data-testid", "block-info"), ra(e, "class", "svelte-22c38v"), kr(e, "sr-only", ! /*show_label*/
+            e = Nu("span"), a && a.c(), t = Du(), n && n.c(), r = ku(), na(e, "data-testid", "block-info"), na(e, "class", "svelte-22c38v"), kr(e, "sr-only", ! /*show_label*/
                 d[0]), kr(e, "hide", ! /*show_label*/
                 d[0]), kr(
                 e,
                 "has-info",
                 /*info*/
                 d[1] != null
             );
         },
         m(h, l) {
             ki(h, e, l), a && a.m(e, null), ki(h, t, l), n && n.m(h, l), ki(h, r, l), i = !0;
         },
         p(h, [l]) {
             a && a.p && (!i || l & /*$$scope*/
-                    8) && Du(
+                    8) && $u(
                     a,
                     s,
                     h,
                     /*$$scope*/
                     h[3],
-                    i ? ku(
+                    i ? xu(
                         s,
                         /*$$scope*/
                         h[3],
                         l,
                         null
-                    ) : Nu(
+                    ) : Ru(
                         /*$$scope*/
                         h[3]
                     ),
                     null
                 ), (!i || l & /*show_label*/
                     1) && kr(e, "sr-only", ! /*show_label*/
                     h[0]), (!i || l & /*show_label*/
@@ -576,119 +576,119 @@
                     2) && kr(
                     e,
                     "has-info",
                     /*info*/
                     h[1] != null
                 ), /*info*/
                 h[1] ? n ? (n.p(h, l), l & /*info*/
-                    2 && Gr(n, 1)) : (n = ia(h), n.c(), Gr(n, 1), n.m(r.parentNode, r)) : n && (Ru(), Ri(n, 1, 1, () => {
+                    2 && Gr(n, 1)) : (n = sa(h), n.c(), Gr(n, 1), n.m(r.parentNode, r)) : n && (Tu(), Ri(n, 1, 1, () => {
                     n = null;
-                }), wu());
+                }), _u());
         },
         i(h) {
             i || (Gr(a, h), Gr(n), i = !0);
         },
         o(h) {
             Ri(a, h), Ri(n), i = !1;
         },
         d(h) {
             h && (Ni(e), Ni(t), Ni(r)), a && a.d(h), n && n.d(h);
         }
     };
 }
 
-function Iu(d, e, t) {
+function Fu(d, e, t) {
     let {
         $$slots: r = {},
         $$scope: i
     } = e, {
         show_label: s = !0
     } = e, {
         info: a = void 0
     } = e;
     return d.$$set = (n) => {
         "show_label" in n && t(0, s = n.show_label), "info" in n && t(1, a = n.info), "$$scope" in n && t(3, i = n.$$scope);
     }, [s, a, r, i];
 }
-class Ou extends bu {
+class zu extends yu {
     constructor(e) {
-        super(), xu(this, e, Iu, $u, Eu, {
+        super(), Eu(this, e, Fu, Ou, Mu, {
             show_label: 0,
             info: 1
         });
     }
 }
 const {
-    SvelteComponent: Fu,
-    append: On,
+    SvelteComponent: Hu,
+    append: Hn,
     attr: qt,
-    bubble: zu,
-    create_component: Hu,
-    destroy_component: Wu,
-    detach: Qa,
-    element: Fn,
-    init: qu,
-    insert: el,
-    listen: Vu,
-    mount_component: Xu,
-    safe_not_equal: Yu,
-    set_data: Gu,
+    bubble: Wu,
+    create_component: qu,
+    destroy_component: Vu,
+    detach: el,
+    element: Wn,
+    init: Xu,
+    insert: tl,
+    listen: Yu,
+    mount_component: Gu,
+    safe_not_equal: Uu,
+    set_data: Zu,
     set_style: Rr,
-    space: Uu,
-    text: Zu,
-    toggle_class: rt,
-    transition_in: Ku,
-    transition_out: ju
+    space: Ku,
+    text: ju,
+    toggle_class: it,
+    transition_in: Ju,
+    transition_out: Qu
 } = window.__gradio__svelte__internal;
 
-function na(d) {
+function aa(d) {
     let e, t;
     return {
         c() {
-            e = Fn("span"), t = Zu(
+            e = Wn("span"), t = ju(
                 /*label*/
                 d[1]
             ), qt(e, "class", "svelte-1lrphxw");
         },
         m(r, i) {
-            el(r, e, i), On(e, t);
+            tl(r, e, i), Hn(e, t);
         },
         p(r, i) {
             i & /*label*/
-                2 && Gu(
+                2 && Zu(
                     t,
                     /*label*/
                     r[1]
                 );
         },
         d(r) {
-            r && Qa(e);
+            r && el(e);
         }
     };
 }
 
-function Ju(d) {
+function ec(d) {
     let e, t, r, i, s, a, n, h = (
         /*show_label*/
-        d[2] && na(d)
+        d[2] && aa(d)
     );
     return i = new /*Icon*/
     d[0]({}), {
         c() {
-            e = Fn("button"), h && h.c(), t = Uu(), r = Fn("div"), Hu(i.$$.fragment), qt(r, "class", "svelte-1lrphxw"), rt(
+            e = Wn("button"), h && h.c(), t = Ku(), r = Wn("div"), qu(i.$$.fragment), qt(r, "class", "svelte-1lrphxw"), it(
                     r,
                     "small",
                     /*size*/
                     d[4] === "small"
-                ), rt(
+                ), it(
                     r,
                     "large",
                     /*size*/
                     d[4] === "large"
-                ), rt(
+                ), it(
                     r,
                     "medium",
                     /*size*/
                     d[4] === "medium"
                 ), e.disabled = /*disabled*/
                 d[7], qt(
                     e,
@@ -701,30 +701,30 @@
                     /*hasPopup*/
                     d[8]
                 ), qt(
                     e,
                     "title",
                     /*label*/
                     d[1]
-                ), qt(e, "class", "svelte-1lrphxw"), rt(
+                ), qt(e, "class", "svelte-1lrphxw"), it(
                     e,
                     "pending",
                     /*pending*/
                     d[3]
-                ), rt(
+                ), it(
                     e,
                     "padded",
                     /*padded*/
                     d[5]
-                ), rt(
+                ), it(
                     e,
                     "highlight",
                     /*highlight*/
                     d[6]
-                ), rt(
+                ), it(
                     e,
                     "transparent",
                     /*transparent*/
                     d[9]
                 ), Rr(e, "color", ! /*disabled*/
                     d[7] && /*_color*/
                     d[12] ? (
@@ -738,37 +738,37 @@
                     e,
                     "margin-left",
                     /*offset*/
                     d[11] + "px"
                 );
         },
         m(l, c) {
-            el(l, e, c), h && h.m(e, null), On(e, t), On(e, r), Xu(i, r, null), s = !0, a || (n = Vu(
+            tl(l, e, c), h && h.m(e, null), Hn(e, t), Hn(e, r), Gu(i, r, null), s = !0, a || (n = Yu(
                 e,
                 "click",
                 /*click_handler*/
                 d[14]
             ), a = !0);
         },
         p(l, [c]) {
             /*show_label*/
-            l[2] ? h ? h.p(l, c) : (h = na(l), h.c(), h.m(e, t)) : h && (h.d(1), h = null), (!s || c & /*size*/
-                    16) && rt(
+            l[2] ? h ? h.p(l, c) : (h = aa(l), h.c(), h.m(e, t)) : h && (h.d(1), h = null), (!s || c & /*size*/
+                    16) && it(
                     r,
                     "small",
                     /*size*/
                     l[4] === "small"
                 ), (!s || c & /*size*/
-                    16) && rt(
+                    16) && it(
                     r,
                     "large",
                     /*size*/
                     l[4] === "large"
                 ), (!s || c & /*size*/
-                    16) && rt(
+                    16) && it(
                     r,
                     "medium",
                     /*size*/
                     l[4] === "medium"
                 ), (!s || c & /*disabled*/
                     128) && (e.disabled = /*disabled*/
                     l[7]), (!s || c & /*label*/
@@ -786,33 +786,33 @@
                 ), (!s || c & /*label*/
                     2) && qt(
                     e,
                     "title",
                     /*label*/
                     l[1]
                 ), (!s || c & /*pending*/
-                    8) && rt(
+                    8) && it(
                     e,
                     "pending",
                     /*pending*/
                     l[3]
                 ), (!s || c & /*padded*/
-                    32) && rt(
+                    32) && it(
                     e,
                     "padded",
                     /*padded*/
                     l[5]
                 ), (!s || c & /*highlight*/
-                    64) && rt(
+                    64) && it(
                     e,
                     "highlight",
                     /*highlight*/
                     l[6]
                 ), (!s || c & /*transparent*/
-                    512) && rt(
+                    512) && it(
                     e,
                     "transparent",
                     /*transparent*/
                     l[9]
                 ), c & /*disabled, _color*/
                 4224 && Rr(e, "color", ! /*disabled*/
                     l[7] && /*_color*/
@@ -829,26 +829,26 @@
                     e,
                     "margin-left",
                     /*offset*/
                     l[11] + "px"
                 );
         },
         i(l) {
-            s || (Ku(i.$$.fragment, l), s = !0);
+            s || (Ju(i.$$.fragment, l), s = !0);
         },
         o(l) {
-            ju(i.$$.fragment, l), s = !1;
+            Qu(i.$$.fragment, l), s = !1;
         },
         d(l) {
-            l && Qa(e), h && h.d(), Wu(i), a = !1, n();
+            l && el(e), h && h.d(), Vu(i), a = !1, n();
         }
     };
 }
 
-function Qu(d, e, t) {
+function tc(d, e, t) {
     let r, {
             Icon: i
         } = e,
         {
             label: s = ""
         } = e,
         {
@@ -878,22 +878,22 @@
         {
             transparent: _ = !1
         } = e,
         {
             background: v = "var(--background-fill-primary)"
         } = e,
         {
-            offset: N = 0
+            offset: A = 0
         } = e;
 
-    function B(x) {
-        zu.call(this, d, x);
+    function T(k) {
+        Wu.call(this, d, k);
     }
-    return d.$$set = (x) => {
-        "Icon" in x && t(0, i = x.Icon), "label" in x && t(1, s = x.label), "show_label" in x && t(2, a = x.show_label), "pending" in x && t(3, n = x.pending), "size" in x && t(4, h = x.size), "padded" in x && t(5, l = x.padded), "highlight" in x && t(6, c = x.highlight), "disabled" in x && t(7, u = x.disabled), "hasPopup" in x && t(8, g = x.hasPopup), "color" in x && t(13, m = x.color), "transparent" in x && t(9, _ = x.transparent), "background" in x && t(10, v = x.background), "offset" in x && t(11, N = x.offset);
+    return d.$$set = (k) => {
+        "Icon" in k && t(0, i = k.Icon), "label" in k && t(1, s = k.label), "show_label" in k && t(2, a = k.show_label), "pending" in k && t(3, n = k.pending), "size" in k && t(4, h = k.size), "padded" in k && t(5, l = k.padded), "highlight" in k && t(6, c = k.highlight), "disabled" in k && t(7, u = k.disabled), "hasPopup" in k && t(8, g = k.hasPopup), "color" in k && t(13, m = k.color), "transparent" in k && t(9, _ = k.transparent), "background" in k && t(10, v = k.background), "offset" in k && t(11, A = k.offset);
     }, d.$$.update = () => {
         d.$$.dirty & /*highlight, color*/
             8256 && t(12, r = c ? "var(--color-accent)" : m);
     }, [
         i,
         s,
         a,
@@ -901,23 +901,23 @@
         h,
         l,
         c,
         u,
         g,
         _,
         v,
-        N,
+        A,
         r,
         m,
-        B
+        T
     ];
 }
-class tl extends Fu {
+class rl extends Hu {
     constructor(e) {
-        super(), qu(this, e, Qu, Ju, Yu, {
+        super(), Xu(this, e, tc, ec, Uu, {
             Icon: 0,
             label: 1,
             show_label: 2,
             pending: 3,
             size: 4,
             padded: 5,
             highlight: 6,
@@ -927,83 +927,83 @@
             transparent: 9,
             background: 10,
             offset: 11
         });
     }
 }
 const {
-    SvelteComponent: ec,
-    append: kn,
+    SvelteComponent: rc,
+    append: xn,
     attr: Nt,
-    detach: tc,
-    init: rc,
-    insert: ic,
-    noop: Rn,
-    safe_not_equal: nc,
-    set_style: Bt,
+    detach: ic,
+    init: nc,
+    insert: sc,
+    noop: Tn,
+    safe_not_equal: ac,
+    set_style: Dt,
     svg_element: yi
 } = window.__gradio__svelte__internal;
 
-function sc(d) {
+function lc(d) {
     let e, t, r, i;
     return {
         c() {
-            e = yi("svg"), t = yi("g"), r = yi("path"), i = yi("path"), Nt(r, "d", "M18,6L6.087,17.913"), Bt(r, "fill", "none"), Bt(r, "fill-rule", "nonzero"), Bt(r, "stroke-width", "2px"), Nt(t, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Nt(i, "d", "M4.364,4.364L19.636,19.636"), Bt(i, "fill", "none"), Bt(i, "fill-rule", "nonzero"), Bt(i, "stroke-width", "2px"), Nt(e, "width", "100%"), Nt(e, "height", "100%"), Nt(e, "viewBox", "0 0 24 24"), Nt(e, "version", "1.1"), Nt(e, "xmlns", "http://www.w3.org/2000/svg"), Nt(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Nt(e, "xml:space", "preserve"), Nt(e, "stroke", "currentColor"), Bt(e, "fill-rule", "evenodd"), Bt(e, "clip-rule", "evenodd"), Bt(e, "stroke-linecap", "round"), Bt(e, "stroke-linejoin", "round");
+            e = yi("svg"), t = yi("g"), r = yi("path"), i = yi("path"), Nt(r, "d", "M18,6L6.087,17.913"), Dt(r, "fill", "none"), Dt(r, "fill-rule", "nonzero"), Dt(r, "stroke-width", "2px"), Nt(t, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Nt(i, "d", "M4.364,4.364L19.636,19.636"), Dt(i, "fill", "none"), Dt(i, "fill-rule", "nonzero"), Dt(i, "stroke-width", "2px"), Nt(e, "width", "100%"), Nt(e, "height", "100%"), Nt(e, "viewBox", "0 0 24 24"), Nt(e, "version", "1.1"), Nt(e, "xmlns", "http://www.w3.org/2000/svg"), Nt(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Nt(e, "xml:space", "preserve"), Nt(e, "stroke", "currentColor"), Dt(e, "fill-rule", "evenodd"), Dt(e, "clip-rule", "evenodd"), Dt(e, "stroke-linecap", "round"), Dt(e, "stroke-linejoin", "round");
         },
         m(s, a) {
-            ic(s, e, a), kn(e, t), kn(t, r), kn(e, i);
+            sc(s, e, a), xn(e, t), xn(t, r), xn(e, i);
         },
-        p: Rn,
-        i: Rn,
-        o: Rn,
+        p: Tn,
+        i: Tn,
+        o: Tn,
         d(s) {
-            s && tc(e);
+            s && ic(e);
         }
     };
 }
-class rl extends ec {
+class il extends rc {
     constructor(e) {
-        super(), rc(this, e, null, sc, nc, {});
+        super(), nc(this, e, null, lc, ac, {});
     }
 }
 const {
-    SvelteComponent: ac,
-    append: lc,
+    SvelteComponent: oc,
+    append: hc,
     attr: kt,
-    detach: oc,
-    init: hc,
-    insert: fc,
-    noop: xn,
-    safe_not_equal: uc,
-    svg_element: sa
+    detach: fc,
+    init: uc,
+    insert: cc,
+    noop: En,
+    safe_not_equal: gc,
+    svg_element: la
 } = window.__gradio__svelte__internal;
 
-function cc(d) {
+function dc(d) {
     let e, t;
     return {
         c() {
-            e = sa("svg"), t = sa("path"), kt(t, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), kt(e, "xmlns", "http://www.w3.org/2000/svg"), kt(e, "width", "100%"), kt(e, "height", "100%"), kt(e, "viewBox", "0 0 24 24"), kt(e, "fill", "none"), kt(e, "stroke", "currentColor"), kt(e, "stroke-width", "1.5"), kt(e, "stroke-linecap", "round"), kt(e, "stroke-linejoin", "round"), kt(e, "class", "feather feather-edit-2");
+            e = la("svg"), t = la("path"), kt(t, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), kt(e, "xmlns", "http://www.w3.org/2000/svg"), kt(e, "width", "100%"), kt(e, "height", "100%"), kt(e, "viewBox", "0 0 24 24"), kt(e, "fill", "none"), kt(e, "stroke", "currentColor"), kt(e, "stroke-width", "1.5"), kt(e, "stroke-linecap", "round"), kt(e, "stroke-linejoin", "round"), kt(e, "class", "feather feather-edit-2");
         },
         m(r, i) {
-            fc(r, e, i), lc(e, t);
+            cc(r, e, i), hc(e, t);
         },
-        p: xn,
-        i: xn,
-        o: xn,
+        p: En,
+        i: En,
+        o: En,
         d(r) {
-            r && oc(e);
+            r && fc(e);
         }
     };
 }
-class gc extends ac {
+class pc extends oc {
     constructor(e) {
-        super(), hc(this, e, null, cc, uc, {});
+        super(), uc(this, e, null, dc, gc, {});
     }
 }
-const dc = [{
+const vc = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -1036,15 +1036,15 @@
         primary: 500,
         secondary: 100
     }, {
         color: "pink",
         primary: 600,
         secondary: 100
     }],
-    aa = {
+    oa = {
         inherit: "inherit",
         current: "currentColor",
         transparent: "transparent",
         black: "#000",
         white: "#fff",
         slate: {
             50: "#f8fafc",
@@ -1329,24 +1329,24 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
-dc.reduce(
+vc.reduce(
     (d, {
         color: e,
         primary: t,
         secondary: r
     }) => ({
         ...d,
         [e]: {
-            primary: aa[e][t],
-            secondary: aa[e][r]
+            primary: oa[e][t],
+            secondary: oa[e][r]
         }
     }), {}
 );
 
 function Mr(d) {
     let e = ["", "k", "M", "G", "T", "P", "E", "Z"],
         t = 0;
@@ -1354,50 +1354,50 @@
         d /= 1e3, t++;
     let r = e[t];
     return (Number.isInteger(d) ? d : d.toFixed(1)) + r;
 }
 
 function xi() {}
 
-function pc(d, e) {
+function mc(d, e) {
     return d != d ? e == e : d !== e || d && typeof d == "object" || typeof d == "function";
 }
-const il = typeof window < "u";
-let la = il ? () => window.performance.now() : () => Date.now(),
-    nl = il ? (d) => requestAnimationFrame(d) : xi;
+const nl = typeof window < "u";
+let ha = nl ? () => window.performance.now() : () => Date.now(),
+    sl = nl ? (d) => requestAnimationFrame(d) : xi;
 const Br = /* @__PURE__ */ new Set();
 
-function sl(d) {
+function al(d) {
     Br.forEach((e) => {
         e.c(d) || (Br.delete(e), e.f());
-    }), Br.size !== 0 && nl(sl);
+    }), Br.size !== 0 && sl(al);
 }
 
-function vc(d) {
+function bc(d) {
     let e;
-    return Br.size === 0 && nl(sl), {
+    return Br.size === 0 && sl(al), {
         promise: new Promise((t) => {
             Br.add(e = {
                 c: d,
                 f: t
             });
         }),
         abort() {
             Br.delete(e);
         }
     };
 }
 const xr = [];
 
-function mc(d, e = xi) {
+function wc(d, e = xi) {
     let t;
     const r = /* @__PURE__ */ new Set();
 
     function i(n) {
-        if (pc(d, n) && (d = n, t)) {
+        if (mc(d, n) && (d = n, t)) {
             const h = !xr.length;
             for (const l of r)
                 l[1](), xr.push(l, d);
             if (h) {
                 for (let l = 0; l < xr.length; l += 2)
                     xr[l][0](xr[l + 1]);
                 xr.length = 0;
@@ -1418,183 +1418,183 @@
     return {
         set: i,
         update: s,
         subscribe: a
     };
 }
 
-function oa(d) {
+function fa(d) {
     return Object.prototype.toString.call(d) === "[object Date]";
 }
 
-function zn(d, e, t, r) {
-    if (typeof t == "number" || oa(t)) {
+function qn(d, e, t, r) {
+    if (typeof t == "number" || fa(t)) {
         const i = r - t,
             s = (t - e) / (d.dt || 1 / 60),
             a = d.opts.stiffness * i,
             n = d.opts.damping * s,
             h = (a - n) * d.inv_mass,
             l = (s + h) * d.dt;
-        return Math.abs(l) < d.opts.precision && Math.abs(i) < d.opts.precision ? r : (d.settled = !1, oa(t) ? new Date(t.getTime() + l) : t + l);
+        return Math.abs(l) < d.opts.precision && Math.abs(i) < d.opts.precision ? r : (d.settled = !1, fa(t) ? new Date(t.getTime() + l) : t + l);
     } else {
         if (Array.isArray(t))
             return t.map(
-                (i, s) => zn(d, e[s], t[s], r[s])
+                (i, s) => qn(d, e[s], t[s], r[s])
             );
         if (typeof t == "object") {
             const i = {};
             for (const s in t)
-                i[s] = zn(d, e[s], t[s], r[s]);
+                i[s] = qn(d, e[s], t[s], r[s]);
             return i;
         } else
             throw new Error(`Cannot spring ${typeof t} values`);
     }
 }
 
-function ha(d, e = {}) {
-    const t = mc(d),
+function ua(d, e = {}) {
+    const t = wc(d),
         {
             stiffness: r = 0.15,
             damping: i = 0.8,
             precision: s = 0.01
         } = e;
     let a, n, h, l = d,
         c = d,
         u = 1,
         g = 0,
         m = !1;
 
-    function _(N, B = {}) {
-        c = N;
-        const x = h = {};
-        return d == null || B.hard || v.stiffness >= 1 && v.damping >= 1 ? (m = !0, a = la(), l = N, t.set(d = c), Promise.resolve()) : (B.soft && (g = 1 / ((B.soft === !0 ? 0.5 : +B.soft) * 60), u = 0), n || (a = la(), m = !1, n = vc((L) => {
+    function _(A, T = {}) {
+        c = A;
+        const k = h = {};
+        return d == null || T.hard || v.stiffness >= 1 && v.damping >= 1 ? (m = !0, a = ha(), l = A, t.set(d = c), Promise.resolve()) : (T.soft && (g = 1 / ((T.soft === !0 ? 0.5 : +T.soft) * 60), u = 0), n || (a = ha(), m = !1, n = bc((x) => {
             if (m)
                 return m = !1, n = null, !1;
             u = Math.min(u + g, 1);
-            const k = {
+            const R = {
                     inv_mass: u,
                     opts: v,
                     settled: !0,
-                    dt: (L - a) * 60 / 1e3
+                    dt: (x - a) * 60 / 1e3
                 },
-                z = zn(k, l, d, c);
-            return a = L, l = d, t.set(d = z), k.settled && (n = null), !k.settled;
-        })), new Promise((L) => {
+                O = qn(R, l, d, c);
+            return a = x, l = d, t.set(d = O), R.settled && (n = null), !R.settled;
+        })), new Promise((x) => {
             n.promise.then(() => {
-                x === h && L();
+                k === h && x();
             });
         }));
     }
     const v = {
         set: _,
-        update: (N, B) => _(N(c, d), B),
+        update: (A, T) => _(A(c, d), T),
         subscribe: t.subscribe,
         stiffness: r,
         damping: i,
         precision: s
     };
     return v;
 }
 const {
-    SvelteComponent: bc,
+    SvelteComponent: yc,
     append: Rt,
     attr: ge,
-    component_subscribe: fa,
-    detach: wc,
-    element: yc,
-    init: _c,
-    insert: Sc,
-    noop: ua,
-    safe_not_equal: Cc,
+    component_subscribe: ca,
+    detach: _c,
+    element: Sc,
+    init: Cc,
+    insert: Ac,
+    noop: ga,
+    safe_not_equal: Nc,
     set_style: _i,
     svg_element: xt,
-    toggle_class: ca
+    toggle_class: da
 } = window.__gradio__svelte__internal, {
-    onMount: Ac
+    onMount: kc
 } = window.__gradio__svelte__internal;
 
-function Nc(d) {
+function Rc(d) {
     let e, t, r, i, s, a, n, h, l, c, u, g;
     return {
         c() {
-            e = yc("div"), t = xt("svg"), r = xt("g"), i = xt("path"), s = xt("path"), a = xt("path"), n = xt("path"), h = xt("g"), l = xt("path"), c = xt("path"), u = xt("path"), g = xt("path"), ge(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), ge(i, "fill", "#FF7C00"), ge(i, "fill-opacity", "0.4"), ge(i, "class", "svelte-43sxxs"), ge(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), ge(s, "fill", "#FF7C00"), ge(s, "class", "svelte-43sxxs"), ge(a, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), ge(a, "fill", "#FF7C00"), ge(a, "fill-opacity", "0.4"), ge(a, "class", "svelte-43sxxs"), ge(n, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), ge(n, "fill", "#FF7C00"), ge(n, "class", "svelte-43sxxs"), _i(r, "transform", "translate(" + /*$top*/
+            e = Sc("div"), t = xt("svg"), r = xt("g"), i = xt("path"), s = xt("path"), a = xt("path"), n = xt("path"), h = xt("g"), l = xt("path"), c = xt("path"), u = xt("path"), g = xt("path"), ge(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), ge(i, "fill", "#FF7C00"), ge(i, "fill-opacity", "0.4"), ge(i, "class", "svelte-43sxxs"), ge(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), ge(s, "fill", "#FF7C00"), ge(s, "class", "svelte-43sxxs"), ge(a, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), ge(a, "fill", "#FF7C00"), ge(a, "fill-opacity", "0.4"), ge(a, "class", "svelte-43sxxs"), ge(n, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), ge(n, "fill", "#FF7C00"), ge(n, "class", "svelte-43sxxs"), _i(r, "transform", "translate(" + /*$top*/
                 d[1][0] + "px, " + /*$top*/
                 d[1][1] + "px)"), ge(l, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), ge(l, "fill", "#FF7C00"), ge(l, "fill-opacity", "0.4"), ge(l, "class", "svelte-43sxxs"), ge(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), ge(c, "fill", "#FF7C00"), ge(c, "class", "svelte-43sxxs"), ge(u, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), ge(u, "fill", "#FF7C00"), ge(u, "fill-opacity", "0.4"), ge(u, "class", "svelte-43sxxs"), ge(g, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), ge(g, "fill", "#FF7C00"), ge(g, "class", "svelte-43sxxs"), _i(h, "transform", "translate(" + /*$bottom*/
                 d[2][0] + "px, " + /*$bottom*/
-                d[2][1] + "px)"), ge(t, "viewBox", "-1200 -1200 3000 3000"), ge(t, "fill", "none"), ge(t, "xmlns", "http://www.w3.org/2000/svg"), ge(t, "class", "svelte-43sxxs"), ge(e, "class", "svelte-43sxxs"), ca(
+                d[2][1] + "px)"), ge(t, "viewBox", "-1200 -1200 3000 3000"), ge(t, "fill", "none"), ge(t, "xmlns", "http://www.w3.org/2000/svg"), ge(t, "class", "svelte-43sxxs"), ge(e, "class", "svelte-43sxxs"), da(
                 e,
                 "margin",
                 /*margin*/
                 d[0]
             );
         },
         m(m, _) {
-            Sc(m, e, _), Rt(e, t), Rt(t, r), Rt(r, i), Rt(r, s), Rt(r, a), Rt(r, n), Rt(t, h), Rt(h, l), Rt(h, c), Rt(h, u), Rt(h, g);
+            Ac(m, e, _), Rt(e, t), Rt(t, r), Rt(r, i), Rt(r, s), Rt(r, a), Rt(r, n), Rt(t, h), Rt(h, l), Rt(h, c), Rt(h, u), Rt(h, g);
         },
         p(m, [_]) {
             _ & /*$top*/
                 2 && _i(r, "transform", "translate(" + /*$top*/
                     m[1][0] + "px, " + /*$top*/
                     m[1][1] + "px)"), _ & /*$bottom*/
                 4 && _i(h, "transform", "translate(" + /*$bottom*/
                     m[2][0] + "px, " + /*$bottom*/
                     m[2][1] + "px)"), _ & /*margin*/
-                1 && ca(
+                1 && da(
                     e,
                     "margin",
                     /*margin*/
                     m[0]
                 );
         },
-        i: ua,
-        o: ua,
+        i: ga,
+        o: ga,
         d(m) {
-            m && wc(e);
+            m && _c(e);
         }
     };
 }
 
-function kc(d, e, t) {
+function xc(d, e, t) {
     let r, i;
-    var s = this && this.__awaiter || function(m, _, v, N) {
-        function B(x) {
-            return x instanceof v ? x : new v(function(L) {
-                L(x);
+    var s = this && this.__awaiter || function(m, _, v, A) {
+        function T(k) {
+            return k instanceof v ? k : new v(function(x) {
+                x(k);
             });
         }
-        return new(v || (v = Promise))(function(x, L) {
-            function k(Y) {
+        return new(v || (v = Promise))(function(k, x) {
+            function R(te) {
                 try {
-                    D(N.next(Y));
-                } catch (O) {
-                    L(O);
+                    D(A.next(te));
+                } catch (q) {
+                    x(q);
                 }
             }
 
-            function z(Y) {
+            function O(te) {
                 try {
-                    D(N.throw(Y));
-                } catch (O) {
-                    L(O);
+                    D(A.throw(te));
+                } catch (q) {
+                    x(q);
                 }
             }
 
-            function D(Y) {
-                Y.done ? x(Y.value) : B(Y.value).then(k, z);
+            function D(te) {
+                te.done ? k(te.value) : T(te.value).then(R, O);
             }
-            D((N = N.apply(m, _ || [])).next());
+            D((A = A.apply(m, _ || [])).next());
         });
     };
     let {
         margin: a = !0
     } = e;
-    const n = ha([0, 0]);
-    fa(d, n, (m) => t(1, r = m));
-    const h = ha([0, 0]);
-    fa(d, h, (m) => t(2, i = m));
+    const n = ua([0, 0]);
+    ca(d, n, (m) => t(1, r = m));
+    const h = ua([0, 0]);
+    ca(d, h, (m) => t(2, i = m));
     let l;
 
     function c() {
         return s(this, void 0, void 0, function*() {
             yield Promise.all([n.set([125, 140]), h.set([-125, -140])]), yield Promise.all([n.set([-125, 140]), h.set([125, -140])]), yield Promise.all([n.set([-125, 0]), h.set([125, -0])]), yield Promise.all([n.set([125, 0]), h.set([-125, 0])]);
         });
     }
@@ -1606,82 +1606,82 @@
     }
 
     function g() {
         return s(this, void 0, void 0, function*() {
             yield Promise.all([n.set([125, 0]), h.set([-125, 0])]), u();
         });
     }
-    return Ac(() => (g(), () => l = !0)), d.$$set = (m) => {
+    return kc(() => (g(), () => l = !0)), d.$$set = (m) => {
         "margin" in m && t(0, a = m.margin);
     }, [a, r, i, n, h];
 }
-class Rc extends bc {
+class Tc extends yc {
     constructor(e) {
-        super(), _c(this, e, kc, Nc, Cc, {
+        super(), Cc(this, e, xc, Rc, Nc, {
             margin: 0
         });
     }
 }
 const {
-    SvelteComponent: xc,
+    SvelteComponent: Ec,
     append: gr,
-    attr: Tt,
-    binding_callbacks: ga,
-    check_outros: al,
-    create_component: ll,
-    create_slot: Tc,
-    destroy_component: ol,
-    destroy_each: hl,
+    attr: Et,
+    binding_callbacks: pa,
+    check_outros: ll,
+    create_component: ol,
+    create_slot: Lc,
+    destroy_component: hl,
+    destroy_each: fl,
     detach: ie,
     element: $t,
     empty: Ir,
     ensure_array_like: Ei,
-    get_all_dirty_from_scope: Ec,
-    get_slot_changes: Lc,
-    group_outros: fl,
-    init: Mc,
+    get_all_dirty_from_scope: Mc,
+    get_slot_changes: Bc,
+    group_outros: ul,
+    init: Dc,
     insert: ne,
-    mount_component: ul,
-    noop: Hn,
-    safe_not_equal: Bc,
+    mount_component: cl,
+    noop: Vn,
+    safe_not_equal: Pc,
     set_data: bt,
-    set_style: sr,
-    space: Et,
+    set_style: nr,
+    space: Lt,
     text: Re,
-    toggle_class: mt,
+    toggle_class: pt,
     transition_in: dr,
     transition_out: pr,
-    update_slot_base: Dc
+    update_slot_base: $c
 } = window.__gradio__svelte__internal, {
-    tick: Pc
+    tick: Ic
 } = window.__gradio__svelte__internal, {
-    onDestroy: $c
+    onDestroy: Oc
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: Ic
-} = window.__gradio__svelte__internal, Oc = (d) => ({}), da = (d) => ({});
+    createEventDispatcher: Fc
+} = window.__gradio__svelte__internal, zc = (d) => ({}), va = (d) => ({});
 
-function pa(d, e, t) {
+function ma(d, e, t) {
     const r = d.slice();
     return r[41] = e[t], r[43] = t, r;
 }
 
-function va(d, e, t) {
+function ba(d, e, t) {
     const r = d.slice();
     return r[41] = e[t], r;
 }
 
-function Fc(d) {
+function Hc(d) {
     let e, t, r, i, s = (
             /*i18n*/
             d[1]("common.error") + ""
         ),
         a, n, h;
-    t = new tl({
+    t = new rl({
         props: {
-            Icon: rl,
+            Icon: il,
             label: (
                 /*i18n*/
                 d[1]("common.clear")
             ),
             disabled: !1
         }
     }), t.$on(
@@ -1689,205 +1689,205 @@
         /*click_handler*/
         d[32]
     );
     const l = (
             /*#slots*/
             d[30].error
         ),
-        c = Tc(
+        c = Lc(
             l,
             d,
             /*$$scope*/
             d[29],
-            da
+            va
         );
     return {
         c() {
-            e = $t("div"), ll(t.$$.fragment), r = Et(), i = $t("span"), a = Re(s), n = Et(), c && c.c(), Tt(e, "class", "clear-status svelte-1yk38uw"), Tt(i, "class", "error svelte-1yk38uw");
+            e = $t("div"), ol(t.$$.fragment), r = Lt(), i = $t("span"), a = Re(s), n = Lt(), c && c.c(), Et(e, "class", "clear-status svelte-1yk38uw"), Et(i, "class", "error svelte-1yk38uw");
         },
         m(u, g) {
-            ne(u, e, g), ul(t, e, null), ne(u, r, g), ne(u, i, g), gr(i, a), ne(u, n, g), c && c.m(u, g), h = !0;
+            ne(u, e, g), cl(t, e, null), ne(u, r, g), ne(u, i, g), gr(i, a), ne(u, n, g), c && c.m(u, g), h = !0;
         },
         p(u, g) {
             const m = {};
             g[0] & /*i18n*/
                 2 && (m.label = /*i18n*/
                     u[1]("common.clear")), t.$set(m), (!h || g[0] & /*i18n*/
                     2) && s !== (s = /*i18n*/
                     u[1]("common.error") + "") && bt(a, s), c && c.p && (!h || g[0] & /*$$scope*/
-                    536870912) && Dc(
+                    536870912) && $c(
                     c,
                     l,
                     u,
                     /*$$scope*/
                     u[29],
-                    h ? Lc(
+                    h ? Bc(
                         l,
                         /*$$scope*/
                         u[29],
                         g,
-                        Oc
-                    ) : Ec(
+                        zc
+                    ) : Mc(
                         /*$$scope*/
                         u[29]
                     ),
-                    da
+                    va
                 );
         },
         i(u) {
             h || (dr(t.$$.fragment, u), dr(c, u), h = !0);
         },
         o(u) {
             pr(t.$$.fragment, u), pr(c, u), h = !1;
         },
         d(u) {
-            u && (ie(e), ie(r), ie(i), ie(n)), ol(t), c && c.d(u);
+            u && (ie(e), ie(r), ie(i), ie(n)), hl(t), c && c.d(u);
         }
     };
 }
 
-function zc(d) {
+function Wc(d) {
     let e, t, r, i, s, a, n, h, l, c = (
         /*variant*/
         d[8] === "default" && /*show_eta_bar*/
         d[18] && /*show_progress*/
-        d[6] === "full" && ma(d)
+        d[6] === "full" && wa(d)
     );
 
-    function u(L, k) {
+    function u(x, R) {
         if (
             /*progress*/
-            L[7]
+            x[7]
         )
-            return qc;
+            return Xc;
         if (
             /*queue_position*/
-            L[2] !== null && /*queue_size*/
-            L[3] !== void 0 && /*queue_position*/
-            L[2] >= 0
+            x[2] !== null && /*queue_size*/
+            x[3] !== void 0 && /*queue_position*/
+            x[2] >= 0
         )
-            return Wc;
+            return Vc;
         if (
             /*queue_position*/
-            L[2] === 0
+            x[2] === 0
         )
-            return Hc;
+            return qc;
     }
     let g = u(d),
         m = g && g(d),
         _ = (
             /*timer*/
-            d[5] && ya(d)
+            d[5] && Sa(d)
         );
-    const v = [Gc, Yc],
-        N = [];
+    const v = [Zc, Uc],
+        A = [];
 
-    function B(L, k) {
+    function T(x, R) {
         return (
             /*last_progress_level*/
-            L[15] != null ? 0 : (
+            x[15] != null ? 0 : (
                 /*show_progress*/
-                L[6] === "full" ? 1 : -1
+                x[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(s = B(d)) && (a = N[s] = v[s](d));
-    let x = ! /*timer*/
-        d[5] && Ra(d);
+    ~(s = T(d)) && (a = A[s] = v[s](d));
+    let k = ! /*timer*/
+        d[5] && Ta(d);
     return {
         c() {
-            c && c.c(), e = Et(), t = $t("div"), m && m.c(), r = Et(), _ && _.c(), i = Et(), a && a.c(), n = Et(), x && x.c(), h = Ir(), Tt(t, "class", "progress-text svelte-1yk38uw"), mt(
+            c && c.c(), e = Lt(), t = $t("div"), m && m.c(), r = Lt(), _ && _.c(), i = Lt(), a && a.c(), n = Lt(), k && k.c(), h = Ir(), Et(t, "class", "progress-text svelte-1yk38uw"), pt(
                 t,
                 "meta-text-center",
                 /*variant*/
                 d[8] === "center"
-            ), mt(
+            ), pt(
                 t,
                 "meta-text",
                 /*variant*/
                 d[8] === "default"
             );
         },
-        m(L, k) {
-            c && c.m(L, k), ne(L, e, k), ne(L, t, k), m && m.m(t, null), gr(t, r), _ && _.m(t, null), ne(L, i, k), ~s && N[s].m(L, k), ne(L, n, k), x && x.m(L, k), ne(L, h, k), l = !0;
+        m(x, R) {
+            c && c.m(x, R), ne(x, e, R), ne(x, t, R), m && m.m(t, null), gr(t, r), _ && _.m(t, null), ne(x, i, R), ~s && A[s].m(x, R), ne(x, n, R), k && k.m(x, R), ne(x, h, R), l = !0;
         },
-        p(L, k) {
+        p(x, R) {
             /*variant*/
-            L[8] === "default" && /*show_eta_bar*/
-                L[18] && /*show_progress*/
-                L[6] === "full" ? c ? c.p(L, k) : (c = ma(L), c.c(), c.m(e.parentNode, e)) : c && (c.d(1), c = null), g === (g = u(L)) && m ? m.p(L, k) : (m && m.d(1), m = g && g(L), m && (m.c(), m.m(t, r))), /*timer*/
-                L[5] ? _ ? _.p(L, k) : (_ = ya(L), _.c(), _.m(t, null)) : _ && (_.d(1), _ = null), (!l || k[0] & /*variant*/
-                    256) && mt(
+            x[8] === "default" && /*show_eta_bar*/
+                x[18] && /*show_progress*/
+                x[6] === "full" ? c ? c.p(x, R) : (c = wa(x), c.c(), c.m(e.parentNode, e)) : c && (c.d(1), c = null), g === (g = u(x)) && m ? m.p(x, R) : (m && m.d(1), m = g && g(x), m && (m.c(), m.m(t, r))), /*timer*/
+                x[5] ? _ ? _.p(x, R) : (_ = Sa(x), _.c(), _.m(t, null)) : _ && (_.d(1), _ = null), (!l || R[0] & /*variant*/
+                    256) && pt(
                     t,
                     "meta-text-center",
                     /*variant*/
-                    L[8] === "center"
-                ), (!l || k[0] & /*variant*/
-                    256) && mt(
+                    x[8] === "center"
+                ), (!l || R[0] & /*variant*/
+                    256) && pt(
                     t,
                     "meta-text",
                     /*variant*/
-                    L[8] === "default"
+                    x[8] === "default"
                 );
-            let z = s;
-            s = B(L), s === z ? ~s && N[s].p(L, k) : (a && (fl(), pr(N[z], 1, 1, () => {
-                    N[z] = null;
-                }), al()), ~s ? (a = N[s], a ? a.p(L, k) : (a = N[s] = v[s](L), a.c()), dr(a, 1), a.m(n.parentNode, n)) : a = null), /*timer*/
-                L[5] ? x && (x.d(1), x = null) : x ? x.p(L, k) : (x = Ra(L), x.c(), x.m(h.parentNode, h));
+            let O = s;
+            s = T(x), s === O ? ~s && A[s].p(x, R) : (a && (ul(), pr(A[O], 1, 1, () => {
+                    A[O] = null;
+                }), ll()), ~s ? (a = A[s], a ? a.p(x, R) : (a = A[s] = v[s](x), a.c()), dr(a, 1), a.m(n.parentNode, n)) : a = null), /*timer*/
+                x[5] ? k && (k.d(1), k = null) : k ? k.p(x, R) : (k = Ta(x), k.c(), k.m(h.parentNode, h));
         },
-        i(L) {
+        i(x) {
             l || (dr(a), l = !0);
         },
-        o(L) {
+        o(x) {
             pr(a), l = !1;
         },
-        d(L) {
-            L && (ie(e), ie(t), ie(i), ie(n), ie(h)), c && c.d(L), m && m.d(), _ && _.d(), ~s && N[s].d(L), x && x.d(L);
+        d(x) {
+            x && (ie(e), ie(t), ie(i), ie(n), ie(h)), c && c.d(x), m && m.d(), _ && _.d(), ~s && A[s].d(x), k && k.d(x);
         }
     };
 }
 
-function ma(d) {
+function wa(d) {
     let e, t = `translateX(${/*eta_level*/
   (d[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            e = $t("div"), Tt(e, "class", "eta-bar svelte-1yk38uw"), sr(e, "transform", t);
+            e = $t("div"), Et(e, "class", "eta-bar svelte-1yk38uw"), nr(e, "transform", t);
         },
         m(r, i) {
             ne(r, e, i);
         },
         p(r, i) {
             i[0] & /*eta_level*/
                 131072 && t !== (t = `translateX(${/*eta_level*/
-      (r[17] || 0) * 100 - 100}%)`) && sr(e, "transform", t);
+      (r[17] || 0) * 100 - 100}%)`) && nr(e, "transform", t);
         },
         d(r) {
             r && ie(e);
         }
     };
 }
 
-function Hc(d) {
+function qc(d) {
     let e;
     return {
         c() {
             e = Re("processing |");
         },
         m(t, r) {
             ne(t, e, r);
         },
-        p: Hn,
+        p: Vn,
         d(t) {
             t && ie(e);
         }
     };
 }
 
-function Wc(d) {
+function Vc(d) {
     let e, t = (
             /*queue_position*/
             d[2] + 1 + ""
         ),
         r, i, s, a;
     return {
         c() {
@@ -1911,22 +1911,22 @@
         },
         d(n) {
             n && (ie(e), ie(r), ie(i), ie(s), ie(a));
         }
     };
 }
 
-function qc(d) {
+function Xc(d) {
     let e, t = Ei(
             /*progress*/
             d[7]
         ),
         r = [];
     for (let i = 0; i < t.length; i += 1)
-        r[i] = wa(va(d, t, i));
+        r[i] = _a(ba(d, t, i));
     return {
         c() {
             for (let i = 0; i < r.length; i += 1)
                 r[i].c();
             e = Ir();
         },
         m(i, s) {
@@ -1939,47 +1939,47 @@
                 128) {
                 t = Ei(
                     /*progress*/
                     i[7]
                 );
                 let a;
                 for (a = 0; a < t.length; a += 1) {
-                    const n = va(i, t, a);
-                    r[a] ? r[a].p(n, s) : (r[a] = wa(n), r[a].c(), r[a].m(e.parentNode, e));
+                    const n = ba(i, t, a);
+                    r[a] ? r[a].p(n, s) : (r[a] = _a(n), r[a].c(), r[a].m(e.parentNode, e));
                 }
                 for (; a < r.length; a += 1)
                     r[a].d(1);
                 r.length = t.length;
             }
         },
         d(i) {
-            i && ie(e), hl(r, i);
+            i && ie(e), fl(r, i);
         }
     };
 }
 
-function ba(d) {
+function ya(d) {
     let e, t = (
             /*p*/
             d[41].unit + ""
         ),
         r, i, s = " ",
         a;
 
     function n(c, u) {
         return (
             /*p*/
-            c[41].length != null ? Xc : Vc
+            c[41].length != null ? Gc : Yc
         );
     }
     let h = n(d),
         l = h(d);
     return {
         c() {
-            l.c(), e = Et(), r = Re(t), i = Re(" | "), a = Re(s);
+            l.c(), e = Lt(), r = Re(t), i = Re(" | "), a = Re(s);
         },
         m(c, u) {
             l.m(c, u), ne(c, e, u), ne(c, r, u), ne(c, i, u), ne(c, a, u);
         },
         p(c, u) {
             h === (h = n(c)) && l ? l.p(c, u) : (l.d(1), l = h(c), l && (l.c(), l.m(e.parentNode, e))), u[0] & /*progress*/
                 128 && t !== (t = /*p*/
@@ -1987,15 +1987,15 @@
         },
         d(c) {
             c && (ie(e), ie(r), ie(i), ie(a)), l.d(c);
         }
     };
 }
 
-function Vc(d) {
+function Yc(d) {
     let e = Mr(
             /*p*/
             d[41].index || 0
         ) + "",
         t;
     return {
         c() {
@@ -2013,15 +2013,15 @@
         },
         d(r) {
             r && ie(t);
         }
     };
 }
 
-function Xc(d) {
+function Gc(d) {
     let e = Mr(
             /*p*/
             d[41].index || 0
         ) + "",
         t, r, i = Mr(
             /*p*/
             d[41].length
@@ -2047,37 +2047,37 @@
         },
         d(a) {
             a && (ie(t), ie(r), ie(s));
         }
     };
 }
 
-function wa(d) {
+function _a(d) {
     let e, t = (
         /*p*/
-        d[41].index != null && ba(d)
+        d[41].index != null && ya(d)
     );
     return {
         c() {
             t && t.c(), e = Ir();
         },
         m(r, i) {
             t && t.m(r, i), ne(r, e, i);
         },
         p(r, i) {
             /*p*/
-            r[41].index != null ? t ? t.p(r, i) : (t = ba(r), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+            r[41].index != null ? t ? t.p(r, i) : (t = ya(r), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(r) {
             r && ie(e), t && t.d(r);
         }
     };
 }
 
-function ya(d) {
+function Sa(d) {
     let e, t = (
             /*eta*/
             d[0] ? `/${/*formatted_eta*/
     d[19]}` : ""
         ),
         r, i;
     return {
@@ -2103,84 +2103,84 @@
         },
         d(s) {
             s && (ie(e), ie(r), ie(i));
         }
     };
 }
 
-function Yc(d) {
+function Uc(d) {
     let e, t;
-    return e = new Rc({
+    return e = new Tc({
         props: {
             margin: (
                 /*variant*/
                 d[8] === "default"
             )
         }
     }), {
         c() {
-            ll(e.$$.fragment);
+            ol(e.$$.fragment);
         },
         m(r, i) {
-            ul(e, r, i), t = !0;
+            cl(e, r, i), t = !0;
         },
         p(r, i) {
             const s = {};
             i[0] & /*variant*/
                 256 && (s.margin = /*variant*/
                     r[8] === "default"), e.$set(s);
         },
         i(r) {
             t || (dr(e.$$.fragment, r), t = !0);
         },
         o(r) {
             pr(e.$$.fragment, r), t = !1;
         },
         d(r) {
-            ol(e, r);
+            hl(e, r);
         }
     };
 }
 
-function Gc(d) {
+function Zc(d) {
     let e, t, r, i, s, a = `${/*last_progress_level*/
   d[15] * 100}%`,
         n = (
             /*progress*/
-            d[7] != null && _a(d)
+            d[7] != null && Ca(d)
         );
     return {
         c() {
-            e = $t("div"), t = $t("div"), n && n.c(), r = Et(), i = $t("div"), s = $t("div"), Tt(t, "class", "progress-level-inner svelte-1yk38uw"), Tt(s, "class", "progress-bar svelte-1yk38uw"), sr(s, "width", a), Tt(i, "class", "progress-bar-wrap svelte-1yk38uw"), Tt(e, "class", "progress-level svelte-1yk38uw");
+            e = $t("div"), t = $t("div"), n && n.c(), r = Lt(), i = $t("div"), s = $t("div"), Et(t, "class", "progress-level-inner svelte-1yk38uw"), Et(s, "class", "progress-bar svelte-1yk38uw"), nr(s, "width", a), Et(i, "class", "progress-bar-wrap svelte-1yk38uw"), Et(e, "class", "progress-level svelte-1yk38uw");
         },
         m(h, l) {
             ne(h, e, l), gr(e, t), n && n.m(t, null), gr(e, r), gr(e, i), gr(i, s), d[31](s);
         },
         p(h, l) {
             /*progress*/
-            h[7] != null ? n ? n.p(h, l) : (n = _a(h), n.c(), n.m(t, null)) : n && (n.d(1), n = null), l[0] & /*last_progress_level*/
+            h[7] != null ? n ? n.p(h, l) : (n = Ca(h), n.c(), n.m(t, null)) : n && (n.d(1), n = null), l[0] & /*last_progress_level*/
                 32768 && a !== (a = `${/*last_progress_level*/
-      h[15] * 100}%`) && sr(s, "width", a);
+      h[15] * 100}%`) && nr(s, "width", a);
         },
-        i: Hn,
-        o: Hn,
+        i: Vn,
+        o: Vn,
         d(h) {
             h && ie(e), n && n.d(), d[31](null);
         }
     };
 }
 
-function _a(d) {
+function Ca(d) {
     let e, t = Ei(
             /*progress*/
             d[7]
         ),
         r = [];
     for (let i = 0; i < t.length; i += 1)
-        r[i] = ka(pa(d, t, i));
+        r[i] = xa(ma(d, t, i));
     return {
         c() {
             for (let i = 0; i < r.length; i += 1)
                 r[i].c();
             e = Ir();
         },
         m(i, s) {
@@ -2193,90 +2193,90 @@
                 16512) {
                 t = Ei(
                     /*progress*/
                     i[7]
                 );
                 let a;
                 for (a = 0; a < t.length; a += 1) {
-                    const n = pa(i, t, a);
-                    r[a] ? r[a].p(n, s) : (r[a] = ka(n), r[a].c(), r[a].m(e.parentNode, e));
+                    const n = ma(i, t, a);
+                    r[a] ? r[a].p(n, s) : (r[a] = xa(n), r[a].c(), r[a].m(e.parentNode, e));
                 }
                 for (; a < r.length; a += 1)
                     r[a].d(1);
                 r.length = t.length;
             }
         },
         d(i) {
-            i && ie(e), hl(r, i);
+            i && ie(e), fl(r, i);
         }
     };
 }
 
-function Sa(d) {
+function Aa(d) {
     let e, t, r, i, s = (
             /*i*/
-            d[43] !== 0 && Uc()
+            d[43] !== 0 && Kc()
         ),
         a = (
             /*p*/
-            d[41].desc != null && Ca(d)
+            d[41].desc != null && Na(d)
         ),
         n = (
             /*p*/
             d[41].desc != null && /*progress_level*/
             d[14] && /*progress_level*/
             d[14][
                 /*i*/
                 d[43]
-            ] != null && Aa()
+            ] != null && ka()
         ),
         h = (
             /*progress_level*/
-            d[14] != null && Na(d)
+            d[14] != null && Ra(d)
         );
     return {
         c() {
-            s && s.c(), e = Et(), a && a.c(), t = Et(), n && n.c(), r = Et(), h && h.c(), i = Ir();
+            s && s.c(), e = Lt(), a && a.c(), t = Lt(), n && n.c(), r = Lt(), h && h.c(), i = Ir();
         },
         m(l, c) {
             s && s.m(l, c), ne(l, e, c), a && a.m(l, c), ne(l, t, c), n && n.m(l, c), ne(l, r, c), h && h.m(l, c), ne(l, i, c);
         },
         p(l, c) {
             /*p*/
-            l[41].desc != null ? a ? a.p(l, c) : (a = Ca(l), a.c(), a.m(t.parentNode, t)) : a && (a.d(1), a = null), /*p*/
+            l[41].desc != null ? a ? a.p(l, c) : (a = Na(l), a.c(), a.m(t.parentNode, t)) : a && (a.d(1), a = null), /*p*/
                 l[41].desc != null && /*progress_level*/
                 l[14] && /*progress_level*/
                 l[14][
                     /*i*/
                     l[43]
-                ] != null ? n || (n = Aa(), n.c(), n.m(r.parentNode, r)) : n && (n.d(1), n = null), /*progress_level*/
-                l[14] != null ? h ? h.p(l, c) : (h = Na(l), h.c(), h.m(i.parentNode, i)) : h && (h.d(1), h = null);
+                ] != null ? n || (n = ka(), n.c(), n.m(r.parentNode, r)) : n && (n.d(1), n = null), /*progress_level*/
+                l[14] != null ? h ? h.p(l, c) : (h = Ra(l), h.c(), h.m(i.parentNode, i)) : h && (h.d(1), h = null);
         },
         d(l) {
             l && (ie(e), ie(t), ie(r), ie(i)), s && s.d(l), a && a.d(l), n && n.d(l), h && h.d(l);
         }
     };
 }
 
-function Uc(d) {
+function Kc(d) {
     let e;
     return {
         c() {
             e = Re(" /");
         },
         m(t, r) {
             ne(t, e, r);
         },
         d(t) {
             t && ie(e);
         }
     };
 }
 
-function Ca(d) {
+function Na(d) {
     let e = (
             /*p*/
             d[41].desc + ""
         ),
         t;
     return {
         c() {
@@ -2292,30 +2292,30 @@
         },
         d(r) {
             r && ie(t);
         }
     };
 }
 
-function Aa(d) {
+function ka(d) {
     let e;
     return {
         c() {
             e = Re("-");
         },
         m(t, r) {
             ne(t, e, r);
         },
         d(t) {
             t && ie(e);
         }
     };
 }
 
-function Na(d) {
+function Ra(d) {
     let e = (100 * /*progress_level*/
             (d[14][
                 /*i*/
                 d[43]
             ] || 0)).toFixed(1) + "",
         t, r;
     return {
@@ -2335,23 +2335,23 @@
         },
         d(i) {
             i && (ie(t), ie(r));
         }
     };
 }
 
-function ka(d) {
+function xa(d) {
     let e, t = (
         /*p*/
         (d[41].desc != null || /*progress_level*/
             d[14] && /*progress_level*/
             d[14][
                 /*i*/
                 d[43]
-            ] != null) && Sa(d)
+            ] != null) && Aa(d)
     );
     return {
         c() {
             t && t.c(), e = Ir();
         },
         m(r, i) {
             t && t.m(r, i), ne(r, e, i);
@@ -2359,30 +2359,30 @@
         p(r, i) {
             /*p*/
             r[41].desc != null || /*progress_level*/
                 r[14] && /*progress_level*/
                 r[14][
                     /*i*/
                     r[43]
-                ] != null ? t ? t.p(r, i) : (t = Sa(r), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+                ] != null ? t ? t.p(r, i) : (t = Aa(r), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(r) {
             r && ie(e), t && t.d(r);
         }
     };
 }
 
-function Ra(d) {
+function Ta(d) {
     let e, t;
     return {
         c() {
             e = $t("p"), t = Re(
                 /*loading_text*/
                 d[9]
-            ), Tt(e, "class", "loading svelte-1yk38uw");
+            ), Et(e, "class", "loading svelte-1yk38uw");
         },
         m(r, i) {
             ne(r, e, i), gr(e, t);
         },
         p(r, i) {
             i[0] & /*loading_text*/
                 512 && bt(
@@ -2393,110 +2393,110 @@
         },
         d(r) {
             r && ie(e);
         }
     };
 }
 
-function Zc(d) {
+function jc(d) {
     let e, t, r, i, s;
-    const a = [zc, Fc],
+    const a = [Wc, Hc],
         n = [];
 
     function h(l, c) {
         return (
             /*status*/
             l[4] === "pending" ? 0 : (
                 /*status*/
                 l[4] === "error" ? 1 : -1
             )
         );
     }
     return ~(t = h(d)) && (r = n[t] = a[t](d)), {
         c() {
-            e = $t("div"), r && r.c(), Tt(e, "class", i = "wrap " + /*variant*/
+            e = $t("div"), r && r.c(), Et(e, "class", i = "wrap " + /*variant*/
                 d[8] + " " + /*show_progress*/
-                d[6] + " svelte-1yk38uw"), mt(e, "hide", ! /*status*/
+                d[6] + " svelte-1yk38uw"), pt(e, "hide", ! /*status*/
                 d[4] || /*status*/
                 d[4] === "complete" || /*show_progress*/
-                d[6] === "hidden"), mt(
+                d[6] === "hidden"), pt(
                 e,
                 "translucent",
                 /*variant*/
                 d[8] === "center" && /*status*/
                 (d[4] === "pending" || /*status*/
                     d[4] === "error") || /*translucent*/
                 d[11] || /*show_progress*/
                 d[6] === "minimal"
-            ), mt(
+            ), pt(
                 e,
                 "generating",
                 /*status*/
                 d[4] === "generating"
-            ), mt(
+            ), pt(
                 e,
                 "border",
                 /*border*/
                 d[12]
-            ), sr(
+            ), nr(
                 e,
                 "position",
                 /*absolute*/
                 d[10] ? "absolute" : "static"
-            ), sr(
+            ), nr(
                 e,
                 "padding",
                 /*absolute*/
                 d[10] ? "0" : "var(--size-8) 0"
             );
         },
         m(l, c) {
             ne(l, e, c), ~t && n[t].m(e, null), d[33](e), s = !0;
         },
         p(l, c) {
             let u = t;
-            t = h(l), t === u ? ~t && n[t].p(l, c) : (r && (fl(), pr(n[u], 1, 1, () => {
+            t = h(l), t === u ? ~t && n[t].p(l, c) : (r && (ul(), pr(n[u], 1, 1, () => {
                     n[u] = null;
-                }), al()), ~t ? (r = n[t], r ? r.p(l, c) : (r = n[t] = a[t](l), r.c()), dr(r, 1), r.m(e, null)) : r = null), (!s || c[0] & /*variant, show_progress*/
+                }), ll()), ~t ? (r = n[t], r ? r.p(l, c) : (r = n[t] = a[t](l), r.c()), dr(r, 1), r.m(e, null)) : r = null), (!s || c[0] & /*variant, show_progress*/
                     320 && i !== (i = "wrap " + /*variant*/
                         l[8] + " " + /*show_progress*/
-                        l[6] + " svelte-1yk38uw")) && Tt(e, "class", i), (!s || c[0] & /*variant, show_progress, status, show_progress*/
-                    336) && mt(e, "hide", ! /*status*/
+                        l[6] + " svelte-1yk38uw")) && Et(e, "class", i), (!s || c[0] & /*variant, show_progress, status, show_progress*/
+                    336) && pt(e, "hide", ! /*status*/
                     l[4] || /*status*/
                     l[4] === "complete" || /*show_progress*/
                     l[6] === "hidden"), (!s || c[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && mt(
+                    2384) && pt(
                     e,
                     "translucent",
                     /*variant*/
                     l[8] === "center" && /*status*/
                     (l[4] === "pending" || /*status*/
                         l[4] === "error") || /*translucent*/
                     l[11] || /*show_progress*/
                     l[6] === "minimal"
                 ), (!s || c[0] & /*variant, show_progress, status*/
-                    336) && mt(
+                    336) && pt(
                     e,
                     "generating",
                     /*status*/
                     l[4] === "generating"
                 ), (!s || c[0] & /*variant, show_progress, border*/
-                    4416) && mt(
+                    4416) && pt(
                     e,
                     "border",
                     /*border*/
                     l[12]
                 ), c[0] & /*absolute*/
-                1024 && sr(
+                1024 && nr(
                     e,
                     "position",
                     /*absolute*/
                     l[10] ? "absolute" : "static"
                 ), c[0] & /*absolute*/
-                1024 && sr(
+                1024 && nr(
                     e,
                     "padding",
                     /*absolute*/
                     l[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(l) {
@@ -2506,15 +2506,15 @@
             pr(r), s = !1;
         },
         d(l) {
             l && ie(e), ~t && n[t].d(), d[33](null);
         }
     };
 }
-var Kc = function(d, e, t, r) {
+var Jc = function(d, e, t, r) {
     function i(s) {
         return s instanceof t ? s : new t(function(a) {
             a(s);
         });
     }
     return new(t || (t = Promise))(function(s, a) {
         function n(c) {
@@ -2536,45 +2536,45 @@
         function l(c) {
             c.done ? s(c.value) : i(c.value).then(n, h);
         }
         l((r = r.apply(d, e || [])).next());
     });
 };
 let Si = [],
-    Tn = !1;
+    Ln = !1;
 
-function jc(d) {
-    return Kc(this, arguments, void 0, function*(e, t = !0) {
+function Qc(d) {
+    return Jc(this, arguments, void 0, function*(e, t = !0) {
         if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && t !== !0)) {
-            if (Si.push(e), !Tn)
-                Tn = !0;
+            if (Si.push(e), !Ln)
+                Ln = !0;
             else
                 return;
-            yield Pc(), requestAnimationFrame(() => {
+            yield Ic(), requestAnimationFrame(() => {
                 let r = [0, 0];
                 for (let i = 0; i < Si.length; i++) {
                     const a = Si[i].getBoundingClientRect();
                     (i === 0 || a.top + window.scrollY <= r[0]) && (r[0] = a.top + window.scrollY, r[1] = i);
                 }
                 window.scrollTo({
                     top: r[0] - 20,
                     behavior: "smooth"
-                }), Tn = !1, Si = [];
+                }), Ln = !1, Si = [];
             });
         }
     });
 }
 
-function Jc(d, e, t) {
+function eg(d, e, t) {
     let r, {
         $$slots: i = {},
         $$scope: s
     } = e;
     this && this.__awaiter;
-    const a = Ic();
+    const a = Fc();
     let {
         i18n: n
     } = e, {
         eta: h = null
     } = e, {
         queue_position: l
     } = e, {
@@ -2586,122 +2586,122 @@
     } = e, {
         timer: m = !0
     } = e, {
         show_progress: _ = "full"
     } = e, {
         message: v = null
     } = e, {
-        progress: N = null
+        progress: A = null
     } = e, {
-        variant: B = "default"
+        variant: T = "default"
     } = e, {
-        loading_text: x = "Loading..."
+        loading_text: k = "Loading..."
     } = e, {
-        absolute: L = !0
+        absolute: x = !0
     } = e, {
-        translucent: k = !1
+        translucent: R = !1
     } = e, {
-        border: z = !1
+        border: O = !1
     } = e, {
         autoscroll: D
-    } = e, Y, O = !1, Z = 0, j = 0, q = null, se = null, ye = 0, ke = null, xe, we = null, Ee = !0;
-    const Qe = () => {
-        t(0, h = t(27, q = t(19, Be = null))), t(25, Z = performance.now()), t(26, j = 0), O = !0, Ce();
+    } = e, te, q = !1, re = 0, j = 0, X = null, se = null, ye = 0, ke = null, xe, we = null, Ee = !0;
+    const et = () => {
+        t(0, h = t(27, X = t(19, Be = null))), t(25, re = performance.now()), t(26, j = 0), q = !0, Ce();
     };
 
     function Ce() {
         requestAnimationFrame(() => {
-            t(26, j = (performance.now() - Z) / 1e3), O && Ce();
+            t(26, j = (performance.now() - re) / 1e3), q && Ce();
         });
     }
 
     function Ae() {
-        t(26, j = 0), t(0, h = t(27, q = t(19, Be = null))), O && (O = !1);
+        t(26, j = 0), t(0, h = t(27, X = t(19, Be = null))), q && (q = !1);
     }
-    $c(() => {
-        O && Ae();
+    Oc(() => {
+        q && Ae();
     });
     let Be = null;
 
-    function st(K) {
-        ga[K ? "unshift" : "push"](() => {
-            we = K, t(16, we), t(7, N), t(14, ke), t(15, xe);
+    function at(U) {
+        pa[U ? "unshift" : "push"](() => {
+            we = U, t(16, we), t(7, A), t(14, ke), t(15, xe);
         });
     }
     const It = () => {
         a("clear_status");
     };
 
-    function wt(K) {
-        ga[K ? "unshift" : "push"](() => {
-            Y = K, t(13, Y);
+    function wt(U) {
+        pa[U ? "unshift" : "push"](() => {
+            te = U, t(13, te);
         });
     }
-    return d.$$set = (K) => {
-        "i18n" in K && t(1, n = K.i18n), "eta" in K && t(0, h = K.eta), "queue_position" in K && t(2, l = K.queue_position), "queue_size" in K && t(3, c = K.queue_size), "status" in K && t(4, u = K.status), "scroll_to_output" in K && t(22, g = K.scroll_to_output), "timer" in K && t(5, m = K.timer), "show_progress" in K && t(6, _ = K.show_progress), "message" in K && t(23, v = K.message), "progress" in K && t(7, N = K.progress), "variant" in K && t(8, B = K.variant), "loading_text" in K && t(9, x = K.loading_text), "absolute" in K && t(10, L = K.absolute), "translucent" in K && t(11, k = K.translucent), "border" in K && t(12, z = K.border), "autoscroll" in K && t(24, D = K.autoscroll), "$$scope" in K && t(29, s = K.$$scope);
+    return d.$$set = (U) => {
+        "i18n" in U && t(1, n = U.i18n), "eta" in U && t(0, h = U.eta), "queue_position" in U && t(2, l = U.queue_position), "queue_size" in U && t(3, c = U.queue_size), "status" in U && t(4, u = U.status), "scroll_to_output" in U && t(22, g = U.scroll_to_output), "timer" in U && t(5, m = U.timer), "show_progress" in U && t(6, _ = U.show_progress), "message" in U && t(23, v = U.message), "progress" in U && t(7, A = U.progress), "variant" in U && t(8, T = U.variant), "loading_text" in U && t(9, k = U.loading_text), "absolute" in U && t(10, x = U.absolute), "translucent" in U && t(11, R = U.translucent), "border" in U && t(12, O = U.border), "autoscroll" in U && t(24, D = U.autoscroll), "$$scope" in U && t(29, s = U.$$scope);
     }, d.$$.update = () => {
         d.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            436207617 && (h === null && t(0, h = q), h != null && q !== h && (t(28, se = (performance.now() - Z) / 1e3 + h), t(19, Be = se.toFixed(1)), t(27, q = h))), d.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            436207617 && (h === null && t(0, h = X), h != null && X !== h && (t(28, se = (performance.now() - re) / 1e3 + h), t(19, Be = se.toFixed(1)), t(27, X = h))), d.$$.dirty[0] & /*eta_from_start, timer_diff*/
             335544320 && t(17, ye = se === null || se <= 0 || !j ? null : Math.min(j / se, 1)), d.$$.dirty[0] & /*progress*/
-            128 && N != null && t(18, Ee = !1), d.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (N != null ? t(14, ke = N.map((K) => {
-                if (K.index != null && K.length != null)
-                    return K.index / K.length;
-                if (K.progress != null)
-                    return K.progress;
+            128 && A != null && t(18, Ee = !1), d.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (A != null ? t(14, ke = A.map((U) => {
+                if (U.index != null && U.length != null)
+                    return U.index / U.length;
+                if (U.progress != null)
+                    return U.progress;
             })) : t(14, ke = null), ke ? (t(15, xe = ke[ke.length - 1]), we && (xe === 0 ? t(16, we.style.transition = "0", we) : t(16, we.style.transition = "150ms", we))) : t(15, xe = void 0)), d.$$.dirty[0] & /*status*/
-            16 && (u === "pending" ? Qe() : Ae()), d.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            20979728 && Y && g && (u === "pending" || u === "complete") && jc(Y, D), d.$$.dirty[0] & /*status, message*/
+            16 && (u === "pending" ? et() : Ae()), d.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            20979728 && te && g && (u === "pending" || u === "complete") && Qc(te, D), d.$$.dirty[0] & /*status, message*/
             8388624, d.$$.dirty[0] & /*timer_diff*/
             67108864 && t(20, r = j.toFixed(1));
     }, [
         h,
         n,
         l,
         c,
         u,
         m,
         _,
-        N,
-        B,
-        x,
-        L,
+        A,
+        T,
         k,
-        z,
-        Y,
+        x,
+        R,
+        O,
+        te,
         ke,
         xe,
         we,
         ye,
         Ee,
         Be,
         r,
         a,
         g,
         v,
         D,
-        Z,
+        re,
         j,
-        q,
+        X,
         se,
         s,
         i,
-        st,
+        at,
         It,
         wt
     ];
 }
-class Qc extends xc {
+class tg extends Ec {
     constructor(e) {
-        super(), Mc(
+        super(), Dc(
             this,
             e,
-            Jc,
-            Zc,
-            Bc, {
+            eg,
+            jc,
+            Pc, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 22,
                 timer: 5,
@@ -2716,32 +2716,32 @@
                 autoscroll: 24
             },
             null,
             [-1, -1]
         );
     }
 }
-var eg = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+var rg = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-function tg(d) {
+function ig(d) {
     return d && d.__esModule && Object.prototype.hasOwnProperty.call(d, "default") ? d.default : d;
 }
-let rg = class Wn {
+let ng = class Xn {
     /**
      * Clone an array or an object. If an object is passed, a shallow clone will be created.
      *
      * @static
      * @param {*} arr The array or object to be cloned.
      * @returns {*} A clone of the array or object.
      */
     static clone(e) {
         let t = Array.isArray(e) ? Array() : {};
         for (let r in e) {
             let i = e[r];
-            typeof i.clone == "function" ? t[r] = i.clone() : t[r] = typeof i == "object" ? Wn.clone(i) : i;
+            typeof i.clone == "function" ? t[r] = i.clone() : t[r] = typeof i == "object" ? Xn.clone(i) : i;
         }
         return t;
     }
     /**
      * Returns a boolean indicating whether or not the two arrays contain the same elements.
      * Only supports 1d, non-nested arrays.
      *
@@ -2985,21 +2985,21 @@
      * @param {Array} arr The array to be copied.
      * @returns {Array} The copy.
      */
     static deepCopy(e) {
         let t = Array();
         for (let r = 0; r < e.length; r++) {
             let i = e[r];
-            i instanceof Array ? t[r] = Wn.deepCopy(i) : t[r] = i;
+            i instanceof Array ? t[r] = Xn.deepCopy(i) : t[r] = i;
         }
         return t;
     }
 };
-var Zr = rg;
-let ig = class cr {
+var Zr = ng;
+let sg = class cr {
     /**
      * Rounds a value to a given number of decimals.
      *
      * @static
      * @param {Number} value A number.
      * @param {Number} decimals The number of decimals.
      * @returns {Number} A number rounded to a given number of decimals.
@@ -3115,16 +3115,16 @@
         return 180 / Math.PI;
     }
     /** Two times PI. */
     static get twoPI() {
         return 2 * Math.PI;
     }
 };
-var Kr = ig;
-let ng = class be {
+var Kr = sg;
+let ag = class be {
     /**
      * The constructor of the class Vector2.
      *
      * @param {(Number|Vector2)} x The initial x coordinate value or, if the single argument, a Vector2 object.
      * @param {Number} y The initial y coordinate value.
      */
     constructor(e, t) {
@@ -3580,21 +3580,21 @@
         for (var r = 0; r < e.length; r++) {
             let i = e[r];
             t.add(i);
         }
         return t.normalize();
     }
 };
-var ar = ng,
-    En, xa;
+var ar = ag,
+    Mn, Ea;
 
 function Or() {
-    if (xa)
-        return En;
-    xa = 1;
+    if (Ea)
+        return Mn;
+    Ea = 1;
     const d = Kr,
         e = Zr,
         t = ar;
     Li();
     class r {
         /**
          * The constructor for the class Vertex.
@@ -3776,22 +3776,22 @@
                 if (e.contains(s[h[l]].value.rings, {
                         value: a
                     }) && h[l] != n)
                     return h[l];
             return null;
         }
     }
-    return En = r, En;
+    return Mn = r, Mn;
 }
-var Ln, Ta;
+var Bn, La;
 
-function cl() {
-    if (Ta)
-        return Ln;
-    Ta = 1, Or(), jr();
+function gl() {
+    if (La)
+        return Bn;
+    La = 1, Or(), jr();
     class d {
         /**
          * The constructor for the class RingConnection.
          *
          * @param {Ring} firstRing A ring.
          * @param {Ring} secondRing A ring.
          */
@@ -3891,26 +3891,26 @@
             for (let s = 0; s < t.length; s++) {
                 let a = t[s];
                 if (a.firstRingId === r && a.secondRingId === i || a.firstRingId === i && a.secondRingId === r)
                     return [...a.vertices];
             }
         }
     }
-    return Ln = d, Ln;
+    return Bn = d, Bn;
 }
-var Mn, Ea;
+var Dn, Ma;
 
 function jr() {
-    if (Ea)
-        return Mn;
-    Ea = 1;
+    if (Ma)
+        return Dn;
+    Ma = 1;
     const d = Zr,
         e = ar;
     Or();
-    const t = cl();
+    const t = gl();
     class r {
         /**
          * The constructor for the class Ring.
          *
          * @param {Number[]} members An array containing the vertex ids of the members of the ring to be created.
          */
         constructor(s) {
@@ -4023,22 +4023,22 @@
         contains(s) {
             for (let a = 0; a < this.members.length; a++)
                 if (this.members[a] == s)
                     return !0;
             return !1;
         }
     }
-    return Mn = r, Mn;
+    return Dn = r, Dn;
 }
-var Bn, La;
+var Pn, Ba;
 
 function Li() {
-    if (La)
-        return Bn;
-    La = 1;
+    if (Ba)
+        return Pn;
+    Ba = 1;
     const d = Zr;
     Or(), jr();
     class e {
         /**
          * The constructor of the class Atom.
          *
          * @param {String} element The one-letter code of the element.
@@ -4457,18 +4457,18 @@
                 Uup: 115,
                 Uuh: 116,
                 Uus: 117,
                 Uuo: 118
             };
         }
     }
-    return Bn = e, Bn;
+    return Pn = e, Pn;
 }
 const Tr = ar;
-let sg = class gl {
+let lg = class dl {
     /**
      * The constructor for the class Line.
      *
      * @param {Vector2} [from=new Vector2(0, 0)] A vector marking the beginning of the line.
      * @param {Vector2} [to=new Vector2(0, 0)] A vector marking the end of the line.
      * @param {string} [elementFrom=null] A one-letter representation of the element associated with the vector marking the beginning of the line.
      * @param {string} [elementTo=null] A one-letter representation of the element associated with the vector marking the end of the line.
@@ -4480,15 +4480,15 @@
     }
     /**
      * Clones this line and returns the clone.
      *
      * @returns {Line} A clone of this line.
      */
     clone() {
-        return new gl(this.from.clone(), this.to.clone(), this.elementFrom, this.elementTo);
+        return new dl(this.from.clone(), this.to.clone(), this.elementFrom, this.elementTo);
     }
     /**
      * Returns the length of this line.
      *
      * @returns {Number} The length of this line.
      */
     getLength() {
@@ -4639,16 +4639,16 @@
      * @returns {Line} This line.
      */
     shorten(e) {
         let t = Tr.subtract(this.from, this.to);
         return t.normalize(), t.multiplyScalar(e / 2), this.to.add(t), this.from.subtract(t), this;
     }
 };
-var Xn = sg;
-let ag = class dl {
+var Zn = lg;
+let og = class pl {
     /**
      * The constructor for the class Edge.
      *
      * @param {Number} sourceId A vertex id.
      * @param {Number} targetId A vertex id.
      * @param {Number} [weight=1] The weight of the edge.
      */
@@ -4656,15 +4656,15 @@
         this.id = null, this.sourceId = e, this.targetId = t, this.weight = r, this.bondType = "-", this.isPartOfAromaticRing = !1, this.center = !1, this.wedge = "";
     }
     /**
      * Set the bond type of this edge. This also sets the edge weight.
      * @param {String} bondType 
      */
     setBondType(e) {
-        this.bondType = e, this.weight = dl.bonds[e];
+        this.bondType = e, this.weight = pl.bonds[e];
     }
     /**
      * An object mapping the bond type to the number of bonds.
      *
      * @returns {Object} The object containing the map.
      */
     static get bonds() {
@@ -4674,30 +4674,30 @@
             "\\": 1,
             "=": 2,
             "#": 3,
             $: 4
         };
     }
 };
-var pl = ag;
+var vl = og;
 
-function lg(d) {
+function hg(d) {
     return d === 1 ? "+" : d === 2 ? "2+" : d === -1 ? "-" : d === -2 ? "2-" : "";
 }
-var og = {
-    getChargeText: lg
+var fg = {
+    getChargeText: hg
 };
 const Er = Kr,
     Ke = ar;
 Or();
 jr();
 const {
-    getChargeText: Ma
-} = og;
-let hg = class {
+    getChargeText: Da
+} = fg;
+let ug = class {
     /**
      * The constructor for the class CanvasWrapper.
      *
      * @param {(String|HTMLElement)} target The canvas id or the canvas HTMLElement.
      * @param {ThemeManager} themeManager Theme manager for setting proper colors.
      * @param {Object} options The smiles drawer options object.
      */
@@ -4814,18 +4814,18 @@
         let c = e.getRightChiral(),
             u = n,
             g = h;
         c && (u = h, g = n);
         let m = Ke.add(u, Ke.multiplyScalar(l[0], this.halfBondThickness)),
             _ = Ke.add(g, Ke.multiplyScalar(l[0], 1.5 + this.halfBondThickness)),
             v = Ke.add(g, Ke.multiplyScalar(l[1], 1.5 + this.halfBondThickness)),
-            N = Ke.add(u, Ke.multiplyScalar(l[1], this.halfBondThickness));
-        r.beginPath(), r.moveTo(m.x, m.y), r.lineTo(_.x, _.y), r.lineTo(v.x, v.y), r.lineTo(N.x, N.y);
-        let B = this.ctx.createRadialGradient(h.x, h.y, this.opts.bondLength, h.x, h.y, 0);
-        B.addColorStop(0.4, this.themeManager.getColor(e.getLeftElement()) || this.themeManager.getColor("C")), B.addColorStop(0.6, this.themeManager.getColor(e.getRightElement()) || this.themeManager.getColor("C")), r.fillStyle = B, r.fill(), r.restore();
+            A = Ke.add(u, Ke.multiplyScalar(l[1], this.halfBondThickness));
+        r.beginPath(), r.moveTo(m.x, m.y), r.lineTo(_.x, _.y), r.lineTo(v.x, v.y), r.lineTo(A.x, A.y);
+        let T = this.ctx.createRadialGradient(h.x, h.y, this.opts.bondLength, h.x, h.y, 0);
+        T.addColorStop(0.4, this.themeManager.getColor(e.getLeftElement()) || this.themeManager.getColor("C")), T.addColorStop(0.6, this.themeManager.getColor(e.getRightElement()) || this.themeManager.getColor("C")), r.fillStyle = T, r.fill(), r.restore();
     }
     /**
      * Draw a dashed wedge on the canvas.
      *
      * @param {Line} line A line.
      */
     drawDashedWedge(e) {
@@ -4841,22 +4841,22 @@
         n[0].normalize(), n[1].normalize();
         let h = e.getRightChiral(),
             l, c, u, g, m = e.clone();
         h ? (l = a, c = s, m.shortenRight(1), u = m.getRightVector().clone(), g = m.getLeftVector().clone()) : (l = s, c = a, m.shortenLeft(1), u = m.getLeftVector().clone(), g = m.getRightVector().clone()), u.x += r, u.y += i, g.x += r, g.y += i;
         let _ = Ke.subtract(c, l).normalize();
         t.strokeStyle = this.themeManager.getColor("C"), t.lineCap = "round", t.lineWidth = this.opts.bondThickness, t.beginPath();
         let v = e.getLength(),
-            N = 1.25 / (v / (this.opts.bondThickness * 3)),
-            B = !1;
-        for (var x = 0; x < 1; x += N) {
-            let L = Ke.multiplyScalar(_, x * v),
-                k = Ke.add(l, L),
-                z = 1.5 * x,
-                D = Ke.multiplyScalar(n[0], z);
-            !B && x > 0.5 && (t.stroke(), t.beginPath(), t.strokeStyle = this.themeManager.getColor(e.getRightElement()) || this.themeManager.getColor("C"), B = !0), k.subtract(D), t.moveTo(k.x, k.y), k.add(Ke.multiplyScalar(D, 2)), t.lineTo(k.x, k.y);
+            A = 1.25 / (v / (this.opts.bondThickness * 3)),
+            T = !1;
+        for (var k = 0; k < 1; k += A) {
+            let x = Ke.multiplyScalar(_, k * v),
+                R = Ke.add(l, x),
+                O = 1.5 * k,
+                D = Ke.multiplyScalar(n[0], O);
+            !T && k > 0.5 && (t.stroke(), t.beginPath(), t.strokeStyle = this.themeManager.getColor(e.getRightElement()) || this.themeManager.getColor("C"), T = !0), R.subtract(D), t.moveTo(R.x, R.y), R.add(Ke.multiplyScalar(D, 2)), t.lineTo(R.x, R.y);
         }
         t.stroke(), t.restore();
     }
     /**
      * Draws a debug text message at a given position
      *
      * @param {Number} x The x coordinate.
@@ -4911,62 +4911,62 @@
     drawText(e, t, r, i, s, a, n, h, l, c = {}) {
         let u = this.ctx,
             g = this.offsetX,
             m = this.offsetY;
         u.save(), u.textAlign = "start", u.textBaseline = "alphabetic";
         let _ = "",
             v = 0;
-        n && (_ = Ma(n), u.font = this.fontSmall, v = u.measureText(_).width);
-        let N = "0",
-            B = 0;
-        h > 0 && (N = h.toString(), u.font = this.fontSmall, B = u.measureText(N).width), n === 1 && r === "N" && c.hasOwnProperty("0O") && c.hasOwnProperty("0O-1") && (c = {
+        n && (_ = Da(n), u.font = this.fontSmall, v = u.measureText(_).width);
+        let A = "0",
+            T = 0;
+        h > 0 && (A = h.toString(), u.font = this.fontSmall, T = u.measureText(A).width), n === 1 && r === "N" && c.hasOwnProperty("0O") && c.hasOwnProperty("0O-1") && (c = {
             "0O": {
                 element: "O",
                 count: 2,
                 hydrogenCount: 0,
                 previousElement: "C",
                 charge: ""
             }
         }, n = 0), u.font = this.fontLarge, u.fillStyle = this.themeManager.getColor("BACKGROUND");
-        let x = u.measureText(r);
-        x.totalWidth = x.width + v, x.height = parseInt(this.fontLarge, 10);
-        let L = x.width > this.opts.fontSizeLarge ? x.width : this.opts.fontSizeLarge;
-        L /= 1.5, u.globalCompositeOperation = "destination-out", u.beginPath(), u.arc(e + g, t + m, L, 0, Er.twoPI, !0), u.closePath(), u.fill(), u.globalCompositeOperation = "source-over";
-        let k = -x.width / 2,
-            z = -x.width / 2;
-        u.fillStyle = this.themeManager.getColor(r), u.fillText(r, e + g + k, t + this.opts.halfFontSizeLarge + m), k += x.width, n && (u.font = this.fontSmall, u.fillText(_, e + g + k, t - this.opts.fifthFontSizeSmall + m), k += v), h > 0 && (u.font = this.fontSmall, u.fillText(N, e + g + z - B, t - this.opts.fifthFontSizeSmall + m), z -= B), u.font = this.fontLarge;
+        let k = u.measureText(r);
+        k.totalWidth = k.width + v, k.height = parseInt(this.fontLarge, 10);
+        let x = k.width > this.opts.fontSizeLarge ? k.width : this.opts.fontSizeLarge;
+        x /= 1.5, u.globalCompositeOperation = "destination-out", u.beginPath(), u.arc(e + g, t + m, x, 0, Er.twoPI, !0), u.closePath(), u.fill(), u.globalCompositeOperation = "source-over";
+        let R = -k.width / 2,
+            O = -k.width / 2;
+        u.fillStyle = this.themeManager.getColor(r), u.fillText(r, e + g + R, t + this.opts.halfFontSizeLarge + m), R += k.width, n && (u.font = this.fontSmall, u.fillText(_, e + g + R, t - this.opts.fifthFontSizeSmall + m), R += v), h > 0 && (u.font = this.fontSmall, u.fillText(A, e + g + O - T, t - this.opts.fifthFontSizeSmall + m), O -= T), u.font = this.fontLarge;
         let D = 0,
-            Y = 0;
+            te = 0;
         if (i === 1) {
-            let O = e + g,
-                Z = t + m + this.opts.halfFontSizeLarge;
-            D = this.hydrogenWidth, z -= D, s === "left" ? O += z : s === "right" || s === "up" && a || s === "down" && a ? O += k : s === "up" && !a ? (Z -= this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, O -= this.halfHydrogenWidth) : s === "down" && !a && (Z += this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, O -= this.halfHydrogenWidth), u.fillText("H", O, Z), k += D;
+            let q = e + g,
+                re = t + m + this.opts.halfFontSizeLarge;
+            D = this.hydrogenWidth, O -= D, s === "left" ? q += O : s === "right" || s === "up" && a || s === "down" && a ? q += R : s === "up" && !a ? (re -= this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, q -= this.halfHydrogenWidth) : s === "down" && !a && (re += this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, q -= this.halfHydrogenWidth), u.fillText("H", q, re), R += D;
         } else if (i > 1) {
-            let O = e + g,
-                Z = t + m + this.opts.halfFontSizeLarge;
-            D = this.hydrogenWidth, u.font = this.fontSmall, Y = u.measureText(i).width, z -= D + Y, s === "left" ? O += z : s === "right" || s === "up" && a || s === "down" && a ? O += k : s === "up" && !a ? (Z -= this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, O -= this.halfHydrogenWidth) : s === "down" && !a && (Z += this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, O -= this.halfHydrogenWidth), u.font = this.fontLarge, u.fillText("H", O, Z), u.font = this.fontSmall, u.fillText(i, O + this.halfHydrogenWidth + Y, Z + this.opts.fifthFontSizeSmall), k += D + this.halfHydrogenWidth + Y;
+            let q = e + g,
+                re = t + m + this.opts.halfFontSizeLarge;
+            D = this.hydrogenWidth, u.font = this.fontSmall, te = u.measureText(i).width, O -= D + te, s === "left" ? q += O : s === "right" || s === "up" && a || s === "down" && a ? q += R : s === "up" && !a ? (re -= this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, q -= this.halfHydrogenWidth) : s === "down" && !a && (re += this.opts.fontSizeLarge + this.opts.quarterFontSizeLarge, q -= this.halfHydrogenWidth), u.font = this.fontLarge, u.fillText("H", q, re), u.font = this.fontSmall, u.fillText(i, q + this.halfHydrogenWidth + te, re + this.opts.fifthFontSizeSmall), R += D + this.halfHydrogenWidth + te;
         }
-        for (let O in c) {
-            if (!c.hasOwnProperty(O))
+        for (let q in c) {
+            if (!c.hasOwnProperty(q))
                 continue;
-            let Z = 0,
+            let re = 0,
                 j = 0,
-                q = c[O].element,
-                se = c[O].count,
-                ye = c[O].hydrogenCount,
-                ke = c[O].charge;
-            u.font = this.fontLarge, se > 1 && ye > 0 && (Z = u.measureText("(").width, j = u.measureText(")").width);
-            let xe = u.measureText(q).width,
+                X = c[q].element,
+                se = c[q].count,
+                ye = c[q].hydrogenCount,
+                ke = c[q].charge;
+            u.font = this.fontLarge, se > 1 && ye > 0 && (re = u.measureText("(").width, j = u.measureText(")").width);
+            let xe = u.measureText(X).width,
                 we = 0,
                 Ee = "",
-                Qe = 0;
-            D = 0, ye > 0 && (D = this.hydrogenWidth), u.font = this.fontSmall, se > 1 && (we = u.measureText(se).width), ke !== 0 && (Ee = Ma(ke), Qe = u.measureText(Ee).width), Y = 0, ye > 1 && (Y = u.measureText(ye).width), u.font = this.fontLarge;
+                et = 0;
+            D = 0, ye > 0 && (D = this.hydrogenWidth), u.font = this.fontSmall, se > 1 && (we = u.measureText(se).width), ke !== 0 && (Ee = Da(ke), et = u.measureText(Ee).width), te = 0, ye > 1 && (te = u.measureText(ye).width), u.font = this.fontLarge;
             let Ce = e + g,
                 Ae = t + m + this.opts.halfFontSizeLarge;
-            u.fillStyle = this.themeManager.getColor(q), se > 0 && (z -= we), se > 1 && ye > 0 && (s === "left" ? (z -= j, u.fillText(")", Ce + z, Ae)) : (u.fillText("(", Ce + k, Ae), k += Z)), s === "left" ? (z -= xe, u.fillText(q, Ce + z, Ae)) : (u.fillText(q, Ce + k, Ae), k += xe), ye > 0 && (s === "left" ? (z -= D + Y, u.fillText("H", Ce + z, Ae), ye > 1 && (u.font = this.fontSmall, u.fillText(ye, Ce + z + D, Ae + this.opts.fifthFontSizeSmall))) : (u.fillText("H", Ce + k, Ae), k += D, ye > 1 && (u.font = this.fontSmall, u.fillText(ye, Ce + k, Ae + this.opts.fifthFontSizeSmall), k += Y))), u.font = this.fontLarge, se > 1 && ye > 0 && (s === "left" ? (z -= Z, u.fillText("(", Ce + z, Ae)) : (u.fillText(")", Ce + k, Ae), k += j)), u.font = this.fontSmall, se > 1 && (s === "left" ? u.fillText(se, Ce + z + Z + j + D + Y + xe, Ae + this.opts.fifthFontSizeSmall) : (u.fillText(se, Ce + k, Ae + this.opts.fifthFontSizeSmall), k += we)), ke !== 0 && (s === "left" ? u.fillText(Ee, Ce + z + Z + j + D + Y + xe, t - this.opts.fifthFontSizeSmall + m) : (u.fillText(Ee, Ce + k, t - this.opts.fifthFontSizeSmall + m), k += Qe));
+            u.fillStyle = this.themeManager.getColor(X), se > 0 && (O -= we), se > 1 && ye > 0 && (s === "left" ? (O -= j, u.fillText(")", Ce + O, Ae)) : (u.fillText("(", Ce + R, Ae), R += re)), s === "left" ? (O -= xe, u.fillText(X, Ce + O, Ae)) : (u.fillText(X, Ce + R, Ae), R += xe), ye > 0 && (s === "left" ? (O -= D + te, u.fillText("H", Ce + O, Ae), ye > 1 && (u.font = this.fontSmall, u.fillText(ye, Ce + O + D, Ae + this.opts.fifthFontSizeSmall))) : (u.fillText("H", Ce + R, Ae), R += D, ye > 1 && (u.font = this.fontSmall, u.fillText(ye, Ce + R, Ae + this.opts.fifthFontSizeSmall), R += te))), u.font = this.fontLarge, se > 1 && ye > 0 && (s === "left" ? (O -= re, u.fillText("(", Ce + O, Ae)) : (u.fillText(")", Ce + R, Ae), R += j)), u.font = this.fontSmall, se > 1 && (s === "left" ? u.fillText(se, Ce + O + re + j + D + te + xe, Ae + this.opts.fifthFontSizeSmall) : (u.fillText(se, Ce + R, Ae + this.opts.fifthFontSizeSmall), R += we)), ke !== 0 && (s === "left" ? u.fillText(Ee, Ce + O + re + j + D + te + xe, t - this.opts.fifthFontSizeSmall + m) : (u.fillText(Ee, Ce + R, t - this.opts.fifthFontSizeSmall + m), R += et));
         }
         u.restore();
     }
     /**
      * Translate the integer indicating the charge to the appropriate text.
      * @param {Number} charge The integer indicating the charge.
      * @returns {String} A string representing a charge.
@@ -5006,21 +5006,21 @@
      * Clear the canvas.
      *
      */
     clear() {
         this.ctx.clearRect(0, 0, this.canvas.offsetWidth, this.canvas.offsetHeight);
     }
 };
-var fg = hg;
-const Ba = Kr,
-    ug = Or(),
-    cg = pl;
+var cg = ug;
+const Pa = Kr,
+    gg = Or(),
+    dg = vl;
 jr();
-const gg = Li();
-let dg = class Ur {
+const pg = Li();
+let vg = class Ur {
     /**
      * The constructor of the class Graph.
      * 
      * @param {Object} parseTree A SMILES parse tree.
      * @param {Boolean} [isomeric=false] A boolean specifying whether or not the SMILES is isomeric.
      */
     constructor(e, t = !1) {
@@ -5031,21 +5031,21 @@
      *
      * @param {Object} node The current node in the parse tree.
      * @param {?Number} parentVertexId=null The id of the previous vertex.
      * @param {Boolean} isBranch=false Whether or not the bond leading to this vertex is a branch bond. Branches are represented by parentheses in smiles (e.g. CC(O)C).
      */
     _init(e, t = 0, r = null, i = !1) {
         const s = e.atom.element ? e.atom.element : e.atom;
-        let a = new gg(s, e.bond);
+        let a = new pg(s, e.bond);
         (s !== "H" || !e.hasNext && r === null) && (a.idx = this._atomIdx, this._atomIdx++), a.branchBond = e.branchBond, a.ringbonds = e.ringbonds, a.bracket = e.atom.element ? e.atom : null, a.class = e.atom.class;
-        let n = new ug(a),
+        let n = new gg(a),
             h = this.vertices[r];
         if (this.addVertex(n), a.idx !== null && this.atomIdxToVertexId.push(n.id), r !== null) {
             n.setParentVertexId(r), n.value.addNeighbouringElement(h.value.element), h.addChild(n.id), h.value.addNeighbouringElement(a.element), h.spanningTreeChildren.push(n.id);
-            let g = new cg(r, n.id, 1);
+            let g = new dg(r, n.id, 1);
             i ? (g.setBondType(n.value.branchBond || "-"), n.id, g.setBondType(n.value.branchBond || "-"), n.id) : (g.setBondType(h.value.bondType || "-"), h.id), this.addEdge(g);
         }
         let l = e.ringbondCount + 1;
         a.bracket && (l += a.bracket.hcount);
         let c = 0;
         if (a.bracket && a.bracket.chirality) {
             a.isStereoCenter = !0, c = a.bracket.hcount;
@@ -5360,111 +5360,111 @@
      */
     kkLayout(e, t, r, i, s, a = 0.1, n = 0.1, h = 2e3, l = 50, c = 1e9) {
         let u = s;
         for (var g = e.length; g--;)
             var m = this.vertices[e[g]].neighbours.length;
         let _ = this.getSubgraphDistanceMatrix(e),
             v = e.length,
-            N = Ba.polyCircumradius(500, v),
-            B = Ba.centralAngle(v),
-            x = 0,
-            L = new Float32Array(v),
-            k = new Float32Array(v),
-            z = Array(v);
+            A = Pa.polyCircumradius(500, v),
+            T = Pa.centralAngle(v),
+            k = 0,
+            x = new Float32Array(v),
+            R = new Float32Array(v),
+            O = Array(v);
         for (g = v; g--;) {
-            let J = this.vertices[e[g]];
-            J.positioned ? (L[g] = J.position.x, k[g] = J.position.y) : (L[g] = t.x + Math.cos(x) * N, k[g] = t.y + Math.sin(x) * N), z[g] = J.positioned, x += B;
+            let Z = this.vertices[e[g]];
+            Z.positioned ? (x[g] = Z.position.x, R[g] = Z.position.y) : (x[g] = t.x + Math.cos(k) * A, R[g] = t.y + Math.sin(k) * A), O[g] = Z.positioned, k += T;
         }
         let D = Array(v);
         for (g = v; g--;) {
             D[g] = new Array(v);
             for (var m = v; m--;)
                 D[g][m] = s * _[g][m];
         }
-        let Y = Array(v);
+        let te = Array(v);
         for (g = v; g--;) {
-            Y[g] = Array(v);
+            te[g] = Array(v);
             for (var m = v; m--;)
-                Y[g][m] = u * Math.pow(_[g][m], -2);
+                te[g][m] = u * Math.pow(_[g][m], -2);
         }
-        let O = Array(v),
-            Z = new Float32Array(v),
+        let q = Array(v),
+            re = new Float32Array(v),
             j = new Float32Array(v);
         for (g = v; g--;)
-            O[g] = Array(v);
+            q[g] = Array(v);
         g = v;
-        let q, se, ye, ke, xe, we, Ee;
+        let X, se, ye, ke, xe, we, Ee;
         for (; g--;) {
-            q = L[g], se = k[g], ye = 0, ke = 0;
-            let J = v;
-            for (; J--;)
-                g !== J && (xe = L[J], we = k[J], Ee = 1 / Math.sqrt((q - xe) * (q - xe) + (se - we) * (se - we)), O[g][J] = [
-                    Y[g][J] * (q - xe - D[g][J] * (q - xe) * Ee),
-                    Y[g][J] * (se - we - D[g][J] * (se - we) * Ee)
-                ], O[J][g] = O[g][J], ye += O[g][J][0], ke += O[g][J][1]);
-            Z[g] = ye, j[g] = ke;
+            X = x[g], se = R[g], ye = 0, ke = 0;
+            let Z = v;
+            for (; Z--;)
+                g !== Z && (xe = x[Z], we = R[Z], Ee = 1 / Math.sqrt((X - xe) * (X - xe) + (se - we) * (se - we)), q[g][Z] = [
+                    te[g][Z] * (X - xe - D[g][Z] * (X - xe) * Ee),
+                    te[g][Z] * (se - we - D[g][Z] * (se - we) * Ee)
+                ], q[Z][g] = q[g][Z], ye += q[g][Z][0], ke += q[g][Z][1]);
+            re[g] = ye, j[g] = ke;
         }
-        let Qe = function(J) {
-                return [Z[J] * Z[J] + j[J] * j[J], Z[J], j[J]];
+        let et = function(Z) {
+                return [re[Z] * re[Z] + j[Z] * j[Z], re[Z], j[Z]];
             },
             Ce = function() {
-                let J = 0,
+                let Z = 0,
                     Te = 0,
-                    et = 0,
+                    tt = 0,
                     Ie = 0;
                 for (g = v; g--;) {
-                    let [Ye, Ue, Ge] = Qe(g);
-                    Ye > J && z[g] === !1 && (J = Ye, Te = g, et = Ue, Ie = Ge);
+                    let [Ye, Ue, Ge] = et(g);
+                    Ye > Z && O[g] === !1 && (Z = Ye, Te = g, tt = Ue, Ie = Ge);
                 }
-                return [Te, J, et, Ie];
+                return [Te, Z, tt, Ie];
             },
-            Ae = function(J, Te, et) {
+            Ae = function(Z, Te, tt) {
                 let Ie = 0,
                     Ye = 0,
                     Ue = 0,
-                    Ge = L[J],
-                    De = k[J],
-                    Ze = D[J],
-                    He = Y[J];
+                    Ge = x[Z],
+                    De = R[Z],
+                    Ze = D[Z],
+                    He = te[Z];
                 for (g = v; g--;) {
-                    if (g === J)
+                    if (g === Z)
                         continue;
-                    let Ft = L[g],
-                        _t = k[g],
+                    let Ft = x[g],
+                        _t = R[g],
                         zt = Ze[g],
                         Gt = He[g],
                         Ut = (Ge - Ft) * (Ge - Ft),
                         Zt = 1 / Math.pow(Ut + (De - _t) * (De - _t), 1.5);
                     Ie += Gt * (1 - zt * (De - _t) * (De - _t) * Zt), Ye += Gt * (1 - zt * Ut * Zt), Ue += Gt * (zt * (Ge - Ft) * (De - _t) * Zt);
                 }
                 Ie === 0 && (Ie = 0.1), Ye === 0 && (Ye = 0.1), Ue === 0 && (Ue = 0.1);
-                let We = Te / Ie + et / Ue;
+                let We = Te / Ie + tt / Ue;
                 We /= Ue / Ie - Ye / Ue;
                 let Le = -(Ue * We + Te) / Ie;
-                L[J] += Le, k[J] += We;
-                let qe = O[J];
-                Te = 0, et = 0, Ge = L[J], De = k[J];
-                let Lt, yt, Vt, Xt, Yt;
+                x[Z] += Le, R[Z] += We;
+                let qe = q[Z];
+                Te = 0, tt = 0, Ge = x[Z], De = R[Z];
+                let Mt, yt, Vt, Xt, Yt;
                 for (g = v; g--;)
-                    J !== g && (Lt = L[g], yt = k[g], Vt = qe[g][0], Xt = qe[g][1], Yt = 1 / Math.sqrt((Ge - Lt) * (Ge - Lt) + (De - yt) * (De - yt)), Le = He[g] * (Ge - Lt - Ze[g] * (Ge - Lt) * Yt), We = He[g] * (De - yt - Ze[g] * (De - yt) * Yt), qe[g] = [Le, We], Te += Le, et += We, Z[g] += Le - Vt, j[g] += We - Xt);
-                Z[J] = Te, j[J] = et;
+                    Z !== g && (Mt = x[g], yt = R[g], Vt = qe[g][0], Xt = qe[g][1], Yt = 1 / Math.sqrt((Ge - Mt) * (Ge - Mt) + (De - yt) * (De - yt)), Le = He[g] * (Ge - Mt - Ze[g] * (Ge - Mt) * Yt), We = He[g] * (De - yt - Ze[g] * (De - yt) * Yt), qe[g] = [Le, We], Te += Le, tt += We, re[g] += Le - Vt, j[g] += We - Xt);
+                re[Z] = Te, j[Z] = tt;
             },
             Be = 0,
-            st = 0,
+            at = 0,
             It = 0,
             wt = 0,
-            K = 0,
+            U = 0,
             Ot = 0;
-        for (; c > a && h > K;)
-            for (K++, [Be, c, st, It] = Ce(), wt = c, Ot = 0; wt > n && l > Ot;)
-                Ot++, Ae(Be, st, It), [wt, st, It] = Qe(Be);
+        for (; c > a && h > U;)
+            for (U++, [Be, c, at, It] = Ce(), wt = c, Ot = 0; wt > n && l > Ot;)
+                Ot++, Ae(Be, at, It), [wt, at, It] = et(Be);
         for (g = v; g--;) {
-            let J = e[g],
-                Te = this.vertices[J];
-            Te.position.x = L[g], Te.position.y = k[g], Te.positioned = !0, Te.forcePositioned = !0;
+            let Z = e[g],
+                Te = this.vertices[Z];
+            Te.position.x = x[g], Te.position.y = R[g], Te.positioned = !0, Te.forcePositioned = !0;
         }
     }
     /**
      * PRIVATE FUNCTION used by getBridges().
      */
     _bridgeDfs(e, t, r, i, s, a, n) {
         t[e] = !0, r[e] = i[e] = ++this._time;
@@ -5517,29 +5517,29 @@
      * PRIVATE FUNCTION used by getConnectedComponents().
      */
     static _ccGetDfs(e, t, r, i) {
         for (var s = 0; s < r[e].length; s++)
             !r[e][s] || t[s] || e === s || (t[s] = !0, i.push(s), Ur._ccGetDfs(s, t, r, i));
     }
 };
-var vl = dg;
-const pg = vl;
-let vg = class gt {
+var ml = vg;
+const mg = ml;
+let bg = class gt {
     /**
      * Returns an array containing arrays, each representing a ring from the smallest set of smallest rings in the graph.
      * 
      * @param {Graph} graph A Graph object.
      * @param {Boolean} [experimental=false] Whether or not to use experimental SSSR.
      * @returns {Array[]} An array containing arrays, each representing a ring from the smallest set of smallest rings in the group.
      */
     static getRings(e, t = !1) {
         let r = e.getComponentsAdjacencyMatrix();
         if (r.length === 0)
             return null;
-        let i = pg.getConnectedComponents(r),
+        let i = mg.getConnectedComponents(r),
             s = Array();
         for (var a = 0; a < i.length; a++) {
             let l = i[a],
                 c = e.getSubgraphAdjacencyMatrix([...l]),
                 u = new Uint16Array(c.length),
                 g = new Uint16Array(c.length);
             for (var n = 0; n < c.length; n++) {
@@ -5557,23 +5557,23 @@
                 u[n] !== 3 && (v = !1);
             if (v && (_ = 2 + m - c.length), _ === 1) {
                 s.push([...l]);
                 continue;
             }
             t && (_ = 999);
             let {
-                d: N,
-                pe: B,
-                pe_prime: x
-            } = gt.getPathIncludedDistanceMatrices(c), L = gt.getRingCandidates(N, B, x), k = gt.getSSSR(L, N, c, B, x, u, g, _);
-            for (var n = 0; n < k.length; n++) {
-                let D = Array(k[n].size),
-                    Y = 0;
-                for (let O of k[n])
-                    D[Y++] = l[O];
+                d: A,
+                pe: T,
+                pe_prime: k
+            } = gt.getPathIncludedDistanceMatrices(c), x = gt.getRingCandidates(A, T, k), R = gt.getSSSR(x, A, c, T, k, u, g, _);
+            for (var n = 0; n < R.length; n++) {
+                let D = Array(R[n].size),
+                    te = 0;
+                for (let q of R[n])
+                    D[te++] = l[q];
                 s.push(D);
             }
         }
         return s;
     }
     /**
      * Creates a printable string from a matrix (2D array).
@@ -5847,16 +5847,16 @@
     static isSupersetOf(e, t) {
         for (var r of t)
             if (!e.has(r))
                 return !1;
         return !0;
     }
 };
-var mg = vg;
-let bg = class {
+var wg = bg;
+let yg = class {
     constructor(e, t) {
         this.colors = e, this.theme = this.colors[t];
     }
     /**
      * Returns the hex code of a color associated with a key from the current theme.
      *
      * @param {String} key The color key in the theme (e.g. C, N, BACKGROUND, ...).
@@ -5871,16 +5871,16 @@
      *
      * @param {String} theme the name of the theme to switch to
      */
     setTheme(e) {
         this.colors.hasOwnProperty(e) && (this.theme = this.colors[e]);
     }
 };
-var Yn = bg;
-let wg = class {
+var Kn = yg;
+let _g = class {
     /**
      * A helper method to extend the default options with user supplied ones.
      */
     static extend() {
         let e = this,
             t = {},
             r = !1,
@@ -5894,30 +5894,30 @@
         for (; i < s; i++) {
             let n = arguments[i];
             a(n);
         }
         return t;
     }
 };
-var Gn = wg;
+var jn = _g;
 const Se = Kr,
-    Dt = Zr,
-    re = ar,
-    Me = Xn;
+    Pt = Zr,
+    ee = ar,
+    Me = Zn;
 Or();
-const yg = pl,
+const Sg = vl,
     Ci = Li(),
-    Da = jr(),
-    Ai = cl(),
-    _g = fg,
-    Pa = vl,
-    Sg = mg,
-    Cg = Yn,
-    Ag = Gn;
-let Ng = class {
+    $a = jr(),
+    Ai = gl(),
+    Cg = cg,
+    Ia = ml,
+    Ag = wg,
+    Ng = Kn,
+    kg = jn;
+let Rg = class {
     /**
      * The constructor for the class SmilesDrawer.
      *
      * @param {Object} options An object containing custom values for different options. It is merged with the default options.
      */
     constructor(e) {
         this.graph = null, this.doubleBondConfigCount = 0, this.doubleBondConfig = null, this.ringIdCounter = 0, this.ringConnectionIdCounter = 0, this.canvasWrapper = null, this.totalOverlapScore = 0, this.defaultOptions = {
@@ -6131,26 +6131,26 @@
                     S: "#f1c40f",
                     B: "#e67e22",
                     SI: "#e67e22",
                     H: "#666",
                     BACKGROUND: "#fff"
                 }
             }
-        }, this.opts = Ag.extend(!0, this.defaultOptions, e), this.opts.halfBondSpacing = this.opts.bondSpacing / 2, this.opts.bondLengthSq = this.opts.bondLength * this.opts.bondLength, this.opts.halfFontSizeLarge = this.opts.fontSizeLarge / 2, this.opts.quarterFontSizeLarge = this.opts.fontSizeLarge / 4, this.opts.fifthFontSizeSmall = this.opts.fontSizeSmall / 5, this.theme = this.opts.themes.dark;
+        }, this.opts = kg.extend(!0, this.defaultOptions, e), this.opts.halfBondSpacing = this.opts.bondSpacing / 2, this.opts.bondLengthSq = this.opts.bondLength * this.opts.bondLength, this.opts.halfFontSizeLarge = this.opts.fontSizeLarge / 2, this.opts.quarterFontSizeLarge = this.opts.fontSizeLarge / 4, this.opts.fifthFontSizeSmall = this.opts.fontSizeSmall / 5, this.theme = this.opts.themes.dark;
     }
     /**
      * Draws the parsed smiles data to a canvas element.
      *
      * @param {Object} data The tree returned by the smiles parser.
      * @param {(String|HTMLCanvasElement)} target The id of the HTML canvas element the structure is drawn to - or the element itself.
      * @param {String} themeName='dark' The name of the theme to use. Built-in themes are 'light' and 'dark'.
      * @param {Boolean} infoOnly=false Only output info on the molecule without drawing anything to the canvas.
      */
     draw(e, t, r = "light", i = !1) {
-        this.initDraw(e, r, i), this.infoOnly || (this.themeManager = new Cg(this.opts.themes, r), this.canvasWrapper = new _g(t, this.themeManager, this.opts)), i || (this.processGraph(), this.canvasWrapper.scale(this.graph.vertices), this.drawEdges(this.opts.debug), this.drawVertices(this.opts.debug), this.canvasWrapper.reset(), this.opts.debug && (console.log(this.graph), console.log(this.rings), console.log(this.ringConnections)));
+        this.initDraw(e, r, i), this.infoOnly || (this.themeManager = new Ng(this.opts.themes, r), this.canvasWrapper = new Cg(t, this.themeManager, this.opts)), i || (this.processGraph(), this.canvasWrapper.scale(this.graph.vertices), this.drawEdges(this.opts.debug), this.drawVertices(this.opts.debug), this.canvasWrapper.reset(), this.opts.debug && (console.log(this.graph), console.log(this.rings), console.log(this.ringConnections)));
     }
     /**
      * Returns the number of rings this edge is a part of.
      *
      * @param {Number} edgeId The id of an edge.
      * @returns {Number} The number of rings the provided edge is part of.
      */
@@ -6221,15 +6221,15 @@
                     let h = this.graph.vertices[s];
                     if (!h.value.isDrawn)
                         continue;
                     let l = n.position.distanceSq(h.position);
                     l > r && (r = l, e = i, t = s);
                 }
         }
-        let a = -re.subtract(this.graph.vertices[e].position, this.graph.vertices[t].position).angle();
+        let a = -ee.subtract(this.graph.vertices[e].position, this.graph.vertices[t].position).angle();
         if (!isNaN(a)) {
             let n = a % 0.523599;
             n < 0.2617995 ? a = a - n : a += 0.523599 - n;
             for (var i = 0; i < this.graph.vertices.length; i++)
                 i !== t && this.graph.vertices[i].position.rotateAround(a, this.graph.vertices[t].position);
             for (var i = 0; i < this.rings.length; i++)
                 this.rings[i].center.rotateAround(a, this.graph.vertices[t].position);
@@ -6274,15 +6274,15 @@
      * Returns the molecular formula of the loaded molecule as a string.
      * 
      * @returns {String} The molecular formula.
      */
     getMolecularFormula(e = null) {
         let t = "",
             r = /* @__PURE__ */ new Map(),
-            i = e === null ? this.graph : new Pa(e, this.opts.isomeric);
+            i = e === null ? this.graph : new Ia(e, this.opts.isomeric);
         for (var s = 0; s < i.vertices.length; s++) {
             let n = i.vertices[s].value;
             if (r.has(n.element) ? r.set(n.element, r.get(n.element) + 1) : r.set(n.element, 1), n.bracket && !n.bracket.chirality && (r.has("H") ? r.set("H", r.get("H") + n.bracket.hcount) : r.set("H", n.bracket.hcount)), !n.bracket) {
                 let h = Ci.maxBonds[n.element] - n.bondCount;
                 n.isPartOfAromaticRing && h--, r.has("H") ? r.set("H", r.get("H") + h) : r.set("H", h);
             }
         }
@@ -6314,15 +6314,15 @@
         for (var r = 0; r < e.value.ringbonds.length; r++)
             for (var i = 0; i < t.value.ringbonds.length; i++)
                 if (e.value.ringbonds[r].id === t.value.ringbonds[i].id)
                     return e.value.ringbonds[r].bondType === "-" ? t.value.ringbonds[i].bond : e.value.ringbonds[r].bond;
         return null;
     }
     initDraw(e, t, r, i) {
-        this.data = e, this.infoOnly = r, this.ringIdCounter = 0, this.ringConnectionIdCounter = 0, this.graph = new Pa(e, this.opts.isomeric), this.rings = Array(), this.ringConnections = Array(), this.originalRings = Array(), this.originalRingConnections = Array(), this.bridgedRing = !1, this.doubleBondConfigCount = null, this.doubleBondConfig = null, this.highlight_atoms = i, this.initRings(), this.initHydrogens();
+        this.data = e, this.infoOnly = r, this.ringIdCounter = 0, this.ringConnectionIdCounter = 0, this.graph = new Ia(e, this.opts.isomeric), this.rings = Array(), this.ringConnections = Array(), this.originalRings = Array(), this.originalRingConnections = Array(), this.bridgedRing = !1, this.doubleBondConfigCount = null, this.doubleBondConfig = null, this.highlight_atoms = i, this.initRings(), this.initHydrogens();
     }
     processGraph() {
         this.position(), this.restoreRingInformation(), this.resolvePrimaryOverlaps();
         let e = this.getOverlapScore();
         this.totalOverlapScore = this.getOverlapScore().total;
         for (var t = 0; t < this.opts.overlapResolutionIterations; t++)
             for (var r = 0; r < this.graph.edges.length; r++) {
@@ -6351,18 +6351,18 @@
                                 if (m.value.rings[0] !== _.value.rings[0])
                                     continue;
                             } else {
                                 if (m.value.rings.length !== 0 || _.value.rings.length !== 0)
                                     continue;
                                 {
                                     let v = m.position.getRotateAwayFromAngle(c.position, u.position, Se.toRad(120)),
-                                        N = _.position.getRotateAwayFromAngle(c.position, u.position, Se.toRad(120));
-                                    this.rotateSubtree(m.id, u.id, v, u.position), this.rotateSubtree(_.id, u.id, N, u.position);
-                                    let B = this.getOverlapScore().total;
-                                    B > this.totalOverlapScore ? (this.rotateSubtree(m.id, u.id, -v, u.position), this.rotateSubtree(_.id, u.id, -N, u.position)) : this.totalOverlapScore = B;
+                                        A = _.position.getRotateAwayFromAngle(c.position, u.position, Se.toRad(120));
+                                    this.rotateSubtree(m.id, u.id, v, u.position), this.rotateSubtree(_.id, u.id, A, u.position);
+                                    let T = this.getOverlapScore().total;
+                                    T > this.totalOverlapScore ? (this.rotateSubtree(m.id, u.id, -v, u.position), this.rotateSubtree(_.id, u.id, -A, u.position)) : this.totalOverlapScore = T;
                                 }
                             }
                         }
                         e = this.getOverlapScore();
                     }
                 }
             }
@@ -6381,27 +6381,27 @@
                         n = s.value.ringbonds[r].bond;
                     if (!e.has(a))
                         e.set(a, [s.id, n]);
                     else {
                         let h = s.id,
                             l = e.get(a)[0],
                             c = e.get(a)[1],
-                            u = new yg(h, l, 1);
+                            u = new Sg(h, l, 1);
                         u.setBondType(c || n || "-");
                         let g = this.graph.addEdge(u),
                             m = this.graph.vertices[l];
                         s.addRingbondChild(l, r), s.value.addNeighbouringElement(m.value.element), m.addRingbondChild(h, r), m.value.addNeighbouringElement(s.value.element), s.edges.push(g), m.edges.push(g), e.delete(a);
                     }
                 }
         }
-        let i = Sg.getRings(this.graph, this.opts.experimentalSSSR);
+        let i = Ag.getRings(this.graph, this.opts.experimentalSSSR);
         if (i !== null) {
             for (var t = 0; t < i.length; t++) {
                 let a = [...i[t]],
-                    n = this.addRing(new Da(a));
+                    n = this.addRing(new $a(a));
                 for (var r = 0; r < a.length; r++)
                     this.graph.vertices[a[r]].value.rings.push(n);
             }
             for (var t = 0; t < this.rings.length - 1; t++)
                 for (var r = t + 1; r < this.rings.length; r++) {
                     let n = this.rings[t],
                         h = this.rings[r],
@@ -6455,15 +6455,15 @@
                 let a = r.getRing(s);
                 t.push(s);
                 for (var n = 0; n < a.neighbours.length; n++) {
                     let h = a.neighbours[n];
                     t.indexOf(h) === -1 && h !== s && Ai.isBridge(r.ringConnections, r.graph.vertices, s, h) && i(h);
                 }
             };
-        return i(e), Dt.unique(t);
+        return i(e), Pt.unique(t);
     }
     /**
      * Checks whether or not a ring is part of a bridged ring.
      *
      * @param {Number} ringId A ring id.
      * @returns {Boolean} A boolean indicating whether or not the supplied ring (by id) is part of a bridged ring system.
      */
@@ -6493,39 +6493,39 @@
                 let m = u.neighbours[n];
                 e.indexOf(m) === -1 && s.add(u.neighbours[n]);
             }
         }
         let h = /* @__PURE__ */ new Set();
         for (let u of i) {
             let g = this.graph.vertices[u],
-                m = Dt.intersection(e, g.value.rings);
+                m = Pt.intersection(e, g.value.rings);
             g.value.rings.length === 1 || m.length === 1 ? r.add(g.id) : h.add(g.id);
         }
         Array();
         let l = Array();
         for (let u of h) {
             let g = this.graph.vertices[u],
                 m = !1;
             for (let _ = 0; _ < g.edges.length; _++)
                 this.edgeRingCount(g.edges[_]) === 1 && (m = !0);
             m ? (g.value.isBridgeNode = !0, r.add(g.id)) : (g.value.isBridge = !0, r.add(g.id));
         }
-        let c = new Da([...r]);
+        let c = new $a([...r]);
         this.addRing(c), c.isBridged = !0, c.neighbours = [...s];
         for (var a = 0; a < e.length; a++)
             c.rings.push(this.getRing(e[a]).clone());
         for (var a = 0; a < c.members.length; a++)
             this.graph.vertices[c.members[a]].value.bridgedRing = c.id;
         for (var a = 0; a < l.length; a++) {
             let g = this.graph.vertices[l[a]];
             g.value.rings = Array();
         }
         for (let u of r) {
             let g = this.graph.vertices[u];
-            g.value.rings = Dt.removeAll(g.value.rings, e), g.value.rings.push(c.id);
+            g.value.rings = Pt.removeAll(g.value.rings, e), g.value.rings.push(c.id);
         }
         for (var a = 0; a < e.length; a++)
             for (var n = a + 1; n < e.length; n++)
                 this.removeRingConnectionsBetween(e[a], e[n]);
         for (let u of s) {
             let g = this.getRingConnections(u, e);
             for (var n = 0; n < g.length; n++)
@@ -6731,15 +6731,15 @@
             t[r] = 0;
         for (var r = 0; r < this.graph.vertices.length; r++)
             for (var i = this.graph.vertices.length; --i > r;) {
                 let n = this.graph.vertices[r],
                     h = this.graph.vertices[i];
                 if (!n.value.isDrawn || !h.value.isDrawn)
                     continue;
-                let l = re.subtract(n.position, h.position).lengthSq();
+                let l = ee.subtract(n.position, h.position).lengthSq();
                 if (l < this.opts.bondLengthSq) {
                     let c = (this.opts.bondLength - Math.sqrt(l)) / this.opts.bondLength;
                     e += c, t[r] += c, t[i] += c;
                 }
             }
         let s = Array();
         for (var r = 0; r < this.graph.vertices.length; r++)
@@ -6771,15 +6771,15 @@
         }
      */
     chooseSide(e, t, r) {
         let i = e.getNeighbours(t.id),
             s = t.getNeighbours(e.id),
             a = i.length,
             n = s.length,
-            h = Dt.merge(i, s),
+            h = Pt.merge(i, s),
             l = [0, 0];
         for (var c = 0; c < h.length; c++)
             this.graph.vertices[h[c]].position.sameSideAs(e.position, t.position, r[0]) ? l[0]++ : l[1]++;
         let u = [0, 0];
         for (var c = 0; c < this.graph.vertices.length; c++)
             this.graph.vertices[c].position.sameSideAs(e.position, t.position, r[0]) ? u[0]++ : u[1]++;
         return {
@@ -6794,15 +6794,15 @@
     /**
      * Sets the center for a ring.
      *
      * @param {Ring} ring A ring.
      */
     setRingCenter(e) {
         let t = e.getSize(),
-            r = new re(0, 0);
+            r = new ee(0, 0);
         for (var i = 0; i < t; i++)
             r.add(this.graph.vertices[e.members[i]].position);
         e.center = r.divide(t);
     }
     /**
      * Gets the center of a ring contained within a bridged ring and containing a given vertex.
      *
@@ -6853,62 +6853,62 @@
             n = s.value.element,
             h = a.value.element;
         if ((!s.value.isDrawn || !a.value.isDrawn) && this.opts.atomVisualization === "default")
             return;
         let l = s.position,
             c = a.position,
             u = this.getEdgeNormals(i),
-            g = Dt.clone(u);
+            g = Pt.clone(u);
         if (g[0].multiplyScalar(10).add(l), g[1].multiplyScalar(10).add(l), i.bondType === "=" || this.getRingbondType(s, a) === "=" || i.isPartOfAromaticRing && this.bridgedRing) {
             let m = this.areVerticesInSameRing(s, a),
                 _ = this.chooseSide(s, a, g);
             if (m) {
-                let N = this.getLargestOrAromaticCommonRing(s, a).center;
+                let A = this.getLargestOrAromaticCommonRing(s, a).center;
                 u[0].multiplyScalar(r.opts.bondSpacing), u[1].multiplyScalar(r.opts.bondSpacing);
-                let B = null;
-                N.sameSideAs(s.position, a.position, re.add(l, u[0])) ? B = new Me(re.add(l, u[0]), re.add(c, u[0]), n, h) : B = new Me(re.add(l, u[1]), re.add(c, u[1]), n, h), B.shorten(this.opts.bondLength - this.opts.shortBondLength * this.opts.bondLength), i.isPartOfAromaticRing ? this.canvasWrapper.drawLine(B, !0) : this.canvasWrapper.drawLine(B), this.canvasWrapper.drawLine(new Me(l, c, n, h));
+                let T = null;
+                A.sameSideAs(s.position, a.position, ee.add(l, u[0])) ? T = new Me(ee.add(l, u[0]), ee.add(c, u[0]), n, h) : T = new Me(ee.add(l, u[1]), ee.add(c, u[1]), n, h), T.shorten(this.opts.bondLength - this.opts.shortBondLength * this.opts.bondLength), i.isPartOfAromaticRing ? this.canvasWrapper.drawLine(T, !0) : this.canvasWrapper.drawLine(T), this.canvasWrapper.drawLine(new Me(l, c, n, h));
             } else if (i.center || s.isTerminal() && a.isTerminal()) {
                 u[0].multiplyScalar(r.opts.halfBondSpacing), u[1].multiplyScalar(r.opts.halfBondSpacing);
-                let v = new Me(re.add(l, u[0]), re.add(c, u[0]), n, h),
-                    N = new Me(re.add(l, u[1]), re.add(c, u[1]), n, h);
-                this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(N);
+                let v = new Me(ee.add(l, u[0]), ee.add(c, u[0]), n, h),
+                    A = new Me(ee.add(l, u[1]), ee.add(c, u[1]), n, h);
+                this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(A);
             } else if (_.anCount == 0 && _.bnCount > 1 || _.bnCount == 0 && _.anCount > 1) {
                 u[0].multiplyScalar(r.opts.halfBondSpacing), u[1].multiplyScalar(r.opts.halfBondSpacing);
-                let v = new Me(re.add(l, u[0]), re.add(c, u[0]), n, h),
-                    N = new Me(re.add(l, u[1]), re.add(c, u[1]), n, h);
-                this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(N);
+                let v = new Me(ee.add(l, u[0]), ee.add(c, u[0]), n, h),
+                    A = new Me(ee.add(l, u[1]), ee.add(c, u[1]), n, h);
+                this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(A);
             } else if (_.sideCount[0] > _.sideCount[1]) {
                 u[0].multiplyScalar(r.opts.bondSpacing), u[1].multiplyScalar(r.opts.bondSpacing);
-                let v = new Me(re.add(l, u[0]), re.add(c, u[0]), n, h);
+                let v = new Me(ee.add(l, u[0]), ee.add(c, u[0]), n, h);
                 v.shorten(this.opts.bondLength - this.opts.shortBondLength * this.opts.bondLength), this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(new Me(l, c, n, h));
             } else if (_.sideCount[0] < _.sideCount[1]) {
                 u[0].multiplyScalar(r.opts.bondSpacing), u[1].multiplyScalar(r.opts.bondSpacing);
-                let v = new Me(re.add(l, u[1]), re.add(c, u[1]), n, h);
+                let v = new Me(ee.add(l, u[1]), ee.add(c, u[1]), n, h);
                 v.shorten(this.opts.bondLength - this.opts.shortBondLength * this.opts.bondLength), this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(new Me(l, c, n, h));
             } else if (_.totalSideCount[0] > _.totalSideCount[1]) {
                 u[0].multiplyScalar(r.opts.bondSpacing), u[1].multiplyScalar(r.opts.bondSpacing);
-                let v = new Me(re.add(l, u[0]), re.add(c, u[0]), n, h);
+                let v = new Me(ee.add(l, u[0]), ee.add(c, u[0]), n, h);
                 v.shorten(this.opts.bondLength - this.opts.shortBondLength * this.opts.bondLength), this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(new Me(l, c, n, h));
             } else if (_.totalSideCount[0] <= _.totalSideCount[1]) {
                 u[0].multiplyScalar(r.opts.bondSpacing), u[1].multiplyScalar(r.opts.bondSpacing);
-                let v = new Me(re.add(l, u[1]), re.add(c, u[1]), n, h);
+                let v = new Me(ee.add(l, u[1]), ee.add(c, u[1]), n, h);
                 v.shorten(this.opts.bondLength - this.opts.shortBondLength * this.opts.bondLength), this.canvasWrapper.drawLine(v), this.canvasWrapper.drawLine(new Me(l, c, n, h));
             }
         } else if (i.bondType === "#") {
             u[0].multiplyScalar(r.opts.bondSpacing / 1.5), u[1].multiplyScalar(r.opts.bondSpacing / 1.5);
-            let m = new Me(re.add(l, u[0]), re.add(c, u[0]), n, h),
-                _ = new Me(re.add(l, u[1]), re.add(c, u[1]), n, h);
+            let m = new Me(ee.add(l, u[0]), ee.add(c, u[0]), n, h),
+                _ = new Me(ee.add(l, u[1]), ee.add(c, u[1]), n, h);
             this.canvasWrapper.drawLine(m), this.canvasWrapper.drawLine(_), this.canvasWrapper.drawLine(new Me(l, c, n, h));
         } else if (i.bondType !== ".") {
             let m = s.value.isStereoCenter,
                 _ = a.value.isStereoCenter;
             i.wedge === "up" ? this.canvasWrapper.drawWedge(new Me(l, c, n, h, m, _)) : i.wedge === "down" ? this.canvasWrapper.drawDashedWedge(new Me(l, c, n, h, m, _)) : this.canvasWrapper.drawLine(new Me(l, c, n, h, m, _));
         }
         if (t) {
-            let m = re.midpoint(l, c);
+            let m = ee.midpoint(l, c);
             this.canvasWrapper.drawDebugText(m.x, m.y, "e: " + e);
         }
     }
     /**
      * Draws the vertices representing atoms to the canvas.
      *
      * @param {Boolean} debug A boolean indicating whether or not to draw debug messages to the canvas.
@@ -6939,19 +6939,19 @@
                     n,
                     this.graph.vertices.length,
                     s.getAttachedPseudoElements()
                 ) : this.opts.atomVisualization === "balls" && this.canvasWrapper.drawBall(i.position.x, i.position.y, l);
             else if (i.getNeighbourCount() === 2 && i.forcePositioned == !0) {
                 let _ = this.graph.vertices[i.neighbours[0]].position,
                     v = this.graph.vertices[i.neighbours[1]].position,
-                    N = re.threePointangle(i.position, _, v);
-                Math.abs(Math.PI - N) < 0.1 && this.canvasWrapper.drawPoint(i.position.x, i.position.y, l);
+                    A = ee.threePointangle(i.position, _, v);
+                Math.abs(Math.PI - A) < 0.1 && this.canvasWrapper.drawPoint(i.position.x, i.position.y, l);
             }
             if (e) {
-                let _ = "v: " + i.id + " " + Dt.print(s.ringbonds);
+                let _ = "v: " + i.id + " " + Pt.print(s.ringbonds);
                 this.canvasWrapper.drawDebugText(i.position.x, i.position.y, _);
             }
         }
         if (this.opts.debug)
             for (var t = 0; t < this.rings.length; t++) {
                 let i = this.rings[t].center;
                 this.canvasWrapper.drawDebugPoint(i.x, i.y, "r: " + this.rings[t].id);
@@ -7012,17 +7012,17 @@
      * @param {(Vertex|null)} [startVertex=null] The first vertex to be positioned inside the ring.
      * @param {(Vertex|null)} [previousVertex=null] The last vertex that was positioned.
      * @param {Boolean} [previousVertex=false] A boolean indicating whether or not this ring was force positioned already - this is needed after force layouting a ring, in order to draw rings connected to it.
      */
     createRing(e, t = null, r = null, i = null) {
         if (e.positioned)
             return;
-        t = t || new re(0, 0);
+        t = t || new ee(0, 0);
         let s = e.getOrderedNeighbours(this.ringConnections),
-            a = r ? re.subtract(r.position, t).angle() : 0,
+            a = r ? ee.subtract(r.position, t).angle() : 0,
             n = Se.polyCircumradius(this.opts.bondLength, e.getSize()),
             h = Se.centralAngle(e.getSize());
         e.centralAngle = h;
         let l = a,
             c = this,
             u = r ? r.id : null;
         if (e.members.indexOf(u) === -1 && (r && (r.positioned = !1), u = e.members[0]), e.isBridged) {
@@ -7046,45 +7046,45 @@
                 v.positioned || v.setPosition(t.x + Math.cos(l) * n, t.y + Math.sin(l) * n), l += h, (!e.isBridged || e.rings.length < 3) && (v.angle = l, v.positioned = !0);
             }, u, i ? i.id : null);
         e.positioned = !0, e.center = t;
         for (var g = 0; g < s.length; g++) {
             let v = this.getRing(s[g].neighbour);
             if (v.positioned)
                 continue;
-            let N = Ai.getVertices(this.ringConnections, e.id, v.id);
-            if (N.length === 2) {
+            let A = Ai.getVertices(this.ringConnections, e.id, v.id);
+            if (A.length === 2) {
                 e.isFused = !0, v.isFused = !0;
-                let B = this.graph.vertices[N[0]],
-                    x = this.graph.vertices[N[1]],
-                    L = re.midpoint(B.position, x.position),
-                    k = re.normals(B.position, x.position);
-                k[0].normalize(), k[1].normalize();
-                let z = Se.polyCircumradius(this.opts.bondLength, v.getSize()),
-                    D = Se.apothem(z, v.getSize());
-                k[0].multiplyScalar(D).add(L), k[1].multiplyScalar(D).add(L);
-                let Y = k[0];
-                re.subtract(t, k[1]).lengthSq() > re.subtract(t, k[0]).lengthSq() && (Y = k[1]);
-                let O = re.subtract(B.position, Y),
-                    Z = re.subtract(x.position, Y);
-                O.clockwise(Z) === -1 ? v.positioned || this.createRing(v, Y, B, x) : v.positioned || this.createRing(v, Y, x, B);
-            } else if (N.length === 1) {
+                let T = this.graph.vertices[A[0]],
+                    k = this.graph.vertices[A[1]],
+                    x = ee.midpoint(T.position, k.position),
+                    R = ee.normals(T.position, k.position);
+                R[0].normalize(), R[1].normalize();
+                let O = Se.polyCircumradius(this.opts.bondLength, v.getSize()),
+                    D = Se.apothem(O, v.getSize());
+                R[0].multiplyScalar(D).add(x), R[1].multiplyScalar(D).add(x);
+                let te = R[0];
+                ee.subtract(t, R[1]).lengthSq() > ee.subtract(t, R[0]).lengthSq() && (te = R[1]);
+                let q = ee.subtract(T.position, te),
+                    re = ee.subtract(k.position, te);
+                q.clockwise(re) === -1 ? v.positioned || this.createRing(v, te, T, k) : v.positioned || this.createRing(v, te, k, T);
+            } else if (A.length === 1) {
                 e.isSpiro = !0, v.isSpiro = !0;
-                let B = this.graph.vertices[N[0]],
-                    x = re.subtract(t, B.position);
-                x.invert(), x.normalize();
-                let L = Se.polyCircumradius(this.opts.bondLength, v.getSize());
-                x.multiplyScalar(L), x.add(B.position), v.positioned || this.createRing(v, x, B);
+                let T = this.graph.vertices[A[0]],
+                    k = ee.subtract(t, T.position);
+                k.invert(), k.normalize();
+                let x = Se.polyCircumradius(this.opts.bondLength, v.getSize());
+                k.multiplyScalar(x), k.add(T.position), v.positioned || this.createRing(v, k, T);
             }
         }
         for (var g = 0; g < e.members.length; g++) {
             let v = this.graph.vertices[e.members[g]],
-                N = v.neighbours;
-            for (var m = 0; m < N.length; m++) {
-                let B = this.graph.vertices[N[m]];
-                B.positioned || (B.value.isConnectedToRing = !0, this.createNextBond(B, v, 0));
+                A = v.neighbours;
+            for (var m = 0; m < A.length; m++) {
+                let T = this.graph.vertices[A[m]];
+                T.positioned || (T.value.isConnectedToRing = !0, this.createNextBond(T, v, 0));
             }
         }
     }
     /**
      * Rotate an entire subtree by an angle around a center.
      *
      * @param {Number} vertexId A vertex id (the root of the sub-tree).
@@ -7109,15 +7109,15 @@
      * @param {Number} parentVertexId A vertex id in the previous direction of the subtree.
      * @param {Number[]} vertexOverlapScores An array containing the vertex overlap scores indexed by vertex id.
      * @returns {Object} An object containing the total overlap score and the center of mass of the subtree weighted by overlap score { value: 0.2, center: new Vector2() }.
      */
     getSubtreeOverlapScore(e, t, r) {
         let i = this,
             s = 0,
-            a = new re(0, 0),
+            a = new ee(0, 0),
             n = 0;
         return this.graph.traverseTree(e, t, function(h) {
             if (!h.value.isDrawn)
                 return;
             let l = r[h.id];
             l > i.opts.overlapSensitivity && (s += l, n++);
             let c = i.graph.vertices[h.id].position.clone();
@@ -7129,15 +7129,15 @@
     }
     /**
      * Returns the current (positioned vertices so far) center of mass.
      * 
      * @returns {Vector2} The current center of mass.
      */
     getCurrentCenterOfMass() {
-        let e = new re(0, 0),
+        let e = new ee(0, 0),
             t = 0;
         for (var r = 0; r < this.graph.vertices.length; r++) {
             let i = this.graph.vertices[r];
             i.positioned && (e.add(i.position), t++);
         }
         return e.divide(t);
     }
@@ -7145,15 +7145,15 @@
      * Returns the current (positioned vertices so far) center of mass in the neighbourhood of a given position.
      *
      * @param {Vector2} vec The point at which to look for neighbours.
      * @param {Number} [r=currentBondLength*2.0] The radius of vertices to include.
      * @returns {Vector2} The current center of mass.
      */
     getCurrentCenterOfMassInNeigbourhood(e, t = this.opts.bondLength * 2) {
-        let r = new re(0, 0),
+        let r = new ee(0, 0),
             i = 0,
             s = t * t;
         for (var a = 0; a < this.graph.vertices.length; a++) {
             let n = this.graph.vertices[a];
             n.positioned && e.distanceSq(n.position) < s && (r.add(n.position), i++);
         }
         return r.divide(i);
@@ -7263,83 +7263,83 @@
             (h.bondType === "/" || h.bondType === "\\") && ++this.doubleBondConfigCount % 2 === 1 && this.doubleBondConfig === null && (this.doubleBondConfig = h.bondType, a = !0, t.parentVertexId === null && e.value.branchBond && (this.doubleBondConfig === "/" ? this.doubleBondConfig = "\\" : this.doubleBondConfig === "\\" && (this.doubleBondConfig = "/")));
         }
         if (!s)
             if (t)
                 if (t.value.rings.length > 0) {
                     let h = t.neighbours,
                         l = null,
-                        c = new re(0, 0);
+                        c = new ee(0, 0);
                     if (t.value.bridgedRing === null && t.value.rings.length > 1)
                         for (var n = 0; n < h.length; n++) {
                             let u = this.graph.vertices[h[n]];
-                            if (Dt.containsAll(u.value.rings, t.value.rings)) {
+                            if (Pt.containsAll(u.value.rings, t.value.rings)) {
                                 l = u;
                                 break;
                             }
                         }
                     if (l === null) {
                         for (var n = 0; n < h.length; n++) {
                             let g = this.graph.vertices[h[n]];
-                            g.positioned && this.areVerticesInSameRing(g, t) && c.add(re.subtract(g.position, t.position));
+                            g.positioned && this.areVerticesInSameRing(g, t) && c.add(ee.subtract(g.position, t.position));
                         }
                         c.invert().normalize().multiplyScalar(this.opts.bondLength).add(t.position);
                     } else
                         c = l.position.clone().rotateAround(Math.PI, t.position);
                     e.previousPosition = t.position, e.setPositionFromVector(c), e.positioned = !0;
                 } else {
-                    let h = new re(this.opts.bondLength, 0);
+                    let h = new ee(this.opts.bondLength, 0);
                     h.rotate(r), h.add(t.position), e.setPositionFromVector(h), e.previousPosition = t.position, e.positioned = !0;
                 }
         else {
-            let h = new re(this.opts.bondLength, 0);
+            let h = new ee(this.opts.bondLength, 0);
             h.rotate(Se.toRad(-60)), e.previousPosition = h, e.setPosition(this.opts.bondLength, 0), e.angle = Se.toRad(-60), e.value.bridgedRing === null && (e.positioned = !0);
         }
         if (e.value.bridgedRing !== null) {
             let h = this.getRing(e.value.bridgedRing);
             if (!h.positioned) {
-                let l = re.subtract(e.previousPosition, e.position);
+                let l = ee.subtract(e.previousPosition, e.position);
                 l.invert(), l.normalize();
                 let c = Se.polyCircumradius(this.opts.bondLength, h.members.length);
                 l.multiplyScalar(c), l.add(e.position), this.createRing(h, l, e);
             }
         } else if (e.value.rings.length > 0) {
             let h = this.getRing(e.value.rings[0]);
             if (!h.positioned) {
-                let l = re.subtract(e.previousPosition, e.position);
+                let l = ee.subtract(e.previousPosition, e.position);
                 l.invert(), l.normalize();
                 let c = Se.polyCircumradius(this.opts.bondLength, h.getSize());
                 l.multiplyScalar(c), l.add(e.position), this.createRing(h, l, e);
             }
         } else {
             e.value.isStereoCenter;
             let h = e.getNeighbours(),
                 l = Array();
             for (var n = 0; n < h.length; n++)
                 this.graph.vertices[h[n]].value.isDrawn && l.push(h[n]);
-            t && (l = Dt.remove(l, t.id));
+            t && (l = Pt.remove(l, t.id));
             let c = e.getAngle();
             if (l.length === 1) {
                 let u = this.graph.vertices[l[0]];
                 if (e.value.bondType === "#" || t && t.value.bondType === "#" || e.value.bondType === "=" && t && t.value.rings.length === 0 && t.value.bondType === "=" && e.value.branchBond !== "-") {
                     if (e.value.drawExplicit = !1, t) {
                         let m = this.graph.getEdge(e.id, t.id);
                         m.center = !0;
                     }
                     let g = this.graph.getEdge(e.id, u.id);
                     g.center = !0, (e.value.bondType === "#" || t && t.value.bondType === "#") && (u.angle = 0), u.drawExplicit = !0, this.createNextBond(u, e, c + u.angle);
                 } else if (t && t.value.rings.length > 0) {
                     let g = Se.toRad(60),
                         m = -g,
-                        _ = new re(this.opts.bondLength, 0),
-                        v = new re(this.opts.bondLength, 0);
+                        _ = new ee(this.opts.bondLength, 0),
+                        v = new ee(this.opts.bondLength, 0);
                     _.rotate(g).add(e.position), v.rotate(m).add(e.position);
-                    let N = this.getCurrentCenterOfMass(),
-                        B = _.distanceSq(N),
-                        x = v.distanceSq(N);
-                    u.angle = B < x ? m : g, this.createNextBond(u, e, c + u.angle);
+                    let A = this.getCurrentCenterOfMass(),
+                        T = _.distanceSq(A),
+                        k = v.distanceSq(A);
+                    u.angle = T < k ? m : g, this.createNextBond(u, e, c + u.angle);
                 } else {
                     let g = e.angle;
                     if (t && t.neighbours.length > 3 ? g > 0 ? g = Math.min(1.0472, g) : g < 0 ? g = Math.max(-1.0472, g) : g = 1.0472 : g || (g = this.getLastVertexWithAngle(e.id).angle, g || (g = 1.0472)), t && !a) {
                         let m = this.graph.getEdge(e.id, u.id).bondType;
                         m === "/" ? (this.doubleBondConfig === "/" || this.doubleBondConfig === "\\" && (g = -g), this.doubleBondConfig = null) : m === "\\" && (this.doubleBondConfig === "/" ? g = -g : this.doubleBondConfig, this.doubleBondConfig = null);
                     }
                     i ? u.angle = g : u.angle = -g, this.createNextBond(u, e, c + u.angle);
@@ -7348,56 +7348,56 @@
                 let u = e.angle;
                 u || (u = 1.0472);
                 let g = this.graph.getTreeDepth(l[0], e.id),
                     m = this.graph.getTreeDepth(l[1], e.id),
                     _ = this.graph.vertices[l[0]],
                     v = this.graph.vertices[l[1]];
                 _.value.subtreeDepth = g, v.value.subtreeDepth = m;
-                let N = this.graph.getTreeDepth(t ? t.id : null, e.id);
-                t && (t.value.subtreeDepth = N);
-                let B = 0,
-                    x = 1;
-                v.value.element === "C" && _.value.element !== "C" && m > 1 && g < 5 ? (B = 1, x = 0) : v.value.element !== "C" && _.value.element === "C" && g > 1 && m < 5 ? (B = 0, x = 1) : m > g && (B = 1, x = 0);
-                let L = this.graph.vertices[l[B]],
-                    k = this.graph.vertices[l[x]];
-                this.graph.getEdge(e.id, L.id), this.graph.getEdge(e.id, k.id);
-                let z = !1;
-                N < g && N < m && (z = !0), k.angle = u, L.angle = -u, this.doubleBondConfig === "\\" ? k.value.branchBond === "\\" && (k.angle = -u, L.angle = u) : this.doubleBondConfig === "/" && k.value.branchBond === "/" && (k.angle = -u, L.angle = u), this.createNextBond(k, e, c + k.angle, z), this.createNextBond(L, e, c + L.angle, z);
+                let A = this.graph.getTreeDepth(t ? t.id : null, e.id);
+                t && (t.value.subtreeDepth = A);
+                let T = 0,
+                    k = 1;
+                v.value.element === "C" && _.value.element !== "C" && m > 1 && g < 5 ? (T = 1, k = 0) : v.value.element !== "C" && _.value.element === "C" && g > 1 && m < 5 ? (T = 0, k = 1) : m > g && (T = 1, k = 0);
+                let x = this.graph.vertices[l[T]],
+                    R = this.graph.vertices[l[k]];
+                this.graph.getEdge(e.id, x.id), this.graph.getEdge(e.id, R.id);
+                let O = !1;
+                A < g && A < m && (O = !0), R.angle = u, x.angle = -u, this.doubleBondConfig === "\\" ? R.value.branchBond === "\\" && (R.angle = -u, x.angle = u) : this.doubleBondConfig === "/" && R.value.branchBond === "/" && (R.angle = -u, x.angle = u), this.createNextBond(R, e, c + R.angle, O), this.createNextBond(x, e, c + x.angle, O);
             } else if (l.length === 3) {
                 let u = this.graph.getTreeDepth(l[0], e.id),
                     g = this.graph.getTreeDepth(l[1], e.id),
                     m = this.graph.getTreeDepth(l[2], e.id),
                     _ = this.graph.vertices[l[0]],
                     v = this.graph.vertices[l[1]],
-                    N = this.graph.vertices[l[2]];
-                _.value.subtreeDepth = u, v.value.subtreeDepth = g, N.value.subtreeDepth = m, g > u && g > m ? (_ = this.graph.vertices[l[1]], v = this.graph.vertices[l[0]], N = this.graph.vertices[l[2]]) : m > u && m > g && (_ = this.graph.vertices[l[2]], v = this.graph.vertices[l[0]], N = this.graph.vertices[l[1]]), t && t.value.rings.length < 1 && _.value.rings.length < 1 && v.value.rings.length < 1 && N.value.rings.length < 1 && this.graph.getTreeDepth(v.id, e.id) === 1 && this.graph.getTreeDepth(N.id, e.id) === 1 && this.graph.getTreeDepth(_.id, e.id) > 1 ? (_.angle = -e.angle, e.angle >= 0 ? (v.angle = Se.toRad(30), N.angle = Se.toRad(90)) : (v.angle = -Se.toRad(30), N.angle = -Se.toRad(90)), this.createNextBond(_, e, c + _.angle), this.createNextBond(v, e, c + v.angle), this.createNextBond(N, e, c + N.angle)) : (_.angle = 0, v.angle = Se.toRad(90), N.angle = -Se.toRad(90), this.createNextBond(_, e, c + _.angle), this.createNextBond(v, e, c + v.angle), this.createNextBond(N, e, c + N.angle));
+                    A = this.graph.vertices[l[2]];
+                _.value.subtreeDepth = u, v.value.subtreeDepth = g, A.value.subtreeDepth = m, g > u && g > m ? (_ = this.graph.vertices[l[1]], v = this.graph.vertices[l[0]], A = this.graph.vertices[l[2]]) : m > u && m > g && (_ = this.graph.vertices[l[2]], v = this.graph.vertices[l[0]], A = this.graph.vertices[l[1]]), t && t.value.rings.length < 1 && _.value.rings.length < 1 && v.value.rings.length < 1 && A.value.rings.length < 1 && this.graph.getTreeDepth(v.id, e.id) === 1 && this.graph.getTreeDepth(A.id, e.id) === 1 && this.graph.getTreeDepth(_.id, e.id) > 1 ? (_.angle = -e.angle, e.angle >= 0 ? (v.angle = Se.toRad(30), A.angle = Se.toRad(90)) : (v.angle = -Se.toRad(30), A.angle = -Se.toRad(90)), this.createNextBond(_, e, c + _.angle), this.createNextBond(v, e, c + v.angle), this.createNextBond(A, e, c + A.angle)) : (_.angle = 0, v.angle = Se.toRad(90), A.angle = -Se.toRad(90), this.createNextBond(_, e, c + _.angle), this.createNextBond(v, e, c + v.angle), this.createNextBond(A, e, c + A.angle));
             } else if (l.length === 4) {
                 let u = this.graph.getTreeDepth(l[0], e.id),
                     g = this.graph.getTreeDepth(l[1], e.id),
                     m = this.graph.getTreeDepth(l[2], e.id),
                     _ = this.graph.getTreeDepth(l[3], e.id),
                     v = this.graph.vertices[l[0]],
-                    N = this.graph.vertices[l[1]],
-                    B = this.graph.vertices[l[2]],
-                    x = this.graph.vertices[l[3]];
-                v.value.subtreeDepth = u, N.value.subtreeDepth = g, B.value.subtreeDepth = m, x.value.subtreeDepth = _, g > u && g > m && g > _ ? (v = this.graph.vertices[l[1]], N = this.graph.vertices[l[0]], B = this.graph.vertices[l[2]], x = this.graph.vertices[l[3]]) : m > u && m > g && m > _ ? (v = this.graph.vertices[l[2]], N = this.graph.vertices[l[0]], B = this.graph.vertices[l[1]], x = this.graph.vertices[l[3]]) : _ > u && _ > g && _ > m && (v = this.graph.vertices[l[3]], N = this.graph.vertices[l[0]], B = this.graph.vertices[l[1]], x = this.graph.vertices[l[2]]), v.angle = -Se.toRad(36), N.angle = Se.toRad(36), B.angle = -Se.toRad(108), x.angle = Se.toRad(108), this.createNextBond(v, e, c + v.angle), this.createNextBond(N, e, c + N.angle), this.createNextBond(B, e, c + B.angle), this.createNextBond(x, e, c + x.angle);
+                    A = this.graph.vertices[l[1]],
+                    T = this.graph.vertices[l[2]],
+                    k = this.graph.vertices[l[3]];
+                v.value.subtreeDepth = u, A.value.subtreeDepth = g, T.value.subtreeDepth = m, k.value.subtreeDepth = _, g > u && g > m && g > _ ? (v = this.graph.vertices[l[1]], A = this.graph.vertices[l[0]], T = this.graph.vertices[l[2]], k = this.graph.vertices[l[3]]) : m > u && m > g && m > _ ? (v = this.graph.vertices[l[2]], A = this.graph.vertices[l[0]], T = this.graph.vertices[l[1]], k = this.graph.vertices[l[3]]) : _ > u && _ > g && _ > m && (v = this.graph.vertices[l[3]], A = this.graph.vertices[l[0]], T = this.graph.vertices[l[1]], k = this.graph.vertices[l[2]]), v.angle = -Se.toRad(36), A.angle = Se.toRad(36), T.angle = -Se.toRad(108), k.angle = Se.toRad(108), this.createNextBond(v, e, c + v.angle), this.createNextBond(A, e, c + A.angle), this.createNextBond(T, e, c + T.angle), this.createNextBond(k, e, c + k.angle);
             }
         }
     }
     /**
      * Gets the vetex sharing the edge that is the common bond of two rings.
      *
      * @param {Vertex} vertex A vertex.
      * @returns {(Number|null)} The id of a vertex sharing the edge that is the common bond of two rings with the vertex provided or null, if none.
      */
     getCommonRingbondNeighbour(e) {
         let t = e.neighbours;
         for (var r = 0; r < t.length; r++) {
             let i = this.graph.vertices[t[r]];
-            if (Dt.containsAll(i.value.rings, e.value.rings))
+            if (Pt.containsAll(i.value.rings, e.value.rings))
                 return i;
         }
         return null;
     }
     /**
      * Check if a vector is inside any ring.
      *
@@ -7455,29 +7455,29 @@
      *
      * @param {Edge} edge An edge.
      * @returns {Vector2[]} An array containing two vectors, representing the normals.
      */
     getEdgeNormals(e) {
         let t = this.graph.vertices[e.sourceId].position,
             r = this.graph.vertices[e.targetId].position;
-        return re.units(t, r);
+        return ee.units(t, r);
     }
     /**
      * Returns an array of vertices that are neighbouring a vertix but are not members of a ring (including bridges).
      *
      * @param {Number} vertexId A vertex id.
      * @returns {Vertex[]} An array of vertices.
      */
     getNonRingNeighbours(e) {
         let t = Array(),
             r = this.graph.vertices[e],
             i = r.neighbours;
         for (var s = 0; s < i.length; s++) {
             let a = this.graph.vertices[i[s]];
-            Dt.intersection(r.value.rings, a.value.rings).length === 0 && a.value.isBridge == !1 && t.push(a);
+            Pt.intersection(r.value.rings, a.value.rings).length === 0 && a.value.isBridge == !1 && t.push(a);
         }
         return t;
     }
     /**
      * Annotaed stereochemistry information for visualization.
      */
     annotateStereochemistry() {
@@ -7486,20 +7486,20 @@
             let a = this.graph.vertices[t];
             if (!a.value.isStereoCenter)
                 continue;
             let n = a.getNeighbours(),
                 h = n.length,
                 l = Array(h);
             for (var r = 0; r < h; r++) {
-                let Z = new Uint8Array(this.graph.vertices.length),
+                let re = new Uint8Array(this.graph.vertices.length),
                     j = Array(Array());
-                Z[a.id] = 1, this.visitStereochemistry(n[r], a.id, Z, j, e, 0);
+                re[a.id] = 1, this.visitStereochemistry(n[r], a.id, re, j, e, 0);
                 for (var i = 0; i < j.length; i++)
-                    j[i].sort(function(q, se) {
-                        return se - q;
+                    j[i].sort(function(X, se) {
+                        return se - X;
                     });
                 l[r] = [r, j];
             }
             let c = 0,
                 u = 0;
             for (var r = 0; r < l.length; r++) {
                 l[r][1].length > c && (c = l[r][1].length);
@@ -7513,60 +7513,60 @@
                 l[r][1].push([n[r]]);
                 for (var i = 0; i < l[r][1].length; i++) {
                     let se = u - l[r][1][i].length;
                     for (var s = 0; s < se; s++)
                         l[r][1][i].push(0);
                 }
             }
-            l.sort(function(Z, j) {
-                for (var q = 0; q < Z[1].length; q++)
-                    for (var se = 0; se < Z[1][q].length; se++) {
-                        if (Z[1][q][se] > j[1][q][se])
+            l.sort(function(re, j) {
+                for (var X = 0; X < re[1].length; X++)
+                    for (var se = 0; se < re[1][X].length; se++) {
+                        if (re[1][X][se] > j[1][X][se])
                             return -1;
-                        if (Z[1][q][se] < j[1][q][se])
+                        if (re[1][X][se] < j[1][X][se])
                             return 1;
                     }
                 return 0;
             });
             let g = new Uint8Array(h);
             for (var r = 0; r < h; r++)
                 g[r] = l[r][0], a.value.priority = r;
             let m = this.graph.vertices[n[g[0]]].position,
                 _ = this.graph.vertices[n[g[1]]].position,
                 v = this.graph.vertices[n[g[2]]].position,
-                N = m.relativeClockwise(_, a.position);
+                A = m.relativeClockwise(_, a.position);
             m.relativeClockwise(v, a.position);
-            let B = N === -1,
-                x = a.value.bracket.chirality === "@" ? -1 : 1,
-                L = Se.parityOfPermutation(g) * x === 1 ? "R" : "S",
-                k = "down",
-                z = "up";
-            (B && L !== "R" || !B && L !== "S") && (a.value.hydrogenDirection = "up", k = "up", z = "down"), a.value.hasHydrogen && (this.graph.getEdge(a.id, n[g[g.length - 1]]).wedge = k);
+            let T = A === -1,
+                k = a.value.bracket.chirality === "@" ? -1 : 1,
+                x = Se.parityOfPermutation(g) * k === 1 ? "R" : "S",
+                R = "down",
+                O = "up";
+            (T && x !== "R" || !T && x !== "S") && (a.value.hydrogenDirection = "up", R = "up", O = "down"), a.value.hasHydrogen && (this.graph.getEdge(a.id, n[g[g.length - 1]]).wedge = R);
             let D = new Array(n.length - 1),
-                Y = a.value.rings.length > 1 && a.value.hasHydrogen,
-                O = a.value.hasHydrogen ? 1 : 0;
-            for (var r = 0; r < g.length - O; r++) {
+                te = a.value.rings.length > 1 && a.value.hasHydrogen,
+                q = a.value.hasHydrogen ? 1 : 0;
+            for (var r = 0; r < g.length - q; r++) {
                 D[r] = new Uint32Array(2);
                 let j = this.graph.vertices[n[g[r]]];
                 D[r][0] += j.value.isStereoCenter ? 0 : 1e5, D[r][0] += this.areVerticesInSameRing(j, a) ? 0 : 1e4, D[r][0] += j.value.isHeteroAtom() ? 1e3 : 0, D[r][0] -= j.value.subtreeDepth === 0 ? 1e3 : 0, D[r][0] += 1e3 - j.value.subtreeDepth, D[r][1] = n[g[r]];
             }
-            if (D.sort(function(Z, j) {
-                    return Z[0] > j[0] ? -1 : Z[0] < j[0] ? 1 : 0;
-                }), !Y) {
-                let Z = D[0][1];
+            if (D.sort(function(re, j) {
+                    return re[0] > j[0] ? -1 : re[0] < j[0] ? 1 : 0;
+                }), !te) {
+                let re = D[0][1];
                 if (a.value.hasHydrogen)
-                    this.graph.getEdge(a.id, Z).wedge = z;
+                    this.graph.getEdge(a.id, re).wedge = O;
                 else {
-                    let j = z;
-                    for (var r = g.length - 1; r >= 0 && (j === k ? j = z : j = k, n[g[r]] !== Z); r--)
+                    let j = O;
+                    for (var r = g.length - 1; r >= 0 && (j === R ? j = O : j = R, n[g[r]] !== re); r--)
                     ;
-                    this.graph.getEdge(a.id, Z).wedge = j;
+                    this.graph.getEdge(a.id, re).wedge = j;
                 }
             }
-            a.value.chirality = L;
+            a.value.chirality = x;
         }
     }
     /**
      * 
      * 
      * @param {Number} vertexId The id of a vertex.
      * @param {(Number|null)} previousVertexId The id of the parent vertex of the vertex.
@@ -7647,27 +7647,27 @@
                     continue;
                 const u = c.getAttachedPseudoElements();
                 u.hasOwnProperty("0O") && u.hasOwnProperty("3C") && (c.isDrawn = !1, i.value.attachPseudoElement("Ac", "", 0));
             }
         }
     }
 };
-var kg = Ng;
-const Rg = Xn,
+var xg = Rg;
+const Tg = Zn,
     je = ar,
-    xg = Kr;
+    Eg = Kr;
 
-function Tg(d) {
+function Lg(d) {
     for (var e = "", t = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789", r = t.length, i = 0; i < d; i++)
         e += t.charAt(Math.floor(Math.random() * r));
     return e;
 }
-let Eg = class dt {
+let Mg = class dt {
     constructor(e, t, r, i = !0) {
-        if (typeof t == "string" || t instanceof String ? this.svg = document.getElementById(t) : this.svg = t, this.container = null, this.opts = r, this.uid = Tg(5), this.gradientId = 0, this.backgroundItems = [], this.paths = [], this.vertices = [], this.gradients = [], this.highlights = [], this.drawingWidth = 0, this.drawingHeight = 0, this.halfBondThickness = this.opts.bondThickness / 2, this.themeManager = e, this.maskElements = [], this.maxX = -Number.MAX_VALUE, this.maxY = -Number.MAX_VALUE, this.minX = Number.MAX_VALUE, this.minY = Number.MAX_VALUE, i)
+        if (typeof t == "string" || t instanceof String ? this.svg = document.getElementById(t) : this.svg = t, this.container = null, this.opts = r, this.uid = Lg(5), this.gradientId = 0, this.backgroundItems = [], this.paths = [], this.vertices = [], this.gradients = [], this.highlights = [], this.drawingWidth = 0, this.drawingHeight = 0, this.halfBondThickness = this.opts.bondThickness / 2, this.themeManager = e, this.maskElements = [], this.maxX = -Number.MAX_VALUE, this.maxY = -Number.MAX_VALUE, this.minX = Number.MAX_VALUE, this.minY = Number.MAX_VALUE, i)
             for (; this.svg.firstChild;)
                 this.svg.removeChild(this.svg.firstChild);
         this.style = document.createElementNS("http://www.w3.org/2000/svg", "style"), this.style.appendChild(document.createTextNode(`
                 .element {
                     font: ${this.opts.fontSizeLarge}pt ${this.opts.fontFamily};
                 }
                 .sub {
@@ -7836,18 +7836,18 @@
             l = e.getLength(),
             c = 1.25 / (l / (this.opts.bondLength / 10)),
             u = this.createGradient(e);
         for (let g = 0; g < 1; g += c) {
             let m = je.multiplyScalar(h, g * l),
                 _ = je.add(a, m),
                 v = this.opts.fontSizeLarge / 2 * g,
-                N = je.multiplyScalar(i[0], v);
-            _.subtract(N);
-            let B = _.clone();
-            B.add(je.multiplyScalar(N, 2)), this.drawLine(new Rg(_, B), null, u);
+                A = je.multiplyScalar(i[0], v);
+            _.subtract(A);
+            let T = _.clone();
+            T.add(je.multiplyScalar(A, 2)), this.drawLine(new Tg(_, T), null, u);
         }
     }
     /**
      * Draws a debug dot at a given coordinate and adds text.
      *
      * @param {Number} x The x coordinate.
      * @param {Number} y The y coordindate.
@@ -7876,15 +7876,15 @@
      *
      * @param {x} x The x coordinate of the ring.
      * @param {y} r The y coordinate of the ring.
      * @param {s} s The size of the ring.
      */
     drawRing(e, t, r) {
         let i = document.createElementNS("http://www.w3.org/2000/svg", "circle"),
-            s = xg.apothemFromSideLength(this.opts.bondLength, r);
+            s = Eg.apothemFromSideLength(this.opts.bondLength, r);
         i.setAttributeNS(null, "cx", e), i.setAttributeNS(null, "cy", t), i.setAttributeNS(null, "r", s - this.opts.bondSpacing), i.setAttributeNS(null, "stroke", this.themeManager.getColor("C")), i.setAttributeNS(null, "stroke-width", this.opts.bondThickness), i.setAttributeNS(null, "fill", "none"), this.paths.push(i);
     }
     /**
      * Draws a line.
      *
      * @param {Line} line A line.
      * @param {Boolean} dashed defaults to false.
@@ -7966,17 +7966,17 @@
         let n = r,
             h = i,
             l = document.createElementNS("http://www.w3.org/2000/svg", "text");
         l.setAttributeNS(null, "class", "element");
         let c = document.createElementNS("http://www.w3.org/2000/svg", "g");
         l.setAttributeNS(null, "fill", "#ffffff"), t === "left" && (e = e.reverse()), (t === "right" || t === "down" || t === "up") && (r -= a.width / 2), t === "left" && (r += a.width / 2), e.forEach((m, _) => {
             const v = m[0],
-                N = m[1];
-            let B = document.createElementNS("http://www.w3.org/2000/svg", "tspan");
-            B.setAttributeNS(null, "fill", this.themeManager.getColor(N)), B.textContent = v, (t === "up" || t === "down") && (B.setAttributeNS(null, "x", "0px"), t === "up" ? B.setAttributeNS(null, "y", `-${0.9 * _}em`) : B.setAttributeNS(null, "y", `${0.9 * _}em`)), l.appendChild(B);
+                A = m[1];
+            let T = document.createElementNS("http://www.w3.org/2000/svg", "tspan");
+            T.setAttributeNS(null, "fill", this.themeManager.getColor(A)), T.textContent = v, (t === "up" || t === "down") && (T.setAttributeNS(null, "x", "0px"), t === "up" ? T.setAttributeNS(null, "y", `-${0.9 * _}em`) : T.setAttributeNS(null, "y", `${0.9 * _}em`)), l.appendChild(T);
         }), l.setAttributeNS(null, "data-direction", t), t === "left" || t === "right" ? (l.setAttributeNS(null, "dominant-baseline", "alphabetic"), l.setAttributeNS(null, "y", "0.36em")) : l.setAttributeNS(null, "dominant-baseline", "central"), t === "left" && l.setAttributeNS(null, "text-anchor", "end"), c.appendChild(l), c.setAttributeNS(null, "style", `transform: translateX(${r}px) translateY(${i}px)`);
         let u = this.opts.fontSizeLarge * 0.75;
         e[0][1].length > 1 && (u = this.opts.fontSizeLarge * 1.1);
         let g = document.createElementNS("http://www.w3.org/2000/svg", "circle");
         g.setAttributeNS(null, "cx", n), g.setAttributeNS(null, "cy", h), g.setAttributeNS(null, "r", u), g.setAttributeNS(null, "fill", "black"), this.maskElements.push(g), this.vertices.push(c);
     }
     /**
@@ -8087,26 +8087,26 @@
             u = [];
         return e.split(`
 `).forEach((g) => {
             let m = dt.measureText(g, r, i, 1);
             if (m.width >= s) {
                 let _ = 0,
                     v = 0,
-                    N = g.split(" "),
-                    B = 0;
-                for (let x = 0; x < N.length; x++) {
-                    let L = dt.measureText(N[x], r, i, 1);
-                    _ + L.width > s && (u.push({
-                        text: N.slice(B, x).join(" "),
+                    A = g.split(" "),
+                    T = 0;
+                for (let k = 0; k < A.length; k++) {
+                    let x = dt.measureText(A[k], r, i, 1);
+                    _ + x.width > s && (u.push({
+                        text: A.slice(T, k).join(" "),
                         width: _,
                         height: v
-                    }), _ = 0, v = 0, B = x), L.height > v && (v = L.height), _ += L.width;
+                    }), _ = 0, v = 0, T = k), x.height > v && (v = x.height), _ += x.width;
                 }
-                B < N.length && u.push({
-                    text: N.slice(B, N.length).join(" "),
+                T < A.length && u.push({
+                    text: A.slice(T, A.length).join(" "),
                     width: _,
                     height: v
                 });
             } else
                 u.push({
                     text: g,
                     width: m.width,
@@ -8119,27 +8119,27 @@
         }), a.appendChild(h), {
             svg: a,
             width: l,
             height: c
         };
     }
 };
-var Un = Eg;
+var Jn = Mg;
 
-function Lg(d) {
+function Bg(d) {
     function e(g, m) {
         var _ = g.length,
             v = _ === 0 || _ > 0 && _ - 1 in g,
-            N = 0;
+            A = 0;
         if (v)
-            for (; N < _ && m.call(g[N], N, g[N]) !== !1; N++)
+            for (; A < _ && m.call(g[A], A, g[A]) !== !1; A++)
         ;
         else
-            for (N in g)
-                if (m.call(g[N], N, g[N]) === !1)
+            for (A in g)
+                if (m.call(g[A], A, g[A]) === !1)
                     break;
     }
 
     function t(g) {
         var m = parseInt(g).toString(16);
         return m.length == 1 ? "0" + m : m;
     }
@@ -8157,40 +8157,40 @@
 `;
     }
 
     function a(g) {
         var m = "";
         return e(g, function(_, v) {
             if (_ = r.apply(null, _.split(",")), _ !== !1) {
-                var N = [],
-                    B, x = 1;
+                var A = [],
+                    T, k = 1;
                 e(v, function() {
-                    B && this[1] === B[1] && this[0] === B[0] + x ? x++ : (B && (N.push(i(B[0], B[1], x)), x = 1), B = this);
-                }), N.push(i(B[0], B[1], x)), m += s(_, N.join(""));
+                    T && this[1] === T[1] && this[0] === T[0] + k ? k++ : (T && (A.push(i(T[0], T[1], k)), k = 1), T = this);
+                }), A.push(i(T[0], T[1], k)), m += s(_, A.join(""));
             }
         }), m;
     }
     var n = function(g) {
         var m = {},
             _ = g.data,
             v = _.length,
-            N = g.width;
+            A = g.width;
         g.height;
-        for (var B = 0, x = 0, L = 0, k; L < v; L += 4)
-            _[L + 3] > 0 && (k = _[L] + "," + _[L + 1] + "," + _[L + 2] + "," + _[L + 3], m[k] = m[k] || [], B = L / 4 % N, x = Math.floor(L / 4 / N), m[k].push([B, x]));
+        for (var T = 0, k = 0, x = 0, R; x < v; x += 4)
+            _[x + 3] > 0 && (R = _[x] + "," + _[x + 1] + "," + _[x + 2] + "," + _[x + 3], m[R] = m[R] || [], T = x / 4 % A, k = Math.floor(x / 4 / A), m[R].push([T, k]));
         return m;
     };
     let h = n(d),
         l = a(h),
         c = '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 -0.5 ' + d.width + " " + d.height + '" shape-rendering="crispEdges"><g shape-rendering="crispEdges">' + l + "</g></svg>";
     var u = document.createElement("div");
     return u.innerHTML = c, u.firstChild;
 }
-var Mg = Lg,
-    ml = {
+var Dg = Bg,
+    bl = {
         exports: {}
     };
 /**
  * chroma.js - JavaScript library for color conversions
  *
  * Copyright (c) 2011-2019, Gregor Aisch
  * All rights reserved.
@@ -8244,15 +8244,15 @@
  * http://www.w3.org/TR/css3-color/#svg-color
  *
  * @preserve
  */
 (function(d, e) {
     (function(t, r) {
         d.exports = r();
-    })(eg, function() {
+    })(rg, function() {
         for (var t = function(o, f, p) {
                 return f === void 0 && (f = 0), p === void 0 && (p = 1), o < f ? f : o > p ? p : o;
             }, r = t, i = function(o) {
                 o._clipped = !1, o._unclipped = o.slice(0);
                 for (var f = 0; f <= 3; f++)
                     f < 3 ? ((o[f] < 0 || o[f] > 255) && (o._clipped = !0), o[f] = r(o[f], 0, 255)) : f === 3 && (o[f] = r(o[f], 0, 1));
                 return o;
@@ -8287,151 +8287,151 @@
                 last: m,
                 PI: _,
                 TWOPI: _ * 2,
                 PITHIRD: _ / 3,
                 DEG2RAD: _ / 180,
                 RAD2DEG: 180 / _
             },
-            N = {
+            A = {
                 format: {},
                 autodetect: []
             },
-            B = v.last,
-            x = v.clip_rgb,
-            L = v.type,
-            k = N,
-            z = function() {
+            T = v.last,
+            k = v.clip_rgb,
+            x = v.type,
+            R = A,
+            O = function() {
                 for (var f = [], p = arguments.length; p--;)
                     f[p] = arguments[p];
                 var b = this;
-                if (L(f[0]) === "object" && f[0].constructor && f[0].constructor === this.constructor)
+                if (x(f[0]) === "object" && f[0].constructor && f[0].constructor === this.constructor)
                     return f[0];
-                var C = B(f),
-                    A = !1;
+                var C = T(f),
+                    N = !1;
                 if (!C) {
-                    A = !0, k.sorted || (k.autodetect = k.autodetect.sort(function(I, V) {
-                        return V.p - I.p;
-                    }), k.sorted = !0);
-                    for (var S = 0, R = k.autodetect; S < R.length; S += 1) {
-                        var E = R[S];
-                        if (C = E.test.apply(E, f), C)
+                    N = !0, R.sorted || (R.autodetect = R.autodetect.sort(function(I, W) {
+                        return W.p - I.p;
+                    }), R.sorted = !0);
+                    for (var S = 0, E = R.autodetect; S < E.length; S += 1) {
+                        var M = E[S];
+                        if (C = M.test.apply(M, f), C)
                             break;
                     }
                 }
-                if (k.format[C]) {
-                    var P = k.format[C].apply(null, A ? f : f.slice(0, -1));
-                    b._rgb = x(P);
+                if (R.format[C]) {
+                    var P = R.format[C].apply(null, N ? f : f.slice(0, -1));
+                    b._rgb = k(P);
                 } else
                     throw new Error("unknown format: " + f);
                 b._rgb.length === 3 && b._rgb.push(1);
             };
-        z.prototype.toString = function() {
-            return L(this.hex) == "function" ? this.hex() : "[" + this._rgb.join(",") + "]";
+        O.prototype.toString = function() {
+            return x(this.hex) == "function" ? this.hex() : "[" + this._rgb.join(",") + "]";
         };
-        var D = z,
-            Y = function() {
+        var D = O,
+            te = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                return new(Function.prototype.bind.apply(Y.Color, [null].concat(o)))();
+                return new(Function.prototype.bind.apply(te.Color, [null].concat(o)))();
             };
-        Y.Color = D, Y.version = "2.4.2";
-        var O = Y,
-            Z = v.unpack,
+        te.Color = D, te.version = "2.4.2";
+        var q = te,
+            re = v.unpack,
             j = Math.max,
-            q = function() {
+            X = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = Z(o, "rgb"),
+                var p = re(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2];
-                b = b / 255, C = C / 255, A = A / 255;
-                var S = 1 - j(b, j(C, A)),
-                    R = S < 1 ? 1 / (1 - S) : 0,
-                    E = (1 - b - S) * R,
-                    P = (1 - C - S) * R,
-                    I = (1 - A - S) * R;
-                return [E, P, I, S];
+                    N = p[2];
+                b = b / 255, C = C / 255, N = N / 255;
+                var S = 1 - j(b, j(C, N)),
+                    E = S < 1 ? 1 / (1 - S) : 0,
+                    M = (1 - b - S) * E,
+                    P = (1 - C - S) * E,
+                    I = (1 - N - S) * E;
+                return [M, P, I, S];
             },
-            se = q,
+            se = X,
             ye = v.unpack,
             ke = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 o = ye(o, "cmyk");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A = o[3],
+                    N = o[3],
                     S = o.length > 4 ? o[4] : 1;
-                return A === 1 ? [0, 0, 0, S] : [
-                    p >= 1 ? 0 : 255 * (1 - p) * (1 - A),
+                return N === 1 ? [0, 0, 0, S] : [
+                    p >= 1 ? 0 : 255 * (1 - p) * (1 - N),
                     // r
-                    b >= 1 ? 0 : 255 * (1 - b) * (1 - A),
+                    b >= 1 ? 0 : 255 * (1 - b) * (1 - N),
                     // g
-                    C >= 1 ? 0 : 255 * (1 - C) * (1 - A),
+                    C >= 1 ? 0 : 255 * (1 - C) * (1 - N),
                     // b
                     S
                 ];
             },
             xe = ke,
-            we = O,
+            we = q,
             Ee = D,
-            Qe = N,
+            et = A,
             Ce = v.unpack,
             Ae = v.type,
             Be = se;
         Ee.prototype.cmyk = function() {
             return Be(this._rgb);
         }, we.cmyk = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(Ee, [null].concat(o, ["cmyk"])))();
-        }, Qe.format.cmyk = xe, Qe.autodetect.push({
+        }, et.format.cmyk = xe, et.autodetect.push({
             p: 2,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 if (o = Ce(o, "cmyk"), Ae(o) === "array" && o.length === 4)
                     return "cmyk";
             }
         });
-        var st = v.unpack,
+        var at = v.unpack,
             It = v.last,
             wt = function(o) {
                 return Math.round(o * 100) / 100;
             },
-            K = function() {
+            U = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = st(o, "hsla"),
+                var p = at(o, "hsla"),
                     b = It(o) || "lsa";
                 return p[0] = wt(p[0] || 0), p[1] = wt(p[1] * 100) + "%", p[2] = wt(p[2] * 100) + "%", b === "hsla" || p.length > 3 && p[3] < 1 ? (p[3] = p.length > 3 ? p[3] : 1, b = "hsla") : p.length = 3, b + "(" + p.join(",") + ")";
             },
-            Ot = K,
-            J = v.unpack,
+            Ot = U,
+            Z = v.unpack,
             Te = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                o = J(o, "rgba");
+                o = Z(o, "rgba");
                 var p = o[0],
                     b = o[1],
                     C = o[2];
                 p /= 255, b /= 255, C /= 255;
-                var A = Math.min(p, b, C),
+                var N = Math.min(p, b, C),
                     S = Math.max(p, b, C),
-                    R = (S + A) / 2,
-                    E, P;
-                return S === A ? (E = 0, P = Number.NaN) : E = R < 0.5 ? (S - A) / (S + A) : (S - A) / (2 - S - A), p == S ? P = (b - C) / (S - A) : b == S ? P = 2 + (C - p) / (S - A) : C == S && (P = 4 + (p - b) / (S - A)), P *= 60, P < 0 && (P += 360), o.length > 3 && o[3] !== void 0 ? [P, E, R, o[3]] : [P, E, R];
+                    E = (S + N) / 2,
+                    M, P;
+                return S === N ? (M = 0, P = Number.NaN) : M = E < 0.5 ? (S - N) / (S + N) : (S - N) / (2 - S - N), p == S ? P = (b - C) / (S - N) : b == S ? P = 2 + (C - p) / (S - N) : C == S && (P = 4 + (p - b) / (S - N)), P *= 60, P < 0 && (P += 360), o.length > 3 && o[3] !== void 0 ? [P, M, E, o[3]] : [P, M, E];
             },
-            et = Te,
+            tt = Te,
             Ie = v.unpack,
             Ye = v.last,
             Ue = Ot,
-            Ge = et,
+            Ge = tt,
             De = Math.round,
             Ze = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 var p = Ie(o, "rgba"),
                     b = Ye(o) || "rgb";
                 return b.substr(0, 3) == "hsl" ? Ue(Ge(p), b) : (p[0] = De(p[0]), p[1] = De(p[1]), p[2] = De(p[2]), (b === "rgba" || p.length > 3 && p[3] < 1) && (p[3] = p.length > 3 ? p[3] : 1, b = "rgba"), b + "(" + p.slice(0, b === "rgb" ? 3 : 4).join(",") + ")");
@@ -8441,34 +8441,34 @@
             Le = Math.round,
             qe = function() {
                 for (var o, f = [], p = arguments.length; p--;)
                     f[p] = arguments[p];
                 f = We(f, "hsl");
                 var b = f[0],
                     C = f[1],
-                    A = f[2],
-                    S, R, E;
+                    N = f[2],
+                    S, E, M;
                 if (C === 0)
-                    S = R = E = A * 255;
+                    S = E = M = N * 255;
                 else {
                     var P = [0, 0, 0],
                         I = [0, 0, 0],
-                        V = A < 0.5 ? A * (1 + C) : A + C - A * C,
-                        F = 2 * A - V,
-                        U = b / 360;
-                    P[0] = U + 1 / 3, P[1] = U, P[2] = U - 1 / 3;
-                    for (var G = 0; G < 3; G++)
-                        P[G] < 0 && (P[G] += 1), P[G] > 1 && (P[G] -= 1), 6 * P[G] < 1 ? I[G] = F + (V - F) * 6 * P[G] : 2 * P[G] < 1 ? I[G] = V : 3 * P[G] < 2 ? I[G] = F + (V - F) * (2 / 3 - P[G]) * 6 : I[G] = F;
-                    o = [Le(I[0] * 255), Le(I[1] * 255), Le(I[2] * 255)], S = o[0], R = o[1], E = o[2];
-                }
-                return f.length > 3 ? [S, R, E, f[3]] : [S, R, E, 1];
-            },
-            Lt = qe,
-            yt = Lt,
-            Vt = N,
+                        W = N < 0.5 ? N * (1 + C) : N + C - N * C,
+                        F = 2 * N - W,
+                        G = b / 360;
+                    P[0] = G + 1 / 3, P[1] = G, P[2] = G - 1 / 3;
+                    for (var Y = 0; Y < 3; Y++)
+                        P[Y] < 0 && (P[Y] += 1), P[Y] > 1 && (P[Y] -= 1), 6 * P[Y] < 1 ? I[Y] = F + (W - F) * 6 * P[Y] : 2 * P[Y] < 1 ? I[Y] = W : 3 * P[Y] < 2 ? I[Y] = F + (W - F) * (2 / 3 - P[Y]) * 6 : I[Y] = F;
+                    o = [Le(I[0] * 255), Le(I[1] * 255), Le(I[2] * 255)], S = o[0], E = o[1], M = o[2];
+                }
+                return f.length > 3 ? [S, E, M, f[3]] : [S, E, M, 1];
+            },
+            Mt = qe,
+            yt = Mt,
+            Vt = A,
             Xt = /^rgb\(\s*(-?\d+),\s*(-?\d+)\s*,\s*(-?\d+)\s*\)$/,
             Yt = /^rgba\(\s*(-?\d+),\s*(-?\d+)\s*,\s*(-?\d+)\s*,\s*([01]|[01]?\.\d+)\)$/,
             Ft = /^rgb\(\s*(-?\d+(?:\.\d+)?)%,\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*\)$/,
             _t = /^rgba\(\s*(-?\d+(?:\.\d+)?)%,\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*,\s*([01]|[01]?\.\d+)\)$/,
             zt = /^hsl\(\s*(-?\d+(?:\.\d+)?),\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*\)$/,
             Gt = /^hsla\(\s*(-?\d+(?:\.\d+)?),\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*,\s*([01]|[01]?\.\d+)\)$/,
             Ut = Math.round,
@@ -8481,74 +8481,74 @@
                     } catch {}
                 if (f = o.match(Xt)) {
                     for (var p = f.slice(1, 4), b = 0; b < 3; b++)
                         p[b] = +p[b];
                     return p[3] = 1, p;
                 }
                 if (f = o.match(Yt)) {
-                    for (var C = f.slice(1, 5), A = 0; A < 4; A++)
-                        C[A] = +C[A];
+                    for (var C = f.slice(1, 5), N = 0; N < 4; N++)
+                        C[N] = +C[N];
                     return C;
                 }
                 if (f = o.match(Ft)) {
-                    for (var S = f.slice(1, 4), R = 0; R < 3; R++)
-                        S[R] = Ut(S[R] * 2.55);
+                    for (var S = f.slice(1, 4), E = 0; E < 3; E++)
+                        S[E] = Ut(S[E] * 2.55);
                     return S[3] = 1, S;
                 }
                 if (f = o.match(_t)) {
-                    for (var E = f.slice(1, 5), P = 0; P < 3; P++)
-                        E[P] = Ut(E[P] * 2.55);
-                    return E[3] = +E[3], E;
+                    for (var M = f.slice(1, 5), P = 0; P < 3; P++)
+                        M[P] = Ut(M[P] * 2.55);
+                    return M[3] = +M[3], M;
                 }
                 if (f = o.match(zt)) {
                     var I = f.slice(1, 4);
                     I[1] *= 0.01, I[2] *= 0.01;
-                    var V = yt(I);
-                    return V[3] = 1, V;
+                    var W = yt(I);
+                    return W[3] = 1, W;
                 }
                 if (f = o.match(Gt)) {
                     var F = f.slice(1, 4);
                     F[1] *= 0.01, F[2] *= 0.01;
-                    var U = yt(F);
-                    return U[3] = +f[4], U;
+                    var G = yt(F);
+                    return G[3] = +f[4], G;
                 }
             };
         Zt.test = function(o) {
             return Xt.test(o) || Yt.test(o) || Ft.test(o) || _t.test(o) || zt.test(o) || Gt.test(o);
         };
-        var Bi = Zt,
-            Di = O,
+        var Pi = Zt,
+            $i = q,
             Fr = D,
-            Jr = N,
+            Jr = A,
             Qr = v.type,
-            Pi = He,
-            ei = Bi;
+            Ii = He,
+            ei = Pi;
         Fr.prototype.css = function(o) {
-            return Pi(this._rgb, o);
-        }, Di.css = function() {
+            return Ii(this._rgb, o);
+        }, $i.css = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(Fr, [null].concat(o, ["css"])))();
         }, Jr.format.css = ei, Jr.autodetect.push({
             p: 5,
             test: function(o) {
                 for (var f = [], p = arguments.length - 1; p-- > 0;)
                     f[p] = arguments[p + 1];
                 if (!f.length && Qr(o) === "string" && ei.test(o))
                     return "css";
             }
         });
         var ti = D,
-            ri = O,
-            ii = N,
-            $i = v.unpack;
+            ri = q,
+            ii = A,
+            Oi = v.unpack;
         ii.format.gl = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            var p = $i(o, "rgba");
+            var p = Oi(o, "rgba");
             return p[0] *= 255, p[1] *= 255, p[2] *= 255, p;
         }, ri.gl = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(ti, [null].concat(o, ["gl"])))();
         }, ti.prototype.gl = function() {
             var o = this._rgb;
@@ -8557,316 +8557,316 @@
         var ni = v.unpack,
             si = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 var p = ni(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
-                    S = Math.min(b, C, A),
-                    R = Math.max(b, C, A),
-                    E = R - S,
-                    P = E * 100 / 255,
-                    I = S / (255 - E) * 100,
-                    V;
-                return E === 0 ? V = Number.NaN : (b === R && (V = (C - A) / E), C === R && (V = 2 + (A - b) / E), A === R && (V = 4 + (b - C) / E), V *= 60, V < 0 && (V += 360)), [V, P, I];
-            },
-            Ii = si,
-            Oi = v.unpack,
-            Fi = Math.floor,
-            zi = function() {
-                for (var o, f, p, b, C, A, S = [], R = arguments.length; R--;)
-                    S[R] = arguments[R];
-                S = Oi(S, "hcg");
-                var E = S[0],
+                    N = p[2],
+                    S = Math.min(b, C, N),
+                    E = Math.max(b, C, N),
+                    M = E - S,
+                    P = M * 100 / 255,
+                    I = S / (255 - M) * 100,
+                    W;
+                return M === 0 ? W = Number.NaN : (b === E && (W = (C - N) / M), C === E && (W = 2 + (N - b) / M), N === E && (W = 4 + (b - C) / M), W *= 60, W < 0 && (W += 360)), [W, P, I];
+            },
+            Fi = si,
+            zi = v.unpack,
+            Hi = Math.floor,
+            Wi = function() {
+                for (var o, f, p, b, C, N, S = [], E = arguments.length; E--;)
+                    S[E] = arguments[E];
+                S = zi(S, "hcg");
+                var M = S[0],
                     P = S[1],
                     I = S[2],
-                    V, F, U;
+                    W, F, G;
                 I = I * 255;
-                var G = P * 255;
+                var Y = P * 255;
                 if (P === 0)
-                    V = F = U = I;
+                    W = F = G = I;
                 else {
-                    E === 360 && (E = 0), E > 360 && (E -= 360), E < 0 && (E += 360), E /= 60;
-                    var ae = Fi(E),
-                        he = E - ae,
+                    M === 360 && (M = 0), M > 360 && (M -= 360), M < 0 && (M += 360), M /= 60;
+                    var ae = Hi(M),
+                        he = M - ae,
                         ue = I * (1 - P),
-                        de = ue + G * (1 - he),
-                        Ve = ue + G * he,
-                        ze = ue + G;
+                        de = ue + Y * (1 - he),
+                        Ve = ue + Y * he,
+                        ze = ue + Y;
                     switch (ae) {
                         case 0:
-                            o = [ze, Ve, ue], V = o[0], F = o[1], U = o[2];
+                            o = [ze, Ve, ue], W = o[0], F = o[1], G = o[2];
                             break;
                         case 1:
-                            f = [de, ze, ue], V = f[0], F = f[1], U = f[2];
+                            f = [de, ze, ue], W = f[0], F = f[1], G = f[2];
                             break;
                         case 2:
-                            p = [ue, ze, Ve], V = p[0], F = p[1], U = p[2];
+                            p = [ue, ze, Ve], W = p[0], F = p[1], G = p[2];
                             break;
                         case 3:
-                            b = [ue, de, ze], V = b[0], F = b[1], U = b[2];
+                            b = [ue, de, ze], W = b[0], F = b[1], G = b[2];
                             break;
                         case 4:
-                            C = [Ve, ue, ze], V = C[0], F = C[1], U = C[2];
+                            C = [Ve, ue, ze], W = C[0], F = C[1], G = C[2];
                             break;
                         case 5:
-                            A = [ze, ue, de], V = A[0], F = A[1], U = A[2];
+                            N = [ze, ue, de], W = N[0], F = N[1], G = N[2];
                             break;
                     }
                 }
-                return [V, F, U, S.length > 3 ? S[3] : 1];
+                return [W, F, G, S.length > 3 ? S[3] : 1];
             },
-            Hi = zi,
-            Wi = v.unpack,
-            qi = v.type,
-            Vi = O,
+            qi = Wi,
+            Vi = v.unpack,
+            Xi = v.type,
+            Yi = q,
             ai = D,
-            li = N,
-            y = Ii;
+            li = A,
+            y = Fi;
         ai.prototype.hcg = function() {
             return y(this._rgb);
-        }, Vi.hcg = function() {
+        }, Yi.hcg = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(ai, [null].concat(o, ["hcg"])))();
-        }, li.format.hcg = Hi, li.autodetect.push({
+        }, li.format.hcg = qi, li.autodetect.push({
             p: 1,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = Wi(o, "hcg"), qi(o) === "array" && o.length === 3)
+                if (o = Vi(o, "hcg"), Xi(o) === "array" && o.length === 3)
                     return "hcg";
             }
         });
         var vr = v.unpack,
-            ht = v.last,
+            ft = v.last,
             Kt = Math.round,
             mr = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 var p = vr(o, "rgba"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
+                    N = p[2],
                     S = p[3],
-                    R = ht(o) || "auto";
-                S === void 0 && (S = 1), R === "auto" && (R = S < 1 ? "rgba" : "rgb"), b = Kt(b), C = Kt(C), A = Kt(A);
-                var E = b << 16 | C << 8 | A,
-                    P = "000000" + E.toString(16);
+                    E = ft(o) || "auto";
+                S === void 0 && (S = 1), E === "auto" && (E = S < 1 ? "rgba" : "rgb"), b = Kt(b), C = Kt(C), N = Kt(N);
+                var M = b << 16 | C << 8 | N,
+                    P = "000000" + M.toString(16);
                 P = P.substr(P.length - 6);
                 var I = "0" + Kt(S * 255).toString(16);
-                switch (I = I.substr(I.length - 2), R.toLowerCase()) {
+                switch (I = I.substr(I.length - 2), E.toLowerCase()) {
                     case "rgba":
                         return "#" + P + I;
                     case "argb":
                         return "#" + I + P;
                     default:
                         return "#" + P;
                 }
             },
             Ne = mr,
-            ft = /^#?([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$/,
-            Xi = /^#?([A-Fa-f0-9]{8}|[A-Fa-f0-9]{4})$/,
+            ut = /^#?([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$/,
+            Gi = /^#?([A-Fa-f0-9]{8}|[A-Fa-f0-9]{4})$/,
             oi = function(o) {
-                if (o.match(ft)) {
+                if (o.match(ut)) {
                     (o.length === 4 || o.length === 7) && (o = o.substr(1)), o.length === 3 && (o = o.split(""), o = o[0] + o[0] + o[1] + o[1] + o[2] + o[2]);
                     var f = parseInt(o, 16),
                         p = f >> 16,
                         b = f >> 8 & 255,
                         C = f & 255;
                     return [p, b, C, 1];
                 }
-                if (o.match(Xi)) {
+                if (o.match(Gi)) {
                     (o.length === 5 || o.length === 9) && (o = o.substr(1)), o.length === 4 && (o = o.split(""), o = o[0] + o[0] + o[1] + o[1] + o[2] + o[2] + o[3] + o[3]);
-                    var A = parseInt(o, 16),
-                        S = A >> 24 & 255,
-                        R = A >> 16 & 255,
-                        E = A >> 8 & 255,
-                        P = Math.round((A & 255) / 255 * 100) / 100;
-                    return [S, R, E, P];
+                    var N = parseInt(o, 16),
+                        S = N >> 24 & 255,
+                        E = N >> 16 & 255,
+                        M = N >> 8 & 255,
+                        P = Math.round((N & 255) / 255 * 100) / 100;
+                    return [S, E, M, P];
                 }
                 throw new Error("unknown hex color: " + o);
             },
             zr = oi,
-            Q = O,
+            K = q,
             Hr = D,
-            Yi = v.type,
-            lr = N,
+            Ui = v.type,
+            lr = A,
             jt = Ne;
         Hr.prototype.hex = function(o) {
             return jt(this._rgb, o);
-        }, Q.hex = function() {
+        }, K.hex = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(Hr, [null].concat(o, ["hex"])))();
         }, lr.format.hex = zr, lr.autodetect.push({
             p: 4,
             test: function(o) {
                 for (var f = [], p = arguments.length - 1; p-- > 0;)
                     f[p] = arguments[p + 1];
-                if (!f.length && Yi(o) === "string" && [3, 4, 5, 6, 7, 8, 9].indexOf(o.length) >= 0)
+                if (!f.length && Ui(o) === "string" && [3, 4, 5, 6, 7, 8, 9].indexOf(o.length) >= 0)
                     return "hex";
             }
         });
-        var Gi = v.unpack,
+        var Zi = v.unpack,
             or = v.TWOPI,
-            Ui = Math.min,
-            Zi = Math.sqrt,
+            Ki = Math.min,
+            ji = Math.sqrt,
             hi = Math.acos,
             fi = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = Gi(o, "rgb"),
+                var p = Zi(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2];
-                b /= 255, C /= 255, A /= 255;
-                var S, R = Ui(b, C, A),
-                    E = (b + C + A) / 3,
-                    P = E > 0 ? 1 - R / E : 0;
-                return P === 0 ? S = NaN : (S = (b - C + (b - A)) / 2, S /= Zi((b - C) * (b - C) + (b - A) * (C - A)), S = hi(S), A > C && (S = or - S), S /= or), [S * 360, P, E];
+                    N = p[2];
+                b /= 255, C /= 255, N /= 255;
+                var S, E = Ki(b, C, N),
+                    M = (b + C + N) / 3,
+                    P = M > 0 ? 1 - E / M : 0;
+                return P === 0 ? S = NaN : (S = (b - C + (b - N)) / 2, S /= ji((b - C) * (b - C) + (b - N) * (C - N)), S = hi(S), N > C && (S = or - S), S /= or), [S * 360, P, M];
             },
-            Ki = fi,
+            Ji = fi,
             ui = v.unpack,
             Wr = v.limit,
             Jt = v.TWOPI,
             qr = v.PITHIRD,
             Qt = Math.cos,
-            ji = function() {
+            Qi = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 o = ui(o, "hsi");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A, S, R;
-                return isNaN(p) && (p = 0), isNaN(b) && (b = 0), p > 360 && (p -= 360), p < 0 && (p += 360), p /= 360, p < 1 / 3 ? (R = (1 - b) / 3, A = (1 + b * Qt(Jt * p) / Qt(qr - Jt * p)) / 3, S = 1 - (R + A)) : p < 2 / 3 ? (p -= 1 / 3, A = (1 - b) / 3, S = (1 + b * Qt(Jt * p) / Qt(qr - Jt * p)) / 3, R = 1 - (A + S)) : (p -= 2 / 3, S = (1 - b) / 3, R = (1 + b * Qt(Jt * p) / Qt(qr - Jt * p)) / 3, A = 1 - (S + R)), A = Wr(C * A * 3), S = Wr(C * S * 3), R = Wr(C * R * 3), [A * 255, S * 255, R * 255, o.length > 3 ? o[3] : 1];
+                    N, S, E;
+                return isNaN(p) && (p = 0), isNaN(b) && (b = 0), p > 360 && (p -= 360), p < 0 && (p += 360), p /= 360, p < 1 / 3 ? (E = (1 - b) / 3, N = (1 + b * Qt(Jt * p) / Qt(qr - Jt * p)) / 3, S = 1 - (E + N)) : p < 2 / 3 ? (p -= 1 / 3, N = (1 - b) / 3, S = (1 + b * Qt(Jt * p) / Qt(qr - Jt * p)) / 3, E = 1 - (N + S)) : (p -= 2 / 3, S = (1 - b) / 3, E = (1 + b * Qt(Jt * p) / Qt(qr - Jt * p)) / 3, N = 1 - (S + E)), N = Wr(C * N * 3), S = Wr(C * S * 3), E = Wr(C * E * 3), [N * 255, S * 255, E * 255, o.length > 3 ? o[3] : 1];
             },
-            Ji = ji,
-            Qi = v.unpack,
-            M = v.type,
-            w = O,
+            en = Qi,
+            tn = v.unpack,
+            B = v.type,
+            w = q,
             $ = D,
-            T = N,
-            H = Ki;
+            L = A,
+            z = Ji;
         $.prototype.hsi = function() {
-            return H(this._rgb);
+            return z(this._rgb);
         }, w.hsi = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply($, [null].concat(o, ["hsi"])))();
-        }, T.format.hsi = Ji, T.autodetect.push({
+        }, L.format.hsi = en, L.autodetect.push({
             p: 2,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = Qi(o, "hsi"), M(o) === "array" && o.length === 3)
+                if (o = tn(o, "hsi"), B(o) === "array" && o.length === 3)
                     return "hsi";
             }
         });
-        var X = v.unpack,
-            ee = v.type,
-            Oe = O,
-            at = D,
-            ut = N,
-            Rl = et;
-        at.prototype.hsl = function() {
-            return Rl(this._rgb);
+        var V = v.unpack,
+            J = v.type,
+            Oe = q,
+            lt = D,
+            ct = A,
+            Tl = tt;
+        lt.prototype.hsl = function() {
+            return Tl(this._rgb);
         }, Oe.hsl = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(at, [null].concat(o, ["hsl"])))();
-        }, ut.format.hsl = Lt, ut.autodetect.push({
+            return new(Function.prototype.bind.apply(lt, [null].concat(o, ["hsl"])))();
+        }, ct.format.hsl = Mt, ct.autodetect.push({
             p: 2,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = X(o, "hsl"), ee(o) === "array" && o.length === 3)
+                if (o = V(o, "hsl"), J(o) === "array" && o.length === 3)
                     return "hsl";
             }
         });
-        var xl = v.unpack,
-            Tl = Math.min,
-            El = Math.max,
-            Ll = function() {
+        var El = v.unpack,
+            Ll = Math.min,
+            Ml = Math.max,
+            Bl = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                o = xl(o, "rgb");
+                o = El(o, "rgb");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A = Tl(p, b, C),
-                    S = El(p, b, C),
-                    R = S - A,
-                    E, P, I;
-                return I = S / 255, S === 0 ? (E = Number.NaN, P = 0) : (P = R / S, p === S && (E = (b - C) / R), b === S && (E = 2 + (C - p) / R), C === S && (E = 4 + (p - b) / R), E *= 60, E < 0 && (E += 360)), [E, P, I];
-            },
-            Ml = Ll,
-            Bl = v.unpack,
-            Dl = Math.floor,
-            Pl = function() {
-                for (var o, f, p, b, C, A, S = [], R = arguments.length; R--;)
-                    S[R] = arguments[R];
-                S = Bl(S, "hsv");
-                var E = S[0],
+                    N = Ll(p, b, C),
+                    S = Ml(p, b, C),
+                    E = S - N,
+                    M, P, I;
+                return I = S / 255, S === 0 ? (M = Number.NaN, P = 0) : (P = E / S, p === S && (M = (b - C) / E), b === S && (M = 2 + (C - p) / E), C === S && (M = 4 + (p - b) / E), M *= 60, M < 0 && (M += 360)), [M, P, I];
+            },
+            Dl = Bl,
+            Pl = v.unpack,
+            $l = Math.floor,
+            Il = function() {
+                for (var o, f, p, b, C, N, S = [], E = arguments.length; E--;)
+                    S[E] = arguments[E];
+                S = Pl(S, "hsv");
+                var M = S[0],
                     P = S[1],
                     I = S[2],
-                    V, F, U;
+                    W, F, G;
                 if (I *= 255, P === 0)
-                    V = F = U = I;
+                    W = F = G = I;
                 else {
-                    E === 360 && (E = 0), E > 360 && (E -= 360), E < 0 && (E += 360), E /= 60;
-                    var G = Dl(E),
-                        ae = E - G,
+                    M === 360 && (M = 0), M > 360 && (M -= 360), M < 0 && (M += 360), M /= 60;
+                    var Y = $l(M),
+                        ae = M - Y,
                         he = I * (1 - P),
                         ue = I * (1 - P * ae),
                         de = I * (1 - P * (1 - ae));
-                    switch (G) {
+                    switch (Y) {
                         case 0:
-                            o = [I, de, he], V = o[0], F = o[1], U = o[2];
+                            o = [I, de, he], W = o[0], F = o[1], G = o[2];
                             break;
                         case 1:
-                            f = [ue, I, he], V = f[0], F = f[1], U = f[2];
+                            f = [ue, I, he], W = f[0], F = f[1], G = f[2];
                             break;
                         case 2:
-                            p = [he, I, de], V = p[0], F = p[1], U = p[2];
+                            p = [he, I, de], W = p[0], F = p[1], G = p[2];
                             break;
                         case 3:
-                            b = [he, ue, I], V = b[0], F = b[1], U = b[2];
+                            b = [he, ue, I], W = b[0], F = b[1], G = b[2];
                             break;
                         case 4:
-                            C = [de, he, I], V = C[0], F = C[1], U = C[2];
+                            C = [de, he, I], W = C[0], F = C[1], G = C[2];
                             break;
                         case 5:
-                            A = [I, he, ue], V = A[0], F = A[1], U = A[2];
+                            N = [I, he, ue], W = N[0], F = N[1], G = N[2];
                             break;
                     }
                 }
-                return [V, F, U, S.length > 3 ? S[3] : 1];
+                return [W, F, G, S.length > 3 ? S[3] : 1];
             },
-            $l = Pl,
-            Il = v.unpack,
-            Ol = v.type,
-            Fl = O,
-            es = D,
-            ts = N,
-            zl = Ml;
-        es.prototype.hsv = function() {
-            return zl(this._rgb);
-        }, Fl.hsv = function() {
+            Ol = Il,
+            Fl = v.unpack,
+            zl = v.type,
+            Hl = q,
+            rs = D,
+            is = A,
+            Wl = Dl;
+        rs.prototype.hsv = function() {
+            return Wl(this._rgb);
+        }, Hl.hsv = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(es, [null].concat(o, ["hsv"])))();
-        }, ts.format.hsv = $l, ts.autodetect.push({
+            return new(Function.prototype.bind.apply(rs, [null].concat(o, ["hsv"])))();
+        }, is.format.hsv = Ol, is.autodetect.push({
             p: 2,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = Il(o, "hsv"), Ol(o) === "array" && o.length === 3)
+                if (o = Fl(o, "hsv"), zl(o) === "array" && o.length === 3)
                     return "hsv";
             }
         });
         var ci = {
                 // Corresponds roughly to RGB brighter/darker
                 Kn: 18,
                 // D65 standard referent
@@ -8879,193 +8879,193 @@
                 // 6 / 29
                 t2: 0.12841855,
                 // 3 * t1 * t1
                 t3: 8856452e-9
                 // t1 * t1 * t1
             },
             br = ci,
-            Hl = v.unpack,
-            rs = Math.pow,
-            Wl = function() {
+            ql = v.unpack,
+            ns = Math.pow,
+            Vl = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = Hl(o, "rgb"),
+                var p = ql(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
-                    S = ql(b, C, A),
-                    R = S[0],
-                    E = S[1],
+                    N = p[2],
+                    S = Xl(b, C, N),
+                    E = S[0],
+                    M = S[1],
                     P = S[2],
-                    I = 116 * E - 16;
-                return [I < 0 ? 0 : I, 500 * (R - E), 200 * (E - P)];
+                    I = 116 * M - 16;
+                return [I < 0 ? 0 : I, 500 * (E - M), 200 * (M - P)];
             },
-            en = function(o) {
-                return (o /= 255) <= 0.04045 ? o / 12.92 : rs((o + 0.055) / 1.055, 2.4);
+            rn = function(o) {
+                return (o /= 255) <= 0.04045 ? o / 12.92 : ns((o + 0.055) / 1.055, 2.4);
             },
-            tn = function(o) {
-                return o > br.t3 ? rs(o, 1 / 3) : o / br.t2 + br.t0;
+            nn = function(o) {
+                return o > br.t3 ? ns(o, 1 / 3) : o / br.t2 + br.t0;
             },
-            ql = function(o, f, p) {
-                o = en(o), f = en(f), p = en(p);
-                var b = tn((0.4124564 * o + 0.3575761 * f + 0.1804375 * p) / br.Xn),
-                    C = tn((0.2126729 * o + 0.7151522 * f + 0.072175 * p) / br.Yn),
-                    A = tn((0.0193339 * o + 0.119192 * f + 0.9503041 * p) / br.Zn);
-                return [b, C, A];
+            Xl = function(o, f, p) {
+                o = rn(o), f = rn(f), p = rn(p);
+                var b = nn((0.4124564 * o + 0.3575761 * f + 0.1804375 * p) / br.Xn),
+                    C = nn((0.2126729 * o + 0.7151522 * f + 0.072175 * p) / br.Yn),
+                    N = nn((0.0193339 * o + 0.119192 * f + 0.9503041 * p) / br.Zn);
+                return [b, C, N];
             },
-            is = Wl,
+            ss = Vl,
             wr = ci,
-            Vl = v.unpack,
-            Xl = Math.pow,
-            Yl = function() {
+            Yl = v.unpack,
+            Gl = Math.pow,
+            Ul = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                o = Vl(o, "lab");
+                o = Yl(o, "lab");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A, S, R, E, P, I;
-                return S = (p + 16) / 116, A = isNaN(b) ? S : S + b / 500, R = isNaN(C) ? S : S - C / 200, S = wr.Yn * nn(S), A = wr.Xn * nn(A), R = wr.Zn * nn(R), E = rn(3.2404542 * A - 1.5371385 * S - 0.4985314 * R), P = rn(-0.969266 * A + 1.8760108 * S + 0.041556 * R), I = rn(0.0556434 * A - 0.2040259 * S + 1.0572252 * R), [E, P, I, o.length > 3 ? o[3] : 1];
+                    N, S, E, M, P, I;
+                return S = (p + 16) / 116, N = isNaN(b) ? S : S + b / 500, E = isNaN(C) ? S : S - C / 200, S = wr.Yn * an(S), N = wr.Xn * an(N), E = wr.Zn * an(E), M = sn(3.2404542 * N - 1.5371385 * S - 0.4985314 * E), P = sn(-0.969266 * N + 1.8760108 * S + 0.041556 * E), I = sn(0.0556434 * N - 0.2040259 * S + 1.0572252 * E), [M, P, I, o.length > 3 ? o[3] : 1];
             },
-            rn = function(o) {
-                return 255 * (o <= 304e-5 ? 12.92 * o : 1.055 * Xl(o, 1 / 2.4) - 0.055);
+            sn = function(o) {
+                return 255 * (o <= 304e-5 ? 12.92 * o : 1.055 * Gl(o, 1 / 2.4) - 0.055);
             },
-            nn = function(o) {
+            an = function(o) {
                 return o > wr.t1 ? o * o * o : wr.t2 * (o - wr.t0);
             },
-            ns = Yl,
-            Gl = v.unpack,
-            Ul = v.type,
-            Zl = O,
-            ss = D,
-            as = N,
-            Kl = is;
-        ss.prototype.lab = function() {
-            return Kl(this._rgb);
-        }, Zl.lab = function() {
+            as = Ul,
+            Zl = v.unpack,
+            Kl = v.type,
+            jl = q,
+            ls = D,
+            os = A,
+            Jl = ss;
+        ls.prototype.lab = function() {
+            return Jl(this._rgb);
+        }, jl.lab = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(ss, [null].concat(o, ["lab"])))();
-        }, as.format.lab = ns, as.autodetect.push({
+            return new(Function.prototype.bind.apply(ls, [null].concat(o, ["lab"])))();
+        }, os.format.lab = as, os.autodetect.push({
             p: 2,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = Gl(o, "lab"), Ul(o) === "array" && o.length === 3)
+                if (o = Zl(o, "lab"), Kl(o) === "array" && o.length === 3)
                     return "lab";
             }
         });
-        var jl = v.unpack,
-            Jl = v.RAD2DEG,
-            Ql = Math.sqrt,
-            eo = Math.atan2,
-            to = Math.round,
-            ro = function() {
+        var Ql = v.unpack,
+            eo = v.RAD2DEG,
+            to = Math.sqrt,
+            ro = Math.atan2,
+            io = Math.round,
+            no = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = jl(o, "lab"),
+                var p = Ql(o, "lab"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
-                    S = Ql(C * C + A * A),
-                    R = (eo(A, C) * Jl + 360) % 360;
-                return to(S * 1e4) === 0 && (R = Number.NaN), [b, S, R];
-            },
-            ls = ro,
-            io = v.unpack,
-            no = is,
-            so = ls,
-            ao = function() {
+                    N = p[2],
+                    S = to(C * C + N * N),
+                    E = (ro(N, C) * eo + 360) % 360;
+                return io(S * 1e4) === 0 && (E = Number.NaN), [b, S, E];
+            },
+            hs = no,
+            so = v.unpack,
+            ao = ss,
+            lo = hs,
+            oo = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = io(o, "rgb"),
+                var p = so(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
-                    S = no(b, C, A),
-                    R = S[0],
-                    E = S[1],
+                    N = p[2],
+                    S = ao(b, C, N),
+                    E = S[0],
+                    M = S[1],
                     P = S[2];
-                return so(R, E, P);
+                return lo(E, M, P);
             },
-            lo = ao,
-            oo = v.unpack,
-            ho = v.DEG2RAD,
-            fo = Math.sin,
-            uo = Math.cos,
-            co = function() {
+            ho = oo,
+            fo = v.unpack,
+            uo = v.DEG2RAD,
+            co = Math.sin,
+            go = Math.cos,
+            po = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = oo(o, "lch"),
+                var p = fo(o, "lch"),
                     b = p[0],
                     C = p[1],
-                    A = p[2];
-                return isNaN(A) && (A = 0), A = A * ho, [b, uo(A) * C, fo(A) * C];
+                    N = p[2];
+                return isNaN(N) && (N = 0), N = N * uo, [b, go(N) * C, co(N) * C];
             },
-            os = co,
-            go = v.unpack,
-            po = os,
-            vo = ns,
-            mo = function() {
+            fs = po,
+            vo = v.unpack,
+            mo = fs,
+            bo = as,
+            wo = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                o = go(o, "lch");
+                o = vo(o, "lch");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A = po(p, b, C),
-                    S = A[0],
-                    R = A[1],
-                    E = A[2],
-                    P = vo(S, R, E),
+                    N = mo(p, b, C),
+                    S = N[0],
+                    E = N[1],
+                    M = N[2],
+                    P = bo(S, E, M),
                     I = P[0],
-                    V = P[1],
+                    W = P[1],
                     F = P[2];
-                return [I, V, F, o.length > 3 ? o[3] : 1];
+                return [I, W, F, o.length > 3 ? o[3] : 1];
             },
-            hs = mo,
-            bo = v.unpack,
-            wo = hs,
-            yo = function() {
+            us = wo,
+            yo = v.unpack,
+            _o = us,
+            So = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = bo(o, "hcl").reverse();
-                return wo.apply(void 0, p);
+                var p = yo(o, "hcl").reverse();
+                return _o.apply(void 0, p);
             },
-            _o = yo,
-            So = v.unpack,
-            Co = v.type,
-            fs = O,
+            Co = So,
+            Ao = v.unpack,
+            No = v.type,
+            cs = q,
             gi = D,
-            sn = N,
-            us = lo;
+            ln = A,
+            gs = ho;
         gi.prototype.lch = function() {
-            return us(this._rgb);
+            return gs(this._rgb);
         }, gi.prototype.hcl = function() {
-            return us(this._rgb).reverse();
-        }, fs.lch = function() {
+            return gs(this._rgb).reverse();
+        }, cs.lch = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(gi, [null].concat(o, ["lch"])))();
-        }, fs.hcl = function() {
+        }, cs.hcl = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(gi, [null].concat(o, ["hcl"])))();
-        }, sn.format.lch = hs, sn.format.hcl = _o, ["lch", "hcl"].forEach(function(o) {
-            return sn.autodetect.push({
+        }, ln.format.lch = us, ln.format.hcl = Co, ["lch", "hcl"].forEach(function(o) {
+            return ln.autodetect.push({
                 p: 2,
                 test: function() {
                     for (var f = [], p = arguments.length; p--;)
                         f[p] = arguments[p];
-                    if (f = So(f, o), Co(f) === "array" && f.length === 3)
+                    if (f = Ao(f, o), No(f) === "array" && f.length === 3)
                         return o;
                 }
             });
         });
-        var Ao = {
+        var ko = {
                 aliceblue: "#f0f8ff",
                 antiquewhite: "#faebd7",
                 aqua: "#00ffff",
                 aquamarine: "#7fffd4",
                 azure: "#f0ffff",
                 beige: "#f5f5dc",
                 bisque: "#ffe4c4",
@@ -9214,1098 +9214,1098 @@
                 violet: "#ee82ee",
                 wheat: "#f5deb3",
                 white: "#ffffff",
                 whitesmoke: "#f5f5f5",
                 yellow: "#ffff00",
                 yellowgreen: "#9acd32"
             },
-            cs = Ao,
-            No = D,
-            gs = N,
-            ko = v.type,
-            Vr = cs,
-            Ro = zr,
-            xo = Ne;
-        No.prototype.name = function() {
-            for (var o = xo(this._rgb, "rgb"), f = 0, p = Object.keys(Vr); f < p.length; f += 1) {
+            ds = ko,
+            Ro = D,
+            ps = A,
+            xo = v.type,
+            Vr = ds,
+            To = zr,
+            Eo = Ne;
+        Ro.prototype.name = function() {
+            for (var o = Eo(this._rgb, "rgb"), f = 0, p = Object.keys(Vr); f < p.length; f += 1) {
                 var b = p[f];
                 if (Vr[b] === o)
                     return b.toLowerCase();
             }
             return o;
-        }, gs.format.named = function(o) {
+        }, ps.format.named = function(o) {
             if (o = o.toLowerCase(), Vr[o])
-                return Ro(Vr[o]);
+                return To(Vr[o]);
             throw new Error("unknown color name: " + o);
-        }, gs.autodetect.push({
+        }, ps.autodetect.push({
             p: 5,
             test: function(o) {
                 for (var f = [], p = arguments.length - 1; p-- > 0;)
                     f[p] = arguments[p + 1];
-                if (!f.length && ko(o) === "string" && Vr[o.toLowerCase()])
+                if (!f.length && xo(o) === "string" && Vr[o.toLowerCase()])
                     return "named";
             }
         });
-        var To = v.unpack,
-            Eo = function() {
+        var Lo = v.unpack,
+            Mo = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = To(o, "rgb"),
+                var p = Lo(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2];
-                return (b << 16) + (C << 8) + A;
+                    N = p[2];
+                return (b << 16) + (C << 8) + N;
             },
-            Lo = Eo,
-            Mo = v.type,
-            Bo = function(o) {
-                if (Mo(o) == "number" && o >= 0 && o <= 16777215) {
+            Bo = Mo,
+            Do = v.type,
+            Po = function(o) {
+                if (Do(o) == "number" && o >= 0 && o <= 16777215) {
                     var f = o >> 16,
                         p = o >> 8 & 255,
                         b = o & 255;
                     return [f, p, b, 1];
                 }
                 throw new Error("unknown num color: " + o);
             },
-            Do = Bo,
-            Po = O,
-            ds = D,
-            ps = N,
-            $o = v.type,
-            Io = Lo;
-        ds.prototype.num = function() {
-            return Io(this._rgb);
-        }, Po.num = function() {
+            $o = Po,
+            Io = q,
+            vs = D,
+            ms = A,
+            Oo = v.type,
+            Fo = Bo;
+        vs.prototype.num = function() {
+            return Fo(this._rgb);
+        }, Io.num = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(ds, [null].concat(o, ["num"])))();
-        }, ps.format.num = Do, ps.autodetect.push({
+            return new(Function.prototype.bind.apply(vs, [null].concat(o, ["num"])))();
+        }, ms.format.num = $o, ms.autodetect.push({
             p: 5,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o.length === 1 && $o(o[0]) === "number" && o[0] >= 0 && o[0] <= 16777215)
+                if (o.length === 1 && Oo(o[0]) === "number" && o[0] >= 0 && o[0] <= 16777215)
                     return "num";
             }
         });
-        var Oo = O,
-            an = D,
-            vs = N,
-            ms = v.unpack,
-            bs = v.type,
-            ws = Math.round;
-        an.prototype.rgb = function(o) {
-            return o === void 0 && (o = !0), o === !1 ? this._rgb.slice(0, 3) : this._rgb.slice(0, 3).map(ws);
-        }, an.prototype.rgba = function(o) {
+        var zo = q,
+            on = D,
+            bs = A,
+            ws = v.unpack,
+            ys = v.type,
+            _s = Math.round;
+        on.prototype.rgb = function(o) {
+            return o === void 0 && (o = !0), o === !1 ? this._rgb.slice(0, 3) : this._rgb.slice(0, 3).map(_s);
+        }, on.prototype.rgba = function(o) {
             return o === void 0 && (o = !0), this._rgb.slice(0, 4).map(function(f, p) {
-                return p < 3 ? o === !1 ? f : ws(f) : f;
+                return p < 3 ? o === !1 ? f : _s(f) : f;
             });
-        }, Oo.rgb = function() {
+        }, zo.rgb = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(an, [null].concat(o, ["rgb"])))();
-        }, vs.format.rgb = function() {
+            return new(Function.prototype.bind.apply(on, [null].concat(o, ["rgb"])))();
+        }, bs.format.rgb = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            var p = ms(o, "rgba");
+            var p = ws(o, "rgba");
             return p[3] === void 0 && (p[3] = 1), p;
-        }, vs.autodetect.push({
+        }, bs.autodetect.push({
             p: 3,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = ms(o, "rgba"), bs(o) === "array" && (o.length === 3 || o.length === 4 && bs(o[3]) == "number" && o[3] >= 0 && o[3] <= 1))
+                if (o = ws(o, "rgba"), ys(o) === "array" && (o.length === 3 || o.length === 4 && ys(o[3]) == "number" && o[3] >= 0 && o[3] <= 1))
                     return "rgb";
             }
         });
         var di = Math.log,
-            Fo = function(o) {
+            Ho = function(o) {
                 var f = o / 100,
                     p, b, C;
                 return f < 66 ? (p = 255, b = f < 6 ? 0 : -155.25485562709179 - 0.44596950469579133 * (b = f - 2) + 104.49216199393888 * di(b), C = f < 20 ? 0 : -254.76935184120902 + 0.8274096064007395 * (C = f - 10) + 115.67994401066147 * di(C)) : (p = 351.97690566805693 + 0.114206453784165 * (p = f - 55) - 40.25366309332127 * di(p), b = 325.4494125711974 + 0.07943456536662342 * (b = f - 50) - 28.0852963507957 * di(b), C = 255), [p, b, C, 1];
             },
-            ys = Fo,
-            zo = ys,
-            Ho = v.unpack,
-            Wo = Math.round,
-            qo = function() {
+            Ss = Ho,
+            Wo = Ss,
+            qo = v.unpack,
+            Vo = Math.round,
+            Xo = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                for (var p = Ho(o, "rgb"), b = p[0], C = p[2], A = 1e3, S = 4e4, R = 0.4, E; S - A > R;) {
-                    E = (S + A) * 0.5;
-                    var P = zo(E);
-                    P[2] / P[0] >= C / b ? S = E : A = E;
+                for (var p = qo(o, "rgb"), b = p[0], C = p[2], N = 1e3, S = 4e4, E = 0.4, M; S - N > E;) {
+                    M = (S + N) * 0.5;
+                    var P = Wo(M);
+                    P[2] / P[0] >= C / b ? S = M : N = M;
                 }
-                return Wo(E);
+                return Vo(M);
             },
-            Vo = qo,
-            ln = O,
+            Yo = Xo,
+            hn = q,
             pi = D,
-            on = N,
-            Xo = Vo;
+            fn = A,
+            Go = Yo;
         pi.prototype.temp = pi.prototype.kelvin = pi.prototype.temperature = function() {
-            return Xo(this._rgb);
-        }, ln.temp = ln.kelvin = ln.temperature = function() {
+            return Go(this._rgb);
+        }, hn.temp = hn.kelvin = hn.temperature = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
             return new(Function.prototype.bind.apply(pi, [null].concat(o, ["temp"])))();
-        }, on.format.temp = on.format.kelvin = on.format.temperature = ys;
-        var Yo = v.unpack,
-            hn = Math.cbrt,
-            Go = Math.pow,
-            Uo = Math.sign,
-            Zo = function() {
+        }, fn.format.temp = fn.format.kelvin = fn.format.temperature = Ss;
+        var Uo = v.unpack,
+            un = Math.cbrt,
+            Zo = Math.pow,
+            Ko = Math.sign,
+            jo = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = Yo(o, "rgb"),
+                var p = Uo(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
-                    S = [fn(b / 255), fn(C / 255), fn(A / 255)],
-                    R = S[0],
-                    E = S[1],
+                    N = p[2],
+                    S = [cn(b / 255), cn(C / 255), cn(N / 255)],
+                    E = S[0],
+                    M = S[1],
                     P = S[2],
-                    I = hn(0.4122214708 * R + 0.5363325363 * E + 0.0514459929 * P),
-                    V = hn(0.2119034982 * R + 0.6806995451 * E + 0.1073969566 * P),
-                    F = hn(0.0883024619 * R + 0.2817188376 * E + 0.6299787005 * P);
+                    I = un(0.4122214708 * E + 0.5363325363 * M + 0.0514459929 * P),
+                    W = un(0.2119034982 * E + 0.6806995451 * M + 0.1073969566 * P),
+                    F = un(0.0883024619 * E + 0.2817188376 * M + 0.6299787005 * P);
                 return [
-                    0.2104542553 * I + 0.793617785 * V - 0.0040720468 * F,
-                    1.9779984951 * I - 2.428592205 * V + 0.4505937099 * F,
-                    0.0259040371 * I + 0.7827717662 * V - 0.808675766 * F
+                    0.2104542553 * I + 0.793617785 * W - 0.0040720468 * F,
+                    1.9779984951 * I - 2.428592205 * W + 0.4505937099 * F,
+                    0.0259040371 * I + 0.7827717662 * W - 0.808675766 * F
                 ];
             },
-            _s = Zo;
+            Cs = jo;
 
-        function fn(o) {
+        function cn(o) {
             var f = Math.abs(o);
-            return f < 0.04045 ? o / 12.92 : (Uo(o) || 1) * Go((f + 0.055) / 1.055, 2.4);
+            return f < 0.04045 ? o / 12.92 : (Ko(o) || 1) * Zo((f + 0.055) / 1.055, 2.4);
         }
-        var Ko = v.unpack,
+        var Jo = v.unpack,
             vi = Math.pow,
-            jo = Math.sign,
-            Jo = function() {
+            Qo = Math.sign,
+            eh = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                o = Ko(o, "lab");
+                o = Jo(o, "lab");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A = vi(p + 0.3963377774 * b + 0.2158037573 * C, 3),
+                    N = vi(p + 0.3963377774 * b + 0.2158037573 * C, 3),
                     S = vi(p - 0.1055613458 * b - 0.0638541728 * C, 3),
-                    R = vi(p - 0.0894841775 * b - 1.291485548 * C, 3);
+                    E = vi(p - 0.0894841775 * b - 1.291485548 * C, 3);
                 return [
-                    255 * un(4.0767416621 * A - 3.3077115913 * S + 0.2309699292 * R),
-                    255 * un(-1.2684380046 * A + 2.6097574011 * S - 0.3413193965 * R),
-                    255 * un(-0.0041960863 * A - 0.7034186147 * S + 1.707614701 * R),
+                    255 * gn(4.0767416621 * N - 3.3077115913 * S + 0.2309699292 * E),
+                    255 * gn(-1.2684380046 * N + 2.6097574011 * S - 0.3413193965 * E),
+                    255 * gn(-0.0041960863 * N - 0.7034186147 * S + 1.707614701 * E),
                     o.length > 3 ? o[3] : 1
                 ];
             },
-            Ss = Jo;
+            As = eh;
 
-        function un(o) {
+        function gn(o) {
             var f = Math.abs(o);
-            return f > 31308e-7 ? (jo(o) || 1) * (1.055 * vi(f, 1 / 2.4) - 0.055) : o * 12.92;
+            return f > 31308e-7 ? (Qo(o) || 1) * (1.055 * vi(f, 1 / 2.4) - 0.055) : o * 12.92;
         }
-        var Qo = v.unpack,
-            eh = v.type,
-            th = O,
-            Cs = D,
-            As = N,
-            rh = _s;
-        Cs.prototype.oklab = function() {
-            return rh(this._rgb);
-        }, th.oklab = function() {
+        var th = v.unpack,
+            rh = v.type,
+            ih = q,
+            Ns = D,
+            ks = A,
+            nh = Cs;
+        Ns.prototype.oklab = function() {
+            return nh(this._rgb);
+        }, ih.oklab = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(Cs, [null].concat(o, ["oklab"])))();
-        }, As.format.oklab = Ss, As.autodetect.push({
+            return new(Function.prototype.bind.apply(Ns, [null].concat(o, ["oklab"])))();
+        }, ks.format.oklab = As, ks.autodetect.push({
             p: 3,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = Qo(o, "oklab"), eh(o) === "array" && o.length === 3)
+                if (o = th(o, "oklab"), rh(o) === "array" && o.length === 3)
                     return "oklab";
             }
         });
-        var ih = v.unpack,
-            nh = _s,
-            sh = ls,
-            ah = function() {
+        var sh = v.unpack,
+            ah = Cs,
+            lh = hs,
+            oh = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                var p = ih(o, "rgb"),
+                var p = sh(o, "rgb"),
                     b = p[0],
                     C = p[1],
-                    A = p[2],
-                    S = nh(b, C, A),
-                    R = S[0],
-                    E = S[1],
+                    N = p[2],
+                    S = ah(b, C, N),
+                    E = S[0],
+                    M = S[1],
                     P = S[2];
-                return sh(R, E, P);
+                return lh(E, M, P);
             },
-            lh = ah,
-            oh = v.unpack,
-            hh = os,
-            fh = Ss,
-            uh = function() {
+            hh = oh,
+            fh = v.unpack,
+            uh = fs,
+            ch = As,
+            gh = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                o = oh(o, "lch");
+                o = fh(o, "lch");
                 var p = o[0],
                     b = o[1],
                     C = o[2],
-                    A = hh(p, b, C),
-                    S = A[0],
-                    R = A[1],
-                    E = A[2],
-                    P = fh(S, R, E),
+                    N = uh(p, b, C),
+                    S = N[0],
+                    E = N[1],
+                    M = N[2],
+                    P = ch(S, E, M),
                     I = P[0],
-                    V = P[1],
+                    W = P[1],
                     F = P[2];
-                return [I, V, F, o.length > 3 ? o[3] : 1];
+                return [I, W, F, o.length > 3 ? o[3] : 1];
             },
-            ch = uh,
-            gh = v.unpack,
-            dh = v.type,
-            ph = O,
-            Ns = D,
-            ks = N,
-            vh = lh;
-        Ns.prototype.oklch = function() {
-            return vh(this._rgb);
-        }, ph.oklch = function() {
+            dh = gh,
+            ph = v.unpack,
+            vh = v.type,
+            mh = q,
+            Rs = D,
+            xs = A,
+            bh = hh;
+        Rs.prototype.oklch = function() {
+            return bh(this._rgb);
+        }, mh.oklch = function() {
             for (var o = [], f = arguments.length; f--;)
                 o[f] = arguments[f];
-            return new(Function.prototype.bind.apply(Ns, [null].concat(o, ["oklch"])))();
-        }, ks.format.oklch = ch, ks.autodetect.push({
+            return new(Function.prototype.bind.apply(Rs, [null].concat(o, ["oklch"])))();
+        }, xs.format.oklch = dh, xs.autodetect.push({
             p: 3,
             test: function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
-                if (o = gh(o, "oklch"), dh(o) === "array" && o.length === 3)
+                if (o = ph(o, "oklch"), vh(o) === "array" && o.length === 3)
                     return "oklch";
             }
         });
-        var Rs = D,
-            mh = v.type;
-        Rs.prototype.alpha = function(o, f) {
-            return f === void 0 && (f = !1), o !== void 0 && mh(o) === "number" ? f ? (this._rgb[3] = o, this) : new Rs([this._rgb[0], this._rgb[1], this._rgb[2], o], "rgb") : this._rgb[3];
+        var Ts = D,
+            wh = v.type;
+        Ts.prototype.alpha = function(o, f) {
+            return f === void 0 && (f = !1), o !== void 0 && wh(o) === "number" ? f ? (this._rgb[3] = o, this) : new Ts([this._rgb[0], this._rgb[1], this._rgb[2], o], "rgb") : this._rgb[3];
         };
-        var bh = D;
-        bh.prototype.clipped = function() {
+        var yh = D;
+        yh.prototype.clipped = function() {
             return this._rgb._clipped || !1;
         };
         var hr = D,
-            wh = ci;
+            _h = ci;
         hr.prototype.darken = function(o) {
             o === void 0 && (o = 1);
             var f = this,
                 p = f.lab();
-            return p[0] -= wh.Kn * o, new hr(p, "lab").alpha(f.alpha(), !0);
+            return p[0] -= _h.Kn * o, new hr(p, "lab").alpha(f.alpha(), !0);
         }, hr.prototype.brighten = function(o) {
             return o === void 0 && (o = 1), this.darken(-o);
         }, hr.prototype.darker = hr.prototype.darken, hr.prototype.brighter = hr.prototype.brighten;
-        var yh = D;
-        yh.prototype.get = function(o) {
+        var Sh = D;
+        Sh.prototype.get = function(o) {
             var f = o.split("."),
                 p = f[0],
                 b = f[1],
                 C = this[p]();
             if (b) {
-                var A = p.indexOf(b) - (p.substr(0, 2) === "ok" ? 2 : 0);
-                if (A > -1)
-                    return C[A];
+                var N = p.indexOf(b) - (p.substr(0, 2) === "ok" ? 2 : 0);
+                if (N > -1)
+                    return C[N];
                 throw new Error("unknown channel " + b + " in mode " + p);
             } else
                 return C;
         };
         var yr = D,
-            _h = v.type,
-            Sh = Math.pow,
-            Ch = 1e-7,
-            Ah = 20;
+            Ch = v.type,
+            Ah = Math.pow,
+            Nh = 1e-7,
+            kh = 20;
         yr.prototype.luminance = function(o) {
-            if (o !== void 0 && _h(o) === "number") {
+            if (o !== void 0 && Ch(o) === "number") {
                 if (o === 0)
                     return new yr([0, 0, 0, this._rgb[3]], "rgb");
                 if (o === 1)
                     return new yr([255, 255, 255, this._rgb[3]], "rgb");
                 var f = this.luminance(),
                     p = "rgb",
-                    b = Ah,
-                    C = function(S, R) {
-                        var E = S.interpolate(R, 0.5, p),
-                            P = E.luminance();
-                        return Math.abs(o - P) < Ch || !b-- ? E : P > o ? C(S, E) : C(E, R);
+                    b = kh,
+                    C = function(S, E) {
+                        var M = S.interpolate(E, 0.5, p),
+                            P = M.luminance();
+                        return Math.abs(o - P) < Nh || !b-- ? M : P > o ? C(S, M) : C(M, E);
                     },
-                    A = (f > o ? C(new yr([0, 0, 0]), this) : C(this, new yr([255, 255, 255]))).rgb();
-                return new yr(A.concat([this._rgb[3]]));
+                    N = (f > o ? C(new yr([0, 0, 0]), this) : C(this, new yr([255, 255, 255]))).rgb();
+                return new yr(N.concat([this._rgb[3]]));
             }
-            return Nh.apply(void 0, this._rgb.slice(0, 3));
+            return Rh.apply(void 0, this._rgb.slice(0, 3));
         };
-        var Nh = function(o, f, p) {
-                return o = cn(o), f = cn(f), p = cn(p), 0.2126 * o + 0.7152 * f + 0.0722 * p;
+        var Rh = function(o, f, p) {
+                return o = dn(o), f = dn(f), p = dn(p), 0.2126 * o + 0.7152 * f + 0.0722 * p;
             },
-            cn = function(o) {
-                return o /= 255, o <= 0.03928 ? o / 12.92 : Sh((o + 0.055) / 1.055, 2.4);
+            dn = function(o) {
+                return o /= 255, o <= 0.03928 ? o / 12.92 : Ah((o + 0.055) / 1.055, 2.4);
             },
-            lt = {},
-            xs = D,
-            Ts = v.type,
-            mi = lt,
-            Es = function(o, f, p) {
+            ot = {},
+            Es = D,
+            Ls = v.type,
+            mi = ot,
+            Ms = function(o, f, p) {
                 p === void 0 && (p = 0.5);
                 for (var b = [], C = arguments.length - 3; C-- > 0;)
                     b[C] = arguments[C + 3];
-                var A = b[0] || "lrgb";
-                if (!mi[A] && !b.length && (A = Object.keys(mi)[0]), !mi[A])
-                    throw new Error("interpolation mode " + A + " is not defined");
-                return Ts(o) !== "object" && (o = new xs(o)), Ts(f) !== "object" && (f = new xs(f)), mi[A](o, f, p).alpha(o.alpha() + p * (f.alpha() - o.alpha()));
-            },
-            Ls = D,
-            kh = Es;
-        Ls.prototype.mix = Ls.prototype.interpolate = function(o, f) {
+                var N = b[0] || "lrgb";
+                if (!mi[N] && !b.length && (N = Object.keys(mi)[0]), !mi[N])
+                    throw new Error("interpolation mode " + N + " is not defined");
+                return Ls(o) !== "object" && (o = new Es(o)), Ls(f) !== "object" && (f = new Es(f)), mi[N](o, f, p).alpha(o.alpha() + p * (f.alpha() - o.alpha()));
+            },
+            Bs = D,
+            xh = Ms;
+        Bs.prototype.mix = Bs.prototype.interpolate = function(o, f) {
             f === void 0 && (f = 0.5);
             for (var p = [], b = arguments.length - 2; b-- > 0;)
                 p[b] = arguments[b + 2];
-            return kh.apply(void 0, [this, o, f].concat(p));
+            return xh.apply(void 0, [this, o, f].concat(p));
         };
-        var Ms = D;
-        Ms.prototype.premultiply = function(o) {
+        var Ds = D;
+        Ds.prototype.premultiply = function(o) {
             o === void 0 && (o = !1);
             var f = this._rgb,
                 p = f[3];
-            return o ? (this._rgb = [f[0] * p, f[1] * p, f[2] * p, p], this) : new Ms([f[0] * p, f[1] * p, f[2] * p, p], "rgb");
+            return o ? (this._rgb = [f[0] * p, f[1] * p, f[2] * p, p], this) : new Ds([f[0] * p, f[1] * p, f[2] * p, p], "rgb");
         };
-        var gn = D,
-            Rh = ci;
-        gn.prototype.saturate = function(o) {
+        var pn = D,
+            Th = ci;
+        pn.prototype.saturate = function(o) {
             o === void 0 && (o = 1);
             var f = this,
                 p = f.lch();
-            return p[1] += Rh.Kn * o, p[1] < 0 && (p[1] = 0), new gn(p, "lch").alpha(f.alpha(), !0);
-        }, gn.prototype.desaturate = function(o) {
+            return p[1] += Th.Kn * o, p[1] < 0 && (p[1] = 0), new pn(p, "lch").alpha(f.alpha(), !0);
+        }, pn.prototype.desaturate = function(o) {
             return o === void 0 && (o = 1), this.saturate(-o);
         };
-        var Bs = D,
-            Ds = v.type;
-        Bs.prototype.set = function(o, f, p) {
+        var Ps = D,
+            $s = v.type;
+        Ps.prototype.set = function(o, f, p) {
             p === void 0 && (p = !1);
             var b = o.split("."),
                 C = b[0],
-                A = b[1],
+                N = b[1],
                 S = this[C]();
-            if (A) {
-                var R = C.indexOf(A) - (C.substr(0, 2) === "ok" ? 2 : 0);
-                if (R > -1) {
-                    if (Ds(f) == "string")
+            if (N) {
+                var E = C.indexOf(N) - (C.substr(0, 2) === "ok" ? 2 : 0);
+                if (E > -1) {
+                    if ($s(f) == "string")
                         switch (f.charAt(0)) {
                             case "+":
-                                S[R] += +f;
+                                S[E] += +f;
                                 break;
                             case "-":
-                                S[R] += +f;
+                                S[E] += +f;
                                 break;
                             case "*":
-                                S[R] *= +f.substr(1);
+                                S[E] *= +f.substr(1);
                                 break;
                             case "/":
-                                S[R] /= +f.substr(1);
+                                S[E] /= +f.substr(1);
                                 break;
                             default:
-                                S[R] = +f;
+                                S[E] = +f;
                         }
-                    else if (Ds(f) === "number")
-                        S[R] = f;
+                    else if ($s(f) === "number")
+                        S[E] = f;
                     else
                         throw new Error("unsupported value for Color.set");
-                    var E = new Bs(S, C);
-                    return p ? (this._rgb = E._rgb, this) : E;
+                    var M = new Ps(S, C);
+                    return p ? (this._rgb = M._rgb, this) : M;
                 }
-                throw new Error("unknown channel " + A + " in mode " + C);
+                throw new Error("unknown channel " + N + " in mode " + C);
             } else
                 return S;
         };
-        var xh = D,
-            Th = function(o, f, p) {
+        var Eh = D,
+            Lh = function(o, f, p) {
                 var b = o._rgb,
                     C = f._rgb;
-                return new xh(
+                return new Eh(
                     b[0] + p * (C[0] - b[0]),
                     b[1] + p * (C[1] - b[1]),
                     b[2] + p * (C[2] - b[2]),
                     "rgb"
                 );
             };
-        lt.rgb = Th;
-        var Eh = D,
-            dn = Math.sqrt,
+        ot.rgb = Lh;
+        var Mh = D,
+            vn = Math.sqrt,
             _r = Math.pow,
-            Lh = function(o, f, p) {
+            Bh = function(o, f, p) {
                 var b = o._rgb,
                     C = b[0],
-                    A = b[1],
+                    N = b[1],
                     S = b[2],
-                    R = f._rgb,
-                    E = R[0],
-                    P = R[1],
-                    I = R[2];
-                return new Eh(
-                    dn(_r(C, 2) * (1 - p) + _r(E, 2) * p),
-                    dn(_r(A, 2) * (1 - p) + _r(P, 2) * p),
-                    dn(_r(S, 2) * (1 - p) + _r(I, 2) * p),
+                    E = f._rgb,
+                    M = E[0],
+                    P = E[1],
+                    I = E[2];
+                return new Mh(
+                    vn(_r(C, 2) * (1 - p) + _r(M, 2) * p),
+                    vn(_r(N, 2) * (1 - p) + _r(P, 2) * p),
+                    vn(_r(S, 2) * (1 - p) + _r(I, 2) * p),
                     "rgb"
                 );
             };
-        lt.lrgb = Lh;
-        var Mh = D,
-            Bh = function(o, f, p) {
+        ot.lrgb = Bh;
+        var Dh = D,
+            Ph = function(o, f, p) {
                 var b = o.lab(),
                     C = f.lab();
-                return new Mh(
+                return new Dh(
                     b[0] + p * (C[0] - b[0]),
                     b[1] + p * (C[1] - b[1]),
                     b[2] + p * (C[2] - b[2]),
                     "lab"
                 );
             };
-        lt.lab = Bh;
-        var Ps = D,
+        ot.lab = Ph;
+        var Is = D,
             Sr = function(o, f, p, b) {
-                var C, A, S, R;
-                b === "hsl" ? (S = o.hsl(), R = f.hsl()) : b === "hsv" ? (S = o.hsv(), R = f.hsv()) : b === "hcg" ? (S = o.hcg(), R = f.hcg()) : b === "hsi" ? (S = o.hsi(), R = f.hsi()) : b === "lch" || b === "hcl" ? (b = "hcl", S = o.hcl(), R = f.hcl()) : b === "oklch" && (S = o.oklch().reverse(), R = f.oklch().reverse());
-                var E, P, I, V, F, U;
-                (b.substr(0, 1) === "h" || b === "oklch") && (C = S, E = C[0], I = C[1], F = C[2], A = R, P = A[0], V = A[1], U = A[2]);
-                var G, ae, he, ue;
-                return !isNaN(E) && !isNaN(P) ? (P > E && P - E > 180 ? ue = P - (E + 360) : P < E && E - P > 180 ? ue = P + 360 - E : ue = P - E, ae = E + p * ue) : isNaN(E) ? isNaN(P) ? ae = Number.NaN : (ae = P, (F == 1 || F == 0) && b != "hsv" && (G = V)) : (ae = E, (U == 1 || U == 0) && b != "hsv" && (G = I)), G === void 0 && (G = I + p * (V - I)), he = F + p * (U - F), b === "oklch" ? new Ps([he, G, ae], b) : new Ps([ae, G, he], b);
-            },
-            Dh = Sr,
-            $s = function(o, f, p) {
-                return Dh(o, f, p, "lch");
+                var C, N, S, E;
+                b === "hsl" ? (S = o.hsl(), E = f.hsl()) : b === "hsv" ? (S = o.hsv(), E = f.hsv()) : b === "hcg" ? (S = o.hcg(), E = f.hcg()) : b === "hsi" ? (S = o.hsi(), E = f.hsi()) : b === "lch" || b === "hcl" ? (b = "hcl", S = o.hcl(), E = f.hcl()) : b === "oklch" && (S = o.oklch().reverse(), E = f.oklch().reverse());
+                var M, P, I, W, F, G;
+                (b.substr(0, 1) === "h" || b === "oklch") && (C = S, M = C[0], I = C[1], F = C[2], N = E, P = N[0], W = N[1], G = N[2]);
+                var Y, ae, he, ue;
+                return !isNaN(M) && !isNaN(P) ? (P > M && P - M > 180 ? ue = P - (M + 360) : P < M && M - P > 180 ? ue = P + 360 - M : ue = P - M, ae = M + p * ue) : isNaN(M) ? isNaN(P) ? ae = Number.NaN : (ae = P, (F == 1 || F == 0) && b != "hsv" && (Y = W)) : (ae = M, (G == 1 || G == 0) && b != "hsv" && (Y = I)), Y === void 0 && (Y = I + p * (W - I)), he = F + p * (G - F), b === "oklch" ? new Is([he, Y, ae], b) : new Is([ae, Y, he], b);
+            },
+            $h = Sr,
+            Os = function(o, f, p) {
+                return $h(o, f, p, "lch");
             };
-        lt.lch = $s, lt.hcl = $s;
-        var Ph = D,
-            $h = function(o, f, p) {
+        ot.lch = Os, ot.hcl = Os;
+        var Ih = D,
+            Oh = function(o, f, p) {
                 var b = o.num(),
                     C = f.num();
-                return new Ph(b + p * (C - b), "num");
+                return new Ih(b + p * (C - b), "num");
             };
-        lt.num = $h;
-        var Ih = Sr,
-            Oh = function(o, f, p) {
-                return Ih(o, f, p, "hcg");
-            };
-        lt.hcg = Oh;
+        ot.num = Oh;
         var Fh = Sr,
             zh = function(o, f, p) {
-                return Fh(o, f, p, "hsi");
+                return Fh(o, f, p, "hcg");
             };
-        lt.hsi = zh;
+        ot.hcg = zh;
         var Hh = Sr,
             Wh = function(o, f, p) {
-                return Hh(o, f, p, "hsl");
+                return Hh(o, f, p, "hsi");
             };
-        lt.hsl = Wh;
+        ot.hsi = Wh;
         var qh = Sr,
             Vh = function(o, f, p) {
-                return qh(o, f, p, "hsv");
+                return qh(o, f, p, "hsl");
             };
-        lt.hsv = Vh;
-        var Xh = D,
+        ot.hsl = Vh;
+        var Xh = Sr,
             Yh = function(o, f, p) {
+                return Xh(o, f, p, "hsv");
+            };
+        ot.hsv = Yh;
+        var Gh = D,
+            Uh = function(o, f, p) {
                 var b = o.oklab(),
                     C = f.oklab();
-                return new Xh(
+                return new Gh(
                     b[0] + p * (C[0] - b[0]),
                     b[1] + p * (C[1] - b[1]),
                     b[2] + p * (C[2] - b[2]),
                     "oklab"
                 );
             };
-        lt.oklab = Yh;
-        var Gh = Sr,
-            Uh = function(o, f, p) {
-                return Gh(o, f, p, "oklch");
+        ot.oklab = Uh;
+        var Zh = Sr,
+            Kh = function(o, f, p) {
+                return Zh(o, f, p, "oklch");
             };
-        lt.oklch = Uh;
-        var pn = D,
-            Zh = v.clip_rgb,
-            vn = Math.pow,
-            mn = Math.sqrt,
-            bn = Math.PI,
-            Is = Math.cos,
-            Os = Math.sin,
-            Kh = Math.atan2,
-            jh = function(o, f, p) {
+        ot.oklch = Kh;
+        var mn = D,
+            jh = v.clip_rgb,
+            bn = Math.pow,
+            wn = Math.sqrt,
+            yn = Math.PI,
+            Fs = Math.cos,
+            zs = Math.sin,
+            Jh = Math.atan2,
+            Qh = function(o, f, p) {
                 f === void 0 && (f = "lrgb"), p === void 0 && (p = null);
                 var b = o.length;
                 p || (p = Array.from(new Array(b)).map(function() {
                     return 1;
                 }));
                 var C = b / p.reduce(function(ae, he) {
                     return ae + he;
                 });
                 if (p.forEach(function(ae, he) {
                         p[he] *= C;
                     }), o = o.map(function(ae) {
-                        return new pn(ae);
+                        return new mn(ae);
                     }), f === "lrgb")
-                    return Jh(o, p);
-                for (var A = o.shift(), S = A.get(f), R = [], E = 0, P = 0, I = 0; I < S.length; I++)
-                    if (S[I] = (S[I] || 0) * p[0], R.push(isNaN(S[I]) ? 0 : p[0]), f.charAt(I) === "h" && !isNaN(S[I])) {
-                        var V = S[I] / 180 * bn;
-                        E += Is(V) * p[0], P += Os(V) * p[0];
+                    return ef(o, p);
+                for (var N = o.shift(), S = N.get(f), E = [], M = 0, P = 0, I = 0; I < S.length; I++)
+                    if (S[I] = (S[I] || 0) * p[0], E.push(isNaN(S[I]) ? 0 : p[0]), f.charAt(I) === "h" && !isNaN(S[I])) {
+                        var W = S[I] / 180 * yn;
+                        M += Fs(W) * p[0], P += zs(W) * p[0];
                     }
-                var F = A.alpha() * p[0];
+                var F = N.alpha() * p[0];
                 o.forEach(function(ae, he) {
                     var ue = ae.get(f);
                     F += ae.alpha() * p[he + 1];
                     for (var de = 0; de < S.length; de++)
                         if (!isNaN(ue[de]))
-                            if (R[de] += p[he + 1], f.charAt(de) === "h") {
-                                var Ve = ue[de] / 180 * bn;
-                                E += Is(Ve) * p[he + 1], P += Os(Ve) * p[he + 1];
+                            if (E[de] += p[he + 1], f.charAt(de) === "h") {
+                                var Ve = ue[de] / 180 * yn;
+                                M += Fs(Ve) * p[he + 1], P += zs(Ve) * p[he + 1];
                             } else
                                 S[de] += ue[de] * p[he + 1];
                 });
-                for (var U = 0; U < S.length; U++)
-                    if (f.charAt(U) === "h") {
-                        for (var G = Kh(P / R[U], E / R[U]) / bn * 180; G < 0;)
-                            G += 360;
-                        for (; G >= 360;)
-                            G -= 360;
-                        S[U] = G;
+                for (var G = 0; G < S.length; G++)
+                    if (f.charAt(G) === "h") {
+                        for (var Y = Jh(P / E[G], M / E[G]) / yn * 180; Y < 0;)
+                            Y += 360;
+                        for (; Y >= 360;)
+                            Y -= 360;
+                        S[G] = Y;
                     } else
-                        S[U] = S[U] / R[U];
-                return F /= b, new pn(S, f).alpha(F > 0.99999 ? 1 : F, !0);
+                        S[G] = S[G] / E[G];
+                return F /= b, new mn(S, f).alpha(F > 0.99999 ? 1 : F, !0);
             },
-            Jh = function(o, f) {
+            ef = function(o, f) {
                 for (var p = o.length, b = [0, 0, 0, 0], C = 0; C < o.length; C++) {
-                    var A = o[C],
+                    var N = o[C],
                         S = f[C] / p,
-                        R = A._rgb;
-                    b[0] += vn(R[0], 2) * S, b[1] += vn(R[1], 2) * S, b[2] += vn(R[2], 2) * S, b[3] += R[3] * S;
+                        E = N._rgb;
+                    b[0] += bn(E[0], 2) * S, b[1] += bn(E[1], 2) * S, b[2] += bn(E[2], 2) * S, b[3] += E[3] * S;
                 }
-                return b[0] = mn(b[0]), b[1] = mn(b[1]), b[2] = mn(b[2]), b[3] > 0.9999999 && (b[3] = 1), new pn(Zh(b));
+                return b[0] = wn(b[0]), b[1] = wn(b[1]), b[2] = wn(b[2]), b[3] > 0.9999999 && (b[3] = 1), new mn(jh(b));
             },
-            St = O,
+            St = q,
             Cr = v.type,
-            Qh = Math.pow,
-            wn = function(o) {
+            tf = Math.pow,
+            _n = function(o) {
                 var f = "rgb",
                     p = St("#ccc"),
                     b = 0,
                     C = [0, 1],
-                    A = [],
+                    N = [],
                     S = [0, 0],
-                    R = !1,
-                    E = [],
+                    E = !1,
+                    M = [],
                     P = !1,
                     I = 0,
-                    V = 1,
+                    W = 1,
                     F = !1,
-                    U = {},
-                    G = !0,
+                    G = {},
+                    Y = !0,
                     ae = 1,
-                    he = function(W) {
-                        if (W = W || ["#fff", "#000"], W && Cr(W) === "string" && St.brewer && St.brewer[W.toLowerCase()] && (W = St.brewer[W.toLowerCase()]), Cr(W) === "array") {
-                            W.length === 1 && (W = [W[0], W[0]]), W = W.slice(0);
-                            for (var te = 0; te < W.length; te++)
-                                W[te] = St(W[te]);
-                            A.length = 0;
-                            for (var oe = 0; oe < W.length; oe++)
-                                A.push(oe / (W.length - 1));
+                    he = function(H) {
+                        if (H = H || ["#fff", "#000"], H && Cr(H) === "string" && St.brewer && St.brewer[H.toLowerCase()] && (H = St.brewer[H.toLowerCase()]), Cr(H) === "array") {
+                            H.length === 1 && (H = [H[0], H[0]]), H = H.slice(0);
+                            for (var Q = 0; Q < H.length; Q++)
+                                H[Q] = St(H[Q]);
+                            N.length = 0;
+                            for (var oe = 0; oe < H.length; oe++)
+                                N.push(oe / (H.length - 1));
                         }
-                        return tt(), E = W;
+                        return rt(), M = H;
                     },
-                    ue = function(W) {
-                        if (R != null) {
-                            for (var te = R.length - 1, oe = 0; oe < te && W >= R[oe];)
+                    ue = function(H) {
+                        if (E != null) {
+                            for (var Q = E.length - 1, oe = 0; oe < Q && H >= E[oe];)
                                 oe++;
                             return oe - 1;
                         }
                         return 0;
                     },
-                    de = function(W) {
-                        return W;
+                    de = function(H) {
+                        return H;
                     },
-                    Ve = function(W) {
-                        return W;
+                    Ve = function(H) {
+                        return H;
                     },
-                    ze = function(W, te) {
+                    ze = function(H, Q) {
                         var oe, le;
-                        if (te == null && (te = !1), isNaN(W) || W === null)
+                        if (Q == null && (Q = !1), isNaN(H) || H === null)
                             return p;
-                        if (te)
-                            le = W;
-                        else if (R && R.length > 2) {
-                            var Xe = ue(W);
-                            le = Xe / (R.length - 2);
+                        if (Q)
+                            le = H;
+                        else if (E && E.length > 2) {
+                            var Xe = ue(H);
+                            le = Xe / (E.length - 2);
                         } else
-                            V !== I ? le = (W - I) / (V - I) : le = 1;
-                        le = Ve(le), te || (le = de(le)), ae !== 1 && (le = Qh(le, ae)), le = S[0] + le * (1 - S[0] - S[1]), le = Math.min(1, Math.max(0, le));
+                            W !== I ? le = (H - I) / (W - I) : le = 1;
+                        le = Ve(le), Q || (le = de(le)), ae !== 1 && (le = tf(le, ae)), le = S[0] + le * (1 - S[0] - S[1]), le = Math.min(1, Math.max(0, le));
                         var _e = Math.floor(le * 1e4);
-                        if (G && U[_e])
-                            oe = U[_e];
+                        if (Y && G[_e])
+                            oe = G[_e];
                         else {
-                            if (Cr(E) === "array")
-                                for (var ce = 0; ce < A.length; ce++) {
-                                    var pe = A[ce];
+                            if (Cr(M) === "array")
+                                for (var ce = 0; ce < N.length; ce++) {
+                                    var pe = N[ce];
                                     if (le <= pe) {
-                                        oe = E[ce];
+                                        oe = M[ce];
                                         break;
                                     }
-                                    if (le >= pe && ce === A.length - 1) {
-                                        oe = E[ce];
+                                    if (le >= pe && ce === N.length - 1) {
+                                        oe = M[ce];
                                         break;
                                     }
-                                    if (le > pe && le < A[ce + 1]) {
-                                        le = (le - pe) / (A[ce + 1] - pe), oe = St.interpolate(E[ce], E[ce + 1], le, f);
+                                    if (le > pe && le < N[ce + 1]) {
+                                        le = (le - pe) / (N[ce + 1] - pe), oe = St.interpolate(M[ce], M[ce + 1], le, f);
                                         break;
                                     }
                                 }
                             else
-                                Cr(E) === "function" && (oe = E(le));
-                            G && (U[_e] = oe);
+                                Cr(M) === "function" && (oe = M(le));
+                            Y && (G[_e] = oe);
                         }
                         return oe;
                     },
-                    tt = function() {
-                        return U = {};
+                    rt = function() {
+                        return G = {};
                     };
                 he(o);
-                var fe = function(W) {
-                    var te = St(ze(W));
-                    return P && te[P] ? te[P]() : te;
+                var fe = function(H) {
+                    var Q = St(ze(H));
+                    return P && Q[P] ? Q[P]() : Q;
                 };
-                return fe.classes = function(W) {
-                    if (W != null) {
-                        if (Cr(W) === "array")
-                            R = W, C = [W[0], W[W.length - 1]];
+                return fe.classes = function(H) {
+                    if (H != null) {
+                        if (Cr(H) === "array")
+                            E = H, C = [H[0], H[H.length - 1]];
                         else {
-                            var te = St.analyze(C);
-                            W === 0 ? R = [te.min, te.max] : R = St.limits(te, "e", W);
+                            var Q = St.analyze(C);
+                            H === 0 ? E = [Q.min, Q.max] : E = St.limits(Q, "e", H);
                         }
                         return fe;
                     }
-                    return R;
-                }, fe.domain = function(W) {
+                    return E;
+                }, fe.domain = function(H) {
                     if (!arguments.length)
                         return C;
-                    I = W[0], V = W[W.length - 1], A = [];
-                    var te = E.length;
-                    if (W.length === te && I !== V)
-                        for (var oe = 0, le = Array.from(W); oe < le.length; oe += 1) {
+                    I = H[0], W = H[H.length - 1], N = [];
+                    var Q = M.length;
+                    if (H.length === Q && I !== W)
+                        for (var oe = 0, le = Array.from(H); oe < le.length; oe += 1) {
                             var Xe = le[oe];
-                            A.push((Xe - I) / (V - I));
+                            N.push((Xe - I) / (W - I));
                         }
                     else {
-                        for (var _e = 0; _e < te; _e++)
-                            A.push(_e / (te - 1));
-                        if (W.length > 2) {
-                            var ce = W.map(function(ve, me) {
-                                    return me / (W.length - 1);
+                        for (var _e = 0; _e < Q; _e++)
+                            N.push(_e / (Q - 1));
+                        if (H.length > 2) {
+                            var ce = H.map(function(ve, me) {
+                                    return me / (H.length - 1);
                                 }),
-                                pe = W.map(function(ve) {
-                                    return (ve - I) / (V - I);
+                                pe = H.map(function(ve) {
+                                    return (ve - I) / (W - I);
                                 });
                             pe.every(function(ve, me) {
                                 return ce[me] === ve;
                             }) || (Ve = function(ve) {
                                 if (ve <= 0 || ve >= 1)
                                     return ve;
                                 for (var me = 0; ve >= pe[me + 1];)
                                     me++;
                                 var At = (ve - pe[me]) / (pe[me + 1] - pe[me]),
                                     rr = ce[me] + At * (ce[me + 1] - ce[me]);
                                 return rr;
                             });
                         }
                     }
-                    return C = [I, V], fe;
-                }, fe.mode = function(W) {
-                    return arguments.length ? (f = W, tt(), fe) : f;
-                }, fe.range = function(W, te) {
-                    return he(W), fe;
-                }, fe.out = function(W) {
-                    return P = W, fe;
-                }, fe.spread = function(W) {
-                    return arguments.length ? (b = W, fe) : b;
-                }, fe.correctLightness = function(W) {
-                    return W == null && (W = !0), F = W, tt(), F ? de = function(te) {
-                        for (var oe = ze(0, !0).lab()[0], le = ze(1, !0).lab()[0], Xe = oe > le, _e = ze(te, !0).lab()[0], ce = oe + (le - oe) * te, pe = _e - ce, ve = 0, me = 1, At = 20; Math.abs(pe) > 0.01 && At-- > 0;)
+                    return C = [I, W], fe;
+                }, fe.mode = function(H) {
+                    return arguments.length ? (f = H, rt(), fe) : f;
+                }, fe.range = function(H, Q) {
+                    return he(H), fe;
+                }, fe.out = function(H) {
+                    return P = H, fe;
+                }, fe.spread = function(H) {
+                    return arguments.length ? (b = H, fe) : b;
+                }, fe.correctLightness = function(H) {
+                    return H == null && (H = !0), F = H, rt(), F ? de = function(Q) {
+                        for (var oe = ze(0, !0).lab()[0], le = ze(1, !0).lab()[0], Xe = oe > le, _e = ze(Q, !0).lab()[0], ce = oe + (le - oe) * Q, pe = _e - ce, ve = 0, me = 1, At = 20; Math.abs(pe) > 0.01 && At-- > 0;)
                             (function() {
-                                return Xe && (pe *= -1), pe < 0 ? (ve = te, te += (me - te) * 0.5) : (me = te, te += (ve - te) * 0.5), _e = ze(te, !0).lab()[0], pe = _e - ce;
+                                return Xe && (pe *= -1), pe < 0 ? (ve = Q, Q += (me - Q) * 0.5) : (me = Q, Q += (ve - Q) * 0.5), _e = ze(Q, !0).lab()[0], pe = _e - ce;
                             })();
-                        return te;
-                    } : de = function(te) {
-                        return te;
+                        return Q;
+                    } : de = function(Q) {
+                        return Q;
                     }, fe;
-                }, fe.padding = function(W) {
-                    return W != null ? (Cr(W) === "number" && (W = [W, W]), S = W, fe) : S;
-                }, fe.colors = function(W, te) {
-                    arguments.length < 2 && (te = "hex");
+                }, fe.padding = function(H) {
+                    return H != null ? (Cr(H) === "number" && (H = [H, H]), S = H, fe) : S;
+                }, fe.colors = function(H, Q) {
+                    arguments.length < 2 && (Q = "hex");
                     var oe = [];
                     if (arguments.length === 0)
-                        oe = E.slice(0);
-                    else if (W === 1)
+                        oe = M.slice(0);
+                    else if (H === 1)
                         oe = [fe(0.5)];
-                    else if (W > 1) {
+                    else if (H > 1) {
                         var le = C[0],
                             Xe = C[1] - le;
-                        oe = ef(0, W, !1).map(function(me) {
-                            return fe(le + me / (W - 1) * Xe);
+                        oe = rf(0, H, !1).map(function(me) {
+                            return fe(le + me / (H - 1) * Xe);
                         });
                     } else {
                         o = [];
                         var _e = [];
-                        if (R && R.length > 2)
-                            for (var ce = 1, pe = R.length, ve = 1 <= pe; ve ? ce < pe : ce > pe; ve ? ce++ : ce--)
-                                _e.push((R[ce - 1] + R[ce]) * 0.5);
+                        if (E && E.length > 2)
+                            for (var ce = 1, pe = E.length, ve = 1 <= pe; ve ? ce < pe : ce > pe; ve ? ce++ : ce--)
+                                _e.push((E[ce - 1] + E[ce]) * 0.5);
                         else
                             _e = C;
                         oe = _e.map(function(me) {
                             return fe(me);
                         });
                     }
-                    return St[te] && (oe = oe.map(function(me) {
-                        return me[te]();
+                    return St[Q] && (oe = oe.map(function(me) {
+                        return me[Q]();
                     })), oe;
-                }, fe.cache = function(W) {
-                    return W != null ? (G = W, fe) : G;
-                }, fe.gamma = function(W) {
-                    return W != null ? (ae = W, fe) : ae;
-                }, fe.nodata = function(W) {
-                    return W != null ? (p = St(W), fe) : p;
+                }, fe.cache = function(H) {
+                    return H != null ? (Y = H, fe) : Y;
+                }, fe.gamma = function(H) {
+                    return H != null ? (ae = H, fe) : ae;
+                }, fe.nodata = function(H) {
+                    return H != null ? (p = St(H), fe) : p;
                 }, fe;
             };
 
-        function ef(o, f, p) {
-            for (var b = [], C = o < f, A = p ? C ? f + 1 : f - 1 : f, S = o; C ? S < A : S > A; C ? S++ : S--)
+        function rf(o, f, p) {
+            for (var b = [], C = o < f, N = p ? C ? f + 1 : f - 1 : f, S = o; C ? S < N : S > N; C ? S++ : S--)
                 b.push(S);
             return b;
         }
         var Xr = D,
-            tf = wn,
-            rf = function(o) {
+            nf = _n,
+            sf = function(o) {
                 for (var f = [1, 1], p = 1; p < o; p++) {
                     for (var b = [1], C = 1; C <= f.length; C++)
                         b[C] = (f[C] || 0) + f[C - 1];
                     f = b;
                 }
                 return f;
             },
-            nf = function(o) {
-                var f, p, b, C, A, S, R;
+            af = function(o) {
+                var f, p, b, C, N, S, E;
                 if (o = o.map(function(F) {
                         return new Xr(F);
                     }), o.length === 2)
                     f = o.map(function(F) {
                         return F.lab();
-                    }), A = f[0], S = f[1], C = function(F) {
-                        var U = [0, 1, 2].map(function(G) {
-                            return A[G] + F * (S[G] - A[G]);
+                    }), N = f[0], S = f[1], C = function(F) {
+                        var G = [0, 1, 2].map(function(Y) {
+                            return N[Y] + F * (S[Y] - N[Y]);
                         });
-                        return new Xr(U, "lab");
+                        return new Xr(G, "lab");
                     };
                 else if (o.length === 3)
                     p = o.map(function(F) {
                         return F.lab();
-                    }), A = p[0], S = p[1], R = p[2], C = function(F) {
-                        var U = [0, 1, 2].map(function(G) {
-                            return (1 - F) * (1 - F) * A[G] + 2 * (1 - F) * F * S[G] + F * F * R[G];
+                    }), N = p[0], S = p[1], E = p[2], C = function(F) {
+                        var G = [0, 1, 2].map(function(Y) {
+                            return (1 - F) * (1 - F) * N[Y] + 2 * (1 - F) * F * S[Y] + F * F * E[Y];
                         });
-                        return new Xr(U, "lab");
+                        return new Xr(G, "lab");
                     };
                 else if (o.length === 4) {
-                    var E;
+                    var M;
                     b = o.map(function(F) {
                         return F.lab();
-                    }), A = b[0], S = b[1], R = b[2], E = b[3], C = function(F) {
-                        var U = [0, 1, 2].map(function(G) {
-                            return (1 - F) * (1 - F) * (1 - F) * A[G] + 3 * (1 - F) * (1 - F) * F * S[G] + 3 * (1 - F) * F * F * R[G] + F * F * F * E[G];
+                    }), N = b[0], S = b[1], E = b[2], M = b[3], C = function(F) {
+                        var G = [0, 1, 2].map(function(Y) {
+                            return (1 - F) * (1 - F) * (1 - F) * N[Y] + 3 * (1 - F) * (1 - F) * F * S[Y] + 3 * (1 - F) * F * F * E[Y] + F * F * F * M[Y];
                         });
-                        return new Xr(U, "lab");
+                        return new Xr(G, "lab");
                     };
                 } else if (o.length >= 5) {
-                    var P, I, V;
+                    var P, I, W;
                     P = o.map(function(F) {
                         return F.lab();
-                    }), V = o.length - 1, I = rf(V), C = function(F) {
-                        var U = 1 - F,
-                            G = [0, 1, 2].map(function(ae) {
+                    }), W = o.length - 1, I = sf(W), C = function(F) {
+                        var G = 1 - F,
+                            Y = [0, 1, 2].map(function(ae) {
                                 return P.reduce(function(he, ue, de) {
-                                    return he + I[de] * Math.pow(U, V - de) * Math.pow(F, de) * ue[ae];
+                                    return he + I[de] * Math.pow(G, W - de) * Math.pow(F, de) * ue[ae];
                                 }, 0);
                             });
-                        return new Xr(G, "lab");
+                        return new Xr(Y, "lab");
                     };
                 } else
                     throw new RangeError("No point in running bezier with only one color.");
                 return C;
             },
-            sf = function(o) {
-                var f = nf(o);
+            lf = function(o) {
+                var f = af(o);
                 return f.scale = function() {
-                    return tf(f);
+                    return nf(f);
                 }, f;
             },
-            yn = O,
+            Sn = q,
             Ct = function(o, f, p) {
                 if (!Ct[p])
                     throw new Error("unknown blend mode " + p);
                 return Ct[p](o, f);
             },
             er = function(o) {
                 return function(f, p) {
-                    var b = yn(p).rgb(),
-                        C = yn(f).rgb();
-                    return yn.rgb(o(b, C));
+                    var b = Sn(p).rgb(),
+                        C = Sn(f).rgb();
+                    return Sn.rgb(o(b, C));
                 };
             },
             tr = function(o) {
                 return function(f, p) {
                     var b = [];
                     return b[0] = o(f[0], p[0]), b[1] = o(f[1], p[1]), b[2] = o(f[2], p[2]), b;
                 };
             },
-            af = function(o) {
+            of = function(o) {
                 return o;
             },
-            lf = function(o, f) {
+            hf = function(o, f) {
                 return o * f / 255;
             },
-            of = function(o, f) {
+            ff = function(o, f) {
                 return o > f ? f : o;
             },
-            hf = function(o, f) {
+            uf = function(o, f) {
                 return o > f ? o : f;
             },
-            ff = function(o, f) {
+            cf = function(o, f) {
                 return 255 * (1 - (1 - o / 255) * (1 - f / 255));
             },
-            uf = function(o, f) {
+            gf = function(o, f) {
                 return f < 128 ? 2 * o * f / 255 : 255 * (1 - 2 * (1 - o / 255) * (1 - f / 255));
             },
-            cf = function(o, f) {
+            df = function(o, f) {
                 return 255 * (1 - (1 - f / 255) / (o / 255));
             },
-            gf = function(o, f) {
+            pf = function(o, f) {
                 return o === 255 ? 255 : (o = 255 * (f / 255) / (1 - o / 255), o > 255 ? 255 : o);
             };
-        Ct.normal = er(tr(af)), Ct.multiply = er(tr(lf)), Ct.screen = er(tr(ff)), Ct.overlay = er(tr(uf)), Ct.darken = er(tr(of)), Ct.lighten = er(tr(hf)), Ct.dodge = er(tr(gf)), Ct.burn = er(tr(cf));
-        for (var df = Ct, _n = v.type, pf = v.clip_rgb, vf = v.TWOPI, mf = Math.pow, bf = Math.sin, wf = Math.cos, Fs = O, yf = function(o, f, p, b, C) {
+        Ct.normal = er(tr(of)), Ct.multiply = er(tr(hf)), Ct.screen = er(tr(cf)), Ct.overlay = er(tr(gf)), Ct.darken = er(tr(ff)), Ct.lighten = er(tr(uf)), Ct.dodge = er(tr(pf)), Ct.burn = er(tr(df));
+        for (var vf = Ct, Cn = v.type, mf = v.clip_rgb, bf = v.TWOPI, wf = Math.pow, yf = Math.sin, _f = Math.cos, Hs = q, Sf = function(o, f, p, b, C) {
                 o === void 0 && (o = 300), f === void 0 && (f = -1.5), p === void 0 && (p = 1), b === void 0 && (b = 1), C === void 0 && (C = [0, 1]);
-                var A = 0,
+                var N = 0,
                     S;
-                _n(C) === "array" ? S = C[1] - C[0] : (S = 0, C = [C, C]);
-                var R = function(E) {
-                    var P = vf * ((o + 120) / 360 + f * E),
-                        I = mf(C[0] + S * E, b),
-                        V = A !== 0 ? p[0] + E * A : p,
-                        F = V * I * (1 - I) / 2,
-                        U = wf(P),
-                        G = bf(P),
-                        ae = I + F * (-0.14861 * U + 1.78277 * G),
-                        he = I + F * (-0.29227 * U - 0.90649 * G),
-                        ue = I + F * (1.97294 * U);
-                    return Fs(pf([ae * 255, he * 255, ue * 255, 1]));
+                Cn(C) === "array" ? S = C[1] - C[0] : (S = 0, C = [C, C]);
+                var E = function(M) {
+                    var P = bf * ((o + 120) / 360 + f * M),
+                        I = wf(C[0] + S * M, b),
+                        W = N !== 0 ? p[0] + M * N : p,
+                        F = W * I * (1 - I) / 2,
+                        G = _f(P),
+                        Y = yf(P),
+                        ae = I + F * (-0.14861 * G + 1.78277 * Y),
+                        he = I + F * (-0.29227 * G - 0.90649 * Y),
+                        ue = I + F * (1.97294 * G);
+                    return Hs(mf([ae * 255, he * 255, ue * 255, 1]));
                 };
-                return R.start = function(E) {
-                    return E == null ? o : (o = E, R);
-                }, R.rotations = function(E) {
-                    return E == null ? f : (f = E, R);
-                }, R.gamma = function(E) {
-                    return E == null ? b : (b = E, R);
-                }, R.hue = function(E) {
-                    return E == null ? p : (p = E, _n(p) === "array" ? (A = p[1] - p[0], A === 0 && (p = p[1])) : A = 0, R);
-                }, R.lightness = function(E) {
-                    return E == null ? C : (_n(E) === "array" ? (C = E, S = E[1] - E[0]) : (C = [E, E], S = 0), R);
-                }, R.scale = function() {
-                    return Fs.scale(R);
-                }, R.hue(p), R;
-            }, _f = D, Sf = "0123456789abcdef", Cf = Math.floor, Af = Math.random, Nf = function() {
+                return E.start = function(M) {
+                    return M == null ? o : (o = M, E);
+                }, E.rotations = function(M) {
+                    return M == null ? f : (f = M, E);
+                }, E.gamma = function(M) {
+                    return M == null ? b : (b = M, E);
+                }, E.hue = function(M) {
+                    return M == null ? p : (p = M, Cn(p) === "array" ? (N = p[1] - p[0], N === 0 && (p = p[1])) : N = 0, E);
+                }, E.lightness = function(M) {
+                    return M == null ? C : (Cn(M) === "array" ? (C = M, S = M[1] - M[0]) : (C = [M, M], S = 0), E);
+                }, E.scale = function() {
+                    return Hs.scale(E);
+                }, E.hue(p), E;
+            }, Cf = D, Af = "0123456789abcdef", Nf = Math.floor, kf = Math.random, Rf = function() {
                 for (var o = "#", f = 0; f < 6; f++)
-                    o += Sf.charAt(Cf(Af() * 16));
-                return new _f(o, "hex");
-            }, Sn = l, zs = Math.log, kf = Math.pow, Rf = Math.floor, xf = Math.abs, Hs = function(o, f) {
+                    o += Af.charAt(Nf(kf() * 16));
+                return new Cf(o, "hex");
+            }, An = l, Ws = Math.log, xf = Math.pow, Tf = Math.floor, Ef = Math.abs, qs = function(o, f) {
                 f === void 0 && (f = null);
                 var p = {
                     min: Number.MAX_VALUE,
                     max: Number.MAX_VALUE * -1,
                     sum: 0,
                     values: [],
                     count: 0
                 };
-                return Sn(o) === "object" && (o = Object.values(o)), o.forEach(function(b) {
-                    f && Sn(b) === "object" && (b = b[f]), b != null && !isNaN(b) && (p.values.push(b), p.sum += b, b < p.min && (p.min = b), b > p.max && (p.max = b), p.count += 1);
+                return An(o) === "object" && (o = Object.values(o)), o.forEach(function(b) {
+                    f && An(b) === "object" && (b = b[f]), b != null && !isNaN(b) && (p.values.push(b), p.sum += b, b < p.min && (p.min = b), b > p.max && (p.max = b), p.count += 1);
                 }), p.domain = [p.min, p.max], p.limits = function(b, C) {
-                    return Ws(p, b, C);
+                    return Vs(p, b, C);
                 }, p;
-            }, Ws = function(o, f, p) {
-                f === void 0 && (f = "equal"), p === void 0 && (p = 7), Sn(o) == "array" && (o = Hs(o));
+            }, Vs = function(o, f, p) {
+                f === void 0 && (f = "equal"), p === void 0 && (p = 7), An(o) == "array" && (o = qs(o));
                 var b = o.min,
                     C = o.max,
-                    A = o.values.sort(function(An, Nn) {
-                        return An - Nn;
+                    N = o.values.sort(function(kn, Rn) {
+                        return kn - Rn;
                     });
                 if (p === 1)
                     return [b, C];
                 var S = [];
                 if (f.substr(0, 1) === "c" && (S.push(b), S.push(C)), f.substr(0, 1) === "e") {
                     S.push(b);
-                    for (var R = 1; R < p; R++)
-                        S.push(b + R / p * (C - b));
+                    for (var E = 1; E < p; E++)
+                        S.push(b + E / p * (C - b));
                     S.push(C);
                 } else if (f.substr(0, 1) === "l") {
                     if (b <= 0)
                         throw new Error("Logarithmic scales are only possible for values > 0");
-                    var E = Math.LOG10E * zs(b),
-                        P = Math.LOG10E * zs(C);
+                    var M = Math.LOG10E * Ws(b),
+                        P = Math.LOG10E * Ws(C);
                     S.push(b);
                     for (var I = 1; I < p; I++)
-                        S.push(kf(10, E + I / p * (P - E)));
+                        S.push(xf(10, M + I / p * (P - M)));
                     S.push(C);
                 } else if (f.substr(0, 1) === "q") {
                     S.push(b);
-                    for (var V = 1; V < p; V++) {
-                        var F = (A.length - 1) * V / p,
-                            U = Rf(F);
-                        if (U === F)
-                            S.push(A[U]);
+                    for (var W = 1; W < p; W++) {
+                        var F = (N.length - 1) * W / p,
+                            G = Tf(F);
+                        if (G === F)
+                            S.push(N[G]);
                         else {
-                            var G = F - U;
-                            S.push(A[U] * (1 - G) + A[U + 1] * G);
+                            var Y = F - G;
+                            S.push(N[G] * (1 - Y) + N[G + 1] * Y);
                         }
                     }
                     S.push(C);
                 } else if (f.substr(0, 1) === "k") {
-                    var ae, he = A.length,
+                    var ae, he = N.length,
                         ue = new Array(he),
                         de = new Array(p),
                         Ve = !0,
                         ze = 0,
-                        tt = null;
-                    tt = [], tt.push(b);
+                        rt = null;
+                    rt = [], rt.push(b);
                     for (var fe = 1; fe < p; fe++)
-                        tt.push(b + fe / p * (C - b));
-                    for (tt.push(C); Ve;) {
-                        for (var W = 0; W < p; W++)
-                            de[W] = 0;
-                        for (var te = 0; te < he; te++)
-                            for (var oe = A[te], le = Number.MAX_VALUE, Xe = void 0, _e = 0; _e < p; _e++) {
-                                var ce = xf(tt[_e] - oe);
-                                ce < le && (le = ce, Xe = _e), de[Xe]++, ue[te] = Xe;
+                        rt.push(b + fe / p * (C - b));
+                    for (rt.push(C); Ve;) {
+                        for (var H = 0; H < p; H++)
+                            de[H] = 0;
+                        for (var Q = 0; Q < he; Q++)
+                            for (var oe = N[Q], le = Number.MAX_VALUE, Xe = void 0, _e = 0; _e < p; _e++) {
+                                var ce = Ef(rt[_e] - oe);
+                                ce < le && (le = ce, Xe = _e), de[Xe]++, ue[Q] = Xe;
                             }
                         for (var pe = new Array(p), ve = 0; ve < p; ve++)
                             pe[ve] = null;
                         for (var me = 0; me < he; me++)
-                            ae = ue[me], pe[ae] === null ? pe[ae] = A[me] : pe[ae] += A[me];
+                            ae = ue[me], pe[ae] === null ? pe[ae] = N[me] : pe[ae] += N[me];
                         for (var At = 0; At < p; At++)
                             pe[At] *= 1 / de[At];
                         Ve = !1;
                         for (var rr = 0; rr < p; rr++)
-                            if (pe[rr] !== tt[rr]) {
+                            if (pe[rr] !== rt[rr]) {
                                 Ve = !0;
                                 break;
                             }
-                        tt = pe, ze++, ze > 200 && (Ve = !1);
+                        rt = pe, ze++, ze > 200 && (Ve = !1);
                     }
                     for (var ir = {}, Ar = 0; Ar < p; Ar++)
                         ir[Ar] = [];
                     for (var Nr = 0; Nr < he; Nr++)
-                        ae = ue[Nr], ir[ae].push(A[Nr]);
+                        ae = ue[Nr], ir[ae].push(N[Nr]);
                     for (var Wt = [], fr = 0; fr < p; fr++)
                         Wt.push(ir[fr][0]), Wt.push(ir[fr][ir[fr].length - 1]);
-                    Wt = Wt.sort(function(An, Nn) {
-                        return An - Nn;
+                    Wt = Wt.sort(function(kn, Rn) {
+                        return kn - Rn;
                     }), S.push(Wt[0]);
                     for (var Yr = 1; Yr < Wt.length; Yr += 2) {
                         var ur = Wt[Yr];
                         !isNaN(ur) && S.indexOf(ur) === -1 && S.push(ur);
                     }
                 }
                 return S;
-            }, qs = {
-                analyze: Hs,
-                limits: Ws
-            }, Vs = D, Tf = function(o, f) {
-                o = new Vs(o), f = new Vs(f);
+            }, Xs = {
+                analyze: qs,
+                limits: Vs
+            }, Ys = D, Lf = function(o, f) {
+                o = new Ys(o), f = new Ys(f);
                 var p = o.luminance(),
                     b = f.luminance();
                 return p > b ? (p + 0.05) / (b + 0.05) : (b + 0.05) / (p + 0.05);
-            }, Xs = D, Ht = Math.sqrt, Pe = Math.pow, Ef = Math.min, Lf = Math.max, Ys = Math.atan2, Gs = Math.abs, bi = Math.cos, Us = Math.sin, Mf = Math.exp, Zs = Math.PI, Bf = function(o, f, p, b, C) {
+            }, Gs = D, Ht = Math.sqrt, Pe = Math.pow, Mf = Math.min, Bf = Math.max, Us = Math.atan2, Zs = Math.abs, bi = Math.cos, Ks = Math.sin, Df = Math.exp, js = Math.PI, Pf = function(o, f, p, b, C) {
                 p === void 0 && (p = 1), b === void 0 && (b = 1), C === void 0 && (C = 1);
-                var A = function(ur) {
-                        return 360 * ur / (2 * Zs);
+                var N = function(ur) {
+                        return 360 * ur / (2 * js);
                     },
                     S = function(ur) {
-                        return 2 * Zs * ur / 360;
+                        return 2 * js * ur / 360;
                     };
-                o = new Xs(o), f = new Xs(f);
-                var R = Array.from(o.lab()),
-                    E = R[0],
-                    P = R[1],
-                    I = R[2],
-                    V = Array.from(f.lab()),
-                    F = V[0],
-                    U = V[1],
-                    G = V[2],
-                    ae = (E + F) / 2,
+                o = new Gs(o), f = new Gs(f);
+                var E = Array.from(o.lab()),
+                    M = E[0],
+                    P = E[1],
+                    I = E[2],
+                    W = Array.from(f.lab()),
+                    F = W[0],
+                    G = W[1],
+                    Y = W[2],
+                    ae = (M + F) / 2,
                     he = Ht(Pe(P, 2) + Pe(I, 2)),
-                    ue = Ht(Pe(U, 2) + Pe(G, 2)),
+                    ue = Ht(Pe(G, 2) + Pe(Y, 2)),
                     de = (he + ue) / 2,
                     Ve = 0.5 * (1 - Ht(Pe(de, 7) / (Pe(de, 7) + Pe(25, 7)))),
                     ze = P * (1 + Ve),
-                    tt = U * (1 + Ve),
+                    rt = G * (1 + Ve),
                     fe = Ht(Pe(ze, 2) + Pe(I, 2)),
-                    W = Ht(Pe(tt, 2) + Pe(G, 2)),
-                    te = (fe + W) / 2,
-                    oe = A(Ys(I, ze)),
-                    le = A(Ys(G, tt)),
+                    H = Ht(Pe(rt, 2) + Pe(Y, 2)),
+                    Q = (fe + H) / 2,
+                    oe = N(Us(I, ze)),
+                    le = N(Us(Y, rt)),
                     Xe = oe >= 0 ? oe : oe + 360,
                     _e = le >= 0 ? le : le + 360,
-                    ce = Gs(Xe - _e) > 180 ? (Xe + _e + 360) / 2 : (Xe + _e) / 2,
+                    ce = Zs(Xe - _e) > 180 ? (Xe + _e + 360) / 2 : (Xe + _e) / 2,
                     pe = 1 - 0.17 * bi(S(ce - 30)) + 0.24 * bi(S(2 * ce)) + 0.32 * bi(S(3 * ce + 6)) - 0.2 * bi(S(4 * ce - 63)),
                     ve = _e - Xe;
-                ve = Gs(ve) <= 180 ? ve : _e <= Xe ? ve + 360 : ve - 360, ve = 2 * Ht(fe * W) * Us(S(ve) / 2);
-                var me = F - E,
-                    At = W - fe,
+                ve = Zs(ve) <= 180 ? ve : _e <= Xe ? ve + 360 : ve - 360, ve = 2 * Ht(fe * H) * Ks(S(ve) / 2);
+                var me = F - M,
+                    At = H - fe,
                     rr = 1 + 0.015 * Pe(ae - 50, 2) / Ht(20 + Pe(ae - 50, 2)),
-                    ir = 1 + 0.045 * te,
-                    Ar = 1 + 0.015 * te * pe,
-                    Nr = 30 * Mf(-Pe((ce - 275) / 25, 2)),
-                    Wt = 2 * Ht(Pe(te, 7) / (Pe(te, 7) + Pe(25, 7))),
-                    fr = -Wt * Us(2 * S(Nr)),
+                    ir = 1 + 0.045 * Q,
+                    Ar = 1 + 0.015 * Q * pe,
+                    Nr = 30 * Df(-Pe((ce - 275) / 25, 2)),
+                    Wt = 2 * Ht(Pe(Q, 7) / (Pe(Q, 7) + Pe(25, 7))),
+                    fr = -Wt * Ks(2 * S(Nr)),
                     Yr = Ht(Pe(me / (p * rr), 2) + Pe(At / (b * ir), 2) + Pe(ve / (C * Ar), 2) + fr * (At / (b * ir)) * (ve / (C * Ar)));
-                return Lf(0, Ef(100, Yr));
-            }, Ks = D, Df = function(o, f, p) {
-                p === void 0 && (p = "lab"), o = new Ks(o), f = new Ks(f);
+                return Bf(0, Mf(100, Yr));
+            }, Js = D, $f = function(o, f, p) {
+                p === void 0 && (p = "lab"), o = new Js(o), f = new Js(f);
                 var b = o.get(p),
                     C = f.get(p),
-                    A = 0;
+                    N = 0;
                 for (var S in b) {
-                    var R = (b[S] || 0) - (C[S] || 0);
-                    A += R * R;
+                    var E = (b[S] || 0) - (C[S] || 0);
+                    N += E * E;
                 }
-                return Math.sqrt(A);
-            }, Pf = D, $f = function() {
+                return Math.sqrt(N);
+            }, If = D, Of = function() {
                 for (var o = [], f = arguments.length; f--;)
                     o[f] = arguments[f];
                 try {
-                    return new(Function.prototype.bind.apply(Pf, [null].concat(o)))(), !0;
+                    return new(Function.prototype.bind.apply(If, [null].concat(o)))(), !0;
                 } catch {
                     return !1;
                 }
-            }, js = O, Js = wn, If = {
+            }, Qs = q, ea = _n, Ff = {
                 cool: function() {
-                    return Js([js.hsl(180, 1, 0.9), js.hsl(250, 0.7, 0.4)]);
+                    return ea([Qs.hsl(180, 1, 0.9), Qs.hsl(250, 0.7, 0.4)]);
                 },
                 hot: function() {
-                    return Js(["#000", "#f00", "#ff0", "#fff"]).mode("rgb");
+                    return ea(["#000", "#f00", "#ff0", "#fff"]).mode("rgb");
                 }
             }, wi = {
                 // sequential
                 OrRd: ["#fff7ec", "#fee8c8", "#fdd49e", "#fdbb84", "#fc8d59", "#ef6548", "#d7301f", "#b30000", "#7f0000"],
                 PuBu: ["#fff7fb", "#ece7f2", "#d0d1e6", "#a6bddb", "#74a9cf", "#3690c0", "#0570b0", "#045a8d", "#023858"],
                 BuPu: ["#f7fcfd", "#e0ecf4", "#bfd3e6", "#9ebcda", "#8c96c6", "#8c6bb1", "#88419d", "#810f7c", "#4d004b"],
                 Oranges: ["#fff5eb", "#fee6ce", "#fdd0a2", "#fdae6b", "#fd8d3c", "#f16913", "#d94801", "#a63603", "#7f2704"],
@@ -10339,30 +10339,30 @@
                 Accent: ["#7fc97f", "#beaed4", "#fdc086", "#ffff99", "#386cb0", "#f0027f", "#bf5b17", "#666666"],
                 Set1: ["#e41a1c", "#377eb8", "#4daf4a", "#984ea3", "#ff7f00", "#ffff33", "#a65628", "#f781bf", "#999999"],
                 Set3: ["#8dd3c7", "#ffffb3", "#bebada", "#fb8072", "#80b1d3", "#fdb462", "#b3de69", "#fccde5", "#d9d9d9", "#bc80bd", "#ccebc5", "#ffed6f"],
                 Dark2: ["#1b9e77", "#d95f02", "#7570b3", "#e7298a", "#66a61e", "#e6ab02", "#a6761d", "#666666"],
                 Paired: ["#a6cee3", "#1f78b4", "#b2df8a", "#33a02c", "#fb9a99", "#e31a1c", "#fdbf6f", "#ff7f00", "#cab2d6", "#6a3d9a", "#ffff99", "#b15928"],
                 Pastel2: ["#b3e2cd", "#fdcdac", "#cbd5e8", "#f4cae4", "#e6f5c9", "#fff2ae", "#f1e2cc", "#cccccc"],
                 Pastel1: ["#fbb4ae", "#b3cde3", "#ccebc5", "#decbe4", "#fed9a6", "#ffffcc", "#e5d8bd", "#fddaec", "#f2f2f2"]
-            }, Cn = 0, Qs = Object.keys(wi); Cn < Qs.length; Cn += 1) {
-            var ea = Qs[Cn];
-            wi[ea.toLowerCase()] = wi[ea];
-        }
-        var Of = wi,
-            Fe = O;
-        Fe.average = jh, Fe.bezier = sf, Fe.blend = df, Fe.cubehelix = yf, Fe.mix = Fe.interpolate = Es, Fe.random = Nf, Fe.scale = wn, Fe.analyze = qs.analyze, Fe.contrast = Tf, Fe.deltaE = Bf, Fe.distance = Df, Fe.limits = qs.limits, Fe.valid = $f, Fe.scales = If, Fe.colors = cs, Fe.brewer = Of;
-        var Ff = Fe;
-        return Ff;
+            }, Nn = 0, ta = Object.keys(wi); Nn < ta.length; Nn += 1) {
+            var ra = ta[Nn];
+            wi[ra.toLowerCase()] = wi[ra];
+        }
+        var zf = wi,
+            Fe = q;
+        Fe.average = Qh, Fe.bezier = lf, Fe.blend = vf, Fe.cubehelix = Sf, Fe.mix = Fe.interpolate = Ms, Fe.random = Rf, Fe.scale = _n, Fe.analyze = Xs.analyze, Fe.contrast = Lf, Fe.deltaE = Pf, Fe.distance = $f, Fe.limits = Xs.limits, Fe.valid = Of, Fe.scales = Ff, Fe.colors = ds, Fe.brewer = zf;
+        var Hf = Fe;
+        return Hf;
     });
-})(ml);
-var Bg = ml.exports;
-const $a = ar,
-    Dg = Mg,
-    Pg = Bg;
-let $g = class {
+})(bl);
+var Pg = bl.exports;
+const Oa = ar,
+    $g = Dg,
+    Ig = Pg;
+let Og = class {
     /**
      * The constructor of the class Graph.
      * 
      * @param {Vector2[]} points The centres of the gaussians.
      * @param {Number[]} weights The weights / amplitudes for each gaussian.
      */
     constructor(e, t, r, i, s = 0.3, a = 0, n = null, h = 1, l = !1) {
@@ -10376,15 +10376,15 @@
             "#b8e186",
             "#7fbc41",
             "#4d9221"
         ]), this.colormap = n, this.canvas = document.createElement("canvas"), this.context = this.canvas.getContext("2d"), this.canvas.width = this.width, this.canvas.height = this.height;
     }
     setFromArray(e, t) {
         this.points = [], e.forEach((r) => {
-            this.points.push(new $a(r[0], r[1]));
+            this.points.push(new Oa(r[0], r[1]));
         }), this.weights = [], t.forEach((r) => {
             this.weights.push(r);
         });
     }
     /**
      * Compute and draw the gaussians.
      */
@@ -10412,20 +10412,20 @@
             let s = -Number.MAX_SAFE_INTEGER,
                 a = Number.MAX_SAFE_INTEGER;
             for (let n = 0; n < this.width; n++)
                 for (let h = 0; h < this.height; h++)
                     e[n][h] < a && (a = e[n][h]), e[n][h] > s && (s = e[n][h]);
             r = Math.max(Math.abs(a), Math.abs(s));
         }
-        const i = Pg.scale(this.colormap).domain([-1, 1]);
+        const i = Ig.scale(this.colormap).domain([-1, 1]);
         for (let s = 0; s < this.width; s++)
             for (let a = 0; a < this.height; a++) {
                 this.normalized || (e[s][a] = e[s][a] / r), this.interval !== 0 && (e[s][a] = Math.round(e[s][a] / this.interval) * this.interval);
                 let [n, h, l] = i(e[s][a]).rgb();
-                this.setPixel(new $a(s, a), n, h, l);
+                this.setPixel(new Oa(s, a), n, h, l);
             }
     }
     /**
      * Get the canvas as an HTML image.
      * 
      * @param {CallableFunction} callback
      */
@@ -10439,41 +10439,41 @@
     }
     /**
      * Get the canvas as an SVG element.
      * 
      * @param {CallableFunction} callback
      */
     getSVG() {
-        return Dg(this.context.getImageData(0, 0, this.width, this.height));
+        return $g(this.context.getImageData(0, 0, this.width, this.height));
     }
     /**
      * Set the colour at a specific point on the canvas.
      * 
      * @param {Vector2} vec The pixel position on the canvas.
      * @param {Number} r The red colour-component.
      * @param {Number} g The green colour-component.
      * @param {Number} b The blue colour-component.
      * @param {Number} a The alpha colour-component.
      */
     setPixel(e, t, r, i) {
         this.context.fillStyle = "rgba(" + t + "," + r + "," + i + "," + this.opacity + ")", this.context.fillRect(e.x, e.y, 1, 1);
     }
 };
-var bl = $g;
-const Ia = Zr,
-    Ig = Li(),
-    Og = kg,
-    Je = Xn,
-    Fg = Un,
-    zg = Yn,
+var wl = Og;
+const Fa = Zr,
+    Fg = Li(),
+    zg = xg,
+    Je = Zn,
+    Hg = Jn,
+    Wg = Kn,
     $e = ar,
-    Hg = bl;
-let Wg = class {
+    qg = wl;
+let Vg = class {
     constructor(e, t = !0) {
-        this.preprocessor = new Og(e), this.opts = this.preprocessor.opts, this.clear = t, this.svgWrapper = null;
+        this.preprocessor = new zg(e), this.opts = this.preprocessor.opts, this.clear = t, this.svgWrapper = null;
     }
     /**
      * Draws the parsed smiles data to an svg element.
      *
      * @param {Object} data The tree returned by the smiles parser.
      * @param {?(String|SVGElement)} target The id of the HTML svg element the structure is drawn to - or the element itself.
      * @param {String} themeName='dark' The name of the theme to use. Built-in themes are 'light' and 'dark'.
@@ -10485,15 +10485,15 @@
         t === null || t === "svg" ? (t = document.createElementNS("http://www.w3.org/2000/svg", "svg"), t.setAttribute("xmlns", "http://www.w3.org/2000/svg"), t.setAttribute("xmlns:xlink", "http://www.w3.org/1999/xlink"), t.setAttributeNS(null, "width", this.opts.width), t.setAttributeNS(null, "height", this.opts.height)) : t instanceof String && (t = document.getElementById(t));
         let h = {
             padding: this.opts.padding,
             compactDrawing: this.opts.compactDrawing
         };
         i !== null && (this.opts.padding += this.opts.weights.additionalPadding, this.opts.compactDrawing = !1);
         let l = this.preprocessor;
-        return l.initDraw(e, r, s, a), s || (this.themeManager = new zg(this.opts.themes, r), (this.svgWrapper === null || this.clear) && (this.svgWrapper = new Fg(this.themeManager, t, this.opts, this.clear))), l.processGraph(), this.svgWrapper.determineDimensions(l.graph.vertices), this.drawAtomHighlights(l.opts.debug), this.drawEdges(l.opts.debug), this.drawVertices(l.opts.debug), i !== null && this.drawWeights(i, n), l.opts.debug && (console.log(l.graph), console.log(l.rings), console.log(l.ringConnections)), this.svgWrapper.constructSvg(), i !== null && (this.opts.padding = h.padding, this.opts.compactDrawing = h.padding), t;
+        return l.initDraw(e, r, s, a), s || (this.themeManager = new Wg(this.opts.themes, r), (this.svgWrapper === null || this.clear) && (this.svgWrapper = new Hg(this.themeManager, t, this.opts, this.clear))), l.processGraph(), this.svgWrapper.determineDimensions(l.graph.vertices), this.drawAtomHighlights(l.opts.debug), this.drawEdges(l.opts.debug), this.drawVertices(l.opts.debug), i !== null && this.drawWeights(i, n), l.opts.debug && (console.log(l.graph), console.log(l.rings), console.log(l.ringConnections)), this.svgWrapper.constructSvg(), i !== null && (this.opts.padding = h.padding, this.opts.compactDrawing = h.padding), t;
     }
     /**
      * Draws the parsed smiles data to a canvas element.
      *
      * @param {Object} data The tree returned by the smiles parser.
      * @param {(String|HTMLCanvasElement)} target The id of the HTML canvas element the structure is drawn to - or the element itself.
      * @param {String} themeName='dark' The name of the theme to use. Built-in themes are 'light' and 'dark'.
@@ -10551,46 +10551,46 @@
             l = n.value.element,
             c = h.value.element;
         if ((!n.value.isDrawn || !h.value.isDrawn) && r.opts.atomVisualization === "default")
             return;
         let u = n.position,
             g = h.position,
             m = r.getEdgeNormals(a),
-            _ = Ia.clone(m);
+            _ = Fa.clone(m);
         if (_[0].multiplyScalar(10).add(u), _[1].multiplyScalar(10).add(u), a.bondType === "=" || r.getRingbondType(n, h) === "=" || a.isPartOfAromaticRing && r.bridgedRing) {
             let v = r.areVerticesInSameRing(n, h),
-                N = r.chooseSide(n, h, _);
+                A = r.chooseSide(n, h, _);
             if (v) {
-                let x = r.getLargestOrAromaticCommonRing(n, h).center;
+                let k = r.getLargestOrAromaticCommonRing(n, h).center;
                 m[0].multiplyScalar(i.bondSpacing), m[1].multiplyScalar(i.bondSpacing);
-                let L = null;
-                x.sameSideAs(n.position, h.position, $e.add(u, m[0])) ? L = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c) : L = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c), L.shorten(i.bondLength - i.shortBondLength * i.bondLength), a.isPartOfAromaticRing ? s.drawLine(L, !0) : s.drawLine(L), s.drawLine(new Je(u, g, l, c));
-            } else if (a.center || n.isTerminal() && h.isTerminal() || N.anCount == 0 && N.bnCount > 1 || N.bnCount == 0 && N.anCount > 1) {
+                let x = null;
+                k.sameSideAs(n.position, h.position, $e.add(u, m[0])) ? x = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c) : x = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c), x.shorten(i.bondLength - i.shortBondLength * i.bondLength), a.isPartOfAromaticRing ? s.drawLine(x, !0) : s.drawLine(x), s.drawLine(new Je(u, g, l, c));
+            } else if (a.center || n.isTerminal() && h.isTerminal() || A.anCount == 0 && A.bnCount > 1 || A.bnCount == 0 && A.anCount > 1) {
                 this.multiplyNormals(m, i.halfBondSpacing);
-                let B = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c),
-                    x = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c);
-                s.drawLine(B), s.drawLine(x);
-            } else if (N.sideCount[0] > N.sideCount[1] || N.totalSideCount[0] > N.totalSideCount[1]) {
+                let T = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c),
+                    k = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c);
+                s.drawLine(T), s.drawLine(k);
+            } else if (A.sideCount[0] > A.sideCount[1] || A.totalSideCount[0] > A.totalSideCount[1]) {
                 this.multiplyNormals(m, i.bondSpacing);
-                let B = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c);
-                B.shorten(i.bondLength - i.shortBondLength * i.bondLength), s.drawLine(B), s.drawLine(new Je(u, g, l, c));
-            } else if (N.sideCount[0] < N.sideCount[1] || N.totalSideCount[0] <= N.totalSideCount[1]) {
+                let T = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c);
+                T.shorten(i.bondLength - i.shortBondLength * i.bondLength), s.drawLine(T), s.drawLine(new Je(u, g, l, c));
+            } else if (A.sideCount[0] < A.sideCount[1] || A.totalSideCount[0] <= A.totalSideCount[1]) {
                 this.multiplyNormals(m, i.bondSpacing);
-                let B = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c);
-                B.shorten(i.bondLength - i.shortBondLength * i.bondLength), s.drawLine(B), s.drawLine(new Je(u, g, l, c));
+                let T = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c);
+                T.shorten(i.bondLength - i.shortBondLength * i.bondLength), s.drawLine(T), s.drawLine(new Je(u, g, l, c));
             }
         } else if (a.bondType === "#") {
             m[0].multiplyScalar(i.bondSpacing / 1.5), m[1].multiplyScalar(i.bondSpacing / 1.5);
             let v = new Je($e.add(u, m[0]), $e.add(g, m[0]), l, c),
-                N = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c);
-            s.drawLine(v), s.drawLine(N), s.drawLine(new Je(u, g, l, c));
+                A = new Je($e.add(u, m[1]), $e.add(g, m[1]), l, c);
+            s.drawLine(v), s.drawLine(A), s.drawLine(new Je(u, g, l, c));
         } else if (a.bondType !== ".") {
             let v = n.value.isStereoCenter,
-                N = h.value.isStereoCenter;
-            a.wedge === "up" ? s.drawWedge(new Je(u, g, l, c, v, N)) : a.wedge === "down" ? s.drawDashedWedge(new Je(u, g, l, c, v, N)) : s.drawLine(new Je(u, g, l, c, v, N));
+                A = h.value.isStereoCenter;
+            a.wedge === "up" ? s.drawWedge(new Je(u, g, l, c, v, A)) : a.wedge === "down" ? s.drawDashedWedge(new Je(u, g, l, c, v, A)) : s.drawLine(new Je(u, g, l, c, v, A));
         }
         if (t) {
             let v = $e.midpoint(u, g);
             s.drawDebugText(v.x, v.y, "e: " + e);
         }
     }
     /**
@@ -10627,46 +10627,46 @@
         for (var n = i.vertices.length, n = 0; n < i.vertices.length; n++) {
             let l = i.vertices[n],
                 c = l.value,
                 u = 0,
                 g = 0,
                 m = l.value.bondCount,
                 _ = c.element,
-                v = Ig.maxBonds[_] - m,
-                N = l.getTextDirection(i.vertices, c.hasAttachedPseudoElements),
-                B = r.terminalCarbons || _ !== "C" || c.hasAttachedPseudoElements ? l.isTerminal() : !1,
-                x = c.element === "C";
-            if (i.vertices.length < 3 && (x = !1), c.element === "N" && c.isPartOfAromaticRing && (v = 0), c.bracket && (v = c.bracket.hcount, u = c.bracket.charge, g = c.bracket.isotope), r.atomVisualization === "allballs")
+                v = Fg.maxBonds[_] - m,
+                A = l.getTextDirection(i.vertices, c.hasAttachedPseudoElements),
+                T = r.terminalCarbons || _ !== "C" || c.hasAttachedPseudoElements ? l.isTerminal() : !1,
+                k = c.element === "C";
+            if (i.vertices.length < 3 && (k = !1), c.element === "N" && c.isPartOfAromaticRing && (v = 0), c.bracket && (v = c.bracket.hcount, u = c.bracket.charge, g = c.bracket.isotope), r.atomVisualization === "allballs")
                 a.drawBall(l.position.x, l.position.y, _);
-            else if (c.isDrawn && (!x || c.drawExplicit || B || c.hasAttachedPseudoElements) || i.vertices.length === 1)
+            else if (c.isDrawn && (!k || c.drawExplicit || T || c.hasAttachedPseudoElements) || i.vertices.length === 1)
                 if (r.atomVisualization === "default") {
-                    let L = c.getAttachedPseudoElements();
-                    c.hasAttachedPseudoElements && i.vertices.length === Object.keys(L).length + 1 && (N = "right"), a.drawText(
+                    let x = c.getAttachedPseudoElements();
+                    c.hasAttachedPseudoElements && i.vertices.length === Object.keys(x).length + 1 && (A = "right"), a.drawText(
                         l.position.x,
                         l.position.y,
                         _,
                         v,
-                        N,
-                        B,
+                        A,
+                        T,
                         u,
                         g,
                         i.vertices.length,
-                        L
+                        x
                     );
                 } else
                     r.atomVisualization === "balls" && a.drawBall(l.position.x, l.position.y, _);
             else if (l.getNeighbourCount() === 2 && l.forcePositioned == !0) {
-                let L = i.vertices[l.neighbours[0]].position,
-                    k = i.vertices[l.neighbours[1]].position,
-                    z = $e.threePointangle(l.position, L, k);
-                Math.abs(Math.PI - z) < 0.1 && a.drawPoint(l.position.x, l.position.y, _);
+                let x = i.vertices[l.neighbours[0]].position,
+                    R = i.vertices[l.neighbours[1]].position,
+                    O = $e.threePointangle(l.position, x, R);
+                Math.abs(Math.PI - O) < 0.1 && a.drawPoint(l.position.x, l.position.y, _);
             }
             if (e) {
-                let L = "v: " + l.id + " " + Ia.print(c.ringbonds);
-                a.drawDebugText(l.position.x, l.position.y, L);
+                let x = "v: " + l.id + " " + Fa.print(c.ringbonds);
+                a.drawDebugText(l.position.x, l.position.y, x);
             }
         }
         if (r.debug)
             for (var n = 0; n < s.length; n++) {
                 let l = s[n].center;
                 a.drawDebugPoint(l.x, l.y, "r: " + s[n].id);
             }
@@ -10686,15 +10686,15 @@
             r.push(
                 new $e(
                     a.position.x - this.svgWrapper.minX,
                     a.position.y - this.svgWrapper.minY
                 )
             );
         }
-        let i = new Hg(
+        let i = new qg(
             r,
             e,
             this.svgWrapper.drawingWidth,
             this.svgWrapper.drawingHeight,
             this.opts.weights.sigma,
             this.opts.weights.interval,
             this.opts.weights.colormap,
@@ -10723,24 +10723,24 @@
      * @param {Array} normals list of normals to multiply
      * @param {Number} spacing value to multiply normals by
      */
     multiplyNormals(e, t) {
         e[0].multiplyScalar(t), e[1].multiplyScalar(t);
     }
 };
-var Mi = Wg;
-const qg = Mi;
-let Vg = class {
+var Mi = Vg;
+const Xg = Mi;
+let Yg = class {
     /**
      * The constructor for the class SmilesDrawer.
      *
      * @param {Object} options An object containing custom values for different options. It is merged with the default options.
      */
     constructor(e) {
-        this.svgDrawer = new qg(e);
+        this.svgDrawer = new Xg(e);
     }
     /**
      * Draws the parsed smiles data to a canvas element.
      *
      * @param {Object} data The tree returned by the smiles parser.
      * @param {(String|HTMLCanvasElement)} target The id of the HTML canvas element the structure is drawn to - or the element itself.
      * @param {String} themeName='dark' The name of the theme to use. Built-in themes are 'light' and 'dark'.
@@ -10765,16 +10765,16 @@
      * 
      * @returns {String} The molecular formula.
      */
     getMolecularFormula() {
         this.svgDrawer.getMolecularFormula();
     }
 };
-var Xg = Vg,
-    Zn = function() {
+var Gg = Yg,
+    Qn = function() {
         function d(r, i) {
             function s() {
                 this.constructor = r;
             }
             s.prototype = i.prototype, r.prototype = new s();
         }
 
@@ -10861,429 +10861,429 @@
             if (s !== a)
                 throw Hr("The number of opening parentheses does not match the number of closing parentheses.", 0);
             var n = {},
                 h = {
                     chain: lr
                 },
                 l = lr,
-                c = function(M) {
-                    for (var w = [], $ = [], T = 0; T < M[1].length; T++)
-                        w.push(M[1][T]);
-                    for (var T = 0; T < M[2].length; T++) {
-                        var H = M[2][T][0] ? M[2][T][0] : "-";
+                c = function(B) {
+                    for (var w = [], $ = [], L = 0; L < B[1].length; L++)
+                        w.push(B[1][L]);
+                    for (var L = 0; L < B[2].length; L++) {
+                        var z = B[2][L][0] ? B[2][L][0] : "-";
                         $.push({
-                            bond: H,
-                            id: M[2][T][1]
+                            bond: z,
+                            id: B[2][L][1]
                         });
                     }
-                    for (var T = 0; T < M[3].length; T++)
-                        w.push(M[3][T]);
-                    for (var T = 0; T < M[6].length; T++)
-                        w.push(M[6][T]);
+                    for (var L = 0; L < B[3].length; L++)
+                        w.push(B[3][L]);
+                    for (var L = 0; L < B[6].length; L++)
+                        w.push(B[6][L]);
                     return {
-                        atom: M[0],
-                        isBracket: !!M[0].element,
+                        atom: B[0],
+                        isBracket: !!B[0].element,
                         branches: w,
                         branchCount: w.length,
                         ringbonds: $,
                         ringbondCount: $.length,
-                        bond: M[4] ? M[4] : "-",
-                        next: M[5],
-                        hasNext: !!M[5]
+                        bond: B[4] ? B[4] : "-",
+                        next: B[5],
+                        hasNext: !!B[5]
                     };
                 },
                 u = "(",
                 g = Ne("(", !1),
                 m = ")",
                 _ = Ne(")", !1),
-                v = function(M) {
-                    var w = M[1] ? M[1] : "-";
-                    return M[2].branchBond = w, M[2];
+                v = function(B) {
+                    var w = B[1] ? B[1] : "-";
+                    return B[2].branchBond = w, B[2];
                 },
-                N = function(M) {
-                    return M;
+                A = function(B) {
+                    return B;
                 },
-                B = /^[\-=#$:\/\\.]/,
-                x = ft(["-", "=", "#", "$", ":", "/", "\\", "."], !1, !1),
-                L = function(M) {
-                    return M;
+                T = /^[\-=#$:\/\\.]/,
+                k = ut(["-", "=", "#", "$", ":", "/", "\\", "."], !1, !1),
+                x = function(B) {
+                    return B;
                 },
-                k = "[",
-                z = Ne("[", !1),
+                R = "[",
+                O = Ne("[", !1),
                 D = "se",
-                Y = Ne("se", !1),
-                O = "as",
-                Z = Ne("as", !1),
+                te = Ne("se", !1),
+                q = "as",
+                re = Ne("as", !1),
                 j = "]",
-                q = Ne("]", !1),
-                se = function(M) {
+                X = Ne("]", !1),
+                se = function(B) {
                     return {
-                        isotope: M[1],
-                        element: M[2],
-                        chirality: M[3],
-                        hcount: M[4],
-                        charge: M[5],
-                        class: M[6]
+                        isotope: B[1],
+                        element: B[2],
+                        chirality: B[3],
+                        hcount: B[4],
+                        charge: B[5],
+                        class: B[6]
                     };
                 },
                 ye = "B",
                 ke = Ne("B", !1),
                 xe = "r",
                 we = Ne("r", !1),
                 Ee = "C",
-                Qe = Ne("C", !1),
+                et = Ne("C", !1),
                 Ce = "l",
                 Ae = Ne("l", !1),
                 Be = /^[NOPSFI]/,
-                st = ft(["N", "O", "P", "S", "F", "I"], !1, !1),
-                It = function(M) {
-                    return M.length > 1 ? M.join("") : M;
+                at = ut(["N", "O", "P", "S", "F", "I"], !1, !1),
+                It = function(B) {
+                    return B.length > 1 ? B.join("") : B;
                 },
                 wt = /^[bcnops]/,
-                K = ft(["b", "c", "n", "o", "p", "s"], !1, !1),
+                U = ut(["b", "c", "n", "o", "p", "s"], !1, !1),
                 Ot = "*",
-                J = Ne("*", !1),
-                Te = function(M) {
-                    return M;
+                Z = Ne("*", !1),
+                Te = function(B) {
+                    return B;
                 },
-                et = /^[A-Z]/,
-                Ie = ft([
+                tt = /^[A-Z]/,
+                Ie = ut([
                     ["A", "Z"]
                 ], !1, !1),
                 Ye = /^[a-z]/,
-                Ue = ft([
+                Ue = ut([
                     ["a", "z"]
                 ], !1, !1),
-                Ge = function(M) {
-                    return M.join("");
+                Ge = function(B) {
+                    return B.join("");
                 },
                 De = "%",
                 Ze = Ne("%", !1),
                 He = /^[1-9]/,
-                We = ft([
+                We = ut([
                     ["1", "9"]
                 ], !1, !1),
                 Le = /^[0-9]/,
-                qe = ft([
+                qe = ut([
                     ["0", "9"]
                 ], !1, !1),
-                Lt = function(M) {
-                    return M.length == 1 ? Number(M) : Number(M.join("").replace("%", ""));
+                Mt = function(B) {
+                    return B.length == 1 ? Number(B) : Number(B.join("").replace("%", ""));
                 },
                 yt = "@",
                 Vt = Ne("@", !1),
                 Xt = "TH",
                 Yt = Ne("TH", !1),
                 Ft = /^[12]/,
-                _t = ft(["1", "2"], !1, !1),
+                _t = ut(["1", "2"], !1, !1),
                 zt = "AL",
                 Gt = Ne("AL", !1),
                 Ut = "SP",
                 Zt = Ne("SP", !1),
-                Bi = /^[1-3]/,
-                Di = ft([
+                Pi = /^[1-3]/,
+                $i = ut([
                     ["1", "3"]
                 ], !1, !1),
                 Fr = "TB",
                 Jr = Ne("TB", !1),
                 Qr = "OH",
-                Pi = Ne("OH", !1),
-                ei = function(M) {
-                    return M[1] ? M[1] == "@" ? "@@" : M[1].join("").replace(",", "") : "@";
+                Ii = Ne("OH", !1),
+                ei = function(B) {
+                    return B[1] ? B[1] == "@" ? "@@" : B[1].join("").replace(",", "") : "@";
                 },
-                ti = function(M) {
-                    return M;
+                ti = function(B) {
+                    return B;
                 },
                 ri = "+",
                 ii = Ne("+", !1),
-                $i = function(M) {
-                    return M[1] ? M[1] != "+" ? Number(M[1].join("")) : 2 : 1;
+                Oi = function(B) {
+                    return B[1] ? B[1] != "+" ? Number(B[1].join("")) : 2 : 1;
                 },
                 ni = "-",
                 si = Ne("-", !1),
-                Ii = function(M) {
-                    return M[1] ? M[1] != "-" ? -Number(M[1].join("")) : -2 : -1;
+                Fi = function(B) {
+                    return B[1] ? B[1] != "-" ? -Number(B[1].join("")) : -2 : -1;
                 },
-                Oi = "H",
-                Fi = Ne("H", !1),
-                zi = function(M) {
-                    return M[1] ? Number(M[1]) : 1;
+                zi = "H",
+                Hi = Ne("H", !1),
+                Wi = function(B) {
+                    return B[1] ? Number(B[1]) : 1;
                 },
-                Hi = ":",
-                Wi = Ne(":", !1),
-                qi = /^[0]/,
-                Vi = ft(["0"], !1, !1),
-                ai = function(M) {
-                    return Number(M[1][0] + M[1][1].join(""));
+                qi = ":",
+                Vi = Ne(":", !1),
+                Xi = /^[0]/,
+                Yi = ut(["0"], !1, !1),
+                ai = function(B) {
+                    return Number(B[1][0] + B[1][1].join(""));
                 },
-                li = function(M) {
-                    return Number(M.join(""));
+                li = function(B) {
+                    return Number(B.join(""));
                 },
                 y = 0,
                 vr = [{
                     line: 1,
                     column: 1
                 }],
-                ht = 0,
+                ft = 0,
                 Kt = [],
                 mr;
             if ("startRule" in i) {
                 if (!(i.startRule in h))
                     throw new Error(`Can't start parsing from rule "` + i.startRule + '".');
                 l = h[i.startRule];
             }
 
-            function Ne(M, w) {
+            function Ne(B, w) {
                 return {
                     type: "literal",
-                    text: M,
+                    text: B,
                     ignoreCase: w
                 };
             }
 
-            function ft(M, w, $) {
+            function ut(B, w, $) {
                 return {
                     type: "class",
-                    parts: M,
+                    parts: B,
                     inverted: w,
                     ignoreCase: $
                 };
             }
 
-            function Xi() {
+            function Gi() {
                 return {
                     type: "end"
                 };
             }
 
-            function oi(M) {
-                var w = vr[M],
+            function oi(B) {
+                var w = vr[B],
                     $;
                 if (w)
                     return w;
-                for ($ = M - 1; !vr[$];)
+                for ($ = B - 1; !vr[$];)
                     $--;
                 for (w = vr[$], w = {
                         line: w.line,
                         column: w.column
-                    }; $ < M;)
+                    }; $ < B;)
                     r.charCodeAt($) === 10 ? (w.line++, w.column = 1) : w.column++, $++;
-                return vr[M] = w, w;
+                return vr[B] = w, w;
             }
 
-            function zr(M, w) {
-                var $ = oi(M),
-                    T = oi(w);
+            function zr(B, w) {
+                var $ = oi(B),
+                    L = oi(w);
                 return {
                     start: {
-                        offset: M,
+                        offset: B,
                         line: $.line,
                         column: $.column
                     },
                     end: {
                         offset: w,
-                        line: T.line,
-                        column: T.column
+                        line: L.line,
+                        column: L.column
                     }
                 };
             }
 
-            function Q(M) {
-                y < ht || (y > ht && (ht = y, Kt = []), Kt.push(M));
+            function K(B) {
+                y < ft || (y > ft && (ft = y, Kt = []), Kt.push(B));
             }
 
-            function Hr(M, w) {
-                return new e(M, null, null, w);
+            function Hr(B, w) {
+                return new e(B, null, null, w);
             }
 
-            function Yi(M, w, $) {
+            function Ui(B, w, $) {
                 return new e(
-                    e.buildMessage(M, w),
-                    M,
+                    e.buildMessage(B, w),
+                    B,
                     w,
                     $
                 );
             }
 
             function lr() {
-                var M, w, $, T, H, X, ee, Oe, at, ut;
-                if (M = y, w = y, $ = Gi(), $ !== n) {
-                    for (T = [], H = jt(); H !== n;)
-                        T.push(H), H = jt();
-                    if (T !== n) {
-                        for (H = [], X = y, ee = or(), ee === n && (ee = null), ee !== n ? (Oe = ui(), Oe !== n ? (ee = [ee, Oe], X = ee) : (y = X, X = n)) : (y = X, X = n); X !== n;)
-                            H.push(X), X = y, ee = or(), ee === n && (ee = null), ee !== n ? (Oe = ui(), Oe !== n ? (ee = [ee, Oe], X = ee) : (y = X, X = n)) : (y = X, X = n);
-                        if (H !== n) {
-                            for (X = [], ee = jt(); ee !== n;)
-                                X.push(ee), ee = jt();
-                            if (X !== n)
-                                if (ee = or(), ee === n && (ee = null), ee !== n)
+                var B, w, $, L, z, V, J, Oe, lt, ct;
+                if (B = y, w = y, $ = Zi(), $ !== n) {
+                    for (L = [], z = jt(); z !== n;)
+                        L.push(z), z = jt();
+                    if (L !== n) {
+                        for (z = [], V = y, J = or(), J === n && (J = null), J !== n ? (Oe = ui(), Oe !== n ? (J = [J, Oe], V = J) : (y = V, V = n)) : (y = V, V = n); V !== n;)
+                            z.push(V), V = y, J = or(), J === n && (J = null), J !== n ? (Oe = ui(), Oe !== n ? (J = [J, Oe], V = J) : (y = V, V = n)) : (y = V, V = n);
+                        if (z !== n) {
+                            for (V = [], J = jt(); J !== n;)
+                                V.push(J), J = jt();
+                            if (V !== n)
+                                if (J = or(), J === n && (J = null), J !== n)
                                     if (Oe = lr(), Oe === n && (Oe = null), Oe !== n) {
-                                        for (at = [], ut = jt(); ut !== n;)
-                                            at.push(ut), ut = jt();
-                                        at !== n ? ($ = [$, T, H, X, ee, Oe, at], w = $) : (y = w, w = n);
+                                        for (lt = [], ct = jt(); ct !== n;)
+                                            lt.push(ct), ct = jt();
+                                        lt !== n ? ($ = [$, L, z, V, J, Oe, lt], w = $) : (y = w, w = n);
                                     } else
                                         y = w, w = n;
                             else
                                 y = w, w = n;
                             else
                                 y = w, w = n;
                         } else
                             y = w, w = n;
                     } else
                         y = w, w = n;
                 } else
                     y = w, w = n;
-                return w !== n && (w = c(w)), M = w, M;
+                return w !== n && (w = c(w)), B = w, B;
             }
 
             function jt() {
-                var M, w, $, T, H, X;
-                return M = y, w = y, r.charCodeAt(y) === 40 ? ($ = u, y++) : ($ = n, Q(g)), $ !== n ? (T = or(), T === n && (T = null), T !== n ? (H = lr(), H !== n ? (r.charCodeAt(y) === 41 ? (X = m, y++) : (X = n, Q(_)), X !== n ? ($ = [$, T, H, X], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = v(w)), M = w, M;
+                var B, w, $, L, z, V;
+                return B = y, w = y, r.charCodeAt(y) === 40 ? ($ = u, y++) : ($ = n, K(g)), $ !== n ? (L = or(), L === n && (L = null), L !== n ? (z = lr(), z !== n ? (r.charCodeAt(y) === 41 ? (V = m, y++) : (V = n, K(_)), V !== n ? ($ = [$, L, z, V], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = v(w)), B = w, B;
             }
 
-            function Gi() {
-                var M, w;
-                return M = y, w = Zi(), w === n && (w = hi(), w === n && (w = Ui(), w === n && (w = fi()))), w !== n && (w = N(w)), M = w, M;
+            function Zi() {
+                var B, w;
+                return B = y, w = ji(), w === n && (w = hi(), w === n && (w = Ki(), w === n && (w = fi()))), w !== n && (w = A(w)), B = w, B;
             }
 
             function or() {
-                var M, w;
-                if (M = y, B.test(r.charAt(y))) {
+                var B, w;
+                if (B = y, T.test(r.charAt(y))) {
                     if (w = r.charAt(y), w === r.charAt(y + 1))
                         throw w = n, Hr("The parser encountered a bond repetition.", y + 1);
                     y++;
                 } else
-                    w = n, Q(x);
-                return w !== n && (w = L(w)), M = w, M;
+                    w = n, K(k);
+                return w !== n && (w = x(w)), B = w, B;
             }
 
-            function Ui() {
-                var M, w, $, T, H, X, ee, Oe, at, ut;
-                return M = y, w = y, r.charCodeAt(y) === 91 ? ($ = k, y++) : ($ = n, Q(z)), $ !== n ? (T = Qi(), T === n && (T = null), T !== n ? (r.substr(y, 2) === D ? (H = D, y += 2) : (H = n, Q(Y)), H === n && (r.substr(y, 2) === O ? (H = O, y += 2) : (H = n, Q(Z)), H === n && (H = hi(), H === n && (H = Ki(), H === n && (H = fi())))), H !== n ? (X = Wr(), X === n && (X = null), X !== n ? (ee = ji(), ee === n && (ee = null), ee !== n ? (Oe = Jt(), Oe === n && (Oe = null), Oe !== n ? (at = Ji(), at === n && (at = null), at !== n ? (r.charCodeAt(y) === 93 ? (ut = j, y++) : (ut = n, Q(q)), ut !== n ? ($ = [$, T, H, X, ee, Oe, at, ut], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = se(w)), M = w, M;
+            function Ki() {
+                var B, w, $, L, z, V, J, Oe, lt, ct;
+                return B = y, w = y, r.charCodeAt(y) === 91 ? ($ = R, y++) : ($ = n, K(O)), $ !== n ? (L = tn(), L === n && (L = null), L !== n ? (r.substr(y, 2) === D ? (z = D, y += 2) : (z = n, K(te)), z === n && (r.substr(y, 2) === q ? (z = q, y += 2) : (z = n, K(re)), z === n && (z = hi(), z === n && (z = Ji(), z === n && (z = fi())))), z !== n ? (V = Wr(), V === n && (V = null), V !== n ? (J = Qi(), J === n && (J = null), J !== n ? (Oe = Jt(), Oe === n && (Oe = null), Oe !== n ? (lt = en(), lt === n && (lt = null), lt !== n ? (r.charCodeAt(y) === 93 ? (ct = j, y++) : (ct = n, K(X)), ct !== n ? ($ = [$, L, z, V, J, Oe, lt, ct], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = se(w)), B = w, B;
             }
 
-            function Zi() {
-                var M, w, $, T;
-                return M = y, w = y, r.charCodeAt(y) === 66 ? ($ = ye, y++) : ($ = n, Q(ke)), $ !== n ? (r.charCodeAt(y) === 114 ? (T = xe, y++) : (T = n, Q(we)), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w === n && (w = y, r.charCodeAt(y) === 67 ? ($ = Ee, y++) : ($ = n, Q(Qe)), $ !== n ? (r.charCodeAt(y) === 108 ? (T = Ce, y++) : (T = n, Q(Ae)), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w === n && (Be.test(r.charAt(y)) ? (w = r.charAt(y), y++) : (w = n, Q(st)))), w !== n && (w = It(w)), M = w, M;
+            function ji() {
+                var B, w, $, L;
+                return B = y, w = y, r.charCodeAt(y) === 66 ? ($ = ye, y++) : ($ = n, K(ke)), $ !== n ? (r.charCodeAt(y) === 114 ? (L = xe, y++) : (L = n, K(we)), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w === n && (w = y, r.charCodeAt(y) === 67 ? ($ = Ee, y++) : ($ = n, K(et)), $ !== n ? (r.charCodeAt(y) === 108 ? (L = Ce, y++) : (L = n, K(Ae)), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w === n && (Be.test(r.charAt(y)) ? (w = r.charAt(y), y++) : (w = n, K(at)))), w !== n && (w = It(w)), B = w, B;
             }
 
             function hi() {
-                var M, w;
-                return M = y, wt.test(r.charAt(y)) ? (w = r.charAt(y), y++) : (w = n, Q(K)), w !== n && (w = N(w)), M = w, M;
+                var B, w;
+                return B = y, wt.test(r.charAt(y)) ? (w = r.charAt(y), y++) : (w = n, K(U)), w !== n && (w = A(w)), B = w, B;
             }
 
             function fi() {
-                var M, w;
-                return M = y, r.charCodeAt(y) === 42 ? (w = Ot, y++) : (w = n, Q(J)), w !== n && (w = Te(w)), M = w, M;
+                var B, w;
+                return B = y, r.charCodeAt(y) === 42 ? (w = Ot, y++) : (w = n, K(Z)), w !== n && (w = Te(w)), B = w, B;
             }
 
-            function Ki() {
-                var M, w, $, T;
-                return M = y, w = y, et.test(r.charAt(y)) ? ($ = r.charAt(y), y++) : ($ = n, Q(Ie)), $ !== n ? (Ye.test(r.charAt(y)) ? (T = r.charAt(y), y++) : (T = n, Q(Ue)), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = Ge(w)), M = w, M;
+            function Ji() {
+                var B, w, $, L;
+                return B = y, w = y, tt.test(r.charAt(y)) ? ($ = r.charAt(y), y++) : ($ = n, K(Ie)), $ !== n ? (Ye.test(r.charAt(y)) ? (L = r.charAt(y), y++) : (L = n, K(Ue)), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = Ge(w)), B = w, B;
             }
 
             function ui() {
-                var M, w, $, T, H;
-                return M = y, w = y, r.charCodeAt(y) === 37 ? ($ = De, y++) : ($ = n, Q(Ze)), $ !== n ? (He.test(r.charAt(y)) ? (T = r.charAt(y), y++) : (T = n, Q(We)), T !== n ? (Le.test(r.charAt(y)) ? (H = r.charAt(y), y++) : (H = n, Q(qe)), H !== n ? ($ = [$, T, H], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w === n && (Le.test(r.charAt(y)) ? (w = r.charAt(y), y++) : (w = n, Q(qe))), w !== n && (w = Lt(w)), M = w, M;
+                var B, w, $, L, z;
+                return B = y, w = y, r.charCodeAt(y) === 37 ? ($ = De, y++) : ($ = n, K(Ze)), $ !== n ? (He.test(r.charAt(y)) ? (L = r.charAt(y), y++) : (L = n, K(We)), L !== n ? (Le.test(r.charAt(y)) ? (z = r.charAt(y), y++) : (z = n, K(qe)), z !== n ? ($ = [$, L, z], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w === n && (Le.test(r.charAt(y)) ? (w = r.charAt(y), y++) : (w = n, K(qe))), w !== n && (w = Mt(w)), B = w, B;
             }
 
             function Wr() {
-                var M, w, $, T, H, X, ee;
-                return M = y, w = y, r.charCodeAt(y) === 64 ? ($ = yt, y++) : ($ = n, Q(Vt)), $ !== n ? (r.charCodeAt(y) === 64 ? (T = yt, y++) : (T = n, Q(Vt)), T === n && (T = y, r.substr(y, 2) === Xt ? (H = Xt, y += 2) : (H = n, Q(Yt)), H !== n ? (Ft.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(_t)), X !== n ? (H = [H, X], T = H) : (y = T, T = n)) : (y = T, T = n), T === n && (T = y, r.substr(y, 2) === zt ? (H = zt, y += 2) : (H = n, Q(Gt)), H !== n ? (Ft.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(_t)), X !== n ? (H = [H, X], T = H) : (y = T, T = n)) : (y = T, T = n), T === n && (T = y, r.substr(y, 2) === Ut ? (H = Ut, y += 2) : (H = n, Q(Zt)), H !== n ? (Bi.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(Di)), X !== n ? (H = [H, X], T = H) : (y = T, T = n)) : (y = T, T = n), T === n && (T = y, r.substr(y, 2) === Fr ? (H = Fr, y += 2) : (H = n, Q(Jr)), H !== n ? (He.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(We)), X !== n ? (Le.test(r.charAt(y)) ? (ee = r.charAt(y), y++) : (ee = n, Q(qe)), ee === n && (ee = null), ee !== n ? (H = [H, X, ee], T = H) : (y = T, T = n)) : (y = T, T = n)) : (y = T, T = n), T === n && (T = y, r.substr(y, 2) === Qr ? (H = Qr, y += 2) : (H = n, Q(Pi)), H !== n ? (He.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(We)), X !== n ? (Le.test(r.charAt(y)) ? (ee = r.charAt(y), y++) : (ee = n, Q(qe)), ee === n && (ee = null), ee !== n ? (H = [H, X, ee], T = H) : (y = T, T = n)) : (y = T, T = n)) : (y = T, T = n)))))), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = ei(w)), M = w, M;
+                var B, w, $, L, z, V, J;
+                return B = y, w = y, r.charCodeAt(y) === 64 ? ($ = yt, y++) : ($ = n, K(Vt)), $ !== n ? (r.charCodeAt(y) === 64 ? (L = yt, y++) : (L = n, K(Vt)), L === n && (L = y, r.substr(y, 2) === Xt ? (z = Xt, y += 2) : (z = n, K(Yt)), z !== n ? (Ft.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K(_t)), V !== n ? (z = [z, V], L = z) : (y = L, L = n)) : (y = L, L = n), L === n && (L = y, r.substr(y, 2) === zt ? (z = zt, y += 2) : (z = n, K(Gt)), z !== n ? (Ft.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K(_t)), V !== n ? (z = [z, V], L = z) : (y = L, L = n)) : (y = L, L = n), L === n && (L = y, r.substr(y, 2) === Ut ? (z = Ut, y += 2) : (z = n, K(Zt)), z !== n ? (Pi.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K($i)), V !== n ? (z = [z, V], L = z) : (y = L, L = n)) : (y = L, L = n), L === n && (L = y, r.substr(y, 2) === Fr ? (z = Fr, y += 2) : (z = n, K(Jr)), z !== n ? (He.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K(We)), V !== n ? (Le.test(r.charAt(y)) ? (J = r.charAt(y), y++) : (J = n, K(qe)), J === n && (J = null), J !== n ? (z = [z, V, J], L = z) : (y = L, L = n)) : (y = L, L = n)) : (y = L, L = n), L === n && (L = y, r.substr(y, 2) === Qr ? (z = Qr, y += 2) : (z = n, K(Ii)), z !== n ? (He.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K(We)), V !== n ? (Le.test(r.charAt(y)) ? (J = r.charAt(y), y++) : (J = n, K(qe)), J === n && (J = null), J !== n ? (z = [z, V, J], L = z) : (y = L, L = n)) : (y = L, L = n)) : (y = L, L = n)))))), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = ei(w)), B = w, B;
             }
 
             function Jt() {
-                var M, w;
-                return M = y, w = qr(), w === n && (w = Qt()), w !== n && (w = ti(w)), M = w, M;
+                var B, w;
+                return B = y, w = qr(), w === n && (w = Qt()), w !== n && (w = ti(w)), B = w, B;
             }
 
             function qr() {
-                var M, w, $, T, H, X;
-                return M = y, w = y, r.charCodeAt(y) === 43 ? ($ = ri, y++) : ($ = n, Q(ii)), $ !== n ? (r.charCodeAt(y) === 43 ? (T = ri, y++) : (T = n, Q(ii)), T === n && (T = y, He.test(r.charAt(y)) ? (H = r.charAt(y), y++) : (H = n, Q(We)), H !== n ? (Le.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(qe)), X === n && (X = null), X !== n ? (H = [H, X], T = H) : (y = T, T = n)) : (y = T, T = n)), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = $i(w)), M = w, M;
+                var B, w, $, L, z, V;
+                return B = y, w = y, r.charCodeAt(y) === 43 ? ($ = ri, y++) : ($ = n, K(ii)), $ !== n ? (r.charCodeAt(y) === 43 ? (L = ri, y++) : (L = n, K(ii)), L === n && (L = y, He.test(r.charAt(y)) ? (z = r.charAt(y), y++) : (z = n, K(We)), z !== n ? (Le.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K(qe)), V === n && (V = null), V !== n ? (z = [z, V], L = z) : (y = L, L = n)) : (y = L, L = n)), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = Oi(w)), B = w, B;
             }
 
             function Qt() {
-                var M, w, $, T, H, X;
-                return M = y, w = y, r.charCodeAt(y) === 45 ? ($ = ni, y++) : ($ = n, Q(si)), $ !== n ? (r.charCodeAt(y) === 45 ? (T = ni, y++) : (T = n, Q(si)), T === n && (T = y, He.test(r.charAt(y)) ? (H = r.charAt(y), y++) : (H = n, Q(We)), H !== n ? (Le.test(r.charAt(y)) ? (X = r.charAt(y), y++) : (X = n, Q(qe)), X === n && (X = null), X !== n ? (H = [H, X], T = H) : (y = T, T = n)) : (y = T, T = n)), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = Ii(w)), M = w, M;
+                var B, w, $, L, z, V;
+                return B = y, w = y, r.charCodeAt(y) === 45 ? ($ = ni, y++) : ($ = n, K(si)), $ !== n ? (r.charCodeAt(y) === 45 ? (L = ni, y++) : (L = n, K(si)), L === n && (L = y, He.test(r.charAt(y)) ? (z = r.charAt(y), y++) : (z = n, K(We)), z !== n ? (Le.test(r.charAt(y)) ? (V = r.charAt(y), y++) : (V = n, K(qe)), V === n && (V = null), V !== n ? (z = [z, V], L = z) : (y = L, L = n)) : (y = L, L = n)), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = Fi(w)), B = w, B;
             }
 
-            function ji() {
-                var M, w, $, T;
-                return M = y, w = y, r.charCodeAt(y) === 72 ? ($ = Oi, y++) : ($ = n, Q(Fi)), $ !== n ? (Le.test(r.charAt(y)) ? (T = r.charAt(y), y++) : (T = n, Q(qe)), T === n && (T = null), T !== n ? ($ = [$, T], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = zi(w)), M = w, M;
+            function Qi() {
+                var B, w, $, L;
+                return B = y, w = y, r.charCodeAt(y) === 72 ? ($ = zi, y++) : ($ = n, K(Hi)), $ !== n ? (Le.test(r.charAt(y)) ? (L = r.charAt(y), y++) : (L = n, K(qe)), L === n && (L = null), L !== n ? ($ = [$, L], w = $) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = Wi(w)), B = w, B;
             }
 
-            function Ji() {
-                var M, w, $, T, H, X, ee;
-                if (M = y, w = y, r.charCodeAt(y) === 58 ? ($ = Hi, y++) : ($ = n, Q(Wi)), $ !== n) {
-                    if (T = y, He.test(r.charAt(y)) ? (H = r.charAt(y), y++) : (H = n, Q(We)), H !== n) {
-                        for (X = [], Le.test(r.charAt(y)) ? (ee = r.charAt(y), y++) : (ee = n, Q(qe)); ee !== n;)
-                            X.push(ee), Le.test(r.charAt(y)) ? (ee = r.charAt(y), y++) : (ee = n, Q(qe));
-                        X !== n ? (H = [H, X], T = H) : (y = T, T = n);
+            function en() {
+                var B, w, $, L, z, V, J;
+                if (B = y, w = y, r.charCodeAt(y) === 58 ? ($ = qi, y++) : ($ = n, K(Vi)), $ !== n) {
+                    if (L = y, He.test(r.charAt(y)) ? (z = r.charAt(y), y++) : (z = n, K(We)), z !== n) {
+                        for (V = [], Le.test(r.charAt(y)) ? (J = r.charAt(y), y++) : (J = n, K(qe)); J !== n;)
+                            V.push(J), Le.test(r.charAt(y)) ? (J = r.charAt(y), y++) : (J = n, K(qe));
+                        V !== n ? (z = [z, V], L = z) : (y = L, L = n);
                     } else
-                        y = T, T = n;
-                    T === n && (qi.test(r.charAt(y)) ? (T = r.charAt(y), y++) : (T = n, Q(Vi))), T !== n ? ($ = [$, T], w = $) : (y = w, w = n);
+                        y = L, L = n;
+                    L === n && (Xi.test(r.charAt(y)) ? (L = r.charAt(y), y++) : (L = n, K(Yi))), L !== n ? ($ = [$, L], w = $) : (y = w, w = n);
                 } else
                     y = w, w = n;
-                return w !== n && (w = ai(w)), M = w, M;
+                return w !== n && (w = ai(w)), B = w, B;
             }
 
-            function Qi() {
-                var M, w, $, T, H;
-                return M = y, w = y, He.test(r.charAt(y)) ? ($ = r.charAt(y), y++) : ($ = n, Q(We)), $ !== n ? (Le.test(r.charAt(y)) ? (T = r.charAt(y), y++) : (T = n, Q(qe)), T === n && (T = null), T !== n ? (Le.test(r.charAt(y)) ? (H = r.charAt(y), y++) : (H = n, Q(qe)), H === n && (H = null), H !== n ? ($ = [$, T, H], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = li(w)), M = w, M;
+            function tn() {
+                var B, w, $, L, z;
+                return B = y, w = y, He.test(r.charAt(y)) ? ($ = r.charAt(y), y++) : ($ = n, K(We)), $ !== n ? (Le.test(r.charAt(y)) ? (L = r.charAt(y), y++) : (L = n, K(qe)), L === n && (L = null), L !== n ? (Le.test(r.charAt(y)) ? (z = r.charAt(y), y++) : (z = n, K(qe)), z === n && (z = null), z !== n ? ($ = [$, L, z], w = $) : (y = w, w = n)) : (y = w, w = n)) : (y = w, w = n), w !== n && (w = li(w)), B = w, B;
             }
             if (mr = l(), mr !== n && y === r.length)
                 return mr;
-            throw mr !== n && y < r.length && Q(Xi()), Yi(
+            throw mr !== n && y < r.length && K(Gi()), Ui(
                 Kt,
-                ht < r.length ? r.charAt(ht) : null,
-                ht < r.length ? zr(ht, ht + 1) : zr(ht, ht)
+                ft < r.length ? r.charAt(ft) : null,
+                ft < r.length ? zr(ft, ft + 1) : zr(ft, ft)
             );
         }
         return {
             SyntaxError: e,
             parse: t
         };
     }();
-const Dn = Zn;
-let Yg = class {
+const $n = Qn;
+let Ug = class {
     /**
      * The constructor for the class Reaction.
      *
      * @param {string} reactionSmiles A reaction SMILES.
      */
     constructor(e) {
         this.reactantsSmiles = [], this.reagentsSmiles = [], this.productsSmiles = [], this.reactantsWeights = [], this.reagentsWeights = [], this.productsWeights = [], this.reactants = [], this.reagents = [], this.products = [];
         let t = e.split(">");
         if (t.length !== 3)
             throw new Error("Invalid reaction SMILES. Did you add fewer than or more than two '>'?");
         t[0] !== "" && (this.reactantsSmiles = t[0].split(".")), t[1] !== "" && (this.reagentsSmiles = t[1].split(".")), t[2] !== "" && (this.productsSmiles = t[2].split("."));
         for (var r = 0; r < this.reactantsSmiles.length; r++)
-            this.reactants.push(Dn.parse(this.reactantsSmiles[r]));
+            this.reactants.push($n.parse(this.reactantsSmiles[r]));
         for (var r = 0; r < this.reagentsSmiles.length; r++)
-            this.reagents.push(Dn.parse(this.reagentsSmiles[r]));
+            this.reagents.push($n.parse(this.reagentsSmiles[r]));
         for (var r = 0; r < this.productsSmiles.length; r++)
-            this.products.push(Dn.parse(this.productsSmiles[r]));
+            this.products.push($n.parse(this.productsSmiles[r]));
     }
 };
-var Gg = Yg;
-const Ug = Gg;
-let Zg = class {
+var Zg = Ug;
+const Kg = Zg;
+let jg = class {
     /**
      * Returns the hex code of a color associated with a key from the current theme.
      *
      * @param {String} reactionSmiles A reaction SMILES.
      * @returns {Reaction} A reaction object.
      */
     static parse(e) {
-        return new Ug(e);
+        return new Kg(e);
     }
 };
-var wl = Zg;
-const Kg = {
+var yl = jg;
+const Jg = {
     C2H4O2: "acetic acid",
     C3H6O: "acetone",
     C2H3N: "acetonitrile",
     C6H6: "benzene",
     CCl4: "carbon tetrachloride",
     C6H5Cl: "chlorobenzene",
     CHCl3: "chloroform",
@@ -11308,21 +11308,21 @@
     CH3NO2: "nitromethane",
     C5H12: "pentane",
     C5H5N: "pyridine",
     C7H8: "toluene",
     C6H15N: "triethyl amine",
     H2O: "water"
 };
-var jg = Kg;
-const Jg = Mi,
-    Pn = Un,
-    Qg = Gn,
-    e0 = Yn,
-    Oa = jg;
-let t0 = class {
+var Qg = Jg;
+const e0 = Mi,
+    In = Jn,
+    t0 = jn,
+    r0 = Kn,
+    za = Qg;
+let i0 = class {
     /**
      * The constructor for the class ReactionDrawer.
      *
      * @param {Object} options An object containing reaction drawing specitic options.
      * @param {Object} moleculeOptions An object containing molecule drawing specific options.
      */
     constructor(e, t) {
@@ -11340,15 +11340,15 @@
                 headSize: 6,
                 thickness: 1,
                 margin: 3
             },
             weights: {
                 normalize: !1
             }
-        }, this.opts = Qg.extend(!0, this.defaultOptions, e), this.drawer = new Jg(t), this.molOpts = this.drawer.opts;
+        }, this.opts = t0.extend(!0, this.defaultOptions, e), this.drawer = new e0(t), this.molOpts = this.drawer.opts;
     }
     /**
      * Draws the parsed reaction smiles data to a canvas element.
      *
      * @param {Object} reaction The reaction object returned by the reaction smiles parser.
      * @param {(String|SVGElement)} target The id of the HTML canvas element the structure is drawn to - or the element itself.
      * @param {String} themeName='dark' The name of the theme to use. Built-in themes are 'light' and 'dark'.
@@ -11357,78 +11357,78 @@
      * @param {String} textBelow='' The text below the arrow.
      * @param {?Object} weights=null The weights for reactants, agents, and products.
      * @param {Boolean} infoOnly=false Only output info on the molecule without drawing anything to the canvas.
      * 
      * @returns {SVGElement} The svg element
      */
     draw(e, t, r = "light", i = null, s = "{reagents}", a = "", n = !1) {
-        if (this.themeManager = new e0(this.molOpts.themes, r), this.opts.weights.normalize) {
-            let B = -Number.MAX_SAFE_INTEGER,
-                x = Number.MAX_SAFE_INTEGER;
+        if (this.themeManager = new r0(this.molOpts.themes, r), this.opts.weights.normalize) {
+            let T = -Number.MAX_SAFE_INTEGER,
+                k = Number.MAX_SAFE_INTEGER;
             if (i.hasOwnProperty("reactants"))
-                for (let k = 0; k < i.reactants.length; k++)
-                    for (let z = 0; z < i.reactants[k].length; z++)
-                        i.reactants[k][z] < x && (x = i.reactants[k][z]), i.reactants[k][z] > B && (B = i.reactants[k][z]);
+                for (let R = 0; R < i.reactants.length; R++)
+                    for (let O = 0; O < i.reactants[R].length; O++)
+                        i.reactants[R][O] < k && (k = i.reactants[R][O]), i.reactants[R][O] > T && (T = i.reactants[R][O]);
             if (i.hasOwnProperty("reagents"))
-                for (let k = 0; k < i.reagents.length; k++)
-                    for (let z = 0; z < i.reagents[k].length; z++)
-                        i.reagents[k][z] < x && (x = i.reagents[k][z]), i.reagents[k][z] > B && (B = i.reagents[k][z]);
+                for (let R = 0; R < i.reagents.length; R++)
+                    for (let O = 0; O < i.reagents[R].length; O++)
+                        i.reagents[R][O] < k && (k = i.reagents[R][O]), i.reagents[R][O] > T && (T = i.reagents[R][O]);
             if (i.hasOwnProperty("products"))
-                for (let k = 0; k < i.products.length; k++)
-                    for (let z = 0; z < i.products[k].length; z++)
-                        i.products[k][z] < x && (x = i.products[k][z]), i.products[k][z] > B && (B = i.products[k][z]);
-            let L = Math.max(Math.abs(x), Math.abs(B));
-            if (L === 0 && (L = 1), i.hasOwnProperty("reactants"))
-                for (let k = 0; k < i.reactants.length; k++)
-                    for (let z = 0; z < i.reactants[k].length; z++)
-                        i.reactants[k][z] /= L;
+                for (let R = 0; R < i.products.length; R++)
+                    for (let O = 0; O < i.products[R].length; O++)
+                        i.products[R][O] < k && (k = i.products[R][O]), i.products[R][O] > T && (T = i.products[R][O]);
+            let x = Math.max(Math.abs(k), Math.abs(T));
+            if (x === 0 && (x = 1), i.hasOwnProperty("reactants"))
+                for (let R = 0; R < i.reactants.length; R++)
+                    for (let O = 0; O < i.reactants[R].length; O++)
+                        i.reactants[R][O] /= x;
             if (i.hasOwnProperty("reagents"))
-                for (let k = 0; k < i.reagents.length; k++)
-                    for (let z = 0; z < i.reagents[k].length; z++)
-                        i.reagents[k][z] /= L;
+                for (let R = 0; R < i.reagents.length; R++)
+                    for (let O = 0; O < i.reagents[R].length; O++)
+                        i.reagents[R][O] /= x;
             if (i.hasOwnProperty("products"))
-                for (let k = 0; k < i.products.length; k++)
-                    for (let z = 0; z < i.products[k].length; z++)
-                        i.products[k][z] /= L;
+                for (let R = 0; R < i.products.length; R++)
+                    for (let O = 0; O < i.products[R].length; O++)
+                        i.products[R][O] /= x;
         }
         let h = null;
         for (t === null || t === "svg" ? (h = document.createElementNS("http://www.w3.org/2000/svg", "svg"), h.setAttribute("xmlns", "http://www.w3.org/2000/svg"), h.setAttributeNS(null, "width", "500"), h.setAttributeNS(null, "height", "500")) : typeof t == "string" || t instanceof String ? h = document.getElementById(t) : h = t; h.firstChild;)
             h.removeChild(h.firstChild);
         let l = [],
             c = 0;
         for (var u = 0; u < e.reactants.length; u++) {
             u > 0 && l.push({
                 width: this.opts.plus.size * this.opts.scale,
                 height: this.opts.plus.size * this.opts.scale,
                 svg: this.getPlus()
             });
-            let B = null;
-            i && i.hasOwnProperty("reactants") && i.reactants.length > u && (B = i.reactants[u]);
-            let x = document.createElementNS("http://www.w3.org/2000/svg", "svg");
-            this.drawer.draw(e.reactants[u], x, r, B, n, [], this.opts.weights.normalize);
-            let L = {
-                width: x.viewBox.baseVal.width * this.opts.scale,
-                height: x.viewBox.baseVal.height * this.opts.scale,
-                svg: x
+            let T = null;
+            i && i.hasOwnProperty("reactants") && i.reactants.length > u && (T = i.reactants[u]);
+            let k = document.createElementNS("http://www.w3.org/2000/svg", "svg");
+            this.drawer.draw(e.reactants[u], k, r, T, n, [], this.opts.weights.normalize);
+            let x = {
+                width: k.viewBox.baseVal.width * this.opts.scale,
+                height: k.viewBox.baseVal.height * this.opts.scale,
+                svg: k
             };
-            l.push(L), L.height > c && (c = L.height);
+            l.push(x), x.height > c && (c = x.height);
         }
         l.push({
             width: this.opts.arrow.length * this.opts.scale,
             height: this.opts.arrow.headSize * 2 * this.opts.scale,
             svg: this.getArrow()
         });
         let g = "";
         for (var u = 0; u < e.reagents.length; u++) {
             u > 0 && (g += ", ");
-            let x = this.drawer.getMolecularFormula(e.reagents[u]);
-            x in Oa && (x = Oa[x]), g += Pn.replaceNumbersWithSubscript(x);
+            let k = this.drawer.getMolecularFormula(e.reagents[u]);
+            k in za && (k = za[k]), g += In.replaceNumbersWithSubscript(k);
         }
         s = s.replace("{reagents}", g);
-        const m = Pn.writeText(
+        const m = In.writeText(
             s,
             this.themeManager,
             this.opts.fontSize * this.opts.scale,
             this.opts.fontFamily,
             this.opts.arrow.length * this.opts.scale
         );
         let _ = (this.opts.arrow.length * this.opts.scale - m.width) / 2;
@@ -11436,15 +11436,15 @@
             svg: m.svg,
             height: m.height,
             width: this.opts.arrow.length * this.opts.scale,
             offsetX: -(this.opts.arrow.length * this.opts.scale + this.opts.spacing) + _,
             offsetY: -(m.height / 2) - this.opts.arrow.margin,
             position: "relative"
         });
-        const v = Pn.writeText(
+        const v = In.writeText(
             a,
             this.themeManager,
             this.opts.fontSize * this.opts.scale,
             this.opts.fontFamily,
             this.opts.arrow.length * this.opts.scale
         );
         _ = (this.opts.arrow.length * this.opts.scale - v.width) / 2, l.push({
@@ -11457,31 +11457,31 @@
         });
         for (var u = 0; u < e.products.length; u++) {
             u > 0 && l.push({
                 width: this.opts.plus.size * this.opts.scale,
                 height: this.opts.plus.size * this.opts.scale,
                 svg: this.getPlus()
             });
-            let x = null;
-            i && i.hasOwnProperty("products") && i.products.length > u && (x = i.products[u]);
-            let L = document.createElementNS("http://www.w3.org/2000/svg", "svg");
-            this.drawer.draw(e.products[u], L, r, x, n, [], this.opts.weights.normalize);
-            let k = {
-                width: L.viewBox.baseVal.width * this.opts.scale,
-                height: L.viewBox.baseVal.height * this.opts.scale,
-                svg: L
+            let k = null;
+            i && i.hasOwnProperty("products") && i.products.length > u && (k = i.products[u]);
+            let x = document.createElementNS("http://www.w3.org/2000/svg", "svg");
+            this.drawer.draw(e.products[u], x, r, k, n, [], this.opts.weights.normalize);
+            let R = {
+                width: x.viewBox.baseVal.width * this.opts.scale,
+                height: x.viewBox.baseVal.height * this.opts.scale,
+                svg: x
             };
-            l.push(k), k.height > c && (c = k.height);
+            l.push(R), R.height > c && (c = R.height);
         }
-        let N = 0;
-        return l.forEach((B) => {
-            let x = B.offsetX ?? 0,
-                L = B.offsetY ?? 0;
-            B.svg.setAttributeNS(null, "x", Math.round(N + x)), B.svg.setAttributeNS(null, "y", Math.round((c - B.height) / 2 + L)), B.svg.setAttributeNS(null, "width", Math.round(B.width)), B.svg.setAttributeNS(null, "height", Math.round(B.height)), h.appendChild(B.svg), B.position !== "relative" && (N += Math.round(B.width + this.opts.spacing + x));
-        }), h.setAttributeNS(null, "viewBox", `0 0 ${N} ${c}`), h.style.width = N + "px", h.style.height = c + "px", h;
+        let A = 0;
+        return l.forEach((T) => {
+            let k = T.offsetX ?? 0,
+                x = T.offsetY ?? 0;
+            T.svg.setAttributeNS(null, "x", Math.round(A + k)), T.svg.setAttributeNS(null, "y", Math.round((c - T.height) / 2 + x)), T.svg.setAttributeNS(null, "width", Math.round(T.width)), T.svg.setAttributeNS(null, "height", Math.round(T.height)), h.appendChild(T.svg), T.position !== "relative" && (A += Math.round(T.width + this.opts.spacing + k));
+        }), h.setAttributeNS(null, "viewBox", `0 0 ${A} ${c}`), h.style.width = A + "px", h.style.height = c + "px", h;
     }
     getPlus() {
         let e = this.opts.plus.size,
             t = this.opts.plus.thickness,
             r = document.createElementNS("http://www.w3.org/2000/svg", "svg"),
             i = document.createElementNS("http://www.w3.org/2000/svg", "rect"),
             s = document.createElementNS("http://www.w3.org/2000/svg", "rect");
@@ -11505,27 +11505,27 @@
             t = this.opts.arrow.length,
             r = document.createElementNS("http://www.w3.org/2000/svg", "svg"),
             i = document.createElementNS("http://www.w3.org/2000/svg", "defs"),
             s = document.createElementNS("http://www.w3.org/2000/svg", "line");
         return i.appendChild(this.getCDArrowhead()), r.appendChild(i), r.setAttributeNS(null, "id", "arrow"), s.setAttributeNS(null, "x1", 0), s.setAttributeNS(null, "y1", -this.opts.arrow.thickness / 2), s.setAttributeNS(null, "x2", t), s.setAttributeNS(null, "y2", -this.opts.arrow.thickness / 2), s.setAttributeNS(null, "stroke-width", this.opts.arrow.thickness), s.setAttributeNS(null, "stroke", this.themeManager.getColor("C")), s.setAttributeNS(null, "marker-end", "url(#arrowhead)"), r.appendChild(s), r.setAttributeNS(null, "viewBox", `0 ${-e / 2} ${t + e * (7 / 4.5)} ${e}`), r;
     }
 };
-var yl = t0;
-const r0 = Zn,
-    i0 = wl,
-    n0 = Mi,
+var _l = i0;
+const n0 = Qn,
     s0 = yl,
-    Fa = Un,
-    a0 = Gn;
-let l0 = class qn {
+    a0 = Mi,
+    l0 = _l,
+    Ha = Jn,
+    o0 = jn;
+let h0 = class Yn {
     constructor(e = {}, t = {}) {
-        this.drawer = new n0(e), this.reactionDrawer = new s0(t, JSON.parse(JSON.stringify(this.drawer.opts)));
+        this.drawer = new a0(e), this.reactionDrawer = new l0(t, JSON.parse(JSON.stringify(this.drawer.opts)));
     }
     static apply(e = {}, t = {}, r = "data-smiles", i = "light", s = null, a = null) {
-        new qn(e, t).apply(r, i, s, a);
+        new Yn(e, t).apply(r, i, s, a);
     }
     apply(e = "data-smiles", t = "light", r = null, i = null) {
         document.querySelectorAll(`[${e}]`).forEach((a) => {
             let n = a.getAttribute(e);
             if (n === null)
                 throw Error("No SMILES provided.");
             let h = t,
@@ -11534,15 +11534,15 @@
                     reactants: [],
                     reagents: [],
                     products: []
                 }, a.hasAttribute("data-smiles-reactant-weights") && (l.reactants = a.getAttribute("data-smiles-reactant-weights").split(";").map((c) => c.split(",").map(parseFloat))), a.hasAttribute("data-smiles-reagent-weights") && (l.reagents = a.getAttribute("data-smiles-reagent-weights").split(";").map((c) => c.split(",").map(parseFloat))), a.hasAttribute("data-smiles-product-weights") && (l.products = a.getAttribute("data-smiles-product-weights").split(";").map((c) => c.split(",").map(parseFloat)))), a.hasAttribute("data-smiles-options") || a.hasAttribute("data-smiles-reaction-options")) {
                 let c = {};
                 a.hasAttribute("data-smiles-options") && (c = JSON.parse(a.getAttribute("data-smiles-options").replaceAll("'", '"')));
                 let u = {};
-                a.hasAttribute("data-smiles-reaction-options") && (u = JSON.parse(a.getAttribute("data-smiles-reaction-options").replaceAll("'", '"'))), new qn(c, u).draw(n, a, h, r, i, l);
+                a.hasAttribute("data-smiles-reaction-options") && (u = JSON.parse(a.getAttribute("data-smiles-reaction-options").replaceAll("'", '"'))), new Yn(c, u).draw(n, a, h, r, i, l);
             } else
                 this.draw(n, a, h, r, i, l);
         });
     }
     /**
      * Draw the smiles to the target.
      * @param {String} smiles The SMILES to be depicted.
@@ -11564,29 +11564,29 @@
             );
             l = JSON.parse(u.replaceAll("'", '"'));
         }
         let c = {
             textAboveArrow: "{reagents}",
             textBelowArrow: ""
         };
-        if (l = a0.extend(!0, c, l), e.includes(">"))
+        if (l = o0.extend(!0, c, l), e.includes(">"))
             try {
                 this.drawReaction(e, t, r, l, a, i);
             } catch (u) {
                 s ? s(u) : console.error(u);
             }
         else
             try {
                 this.drawMolecule(e, t, r, a, i);
             } catch (u) {
                 s ? s(u) : console.error(u);
             }
     }
     drawMolecule(e, t, r, i, s) {
-        let a = r0.parse(e);
+        let a = n0.parse(e);
         if (t === null || t === "svg") {
             let n = this.drawer.draw(a, null, r, i),
                 h = this.getDimensions(n);
             n.setAttributeNS(null, "width", "" + h.w), n.setAttributeNS(null, "height", "" + h.h), s && s(n);
         } else if (t === "canvas") {
             let n = this.svgToCanvas(this.drawer.draw(a, null, r, i));
             s && s(n);
@@ -11596,15 +11596,15 @@
         } else
             t instanceof HTMLImageElement ? (this.svgToImg(this.drawer.draw(a, null, r, i), t), s && s(t)) : t instanceof SVGElement ? (this.drawer.draw(a, t, r, i), s && s(t)) : document.querySelectorAll(t).forEach((h) => {
                 let l = h.nodeName.toLowerCase();
                 l === "svg" ? (this.drawer.draw(a, h, r, i), s && s(h)) : l === "canvas" ? (this.svgToCanvas(this.drawer.draw(a, null, r, i), h), s && s(h)) : l === "img" && (this.svgToImg(this.drawer.draw(a, null, r, i), h), s && s(h));
             });
     }
     drawReaction(e, t, r, i, s, a) {
-        let n = i0.parse(e);
+        let n = s0.parse(e);
         if (t === null || t === "svg") {
             let h = this.reactionDrawer.draw(n, null, r),
                 l = this.getDimensions(h);
             h.setAttributeNS(null, "width", "" + l.w), h.setAttributeNS(null, "height", "" + l.h), a && a(h);
         } else if (t === "canvas") {
             let h = this.svgToCanvas(this.reactionDrawer.draw(n, null, r, s, i.textAboveArrow, i.textBelowArrow));
             a && a(h);
@@ -11616,20 +11616,20 @@
                 let c = l.nodeName.toLowerCase();
                 c === "svg" ? (this.reactionDrawer.draw(n, l, r, s, i.textAboveArrow, i.textBelowArrow), this.reactionDrawer.opts.scale <= 0 && (l.style.width = null, l.style.height = null), a && a(l)) : c === "canvas" ? (this.svgToCanvas(this.reactionDrawer.draw(n, null, r, s, i.textAboveArrow, i.textBelowArrow), l), a && a(l)) : c === "img" && (this.svgToImg(this.reactionDrawer.draw(n, null, r, s, i.textAboveArrow, i.textBelowArrow), l), a && a(l));
             });
     }
     svgToCanvas(e, t = null) {
         t === null && (t = document.createElement("canvas"));
         let r = this.getDimensions(t, e);
-        return Fa.svgToCanvas(e, t, r.w, r.h), t;
+        return Ha.svgToCanvas(e, t, r.w, r.h), t;
     }
     svgToImg(e, t = null) {
         t === null && (t = document.createElement("img"));
         let r = this.getDimensions(t, e);
-        return Fa.svgToImg(e, t, r.w, r.h), t;
+        return Ha.svgToImg(e, t, r.w, r.h), t;
     }
     /**
      * 
      * @param {HTMLImageElement|HTMLCanvasElement|SVGElement} element 
      * @param {SVGElement} svg 
      * @returns {{w: Number, h: Number}} The width and height.
      */
@@ -11638,337 +11638,337 @@
             i = this.drawer.opts.height;
         return this.drawer.opts.scale <= 0 ? (r === null && (r = e.width), i === null && (i = e.height), e.style.width !== "" && (r = parseInt(e.style.width)), e.style.height !== "" && (i = parseInt(e.style.height))) : t && (r = parseFloat(t.style.width), i = parseFloat(t.style.height)), {
             w: r,
             h: i
         };
     }
 };
-var o0 = l0;
-const _l = Xg,
-    Sl = Zn,
-    Cl = wl,
-    h0 = Mi,
-    f0 = yl,
-    Al = o0,
-    u0 = bl;
-var c0 = !!(typeof window < "u" && window.document && window.document.createElement),
-    nt = {
+var f0 = h0;
+const Sl = Gg,
+    Cl = Qn,
+    Al = yl,
+    u0 = Mi,
+    c0 = _l,
+    Nl = f0,
+    g0 = wl;
+var d0 = !!(typeof window < "u" && window.document && window.document.createElement),
+    st = {
         Version: "1.0.0"
     };
-nt.Drawer = _l;
-nt.Parser = Sl;
-nt.SvgDrawer = h0;
-nt.ReactionDrawer = f0;
-nt.ReactionParser = Cl;
-nt.GaussDrawer = u0;
-nt.clean = function(d) {
+st.Drawer = Sl;
+st.Parser = Cl;
+st.SvgDrawer = u0;
+st.ReactionDrawer = c0;
+st.ReactionParser = Al;
+st.GaussDrawer = g0;
+st.clean = function(d) {
     return d.replace(/[^A-Za-z0-9@\.\+\-\?!\(\)\[\]\{\}/\\=#\$:\*]/g, "");
 };
-nt.apply = function(d, e = "canvas[data-smiles]", t = "light", r = null) {
-    let i = new _l(d),
+st.apply = function(d, e = "canvas[data-smiles]", t = "light", r = null) {
+    let i = new Sl(d),
         s = document.querySelectorAll(e);
     for (var a = 0; a < s.length; a++) {
         let n = s[a];
-        nt.parse(n.getAttribute("data-smiles"), function(h) {
+        st.parse(n.getAttribute("data-smiles"), function(h) {
             i.draw(h, n, t, !1);
         }, function(h) {
             r && r(h);
         });
     }
 };
-nt.parse = function(d, e, t) {
+st.parse = function(d, e, t) {
     try {
-        e && e(Sl.parse(d));
+        e && e(Cl.parse(d));
     } catch (r) {
         t && t(r);
     }
 };
-nt.parseReaction = function(d, e, t) {
+st.parseReaction = function(d, e, t) {
     try {
-        e && e(Cl.parse(d));
+        e && e(Al.parse(d));
     } catch (r) {
         t && t(r);
     }
 };
-c0 && (window.SmilesDrawer = nt, window.SmiDrawer = Al);
-nt.SmiDrawer = Al;
+d0 && (window.SmilesDrawer = st, window.SmiDrawer = Nl);
+st.SmiDrawer = Nl;
 Array.prototype.fill || Object.defineProperty(Array.prototype, "fill", {
     value: function(d) {
         if (this == null)
             throw new TypeError("this is null or not defined");
         for (var e = Object(this), t = e.length >>> 0, r = arguments[1], i = r >> 0, s = i < 0 ? Math.max(t + i, 0) : Math.min(i, t), a = arguments[2], n = a === void 0 ? t : a >> 0, h = n < 0 ? Math.max(t + n, 0) : Math.min(n, t); s < h;)
             e[s] = d, s++;
         return e;
     }
 });
-var g0 = nt;
-const za = /* @__PURE__ */ tg(g0),
+var p0 = st;
+const Wa = /* @__PURE__ */ ig(p0),
     {
-        SvelteComponent: d0,
-        append: p0,
+        SvelteComponent: v0,
+        append: m0,
         attr: Ti,
-        binding_callbacks: v0,
-        detach: Kn,
-        element: Nl,
-        empty: m0,
-        init: b0,
-        insert: jn,
-        noop: Vn,
-        safe_not_equal: w0,
-        svg_element: y0
+        binding_callbacks: b0,
+        detach: es,
+        element: kl,
+        empty: w0,
+        init: y0,
+        insert: ts,
+        noop: Gn,
+        safe_not_equal: _0,
+        svg_element: S0
     } = window.__gradio__svelte__internal,
     {
-        afterUpdate: _0
+        afterUpdate: C0
     } = window.__gradio__svelte__internal;
 
-function S0(d) {
+function A0(d) {
     let e;
     return {
         c() {
-            e = Nl("div"), e.textContent = "No molecule to display", Ti(e, "class", "text-center my-10 py-10 text-gray-600");
+            e = kl("div"), e.textContent = "No molecule to display", Ti(e, "class", "text-center my-10 py-10 text-gray-600");
         },
         m(t, r) {
-            jn(t, e, r);
+            ts(t, e, r);
         },
-        p: Vn,
+        p: Gn,
         d(t) {
-            t && Kn(e);
+            t && es(e);
         }
     };
 }
 
-function C0(d) {
+function N0(d) {
     let e, t;
     return {
         c() {
-            e = Nl("div"), t = y0("svg"), Ti(
+            e = kl("div"), t = S0("svg"), Ti(
                 t,
                 "data-smiles",
                 /*smiles*/
                 d[0]
             ), Ti(t, "class", "svelte-zjukdr");
         },
         m(r, i) {
-            jn(r, e, i), p0(e, t), d[2](t);
+            ts(r, e, i), m0(e, t), d[2](t);
         },
         p(r, i) {
             i & /*smiles*/
                 1 && Ti(
                     t,
                     "data-smiles",
                     /*smiles*/
                     r[0]
                 );
         },
         d(r) {
-            r && Kn(e), d[2](null);
+            r && es(e), d[2](null);
         }
     };
 }
 
-function A0(d) {
+function k0(d) {
     let e;
 
     function t(s, a) {
         return (
             /*smiles*/
-            s[0].length > 0 ? C0 : S0
+            s[0].length > 0 ? N0 : A0
         );
     }
     let r = t(d),
         i = r(d);
     return {
         c() {
-            i.c(), e = m0();
+            i.c(), e = w0();
         },
         m(s, a) {
-            i.m(s, a), jn(s, e, a);
+            i.m(s, a), ts(s, e, a);
         },
         p(s, [a]) {
             r === (r = t(s)) && i ? i.p(s, a) : (i.d(1), i = r(s), i && (i.c(), i.m(e.parentNode, e)));
         },
-        i: Vn,
-        o: Vn,
+        i: Gn,
+        o: Gn,
         d(s) {
-            s && Kn(e), i.d(s);
+            s && es(e), i.d(s);
         }
     };
 }
 
-function N0(d, e, t) {
+function R0(d, e, t) {
     let {
         smiles: r = ""
     } = e;
     const i = {
         width: 300,
         height: 200
     };
-    let s = new za.SvgDrawer(i),
+    let s = new Wa.SvgDrawer(i),
         a;
-    _0(() => {
-        za.parse(r, function(h) {
+    C0(() => {
+        Wa.parse(r, function(h) {
             s.draw(h, a, "light");
         });
     });
 
     function n(h) {
-        v0[h ? "unshift" : "push"](() => {
+        b0[h ? "unshift" : "push"](() => {
             a = h, t(1, a);
         });
     }
     return d.$$set = (h) => {
         "smiles" in h && t(0, r = h.smiles);
     }, [r, a, n];
 }
-class k0 extends d0 {
+class x0 extends v0 {
     constructor(e) {
-        super(), b0(this, e, N0, A0, w0, {
+        super(), y0(this, e, R0, k0, _0, {
             smiles: 0
         });
     }
 }
 const {
-    SvelteComponent: R0,
-    attr: x0,
-    create_component: T0,
-    destroy_component: E0,
-    detach: L0,
-    element: M0,
-    init: B0,
-    insert: D0,
-    mount_component: P0,
-    safe_not_equal: $0,
-    set_style: Ha,
-    toggle_class: Wa,
-    transition_in: I0,
-    transition_out: O0
+    SvelteComponent: T0,
+    attr: E0,
+    create_component: L0,
+    destroy_component: M0,
+    detach: B0,
+    element: D0,
+    init: P0,
+    insert: $0,
+    mount_component: I0,
+    safe_not_equal: O0,
+    set_style: qa,
+    toggle_class: Va,
+    transition_in: F0,
+    transition_out: z0
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: F0
+    createEventDispatcher: H0
 } = window.__gradio__svelte__internal;
 
-function z0(d) {
+function W0(d) {
     let e, t, r;
-    return t = new tl({
+    return t = new rl({
         props: {
-            Icon: rl,
+            Icon: il,
             label: "Finish drawing",
             size: "large"
         }
     }), t.$on(
         "click",
         /*click_handler*/
         d[2]
     ), {
         c() {
-            e = M0("div"), T0(t.$$.fragment), x0(e, "class", "svelte-181q4hi"), Wa(e, "not-absolute", ! /*absolute*/
-                d[0]), Ha(
+            e = D0("div"), L0(t.$$.fragment), E0(e, "class", "svelte-181q4hi"), Va(e, "not-absolute", ! /*absolute*/
+                d[0]), qa(
                 e,
                 "position",
                 /*absolute*/
                 d[0] ? "absolute" : "static"
             );
         },
         m(i, s) {
-            D0(i, e, s), P0(t, e, null), r = !0;
+            $0(i, e, s), I0(t, e, null), r = !0;
         },
         p(i, [s]) {
             (!r || s & /*absolute*/
-                1) && Wa(e, "not-absolute", ! /*absolute*/
+                1) && Va(e, "not-absolute", ! /*absolute*/
                     i[0]), s & /*absolute*/
-                1 && Ha(
+                1 && qa(
                     e,
                     "position",
                     /*absolute*/
                     i[0] ? "absolute" : "static"
                 );
         },
         i(i) {
-            r || (I0(t.$$.fragment, i), r = !0);
+            r || (F0(t.$$.fragment, i), r = !0);
         },
         o(i) {
-            O0(t.$$.fragment, i), r = !1;
+            z0(t.$$.fragment, i), r = !1;
         },
         d(i) {
-            i && L0(e), E0(t);
+            i && B0(e), M0(t);
         }
     };
 }
 
-function H0(d, e, t) {
+function q0(d, e, t) {
     let {
         absolute: r = !0
     } = e;
-    const i = F0(),
+    const i = H0(),
         s = (a) => {
             i("clear"), a.stopPropagation();
         };
     return d.$$set = (a) => {
         "absolute" in a && t(0, r = a.absolute);
     }, [r, i, s];
 }
-class W0 extends R0 {
+class V0 extends T0 {
     constructor(e) {
-        super(), B0(this, e, H0, z0, $0, {
+        super(), P0(this, e, q0, W0, O0, {
             absolute: 0
         });
     }
 }
 const {
-    SvelteComponent: q0,
-    append: V0,
-    attr: $n,
-    create_component: X0,
-    destroy_component: Y0,
-    detach: qa,
-    element: Va,
-    init: G0,
-    insert: Xa,
-    mount_component: U0,
-    noop: Z0,
-    safe_not_equal: K0,
-    space: j0,
-    transition_in: J0,
-    transition_out: Q0
+    SvelteComponent: X0,
+    append: Y0,
+    attr: On,
+    create_component: G0,
+    destroy_component: U0,
+    detach: Xa,
+    element: Ya,
+    init: Z0,
+    insert: Ga,
+    mount_component: K0,
+    noop: j0,
+    safe_not_equal: J0,
+    space: Q0,
+    transition_in: ed,
+    transition_out: td
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: ed
+    createEventDispatcher: rd
 } = window.__gradio__svelte__internal;
 
-function td(d) {
+function id(d) {
     let e, t, r, i, s;
-    return e = new W0({}), e.$on(
+    return e = new V0({}), e.$on(
         "clear",
         /*getsmiles*/
         d[0]
     ), {
         c() {
-            X0(e.$$.fragment), t = j0(), r = Va("div"), i = Va("iframe"), $n(
+            G0(e.$$.fragment), t = Q0(), r = Ya("div"), i = Ya("iframe"), On(
                 i,
                 "srcdoc",
                 /*ketcherDoc*/
                 d[1]
-            ), $n(i, "class", "svelte-rryiqv"), $n(r, "class", "composerWrapper");
+            ), On(i, "class", "svelte-rryiqv"), On(r, "class", "composerWrapper");
         },
         m(a, n) {
-            U0(e, a, n), Xa(a, t, n), Xa(a, r, n), V0(r, i), s = !0;
+            K0(e, a, n), Ga(a, t, n), Ga(a, r, n), Y0(r, i), s = !0;
         },
-        p: Z0,
+        p: j0,
         i(a) {
-            s || (J0(e.$$.fragment, a), s = !0);
+            s || (ed(e.$$.fragment, a), s = !0);
         },
         o(a) {
-            Q0(e.$$.fragment, a), s = !1;
+            td(e.$$.fragment, a), s = !1;
         },
         d(a) {
-            a && (qa(t), qa(r)), Y0(e, a);
+            a && (Xa(t), Xa(r)), U0(e, a);
         }
     };
 }
 
-function rd(d) {
-    const e = ed();
+function nd(d) {
+    const e = rd();
 
     function t() {
         document.querySelector("iframe").contentWindow.ketcher.getSmiles().then((a) => {
             e("moleculesketched", {
                 smiles: a
             });
         });
@@ -12057,51 +12057,51 @@
       };
 
     <\/script>
   </body>
 </html>
 `];
 }
-class id extends q0 {
+class sd extends X0 {
     constructor(e) {
-        super(), G0(this, e, rd, td, K0, {});
+        super(), Z0(this, e, nd, id, J0, {});
     }
 }
 const {
-    SvelteComponent: nd,
-    append: ct,
-    assign: sd,
-    attr: pt,
-    binding_callbacks: ad,
-    check_outros: Ya,
+    SvelteComponent: ad,
+    append: Tt,
+    assign: ld,
+    attr: vt,
+    binding_callbacks: od,
+    check_outros: Fn,
     create_component: Dr,
     destroy_component: Pr,
-    detach: Jn,
-    element: nr,
-    flush: it,
-    get_spread_object: ld,
-    get_spread_update: od,
-    group_outros: Ga,
-    init: hd,
-    insert: Qn,
-    listen: In,
+    detach: Bi,
+    element: sr,
+    flush: nt,
+    get_spread_object: hd,
+    get_spread_update: fd,
+    group_outros: zn,
+    init: ud,
+    insert: Di,
+    listen: Un,
     mount_component: $r,
-    noop: fd,
-    run_all: ud,
-    safe_not_equal: cd,
-    set_data: gd,
+    noop: Rl,
+    run_all: cd,
+    safe_not_equal: gd,
+    set_data: dd,
     set_input_value: Ua,
-    set_style: kl,
+    set_style: xl,
     space: Lr,
-    text: dd,
-    toggle_class: pd,
-    transition_in: vt,
-    transition_out: Pt
+    text: pd,
+    toggle_class: vd,
+    transition_in: Qe,
+    transition_out: mt
 } = window.__gradio__svelte__internal, {
-    tick: vd
+    tick: md
 } = window.__gradio__svelte__internal;
 
 function Za(d) {
     let e, t;
     const r = [{
             autoscroll: (
                 /*gradio*/
@@ -12114,31 +12114,31 @@
             )
         },
         /*loading_status*/
         d[10]
     ];
     let i = {};
     for (let s = 0; s < r.length; s += 1)
-        i = sd(i, r[s]);
-    return e = new Qc({
+        i = ld(i, r[s]);
+    return e = new tg({
         props: i
     }), e.$on(
         "clear_status",
         /*clear_status_handler*/
         d[19]
     ), {
         c() {
             Dr(e.$$.fragment);
         },
         m(s, a) {
             $r(e, s, a), t = !0;
         },
         p(s, a) {
             const n = a & /*gradio, loading_status*/
-                1026 ? od(r, [
+                1026 ? fd(r, [
                     a & /*gradio*/
                     2 && {
                         autoscroll: (
                             /*gradio*/
                             s[1].autoscroll
                         )
                     },
@@ -12146,207 +12146,236 @@
                     2 && {
                         i18n: (
                             /*gradio*/
                             s[1].i18n
                         )
                     },
                     a & /*loading_status*/
-                    1024 && ld(
+                    1024 && hd(
                         /*loading_status*/
                         s[10]
                     )
                 ]) : {};
             e.$set(n);
         },
         i(s) {
-            t || (vt(e.$$.fragment, s), t = !0);
+            t || (Qe(e.$$.fragment, s), t = !0);
         },
         o(s) {
-            Pt(e.$$.fragment, s), t = !1;
+            mt(e.$$.fragment, s), t = !1;
         },
         d(s) {
             Pr(e, s);
         }
     };
 }
 
-function md(d) {
+function bd(d) {
     let e;
     return {
         c() {
-            e = dd(
+            e = pd(
                 /*label*/
                 d[2]
             );
         },
         m(t, r) {
-            Qn(t, e, r);
+            Di(t, e, r);
         },
         p(t, r) {
             r & /*label*/
-                4 && gd(
+                4 && dd(
                     e,
                     /*label*/
                     t[2]
                 );
         },
         d(t) {
-            t && Jn(e);
+            t && Bi(e);
         }
     };
 }
 
 function Ka(d) {
+    let e, t, r, i, s, a, n, h, l;
+    return i = new pc({}), {
+        c() {
+            e = sr("div"), t = sr("button"), r = sr("div"), Dr(i.$$.fragment), s = Lr(), a = sr("span"), a.textContent = "Draw molecule", vt(r, "class", "w-4 h-4 mr-2"), vt(t, "class", "flex items-center svelte-q9tvhg"), vt(e, "class", "w-full flex justify-center");
+        },
+        m(c, u) {
+            Di(c, e, u), Tt(e, t), Tt(t, r), $r(i, r, null), Tt(t, s), Tt(t, a), n = !0, h || (l = Un(
+                t,
+                "click",
+                /*showEditor*/
+                d[17]
+            ), h = !0);
+        },
+        p: Rl,
+        i(c) {
+            n || (Qe(i.$$.fragment, c), n = !0);
+        },
+        o(c) {
+            mt(i.$$.fragment, c), n = !1;
+        },
+        d(c) {
+            c && Bi(e), Pr(i), h = !1, l();
+        }
+    };
+}
+
+function ja(d) {
     let e, t, r;
-    return t = new id({}), t.$on(
+    return t = new sd({}), t.$on(
         "moleculesketched",
         /*handleMolecule*/
         d[16]
     ), {
         c() {
-            e = nr("div"), Dr(t.$$.fragment), pt(e, "class", "absolute top-0 left-0 w-full z-10"), kl(e, "height", "100%");
+            e = sr("div"), Dr(t.$$.fragment), vt(e, "class", "absolute top-0 left-0 w-full z-10"), xl(e, "height", "100%");
         },
         m(i, s) {
-            Qn(i, e, s), $r(t, e, null), r = !0;
+            Di(i, e, s), $r(t, e, null), r = !0;
         },
-        p: fd,
+        p: Rl,
         i(i) {
-            r || (vt(t.$$.fragment, i), r = !0);
+            r || (Qe(t.$$.fragment, i), r = !0);
         },
         o(i) {
-            Pt(t.$$.fragment, i), r = !1;
+            mt(t.$$.fragment, i), r = !1;
         },
         d(i) {
-            i && Jn(e), Pr(t);
+            i && Bi(e), Pr(t);
         }
     };
 }
 
-function bd(d) {
-    let e, t, r, i, s, a, n, h, l, c, u, g, m, _, v, N, B, x, L, k, z, D = (
+function wd(d) {
+    let e, t, r, i, s, a, n, h, l, c, u, g, m, _, v, A = (
         /*loading_status*/
         d[10] && Za(d)
     );
-    i = new Ou({
+    i = new zu({
         props: {
             show_label: (
                 /*show_label*/
                 d[7]
             ),
             info: void 0,
             $$slots: {
-                default: [md]
+                default: [bd]
             },
             $$scope: {
                 ctx: d
             }
         }
-    }), c = new k0({
+    }), c = new x0({
         props: {
             smiles: (
                 /*value*/
                 d[0]
             )
         }
-    }), v = new gc({});
-    let Y = (
-        /*showeditor*/
-        d[14] && Ka(d)
-    );
+    });
+    let T = (
+            /*interactive*/
+            d[11] && Ka(d)
+        ),
+        k = (
+            /*showeditor*/
+            d[14] && ja(d)
+        );
     return {
         c() {
-            e = nr("div"), D && D.c(), t = Lr(), r = nr("label"), Dr(i.$$.fragment), s = Lr(), a = nr("input"), l = Lr(), Dr(c.$$.fragment), u = Lr(), g = nr("div"), m = nr("button"), _ = nr("div"), Dr(v.$$.fragment), N = Lr(), B = nr("span"), B.textContent = "Draw molecule", x = Lr(), Y && Y.c(), pt(a, "data-testid", "textbox"), pt(a, "type", "text"), pt(a, "class", "scroll-hide svelte-q9tvhg"), pt(
+            e = sr("div"), A && A.c(), t = Lr(), r = sr("label"), Dr(i.$$.fragment), s = Lr(), a = sr("input"), l = Lr(), Dr(c.$$.fragment), u = Lr(), T && T.c(), g = Lr(), k && k.c(), vt(a, "data-testid", "textbox"), vt(a, "type", "text"), vt(a, "class", "scroll-hide svelte-q9tvhg"), vt(
                     a,
                     "placeholder",
                     /*placeholder*/
                     d[6]
                 ), a.disabled = n = ! /*interactive*/
-                d[11], pt(a, "dir", h = /*rtl*/
-                    d[12] ? "rtl" : "ltr"), pt(r, "class", "svelte-q9tvhg"), pd(r, "container", yd), pt(_, "class", "w-4 h-4 mr-2"), pt(m, "class", "flex items-center svelte-q9tvhg"), pt(g, "class", "w-full flex justify-center"), kl(e, "min-height", "70vh");
+                d[11], vt(a, "dir", h = /*rtl*/
+                    d[12] ? "rtl" : "ltr"), vt(r, "class", "svelte-q9tvhg"), vd(r, "container", _d), xl(e, "min-height", "70vh");
         },
-        m(O, Z) {
-            Qn(O, e, Z), D && D.m(e, null), ct(e, t), ct(e, r), $r(i, r, null), ct(r, s), ct(r, a), Ua(
+        m(x, R) {
+            Di(x, e, R), A && A.m(e, null), Tt(e, t), Tt(e, r), $r(i, r, null), Tt(r, s), Tt(r, a), Ua(
                 a,
                 /*value*/
                 d[0]
-            ), d[21](a), ct(e, l), $r(c, e, null), ct(e, u), ct(e, g), ct(g, m), ct(m, _), $r(v, _, null), ct(m, N), ct(m, B), ct(e, x), Y && Y.m(e, null), L = !0, k || (z = [
-                In(
+            ), d[21](a), Tt(e, l), $r(c, e, null), Tt(e, u), T && T.m(e, null), Tt(e, g), k && k.m(e, null), m = !0, _ || (v = [
+                Un(
                     a,
                     "input",
                     /*input_input_handler*/
                     d[20]
                 ),
-                In(
+                Un(
                     a,
                     "keypress",
                     /*handle_keypress*/
                     d[15]
-                ),
-                In(
-                    m,
-                    "click",
-                    /*showEditor*/
-                    d[17]
                 )
-            ], k = !0);
+            ], _ = !0);
         },
-        p(O, Z) {
+        p(x, R) {
             /*loading_status*/
-            O[10] ? D ? (D.p(O, Z), Z & /*loading_status*/
-                1024 && vt(D, 1)) : (D = Za(O), D.c(), vt(D, 1), D.m(e, t)) : D && (Ga(), Pt(D, 1, 1, () => {
-                D = null;
-            }), Ya());
-            const j = {};
-            Z & /*show_label*/
-                128 && (j.show_label = /*show_label*/
-                    O[7]), Z & /*$$scope, label*/
-                33554436 && (j.$$scope = {
-                    dirty: Z,
-                    ctx: O
-                }), i.$set(j), (!L || Z & /*placeholder*/
-                    64) && pt(
+            x[10] ? A ? (A.p(x, R), R & /*loading_status*/
+                1024 && Qe(A, 1)) : (A = Za(x), A.c(), Qe(A, 1), A.m(e, t)) : A && (zn(), mt(A, 1, 1, () => {
+                A = null;
+            }), Fn());
+            const O = {};
+            R & /*show_label*/
+                128 && (O.show_label = /*show_label*/
+                    x[7]), R & /*$$scope, label*/
+                16777220 && (O.$$scope = {
+                    dirty: R,
+                    ctx: x
+                }), i.$set(O), (!m || R & /*placeholder*/
+                    64) && vt(
                     a,
                     "placeholder",
                     /*placeholder*/
-                    O[6]
-                ), (!L || Z & /*interactive*/
+                    x[6]
+                ), (!m || R & /*interactive*/
                     2048 && n !== (n = ! /*interactive*/
-                        O[11])) && (a.disabled = n), (!L || Z & /*rtl*/
+                        x[11])) && (a.disabled = n), (!m || R & /*rtl*/
                     4096 && h !== (h = /*rtl*/
-                        O[12] ? "rtl" : "ltr")) && pt(a, "dir", h), Z & /*value*/
+                        x[12] ? "rtl" : "ltr")) && vt(a, "dir", h), R & /*value*/
                 1 && a.value !== /*value*/
-                O[0] && Ua(
+                x[0] && Ua(
                     a,
                     /*value*/
-                    O[0]
+                    x[0]
                 );
-            const q = {};
-            Z & /*value*/
-                1 && (q.smiles = /*value*/
-                    O[0]), c.$set(q), /*showeditor*/
-                O[14] ? Y ? (Y.p(O, Z), Z & /*showeditor*/
-                    16384 && vt(Y, 1)) : (Y = Ka(O), Y.c(), vt(Y, 1), Y.m(e, null)) : Y && (Ga(), Pt(Y, 1, 1, () => {
-                    Y = null;
-                }), Ya());
+            const D = {};
+            R & /*value*/
+                1 && (D.smiles = /*value*/
+                    x[0]), c.$set(D), /*interactive*/
+                x[11] ? T ? (T.p(x, R), R & /*interactive*/
+                    2048 && Qe(T, 1)) : (T = Ka(x), T.c(), Qe(T, 1), T.m(e, g)) : T && (zn(), mt(T, 1, 1, () => {
+                    T = null;
+                }), Fn()), /*showeditor*/
+                x[14] ? k ? (k.p(x, R), R & /*showeditor*/
+                    16384 && Qe(k, 1)) : (k = ja(x), k.c(), Qe(k, 1), k.m(e, null)) : k && (zn(), mt(k, 1, 1, () => {
+                    k = null;
+                }), Fn());
         },
-        i(O) {
-            L || (vt(D), vt(i.$$.fragment, O), vt(c.$$.fragment, O), vt(v.$$.fragment, O), vt(Y), L = !0);
+        i(x) {
+            m || (Qe(A), Qe(i.$$.fragment, x), Qe(c.$$.fragment, x), Qe(T), Qe(k), m = !0);
         },
-        o(O) {
-            Pt(D), Pt(i.$$.fragment, O), Pt(c.$$.fragment, O), Pt(v.$$.fragment, O), Pt(Y), L = !1;
+        o(x) {
+            mt(A), mt(i.$$.fragment, x), mt(c.$$.fragment, x), mt(T), mt(k), m = !1;
         },
-        d(O) {
-            O && Jn(e), D && D.d(), Pr(i), d[21](null), Pr(c), Pr(v), Y && Y.d(), k = !1, ud(z);
+        d(x) {
+            x && Bi(e), A && A.d(), Pr(i), d[21](null), Pr(c), T && T.d(), k && k.d(), _ = !1, cd(v);
         }
     };
 }
 
-function wd(d) {
+function yd(d) {
     let e, t;
-    return e = new tu({
+    return e = new iu({
         props: {
             visible: (
                 /*visible*/
                 d[5]
             ),
             elem_id: (
                 /*elem_id*/
@@ -12363,15 +12392,15 @@
             min_width: (
                 /*min_width*/
                 d[9]
             ),
             allow_overflow: !1,
             padding: !0,
             $$slots: {
-                default: [bd]
+                default: [wd]
             },
             $$scope: {
                 ctx: d
             }
         }
     }), {
         c() {
@@ -12388,61 +12417,61 @@
                 8 && (s.elem_id = /*elem_id*/
                     r[3]), i & /*elem_classes*/
                 16 && (s.elem_classes = /*elem_classes*/
                     r[4]), i & /*scale*/
                 256 && (s.scale = /*scale*/
                     r[8]), i & /*min_width*/
                 512 && (s.min_width = /*min_width*/
-                    r[9]), i & /*$$scope, showeditor, value, placeholder, interactive, rtl, el, show_label, label, gradio, loading_status*/
-                33586375 && (s.$$scope = {
+                    r[9]), i & /*$$scope, showeditor, interactive, value, placeholder, rtl, el, show_label, label, gradio, loading_status*/
+                16809159 && (s.$$scope = {
                     dirty: i,
                     ctx: r
                 }), e.$set(s);
         },
         i(r) {
-            t || (vt(e.$$.fragment, r), t = !0);
+            t || (Qe(e.$$.fragment, r), t = !0);
         },
         o(r) {
-            Pt(e.$$.fragment, r), t = !1;
+            mt(e.$$.fragment, r), t = !1;
         },
         d(r) {
             Pr(e, r);
         }
     };
 }
-const yd = !0;
+const _d = !0;
 
-function _d(d, e, t) {
-    var r = this && this.__awaiter || function(q, se, ye, ke) {
+function Sd(d, e, t) {
+    var r = this && this.__awaiter || function(X, se, ye, ke) {
         function xe(we) {
             return we instanceof ye ? we : new ye(function(Ee) {
                 Ee(we);
             });
         }
         return new(ye || (ye = Promise))(function(we, Ee) {
-            function Qe(Be) {
+            function et(Be) {
                 try {
                     Ae(ke.next(Be));
-                } catch (st) {
-                    Ee(st);
+                } catch (at) {
+                    Ee(at);
                 }
             }
 
             function Ce(Be) {
                 try {
                     Ae(ke.throw(Be));
-                } catch (st) {
-                    Ee(st);
+                } catch (at) {
+                    Ee(at);
                 }
             }
 
             function Ae(Be) {
-                Be.done ? we(Be.value) : xe(Be.value).then(Qe, Ce);
+                Be.done ? we(Be.value) : xe(Be.value).then(et, Ce);
             }
-            Ae((ke = ke.apply(q, se || [])).next());
+            Ae((ke = ke.apply(X, se || [])).next());
         });
     };
     let {
         gradio: i
     } = e, {
         label: s = "Textbox"
     } = e, {
@@ -12462,82 +12491,82 @@
     } = e, {
         min_width: m = void 0
     } = e, {
         loading_status: _ = void 0
     } = e, {
         value_is_output: v = !1
     } = e, {
-        interactive: N
+        interactive: A
     } = e, {
-        rtl: B = !1
-    } = e, x;
+        rtl: T = !1
+    } = e, k;
 
-    function L() {
+    function x() {
         i.dispatch("change"), v || i.dispatch("input");
     }
 
-    function k(q) {
+    function R(X) {
         return r(this, void 0, void 0, function*() {
-            yield vd(), q.key === "Enter" && (q.preventDefault(), i.dispatch("submit"));
+            yield md(), X.key === "Enter" && (X.preventDefault(), i.dispatch("submit"));
         });
     }
-    let z = !1;
+    let O = !1;
 
-    function D(q) {
-        t(0, l = q.detail.smiles), t(14, z = !1);
+    function D(X) {
+        t(0, l = X.detail.smiles), t(14, O = !1);
     }
 
-    function Y() {
-        t(14, z = !0);
+    function te() {
+        t(14, O = !0);
     }
-    const O = () => i.dispatch("clear_status", _);
+    const q = () => i.dispatch("clear_status", _);
 
-    function Z() {
+    function re() {
         l = this.value, t(0, l);
     }
 
-    function j(q) {
-        ad[q ? "unshift" : "push"](() => {
-            x = q, t(13, x);
+    function j(X) {
+        od[X ? "unshift" : "push"](() => {
+            k = X, t(13, k);
         });
     }
-    return d.$$set = (q) => {
-        "gradio" in q && t(1, i = q.gradio), "label" in q && t(2, s = q.label), "elem_id" in q && t(3, a = q.elem_id), "elem_classes" in q && t(4, n = q.elem_classes), "visible" in q && t(5, h = q.visible), "value" in q && t(0, l = q.value), "placeholder" in q && t(6, c = q.placeholder), "show_label" in q && t(7, u = q.show_label), "scale" in q && t(8, g = q.scale), "min_width" in q && t(9, m = q.min_width), "loading_status" in q && t(10, _ = q.loading_status), "value_is_output" in q && t(18, v = q.value_is_output), "interactive" in q && t(11, N = q.interactive), "rtl" in q && t(12, B = q.rtl);
+    return d.$$set = (X) => {
+        "gradio" in X && t(1, i = X.gradio), "label" in X && t(2, s = X.label), "elem_id" in X && t(3, a = X.elem_id), "elem_classes" in X && t(4, n = X.elem_classes), "visible" in X && t(5, h = X.visible), "value" in X && t(0, l = X.value), "placeholder" in X && t(6, c = X.placeholder), "show_label" in X && t(7, u = X.show_label), "scale" in X && t(8, g = X.scale), "min_width" in X && t(9, m = X.min_width), "loading_status" in X && t(10, _ = X.loading_status), "value_is_output" in X && t(18, v = X.value_is_output), "interactive" in X && t(11, A = X.interactive), "rtl" in X && t(12, T = X.rtl);
     }, d.$$.update = () => {
         d.$$.dirty & /*value*/
             1 && l === null && t(0, l = ""), d.$$.dirty & /*value*/
-            1 && L();
+            1 && x();
     }, [
         l,
         i,
         s,
         a,
         n,
         h,
         c,
         u,
         g,
         m,
         _,
-        N,
-        B,
-        x,
-        z,
+        A,
+        T,
         k,
+        O,
+        R,
         D,
-        Y,
+        te,
         v,
-        O,
-        Z,
+        q,
+        re,
         j
     ];
 }
-class Md extends nd {
+class Bd extends ad {
     constructor(e) {
-        super(), hd(this, e, _d, wd, cd, {
+        super(), ud(this, e, Sd, yd, gd, {
             gradio: 1,
             label: 2,
             elem_id: 3,
             elem_classes: 4,
             visible: 5,
             value: 0,
             placeholder: 6,
@@ -12552,118 +12581,118 @@
     }
     get gradio() {
         return this.$$.ctx[1];
     }
     set gradio(e) {
         this.$$set({
             gradio: e
-        }), it();
+        }), nt();
     }
     get label() {
         return this.$$.ctx[2];
     }
     set label(e) {
         this.$$set({
             label: e
-        }), it();
+        }), nt();
     }
     get elem_id() {
         return this.$$.ctx[3];
     }
     set elem_id(e) {
         this.$$set({
             elem_id: e
-        }), it();
+        }), nt();
     }
     get elem_classes() {
         return this.$$.ctx[4];
     }
     set elem_classes(e) {
         this.$$set({
             elem_classes: e
-        }), it();
+        }), nt();
     }
     get visible() {
         return this.$$.ctx[5];
     }
     set visible(e) {
         this.$$set({
             visible: e
-        }), it();
+        }), nt();
     }
     get value() {
         return this.$$.ctx[0];
     }
     set value(e) {
         this.$$set({
             value: e
-        }), it();
+        }), nt();
     }
     get placeholder() {
         return this.$$.ctx[6];
     }
     set placeholder(e) {
         this.$$set({
             placeholder: e
-        }), it();
+        }), nt();
     }
     get show_label() {
         return this.$$.ctx[7];
     }
     set show_label(e) {
         this.$$set({
             show_label: e
-        }), it();
+        }), nt();
     }
     get scale() {
         return this.$$.ctx[8];
     }
     set scale(e) {
         this.$$set({
             scale: e
-        }), it();
+        }), nt();
     }
     get min_width() {
         return this.$$.ctx[9];
     }
     set min_width(e) {
         this.$$set({
             min_width: e
-        }), it();
+        }), nt();
     }
     get loading_status() {
         return this.$$.ctx[10];
     }
     set loading_status(e) {
         this.$$set({
             loading_status: e
-        }), it();
+        }), nt();
     }
     get value_is_output() {
         return this.$$.ctx[18];
     }
     set value_is_output(e) {
         this.$$set({
             value_is_output: e
-        }), it();
+        }), nt();
     }
     get interactive() {
         return this.$$.ctx[11];
     }
     set interactive(e) {
         this.$$set({
             interactive: e
-        }), it();
+        }), nt();
     }
     get rtl() {
         return this.$$.ctx[12];
     }
     set rtl(e) {
         this.$$set({
             rtl: e
-        }), it();
+        }), nt();
     }
 }
 export {
-    Md as
+    Bd as
     default
 };
```

### Comparing `gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/component/style.css` & `gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/backend/gradio_molecule2d/templates/example/index.js` & `gradio_molecule2d-0.0.2/backend/gradio_molecule2d/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/demo/css.css` & `gradio_molecule2d-0.0.2/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/demo/space.py` & `gradio_molecule2d-0.0.2/demo/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_molecule2d`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_molecule2d/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_molecule2d"></a>  
 </div>
 
-Input smiles strings and visualize them
+Input chemical molecules as smiles strings and visualize them
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
 ## Installation
 
 ```bash
```

### Comparing `gradio_molecule2d-0.0.1/frontend/ClearButton.svelte` & `gradio_molecule2d-0.0.2/frontend/ClearButton.svelte`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/frontend/Editor.svelte` & `gradio_molecule2d-0.0.2/frontend/Editor.svelte`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/frontend/Example.svelte` & `gradio_molecule2d-0.0.2/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/frontend/Index.svelte` & `gradio_molecule2d-0.0.2/frontend/Index.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,14 @@
   export let scale: number | null = null;
   export let min_width: number | undefined = undefined;
   export let loading_status: LoadingStatus | undefined = undefined;
   export let value_is_output = false;
   export let interactive: boolean;
   export let rtl = false;
 
-  let retrieveSmiles;
-
   let el: HTMLTextAreaElement | HTMLInputElement;
   const container = true;
 
   function handle_change(): void {
     gradio.dispatch("change");
     if (!value_is_output) {
       gradio.dispatch("input");
@@ -108,20 +106,22 @@
         dir={rtl ? "rtl" : "ltr"}
         on:keypress={handle_keypress}
       />
     </label>
 
     <Viewer smiles={value} />
 
-    <div class="w-full flex justify-center">
-      <button on:click={showEditor} class="flex items-center">
-        <div class="w-4 h-4 mr-2"><Sketch /></div>
-        <span>Draw molecule</span>
-      </button>
-    </div>
+    {#if interactive}
+      <div class="w-full flex justify-center">
+        <button on:click={showEditor} class="flex items-center">
+          <div class="w-4 h-4 mr-2"><Sketch /></div>
+          <span>Draw molecule</span>
+        </button>
+      </div>
+    {/if}
 
     {#if showeditor}
       <div class="absolute top-0 left-0 w-full z-10" style="height: 100%">
         <Editor on:moleculesketched={handleMolecule} />
       </div>
     {/if}
   </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 visible} {elem_id} {elem_classes} {scale} {min_width} allow_overflow={false}
 padding={true} >
 {#if loading_status}
 ...loading_status} on:clear_status={() => gradio.dispatch("clear_status",
 loading_status)} /> {/if}
 show_label} info={undefined}>{label}
 placeholder} disabled={!interactive} dir={rtl ? "rtl" : "ltr"} on:keypress=
-{handle_keypress} />
+{handle_keypress} /> {#if interactive}
 Draw molecule
-{#if showeditor}
+{/if} {#if showeditor}
 {/if}
```

### Comparing `gradio_molecule2d-0.0.1/frontend/Viewer.svelte` & `gradio_molecule2d-0.0.2/frontend/Viewer.svelte`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/frontend/package-lock.json` & `gradio_molecule2d-0.0.2/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/frontend/package.json` & `gradio_molecule2d-0.0.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_molecule2d-0.0.1/README.md` & `gradio_molecule2d-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 colorTo: yellow
 sdk: gradio
 pinned: false
 app_file: space.py
 ---
 
 # `gradio_molecule2d`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_molecule2d/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_molecule2d"></a>  
 
-Input smiles strings and visualize them
+Input chemical molecules as smiles strings and visualize them
 
 ## Installation
 
 ```bash
 pip install gradio_molecule2d
 ```
```

### Comparing `gradio_molecule2d-0.0.1/pyproject.toml` & `gradio_molecule2d-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_molecule2d"
-version = "0.0.1"
-description = "Input smiles strings and visualize them"
+version = "0.0.2"
+description = "Input chemical molecules as smiles strings and visualize them"
 readme = "README.md"
 license = "mit"
 requires-python = ">=3.8"
-authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
+authors = [{ name = "Simon Dürr", email = "dev@simonduerr.eu" }]
 keywords = ["gradio-custom-component", "gradio-template-SimpleTextbox", "chemistry", "smiles"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gradio_molecule2d-0.0.1/PKG-INFO` & `gradio_molecule2d-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: gradio_molecule2d
-Version: 0.0.1
-Summary: Input smiles strings and visualize them
-Author-email: YOUR NAME <YOUREMAIL@domain.com>
+Version: 0.0.2
+Summary: Input chemical molecules as smiles strings and visualize them
+Author-email: Simon Dürr <dev@simonduerr.eu>
 License-Expression: MIT
 Keywords: chemistry,gradio-custom-component,gradio-template-SimpleTextbox,smiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -31,17 +31,17 @@
 colorTo: yellow
 sdk: gradio
 pinned: false
 app_file: space.py
 ---
 
 # `gradio_molecule2d`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_molecule2d/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_molecule2d"></a>  
 
-Input smiles strings and visualize them
+Input chemical molecules as smiles strings and visualize them
 
 ## Installation
 
 ```bash
 pip install gradio_molecule2d
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

