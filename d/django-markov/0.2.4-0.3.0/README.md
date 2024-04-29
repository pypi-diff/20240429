# Comparing `tmp/django_markov-0.2.4.tar.gz` & `tmp/django_markov-0.3.0.tar.gz`

## Comparing `django_markov-0.2.4.tar` & `django_markov-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/admin.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/apps.py
--rw-r--r--   0        0        0    13249 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/py.typed
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/text_models.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/urls.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/views.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0001_initial.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0003_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/settings.py
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/test_models.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/urls.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.4/.gitignore
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.4/LICENSE
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 django_markov-0.2.4/README.md
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 django_markov-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/admin.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/apps.py
+-rw-r--r--   0        0        0    19736 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/py.typed
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/text_models.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/urls.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/views.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/migrations/0003_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.3.0/src/django_markov/migrations/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 django_markov-0.3.0/tests/settings.py
+-rw-r--r--   0        0        0    12306 2020-02-02 00:00:00.000000 django_markov-0.3.0/tests/test_models.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.3.0/tests/urls.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 django_markov-0.3.0/README.md
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 django_markov-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 django_markov-0.3.0/PKG-INFO
```

### Comparing `django_markov-0.2.4/src/django_markov/models.py` & `django_markov-0.3.0/src/django_markov/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,14 +57,23 @@
         return 2
     return settings.MARKOV_STATE_SIZE
 
 
 STATE_SIZE = _get_default_state_size()
 
 
+def _get_default_compile_setting() -> bool:
+    """Get the default value from settings."""
+    if not hasattr(settings, "MARKOV_STORE_COMPILED_MODELS") or not isinstance(
+        settings.MARKOV_STORE_COMPILED_MODELS, bool
+    ):
+        return False
+    return settings.MARKOV_STORE_COMPILED_MODELS
+
+
 class MarkovTextModel(models.Model):
     """Stores a compiled markov text model.
 
     Attributes:
         created (datetime.datetime): Date and time when the model was created.
         modified (datetime.datetime): Date and time when the model was last modified.
         data (JSON): The text model as JSON.
@@ -144,42 +153,123 @@
         text_model = self._as_text_model()
         if not text_model:
             return None
         if text_model.chain.compiled:
             return text_model
         return text_model.compile(inplace=True)  # type: ignore
 
+    async def aadd_new_corpus_data_to_model(
+        self,
+        corpus_entries: list[str],
+        *,
+        char_limit: int | None = None,
+        weights: list[float] | None = None,
+    ) -> None:
+        """Takes a list of new corpus entries and incorporates them into the model.
+        Unlike `aupdate_model_from_corpus`, this method is additive. This works by
+        first creating a text model based on the new entries, and then uses
+        `markovify.combine` to add them to the existing text model. Note that
+        this will fail if the stored model is compiled.
+
+        Args:
+            corpus_entries (list[str]): A list of text sentences to add.
+            char_limit (int | None): The character limit to use for the new corpus.
+                Use `0` for no limit.
+            weights (list[float] | None): The weighting to use for combine
+                operation, the first value representing the saved model, and the second
+                representing the new entries.
+
+        Raises:
+            MarkovCombineError: If the stored model is already compiled.
+            MarkovEmptyError: If the new models are empty.
+        """
+        saved_model = self._as_text_model()
+        if self.data is None or self.data == "" or saved_model is None:
+            # There's no existing model, use update instead.
+            return await self.aupdate_model_from_corpus(
+                corpus_entries=corpus_entries, char_limit=char_limit
+            )
+        if char_limit is None:
+            char_limit = _get_corpus_char_limit()
+        if weights is not None and len(weights) != 2:  # noqa: PLR2004
+            msg = "If provided, weights must have exactly two entries!"
+            raise ValueError(msg)
+        corpus = " ".join(corpus_entries)
+        if len(corpus_entries) == 0 or corpus.replace(" ", "") == "":
+            msg = "There are no corpus entries to add!"
+            raise MarkovEmptyError(msg)
+        if saved_model.chain.compiled:
+            msg = "Saved model is compiled, cannot combine!"
+            raise MarkovCombineError(msg)
+        new_model = POSifiedText(corpus, state_size=saved_model.state_size)
+        try:
+            combined_model = markovify.combine(
+                [saved_model, new_model], weights=weights
+            )
+        except ValueError as ve:  # no cov
+            # If markovify raises any other unexpected error.
+            msg = f"The following error occurred while combining: {ve}"
+            raise MarkovCombineError(msg) from ve
+        if (
+            combined_model is not None and type(combined_model) is POSifiedText
+        ):  # no cov
+            self.data = combined_model.to_json()
+            await self.asave()
+
+    def add_new_corpus_data_to_model(
+        self,
+        corpus_entries: list[str],
+        *,
+        char_limit: int | None = None,
+        weights: list[float] | None = None,
+    ) -> None:
+        """Sync wrapper for `aadd_new_corpus_data_to_model`.
+
+        Args:
+            corpus_entries (list[str]): A list of text sentences to add.
+            char_limit (int | None): The character limit to use for the new corpus.
+                Use `0` for no limit.
+            weights (list[float] | None): The weighting to use for combine
+                operation, the first value representing the saved model, and the second
+                representing the new entries.
+
+        Raises:
+            MarkovCombineError: If the stored model is already compiled.
+            MarkovEmptyError: If the new models are empty.
+            ValueError: If weights are supplied, and they do not have a length of two.
+        """
+        return async_to_sync(self.aadd_new_corpus_data_to_model)(
+            corpus_entries=corpus_entries, char_limit=char_limit, weights=weights
+        )
+
     async def aupdate_model_from_corpus(
         self,
         corpus_entries: list[str],
         *,
         char_limit: int | None = None,
         store_compiled: bool | None = None,
     ) -> None:
-        """Takes the corpus and updates the model, saving it.
-        The corpus must not exceed the char_limit.
+        """Takes the a list of entries as the new full corpus and recreates the model,
+        saving it. The corpus must not exceed the char_limit.
 
         Args:
             corpus_entries (list[str]): The corpus as a list of text sentences.
             char_limit (int | None): The maximum number of characters
                 to allow in the corpus.
             store_compiled (bool | None): Whether to store the model in it's compiled
                 state. If None, defaults to settings.MARKOV_STORE_COMPILED_MODELS or
                 False.
+
+        Raises:
+            ValueError: If the corpus is beyond the maximum character limit.
         """
         if not char_limit:
             char_limit = _get_corpus_char_limit()
