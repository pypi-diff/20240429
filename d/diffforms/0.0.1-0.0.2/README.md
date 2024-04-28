# Comparing `tmp/diffforms-0.0.1.tar.gz` & `tmp/diffforms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffforms-0.0.1.tar", last modified: Fri Apr 19 21:50:56 2024, max compression
+gzip compressed data, was "diffforms-0.0.2.tar", last modified: Sun Apr 28 22:26:12 2024, max compression
```

## Comparing `diffforms-0.0.1.tar` & `diffforms-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 21:50:56.473482 diffforms-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-19 21:48:17.000000 diffforms-0.0.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      450 2024-04-19 21:50:56.473097 diffforms-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1532 2024-04-10 18:51:30.000000 diffforms-0.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 21:50:56.469398 diffforms-0.0.1/diffforms/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-01-28 20:24:51.000000 diffforms-0.0.1/diffforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    19606 2024-04-19 20:23:43.000000 diffforms-0.0.1/diffforms/core.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 20:24:51.000000 diffforms-0.0.1/diffforms/release.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 21:50:56.472390 diffforms-0.0.1/diffforms.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      450 2024-04-19 21:50:56.000000 diffforms-0.0.1/diffforms.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-19 21:50:56.000000 diffforms-0.0.1/diffforms.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-19 21:50:56.000000 diffforms-0.0.1/diffforms.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       28 2024-04-19 21:50:56.000000 diffforms-0.0.1/diffforms.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-19 21:50:56.000000 diffforms-0.0.1/diffforms.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       27 2024-04-19 21:14:04.000000 diffforms-0.0.1/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-19 21:50:56.473619 diffforms-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-19 21:49:01.000000 diffforms-0.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-28 22:26:12.826621 diffforms-0.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      537 2024-04-28 22:26:12.826097 diffforms-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1479 2024-04-25 21:40:15.000000 diffforms-0.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-28 22:26:12.822614 diffforms-0.0.2/diffforms/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.2/diffforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20219 2024-04-28 22:17:06.000000 diffforms-0.0.2/diffforms/core.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2024-04-28 22:25:47.000000 diffforms-0.0.2/diffforms/release.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-28 22:26:12.825654 diffforms-0.0.2/diffforms.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      537 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.2/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-28 22:26:12.826704 diffforms-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.2/setup.py
```

### Comparing `diffforms-0.0.1/README.md` & `diffforms-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 General
 =======