-        if (
-            store_compiled is None
-            and hasattr(settings, "MARKOV_STORE_COMPILED_MODELS")
-            and isinstance(settings.MARKOV_STORE_COMPILED_MODELS, bool)
-        ):
-            store_compiled = settings.MARKOV_STORE_COMPILED_MODELS
-        else:
-            store_compiled = False
+        if store_compiled is None:
+            store_compiled = _get_default_compile_setting()
         corpus = " ".join(corpus_entries)
         if char_limit != 0 and char_limit < len(corpus):
             msg = f"Supplied corpus is over the maximum character limit: {char_limit}"
             raise ValueError(msg)
         updated_model = POSifiedText(corpus, state_size=STATE_SIZE)
         if store_compiled:
             updated_model.compile(inplace=True)
@@ -189,15 +279,29 @@
     def update_model_from_corpus(
         self,
         corpus_entries: list[str],
         *,
         char_limit: int | None = None,
         store_compiled: bool | None = None,
     ) -> None:
-        """Sync wrapper for the async version"""
+        """Sync wrapper for the async version
+        Takes the a list of entries as the new full corpus and recreates the model,
+        saving it. The corpus must not exceed the char_limit.
+
+        Args:
+            corpus_entries (list[str]): The corpus as a list of text sentences.
+            char_limit (int | None): The maximum number of characters
+                to allow in the corpus.
+            store_compiled (bool | None): Whether to store the model in it's compiled
+                state. If None, defaults to settings.MARKOV_STORE_COMPILED_MODELS or
+                False.
+
+        Raises:
+            ValueError: If the corpus is beyond the maximum character limit.
+        """
         async_to_sync(self.aupdate_model_from_corpus)(  # no cov
             corpus_entries=corpus_entries,
             char_limit=char_limit,
             store_compiled=store_compiled,
         )
 
     def generate_sentence(self, char_limit: int = 0, tries: int = 0) -> str | None:
@@ -270,14 +374,19 @@
                 weights to put on each source. Optional, but can only be used with
                 mode='strict'.
 
         Returns:
             Either a new MarkovTextModel instance
                 persisted to the database or a POSifiedText object to manipulate at a
                 low level, and the total number of models combined.
+
+        Raises:
+            ValueError: If any of the parameter combinations is invalid
+            MarkovCombineError: If models are incompatible for combining or a markovify
+                error is raised.
         """
         # First we check to ensure that the models are combinable.
         empty_models = []
         compiled_models = []
         workable_models = []
         invalid_state_sizes = []
         if mode not in ["strict", "permissive"]:
@@ -344,11 +453,43 @@
         *,
         return_type: Literal["model_instance", "text_model"] = "model_instance",
         mode: Literal["strict", "permissive"] = "strict",
         weights: list[float] | None = None,
     ) -> tuple["MarkovTextModel | POSifiedText", int]:
         """
         Sync wrapper of acombine_models.
+
+        Combine multiple MarkovTextModels into a single model.
+
+        Models cannot be combined if any of the following is true:
+            - They are empty of data.
+            - They are stored in compiled state.
+            - The state size between models is not the same.
+            - The underlying text models are not the same type (if you subclass).
+            - You supply weights, but not the same number as the models to combine
+                or if you use permissive mode.
+
+        Args:
+            models (list[MarkovTextModel]): A list of MarkovTextModel instances to
+                combine.
+            return_type (Literal["model_instance", "text_model"]): The desired result
+                 type.
+            mode (Literal["strict", "permissive"]): strict indicates that an exception
+                should be raised if any of the candidate models are incompatible, or
+                if those specific instances should simply be dropped from the operation.
+            weights (list[float] | None): A list of floats representing the relative
+                weights to put on each source. Optional, but can only be used with
+                mode='strict'.
+
+        Returns:
+            Either a new MarkovTextModel instance
+                persisted to the database or a POSifiedText object to manipulate at a
+                low level, and the total number of models combined.
+
+        Raises:
+            ValueError: If any of the parameter combinations is invalid
+            MarkovCombineError: If models are incompatible for combining or a markovify
+                error is raised.
         """
         return async_to_sync(cls.acombine_models)(  # no cov
             models=models, return_type=return_type, mode=mode, weights=weights
         )
```

### Comparing `django_markov-0.2.4/src/django_markov/text_models.py` & `django_markov-0.3.0/src/django_markov/text_models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/src/django_markov/migrations/0001_initial.py` & `django_markov-0.3.0/src/django_markov/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py` & `django_markov-0.3.0/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/src/django_markov/migrations/0003_markovtextmodel_compiled.py` & `django_markov-0.3.0/src/django_markov/migrations/0003_markovtextmodel_compiled.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/tests/settings.py` & `django_markov-0.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/tests/test_models.py` & `django_markov-0.3.0/tests/test_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from faker import Faker
 
 from django_markov.models import (
     MarkovCombineError,
     MarkovEmptyError,
     MarkovTextModel,
     _get_corpus_char_limit,
+    _get_default_compile_setting,
     _get_default_state_size,
 )
 from django_markov.text_models import POSifiedText
 
 pytestmark = pytest.mark.django_db(transaction=True)
 
 
@@ -39,14 +40,25 @@
 
 
 def test_get_char_limit_missing_settings(settings):
     del settings.MARKOV_CORPUS_MAX_CHAR_LIMIT
     assert _get_corpus_char_limit() == 0  # Setting was not present
 
 
+@pytest.mark.parametrize("override_value", [False, True])
+def test_get_compile_default_setting(settings, override_value):
+    settings.MARKOV_STORE_COMPILED_MODELS = override_value
+    assert _get_default_compile_setting() == override_value
+
+
+def test_get_compile_default_missing_settings(settings):
+    del settings.MARKOV_STORE_COMPILED_MODELS
+    assert not _get_default_compile_setting()
+
+
 @pytest.mark.parametrize(
     "override_value,expected_result",
     [
         (None, 2),
         ("I'm a string!", 2),
         (3, 3),
     ],
@@ -280,7 +292,86 @@
         await clean_model.arefresh_from_db()
         models_to_combine.append(clean_model)
     result, total_combined = await MarkovTextModel.acombine_models(
         models=models_to_combine, mode=mode, return_type=result_type, weights=weights
     )
     assert isinstance(result, expected_result_type)
     assert total_combined == num_clean
+
+
+def test_add_data_to_compiled_model_raises_exception(
+    compiled_model, sample_corpus
+) -> None:
+    old_modify = compiled_model.modified
+    old_data = compiled_model.data
+    with pytest.raises(MarkovCombineError):
+        compiled_model.add_new_corpus_data_to_model(
+            [sample_corpus, "This is not going to work."]
+        )
+    compiled_model.refresh_from_db()
+    assert compiled_model.modified == old_modify
+    assert compiled_model.data == old_data
+
+
+@pytest.mark.parametrize(
+    "corpus_entries,char_limit,weights,expected_exception",
+    [
+        ([], None, None, MarkovEmptyError),
+        ([], None, [1.0, 1.0], MarkovEmptyError),
+        (["I like springtime.", "Does this bring joy?"], None, [1.0], ValueError),
+        (["I like springtime.", "Does this bring joy?"], 0, [], ValueError),
+        (
+            ["I like springtime.", "Does this bring joy?"],
+            None,
+            [1.0, 1.3, 1.0],
+            ValueError,
+        ),
+    ],
+)
+def test_add_data_to_model_invocation_failures(
+    text_model, sample_corpus, corpus_entries, char_limit, weights, expected_exception
+):
+    text_model.update_model_from_corpus([sample_corpus], store_compiled=False)
+    text_model.refresh_from_db()
+    old_data = text_model.data
+    old_modify = text_model.modified
+    with pytest.raises(expected_exception):
+        text_model.add_new_corpus_data_to_model(
+            corpus_entries=corpus_entries, weights=weights
+        )
+    text_model.refresh_from_db()
+    assert text_model.modified == old_modify
+    assert text_model.data == old_data
+
+
+@pytest.mark.parametrize(
+    "corpus_entries,char_limit,weights",
+    [
+        (["I like springtime.", "Does this bring joy?"], None, None),
+        (["I like springtime.", "Does this bring joy?"], 0, None),
+        (["I like springtime.", "Does this bring joy?"], None, [1.0, 1.0]),
+    ],
+)
+def test_add_data_to_model_success(
+    text_model, sample_corpus, corpus_entries, char_limit, weights
+):
+    text_model.update_model_from_corpus([sample_corpus], store_compiled=False)
+    text_model.refresh_from_db()
+    old_data = text_model.data
+    old_modify = text_model.modified
+    text_model.add_new_corpus_data_to_model(
+        corpus_entries=corpus_entries, char_limit=char_limit, weights=weights
+    )
+    text_model.refresh_from_db()
+    assert text_model.data != old_data
+    assert text_model.modified > old_modify
+
+
+def test_add_data_to_empty_model_falls_back_to_update(text_model):
+    assert not text_model.data
+    old_modify = text_model.modified
+    text_model.add_new_corpus_data_to_model(
+        corpus_entries=["I like springtime.", "Does this bring joy?"]
+    )
+    text_model.refresh_from_db()
+    assert text_model.data is not None
+    assert text_model.modified > old_modify
```

### Comparing `django_markov-0.2.4/tests/urls.py` & `django_markov-0.3.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/LICENSE` & `django_markov-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.4/README.md` & `django_markov-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -108,14 +108,28 @@
             "Prepare to die.",
         ],
         char_limit=0,  # Unlimited
     )
     return text_model
 ```
 
+You can also later add to that model with new entries, as long as you haven't stored it in a compiled state.
+
+```python
+from django_markov.models import MarkovTextModel
+
+my_markov_model_instance = MarkovTextModel.objects.first()
+my_markov_model_instance.add_new_corpus_data_to_model(
+    corpus_entries=[
+        "I like burgers and fries.",
+        "I once ate a pickle larger than my hand.",
+    ]
+)
+```
+
 Once you have a model initialized, you can have it generate a sentence. For example,
 say that you have a text model in your database already, and you want a sentence generated.
 
 ```python
 from django_markov.models import MarkovTextModel
```

### Comparing `django_markov-0.2.4/pyproject.toml` & `django_markov-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-markov"
-version = "0.2.4"
+version = "0.3.0"
 description = "django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences."
 authors = [
     { name = "Daniel Andrlik", email = "daniel@andrlik.org" }
 ]
 dependencies = [
     "django>=4.2",
     "markovify>=0.9.4",
@@ -70,14 +70,15 @@
     "django-coverage-plugin>=3.1.0",
     "argon2-cffi>=23.1.0",
     "django-environ>=0.11.2",
     "django-extensions>=3.2.3",
     "pytest-mock>=3.14.0",
     "faker>=24.4.0",
     "bandit[toml]>=1.7.8",
+    "mike>=2.0.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/django_markov"]
@@ -224,15 +225,15 @@
   "--reuse-db"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.bumpversion]
-current_version = "0.2.4"
+current_version = "0.3.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_markov-0.2.4/PKG-INFO` & `django_markov-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-markov
-Version: 0.2.4
+Version: 0.3.0
 Summary: django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences.
 Project-URL: Repository, https://github.com/andrlik/django-markov
 Project-URL: Documentation, https://andrlik.github.io/django-markov
 Project-URL: Homepage, https://andrlik.github.io/django-markov
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
@@ -141,14 +141,28 @@
             "Prepare to die.",
         ],
         char_limit=0,  # Unlimited
     )
     return text_model
 ```
 
+You can also later add to that model with new entries, as long as you haven't stored it in a compiled state.
+
+```python
+from django_markov.models import MarkovTextModel
+
+my_markov_model_instance = MarkovTextModel.objects.first()
+my_markov_model_instance.add_new_corpus_data_to_model(
+    corpus_entries=[
+        "I like burgers and fries.",
+        "I once ate a pickle larger than my hand.",
+    ]
+)
+```
+
 Once you have a model initialized, you can have it generate a sentence. For example,
 say that you have a text model in your database already, and you want a sentence generated.
 
 ```python
 from django_markov.models import MarkovTextModel
```