-The Diffform python package implements differential forms and poly-forms from differential geometry. It includes some of the usual operations found in exterior calculus, include exterior product, differential operator. The main advatage of this package over other differential form packages ( e.g. [pycartan](https://github.com/TUD-RST/pycartan) ) is that it allows for polyforms and there is no dependence on basis forms. However, this removes some useful operations like insertion of vector fields (which is done using substitutions).
+The Diffform python package implements differential forms and poly-forms from differential geometry. It includes some of the usual operations found in exterior calculus, include exterior product, differential operator. The main advatage of this package over other differential form packages ( e.g. [pycartan](https://github.com/TUD-RST/pycartan) ) is that it allows for polyforms and there is no dependence on basis forms. However, this removes some useful operations like insertion of vector fields.
 
 This package is a part-time project during my PhD so updates should be suspected to end eventually. Bugs and mistakes may (possibly will) be prevalent.
 
 Documentary will be implemented when I find the time, in the mean time I will try to provide comments in the code as a type of documentation.
 
 ToDo List
 =========
 This is the list of possible implementation, in an approximate order of priority (interest to me):
 
 - [X] Differential Forms
 - [X] Exterior Product
 - [X] Simplification of Forms
 - [X] Exterior Differential Operator
-- [X] Substitution of factors/forms
-- [ ] Sympy function integration
-- [ ] Arbitrary sympy factors (up to user to keep track of type)
-- [ ] Integration of forms (bounds/limits of polyforms? Inheret bounds?
-- [ ] More?
-
+- [ ] Substitution of factors/forms
+- [ ] Vector fields
+- [ ] Generic tensor product
+- [ ] Insertion of vector fields
+- [ ] Hodge star given metric 
 
 Dependencies
 ============
 Make sure you have the following python packages:
 
+- wheel (needed for installing through pip)
 - sympy
 
 Installation
 ============
-Until I implement an installation method, the `core.py` file can be copied and imported to gain all functionality.
+Package should be uploaded to pip fairly frequently and is currently under [diffforms](https://pypi.org/project/diffforms/)
```

### Comparing `diffforms-0.0.1/diffforms/core.py` & `diffforms-0.0.2/diffforms/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,149 @@
 from sympy import Symbol, I, Integer, AtomicExpr, Rational, latex, Number, Expr, symbols, simplify, Function
 from sympy.physics.units.quantities import Quantity
 from IPython.display import Math
+from sympy.combinatorics import Permutation
+from itertools import permutations
 import re
 import numbers
+from math import factorial
+
 MAX_DEGREE = 4
 
 def remove_latex_arguments(object):
     if hasattr(object,'atoms'):
         functions = object.atoms(Function)
         reps = {}
         for fun in functions:
             if hasattr(fun, 'name'):
                 reps[fun] = Symbol(fun.name)
         object = object.subs(reps)
     latex_str = latex(object)
-    latex_str = re.sub(r"\\frac{d}{d ([\\\S]+)}",r"\\partial_{\g<1>}",latex_str)
-    latex_str = re.sub(r"\\frac{\\partial}{\\partial ([\\\S]+)}",r"\\partial_{\g<1>}",latex_str)
-    latex_str = re.sub(r"\\frac{d}{d (\S)}",r"\\partial_{\g<1>}",latex_str)
-    latex_str = re.sub(r"\\frac{d\^{(\d)}}{d (\S)\^{[\d]}}",r"\\partial^{\g<1>}_{\g<2>}",latex_str)
-    latex_str = re.sub(r"\\frac{d\^{\d}}{d ([\S]+)d ([\S]+)}",r"\\partial^2_{\g<1> \g<2>}",latex_str)
     return latex_str
 
 def display_no_arg(object):
     latex_str = remove_latex_arguments(object)
     display(Math(latex_str))
 
 def set_max_degree(max_degree: int):
     MAX_DEGREE=max_degree
 
 def constants(names:str)->symbols:
     """ Uses the Quantity function to create constant symbols. """
     names = re.sub(r'[\s+]', ' ', names)
     return [Quantity(c) for c in names.split(' ')]
 
+class VectorField():
+    def __init__(self,symbol):
+        """
+        Class: Vector Field
+
+        This class represents a single term in a vector fields component expansion, however, it is purely symbolic so no basis is required.
+
+        """
+        self.symbol = symbol
+    
+    def __eq__(self,other): return self.symbol == other.symbol
+    def __hash(self): return hash(self.symbol)
+
+    def __mull__(self,other):
+        #TODO: Implement
+        """
+        Pseudo Code:
+
+        IF other is a (VectorField or DifferentialForm):
+            return TensorProduct(self,other)
+        ELIF other is a (Tensor or DifferentialFormMul):
+            return SUM([TensorProduct(self,term) term in other])
+        """
+        pass
+    
+    def __add__(self,other):
+        #TODO: Implement
+        pass
+
+    def _repr_latex_(self):
+        return "$\\partial_{"+str(self.symbol)+"}$"
+
+    __repr__ = _repr_latex_
+    _latex   = _repr_latex_
+    _print   = _repr_latex_
+
+class Tensor():
+    def __init__(self):
+        self.__sympy__ = True
+        self.comps_list = []
+        self.factors = []
+    
+    def __add__(self,other):
+        ret = Tensor()
+        ret.comps_list += self.comps_list
+        ret.factors += self.factors
+        if isinstance(other,Tensor):
+            ret.comps_list +=  (other.comps_list)
+            ret.factors += other.factors
+        elif isinstance(other,DifferentialForm):
+            if isinstance(other.symbol,Number):
+                ret.comps_list += [[DifferentialForm(Number(1),0,exact=True)]]
+                ret.factors += [other.symbol]
+            elif isinstance(other.symbol,AtomicExpr):
+                ret.comps_list += [[DifferentialForm(Number(1),0,exact=True)]]
+                ret.factors += [other.symbol]
+            else:
+                ret.comps_list += [[other]]
+                ret.factors += [Number(1)]
+        elif isinstance(other,VectorField):
+            ret.comps_list += [[other]]
+            ret.factors += [Number(1)]
+        elif isinstance(other,DifferentialFormMul):
+            #TODO: Convert differential form to tensor and add it on
+            pass
+        elif isinstance(other,float) or isinstance(other,int):
+            ret = self + DifferentialForm(Rational(other),0)
+        elif isinstance(other,AtomicExpr):
+            ret = self + DifferentialForm(other,0)
+        else:
+            raise NotImplementedError
+        
+    def __mull__(self,other):
+        #TODO: Implement this probably through TensorProduct(?)
+        pass
+
+    def _repr_latex_(self):
+        latex_str = "$" + "+".join([ "(" + remove_latex_arguments(self.factors[i]) + ")" + r" \otimes ".join([str(f) for f in self.comps_list[i]]) for i in range(len(self.comps_list))]) + "$"
+        if latex_str == "$$":
+            return "$0$"
+        return latex_str
+    
+    _sympystr = _repr_latex_
+
 class DifferentialForm():
     def __init__(self,symbol,degree=0, exact=False):
         """
         Class: Differential Form
 
         This is the basic class of this package. It holds all the information needed for a generic differential form.
         
         """
         self.degree = degree
         self.symbol = symbol
         self.exact = exact
         if degree < 0 or degree > MAX_DEGREE:
-            self.symbol = Number(0)
+            self.symbol = Ratioanl(0)
         
     def __eq__(self,other): return (self.symbol == other.symbol) and (self.degree == other.degree)
     def __hash__(self): return hash((str(self.symbol),self.degree))
 
-    def __mul__(self,other):
-        if isinstance(other,AtomicExpr):
-            return DifferentialFormMul(self,other)
-        elif isinstance(other,Expr):
-            return DifferentialFormMul(self,other)
-        elif isinstance(other,int):
-            return DifferentialFormMul(self,Number(other))
-        elif isinstance(other,float):
-            return DifferentialFormMul(self,Number(other))
-        elif isinstance(other,DifferentialForm):
-            ret = DifferentialFormMul()
-            ret.forms_list = [[self,other]]
-            ret.factors = [1]
+    def __mul__(self,other): return WedgeProduct(self,other)
+    def __rmul__(self,other): return WedgeProduct(other,self)
+    def __div__(self,other): return WedgeProduct(self,1/other)
 
-            ret.remove_squares()
-            ret.remove_above_top()
-            ret.sort_form_sums()
-            ret.collect_forms()
-            return ret
-        elif isinstance(other,DifferentialFormMul):
-            return DifferentialFormMul(self,1)*other
-        else:
-            raise NotImplementedError("Not implemented multiplication of type '"+str(type(self).__name__)+" * "+str(type(other).__name__)+"'")
-    
     def __add__(self,other):
         ret = DifferentialFormMul()
-        if isinstance(other,AtomicExpr):
-            ret.forms_list = [[self],[DifferentialForm(Integer(1),0)]]
-            ret.factors = [1,other]
-        elif isinstance(other,Expr):
-            ret.forms_list = [[self],[DifferentialForm(Integer(1),0)]]
-            ret.factors = [1,other]
-        elif isinstance(other,int):
-            ret.forms_list = [[self],[DifferentialForm(Integer(1),0)]]
-            ret.factors = [1,other]
-        elif isinstance(other,float):
+        if isinstance(other,AtomicExpr) or isinstance(other,float) or isinstance(other,int):
             ret.forms_list = [[self],[DifferentialForm(Integer(1),0)]]
             ret.factors = [1,other]
         elif isinstance(other,DifferentialForm):
             ret.forms_list = [[self],[other]]
             ret.factors = [1,1]
         elif isinstance(other,DifferentialFormMul):
             ret.forms_list = [[self]]+other.forms_list
@@ -108,35 +162,36 @@
         else:
             return (self.degree) < other.degree
 
     def __neg__(self): return DifferentialFormMul(self,-1)
     def __sub__(self,other): return self + (-other)
     def __rsub__(self,other): return (-self) + other
     def __radd__(self,other): return self + other
-    def __rmul__(self,other): return self * other
 
     def __str__(self):
         return latex(self.symbol)
 
-    def __repr__(self):
-        return self.symbol._repr_latex_()
-
     def _repr_latex_(self):
         return self.symbol._repr_latex_()
-
-    def _latex(self,printer):
-        return self._repr_latex_()
     
-    def _print(self):
-        return self._repr_latex_()
+    __repr__ = _repr_latex_
+    _latex   = _repr_latex_
+    _print   = _repr_latex_
     
     def __eq__(self,other):
         if isinstance(other,DifferentialForm):
             return str(self.symbol) == str(other.symbol) and self.degree == other.degree
     
+    def insert(self,vector:VectorField):
+        if isinstance(vector,VectorField):
+            if self.symbol == vector.symbol: return 1
+            else: return 0
+        else:
+            raise NotImplementedError
+
     @property
     def d(self):
         if self.exact: return DifferentialForm(Number(0),self.degree+1,exact=True)
         elif isinstance(self.symbol,Number): return DifferentialForm(Number(0),self.degree+1,exact=True)
         else:
             dsymbol = symbols(r"d\left("+str(self.symbol)+r"\right)")
             return DifferentialForm(dsymbol,degree=self.degree+1,exact=True)
@@ -155,146 +210,34 @@
         else:
             self.forms_list = [[form]]
             self.factors = [factor]
  
     def __add__(self,other):
         ret = DifferentialFormMul()
         if isinstance(other,DifferentialFormMul):
-            ret.forms_list += (self.forms_list)
-            ret.forms_list += (other.forms_list)
+            ret.forms_list += (self.forms_list) + (other.forms_list)
             ret.factors += self.factors + other.factors
-
-            ret.sort_form_sums()
-            ret.collect_forms()
-            return ret
         elif isinstance(other,DifferentialForm):
-            ret.forms_list += self.forms_list
-            ret.factors += self.factors
-            if isinstance(other.symbol,Number):
-                ret.forms_list += [[DifferentialForm(Number(1),0,exact=True)]]
-                ret.factors += [other.symbol]
-            elif isinstance(other.symbol,Expr):
-                ret.forms_list += [[DifferentialForm(Number(1),0,exact=True)]]
-                ret.factors += [other.symbol]
-            elif isinstance(other.symbol,AtomicExpr):
-                ret.forms_list += [[DifferentialForm(Number(1),0,exact=True)]]
-                ret.factors += [other.symbol]
-            else:
-                ret.forms_list += [[other]]
-                ret.factors += [1]
-            ret.collect_forms()
-            return ret
-        elif isinstance(other,int):
-            return self + DifferentialForm(Integer(other),0)
-        elif isinstance(other,float):
-            return self + DifferentialForm(Rational(other),0)
-        elif isinstance(other,AtomicExpr):
-            return self + DifferentialForm(other,0)
-        elif isinstance(other,Expr):
-            return self + DifferentialForm(other,0)
-        else:
-            raise NotImplementedError
-    
-    def __mul__(self,other):
-        ret = DifferentialFormMul()
-        if isinstance(other,int):
-            ret.forms_list = self.forms_list
-            ret.factors = [Integer(other)*f for f in self.factors]
-
-        elif isinstance(other,float):
-            ret.forms_list = self.forms_list
-            ret.factors = [Rational(other)*f for f in self.factors]
-
+            ret.forms_list += self.forms_list + [[other]]
+            ret.factors += self.factors + [1]
+        elif isinstance(other,(float,int)):
+            ret = self + DifferentialForm(Rational(other),0)
         elif isinstance(other,AtomicExpr):
-            ret.forms_list = self.forms_list
-            ret.factors = [(other)*f for f in self.factors]
-
-        elif isinstance(other,Expr):
-            ret.forms_list = self.forms_list
-            ret.factors = [(other)*f for f in self.factors]            
-
-        elif isinstance(other,DifferentialForm):
-            ret.forms_list = [fl+[other] for fl in self.forms_list]
-            ret.factors = self.factors
-
-            ret.remove_squares()
-            ret.remove_above_top()
-            ret.sort_form_sums()
-            ret.collect_forms()
-        
-        elif isinstance(other,DifferentialFormMul):
-            for i in range(len(self.forms_list)):
-                for j in range(len(other.forms_list)):
-                    ret.forms_list.append(self.forms_list[i]+other.forms_list[j])
-                    ret.factors.append(self.factors[i]*other.factors[j])
-
-            ret.remove_squares()
-            ret.remove_above_top()
-            ret.sort_form_sums()
-            ret.collect_forms()
+            ret = self + DifferentialForm(other,0)
         else:
             raise NotImplementedError
-        
-        ret.remove_squares()
-        ret.remove_above_top()
-        ret.sort_form_sums()
-        ret.collect_forms()
+        ret = simplify(ret)
 
         return ret
     
-    def __rmul__(self,other):
-        ret = DifferentialFormMul()
-        if isinstance(other,int):
-            ret.forms_list = self.forms_list
-            ret.factors = [Integer(other)*f for f in self.factors]
-
-        elif isinstance(other,float):
-            ret.forms_list = self.forms_list
-            ret.factors = [Rational(other)*f for f in self.factors]
-
-        elif isinstance(other,AtomicExpr):
-            ret.forms_list = self.forms_list
-            ret.factors = [(other)*f for f in self.factors]
-
-        elif isinstance(other,Expr):
-            ret.forms_list = self.forms_list
-            ret.factors = [(other)*f for f in self.factors]            
-
-        elif isinstance(other,DifferentialForm):
-            ret.forms_list = [[other]+fl for fl in self.forms_list]
-            ret.factors = self.factors
-
-            ret.remove_squares()
-            ret.remove_above_top()
-            ret.sort_form_sums()
-            ret.collect_forms()
-        elif isinstance(other,DifferentialFormMul):
-            for i in range(len(self.forms_list)):
-                for j in range(len(other.forms_list)):
-                    ret.forms_list.append(other.forms_list[j]+self.forms_list[i])
-                    ret.factors.append(self.factors[i]*other.factors[j])
-
-            ret.remove_squares()
-            ret.remove_above_top()
-            ret.sort_form_sums()
-            ret.collect_forms()
-        else:
-            raise NotImplementedError
-        
-            ret.remove_squares()
-            ret.remove_above_top()
-            ret.sort_form_sums()
-            ret.collect_forms()
-        return ret
-
-    def __div__(self,other):
-        return self*(1/other)
+    def __mul__(self,other): return WedgeProduct(self,other)
     
-    def __rdiv__(self,other):
-        return self*(1/other)
+    def __rmul__(self,other): return WedgeProduct(other,self)
+
+    def __div__(self,other): return WedgeProduct(self,(1/other))
 
     def __radd__(self,other): return self + other
     def __neg__(self):
         ret = DifferentialFormMul()
         ret.forms_list = self.forms_list
         ret.factors = [-f for f in self.factors]
         return ret
@@ -362,28 +305,24 @@
                 del new_forms_list[i]
                 del new_factors[i]
                 continue
             if len(new_forms_list[i]) > 1 and '1' in new_forms_strings:
                 new_forms_list[i].pop(new_forms_strings.index('1'))
             i+=1
 
-
-
-
         self.forms_list = new_forms_list
         self.factors = new_factors
             
     def _repr_latex_(self):
         latex_str = "$" + "+".join([ "(" + remove_latex_arguments(self.factors[i]) + ")" + r" \wedge ".join([str(f) for f in self.forms_list[i]]) for i in range(len(self.forms_list))]) + "$"
         if latex_str == "$$":
             return "$0$"
         return latex_str
     
-    def _sympystr(self,printer):
-        return self._repr_latex_()
+    _sympystr = _repr_latex_
 
     @property
     def d(self):
         ret = DifferentialFormMul()
         new_forms_list = []
         new_factors_list = []
         for i in range(len(self.forms_list)):
@@ -431,15 +370,17 @@
         if isinstance(target,DifferentialForm):
             new_forms_list = []
             new_factors_list = []
             for i in range(len(ret.forms_list)):
                 if target in ret.forms_list[i]:
                     j = ret.forms_list[i].index(target)
                     if isinstance(sub,DifferentialForm):
-                        new_forms_list +=[ret.forms_list[i][:j] + [sub] + ret.forms_list[i][j+1:]]
+                        print(ret.forms_list[i], sub)
+                        print([ret.forms_list[i][:j] + [sub] + ret.forms_list[i][j+1:]])
+                        new_forms_list += [ret.forms_list[i][:j] + [sub] + ret.forms_list[i][j+1:]]
                         new_factors_list.append(ret.factors[i])
                     elif isinstance(sub,DifferentialFormMul):
                         for k in range(len(sub.factors)):
                             s = sub.forms_list[k]
                             f = sub.factors[k]
                             new_forms_list+= [ret.forms_list[i][:j] + s + ret.forms_list[i][j+1:]]
                             new_factors_list.append(ret.factors[i]*f)
@@ -462,52 +403,127 @@
                         match_index = j
                         break
                 if match_index != -1:
                     if isinstance(sub,DifferentialFormMul):
                         for k in range(len(sub.factors)):
                             s = sub.forms_list[k]
                             f = sub.factors[k]
-                            new_forms_list += [ret.forms_list[i][:match_index] + s + ret.forms_list[i][match_index+len(target.forms_list)+1:]]
+                            new_forms_list += [ret.forms_list[i][:match_index] + s + ret.forms_list[i][match_index+len(target.forms_list[0])+1:]]
                             new_factors_list.append(ret.factors[i]*f/target.factors[0])
                     elif isinstance(sub,DifferentialForm):
-                        new_forms_list += [ret.forms_list[i][:match_index] + [sub] + ret.forms_list[i][match_index+len(target.forms_list):]]
+                        new_forms_list += [ret.forms_list[i][:match_index] + [sub] + ret.forms_list[i][match_index+len(target.forms_list[0]):]]
                         new_factors_list.append(ret.factors[i]/target.factors[0])
+                    elif isinstance(sub,float) or isinstance(sub,int) or isinstance(sub,AtomicExpr):
+                        new_forms_list +=[ret.forms_list[i][:match_index] + ret.forms_list[i][match_index+len(target.forms_list[0]):]]
+                        new_factors_list.append(ret.factors[i]*sub/target.factors[0])
                 else:
                     new_forms_list += [ret.forms_list[i]]
                     new_factors_list.append(ret.factors[i])
             ret.factors = new_factors_list
             ret.forms_list = new_forms_list
         elif isinstance(target,dict):
             for key in target:
                 ret = ret.subs(key,target[key])
 
         if not isinstance(sub,DifferentialForm) and not isinstance(sub,DifferentialFormMul) and sub != None:
             for i in range(len(self.factors)):
                     ret.factors[i] = ret.factors[i].subs(target,sub)
 
-        ret.remove_squares()
-        ret.remove_above_top()
-        ret.sort_form_sums()
-        ret.collect_forms()
+        ret = simplify(ret)
+        return ret
+
+    def insert(self,vect:VectorField):
+        ret = DifferentialFormMul()
+        if isinstance(vect,VectorField):
+            for i in range(len(self.factors)):
+                sign = 1
+                for j in range(len(self.forms_list[i])):
+                    if self.forms_list[i][j].symbol == vect.symbol:
+                        ret.forms_list += [self.forms_list[i][:j] + self.forms_list[i][j+1:]]
+                        ret.factors += [self.factors[i]*sign]
+                        break
+                    else:
+                        sign *= (-1)**self.forms_list[i][j].degree
+        else:
+            raise NotImplementedError
+        
+        return ret
+
+    def to_tensor(self):
+        ret = Tensor()
+        for i in range(len(self.factors)):
+            L = len(self.forms_list[i])
+            for perm in permutations(list(range(L)),L):
+                parity = (len(Permutation(perm).full_cyclic_form)-1)%2
+                ret.comps_list += [[self.forms_list[i][p] for p in perm]]
+                ret.factors += [(-1)**parity*self.factors[i]/factorial]
         return ret
-    
 
 
 def d(form):
-    if isinstance(form,DifferentialForm) or isinstance(form,DifferentialFormMul):
+    if isinstance(form,(DifferentialForm,DifferentialFormMul)):
         return form.d
-    elif isinstance(form,Expr):
+    
+    elif isinstance(form,AtomicExpr):
         ret = DifferentialFormMul()
         new_forms_list = []
         new_factors_list = []
         for f in form.free_symbols:
             dform = form.diff(f)
             if dform != 0:
                 new_forms_list += [[DifferentialForm(f,0).d]]
                 new_factors_list += [dform]
         
         ret.forms_list = new_forms_list
         ret.factors = new_factors_list
         return ret
-    elif isinstance(form,numbers.Number):
-        return 0
+
     raise NotImplementedError
+
+def WedgeProduct(left,right):
+    ret = DifferentialFormMul()
+    if isinstance(left,(int,float,Number)):
+        if isinstance(right,(int,float,Number)):
+            return left*right
+        elif isinstance(right,DifferentialForm):
+            ret.forms_list = [[right]]
+            ret.factors = [left]
+        elif isinstance(right,DifferentialFormMul):
+            ret.forms_list = right.forms_list
+            ret.factors = [left*f for f in right.factors]
+        else:
+            raise NotImplementedError
+    elif isinstance(left, DifferentialForm):
+        if isinstance(right,(int,float,Number)):
+            ret.forms_list = [[left]]
+            ret.factors = [right]
+        elif isinstance(right,DifferentialForm):
+            ret.forms_list = [[left,right]]
+            ret.factors = [1]
+        elif isinstance(right,DifferentialFormMul):
+            ret.forms_list = [[left]+rf for rf in right.forms_list]
+            ret.factors = right.factors
+        else:
+            raise NotImplementedError
+    elif isinstance(left,DifferentialFormMul):
+        if isinstance(right,(int,float,Number)):
+            ret.forms_list = left.forms_list
+            ret.factors = [right*f for f in left.factors]
+        elif isinstance(right,DifferentialForm):
+            ret.forms_list = [lf+[right] for lf in left.forms_list]
+            ret.factors = left.factors
+        elif isinstance(right,DifferentialFormMul):
+            for i in range(len(left.forms_list)):
+                for j in range(len(right.forms_list)):
+                    ret.forms_list.append(left.forms_list[i]+right.forms_list[j])
+                    ret.factors.append(left.factors[i]*right.factors[j])
+        else:
+            raise NotImplementedError
+    else:
+        raise NotImplementedError
+    
+    ret = simplify(ret)
+    return ret
+
+def TensorProduct(left,right):
+    ret = Tensor()
+    # TODO: Implement in similar way to WedgeProduct is implemented
```

### Comparing `diffforms-0.0.1/setup.py` & `diffforms-0.0.2/setup.py`

 * *Files identical despite different names*

