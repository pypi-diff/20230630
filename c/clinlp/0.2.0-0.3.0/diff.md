# Comparing `tmp/clinlp-0.2.0.tar.gz` & `tmp/clinlp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.2.0.tar", max compression
+gzip compressed data, was "clinlp-0.3.0.tar", max compression
```

## Comparing `clinlp-0.2.0.tar` & `clinlp-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-06-07 14:24:05.405783 clinlp-0.2.0/LICENSE
--rw-r--r--   0        0        0     8573 2023-06-07 14:24:05.405783 clinlp-0.2.0/README.md
--rw-r--r--   0        0        0       54 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/__init__.py
--rw-r--r--   0        0        0      285 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/__init__.py
--rw-r--r--   0        0        0     1403 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/normalizer.py
--rw-r--r--   0        0        0    10756 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/qualifier.py
--rw-r--r--   0        0        0     2308 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/sentencizer.py
--rw-r--r--   0        0        0     8447 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/language.py
--rw-r--r--   0        0        0        0 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/resources/__init__.py
--rw-r--r--   0        0        0    24446 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/resources/psynlp_context_rules.json
--rw-r--r--   0        0        0      547 2023-06-07 14:24:05.405783 clinlp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9131 1970-01-01 00:00:00.000000 clinlp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-30 10:48:23.948456 clinlp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9454 2023-06-30 10:48:23.948456 clinlp-0.3.0/README.md
+-rw-r--r--   0        0        0      162 2023-06-30 10:48:23.948456 clinlp-0.3.0/clinlp/__init__.py
+-rw-r--r--   0        0        0     8597 2023-06-30 10:48:23.948456 clinlp-0.3.0/clinlp/language.py
+-rw-r--r--   0        0        0     1603 2023-06-30 10:48:23.948456 clinlp-0.3.0/clinlp/normalizer.py
+-rw-r--r--   0        0        0      197 2023-06-30 10:48:23.948456 clinlp-0.3.0/clinlp/qualifier/__init__.py
+-rw-r--r--   0        0        0    11580 2023-06-30 10:48:23.948456 clinlp-0.3.0/clinlp/qualifier/context_algorithm.py
+-rw-r--r--   0        0        0      975 2023-06-30 10:48:23.952451 clinlp-0.3.0/clinlp/qualifier/qualifier.py
+-rw-r--r--   0        0        0     4374 2023-06-30 10:48:23.952451 clinlp-0.3.0/clinlp/qualifier/transformer.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:48:23.952451 clinlp-0.3.0/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    24490 2023-06-30 10:48:23.952451 clinlp-0.3.0/clinlp/resources/psynlp_context_rules.json
+-rw-r--r--   0        0        0     2272 2023-06-30 10:48:23.952451 clinlp-0.3.0/clinlp/sentencizer.py
+-rw-r--r--   0        0        0     1815 2023-06-30 10:48:23.952451 clinlp-0.3.0/clinlp/util.py
+-rw-r--r--   0        0        0      677 2023-06-30 10:48:23.952451 clinlp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 clinlp-0.3.0/PKG-INFO
```

### Comparing `clinlp-0.2.0/LICENSE` & `clinlp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.2.0/README.md` & `clinlp-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ]
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 
 # Qualifiers
-nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
+nlp.add_pipe('clinlp_context_algorithm', config={'phrase_matcher_attr': 'NORM'})
 
 text = (
     "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
     "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
     "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
@@ -92,15 +92,17 @@
 
 Currently, `clinlp` offers the following components, tailored to Dutch Clinical text, further discussed below: 
 
 1. [Tokenizer](#tokenizer)
 2. [Normalizer](#normalizer)
 3. [Sentence splitter](#sentence-splitter)
 4. [Entity matcher (builtin Spacy)](#entity-matcher)
-5. [Context detection](#context-detection)
+5. [Qualifier detection (=context)](#qualifier-detection)
+    - [Context Algorithm](#context-algorithm)
+    - [Transformer based negation detection](#transformer-based-negation-detection)
 
 ### Tokenizer
 
 The `clinlp` tokenizer is built into the blank model:
 
 ```python
 nlp = spacy.blank('clinlp')
@@ -155,33 +157,51 @@
 For more info, it's useful to check out these spaCy documentation pages:
 * [Rule based matching](https://spacy.io/usage/rule-based-matching)
 * [[spaCy API] Matcher](https://spacy.io/api/matcher)
 * [[spaCy API] PhraseMatcher](https://spacy.io/api/phrasematcher)
 
 Note that the `DependencyMatcher` cannot be used, and neither are part of speech tags available, as no good models for determining this information for clinical text exist (yet).  
 
-### Context detection
+### Qualifier detection
 
-After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) for this purpose. This algorithm is fairly accurate, and quite transparent and fast. Better solutions will hopefully be added to `clinlp` in the future. 
+After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002), and a [transformer-based negation detector](https://doi.org/10.48550/arxiv.2209.00470). 
 
-A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
+#### Context Algorithm
+
+The rule-based Context Algorithm is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
 
 ```python
-nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
+nlp.add_pipe('clinlp_context_algorithm', config={'phrase_matcher_attr': 'NORM'})
 ```
 
-A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows: 
+A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows:
 
 ```python
-from clinlp.component.qualifier import parse_rules
+cm = nlp.add_pipe('clinlp_context_algorithm', config={'rules': '/path/to/my_own_ruleset.json'})
+```
+
+#### Transformer based negation detection
 
-cm = nlp.add_pipe('clinlp_context_matcher', config={'default_rules': None})
-cm.add_rules(parse_rules('my_custom_rules.json'))
+`clinlp` also includes a wrapper around the transformer based negation detector, as described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformer can be found on [huggingface](https://huggingface.co/UMCU/MedRoBERTa.nl_NegationDetection). It is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
+
+First, install the additional dependencies:
+
+```bash
+pip install "clinlp[transformers]"
 ```
 
+Then add it using:
+
+```python
+tn = nlp.add_pipe('clinlp_negation_transformer')
+```
+
+Some configuration options, like the number of tokens to consider, can be specified in the `config` argument. 
+
+
 ### Where to go from here
 
 We hope to extend `clinlp` with new functionality and more complete documentation in the near future. In the meantime, if any questions or problems arise, we recommend:
 
 * Checking the source code 
 * Getting in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new))
```

### Comparing `clinlp-0.2.0/clinlp/component/normalizer.py` & `clinlp-0.3.0/clinlp/normalizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import unicodedata
 
-import spacy
 from spacy import Language
 from spacy.tokens import Doc
 
+from clinlp.util import clinlp_autocomponent
 
-@spacy.language.Language.factory(
-    "clinlp_normalizer",
-    assigns=["token.norm"],
-    default_config={"lowercase": True, "map_non_ascii": True},
-)
+_defaults_normalizer = {"lowercase": True, "map_non_ascii": True}
+
+
+@Language.factory("clinlp_normalizer", assigns=["token.norm"], default_config=_defaults_normalizer)
+@clinlp_autocomponent
 class Normalizer:
-    def __init__(self, nlp: Language, name: str, lowercase=True, map_non_ascii=True):
+    def __init__(
+        self, lowercase=_defaults_normalizer["lowercase"], map_non_ascii=_defaults_normalizer["map_non_ascii"]
+    ):
         self.lowercase = lowercase
         self.map_non_ascii = map_non_ascii
 
     @staticmethod
     def _lowercase(text: str) -> str:
         return text.lower()
 
     @staticmethod
     def _map_non_ascii_char(char: str) -> str:
-        """
-        TODO: What if there's a non-mappable ascii (µ) and a mappable (é) in the same string?
-        """
+        if len(char) != 1:
+            raise ValueError("Please only use the _map_non_ascii_char method on strings of length 1.")
 
-        s = unicodedata.normalize("NFD", char)
-        s = str(s.encode("ascii", "ignore").decode("utf-8"))
+        normalized_char = unicodedata.normalize("NFD", char)
+        normalized_char = str(normalized_char.encode("ascii", "ignore").decode("utf-8"))
 
-        return s if len(s) > 0 else char
+        return normalized_char if len(normalized_char) > 0 else char
 
     def _map_non_ascii_string(self, text: str) -> str:
         return "".join(self._map_non_ascii_char(char) for char in text)
 
     def __call__(self, doc: Doc):
         if len(doc) == 0:
             return doc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `clinlp-0.2.0/clinlp/component/qualifier.py` & `clinlp-0.3.0/clinlp/qualifier/context_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-""" Implements qualifier detection for entities. The Qualifier class is reusable. The other classes implement
-the context algorithm (https://doi.org/10.1016%2Fj.jbi.2009.05.002) """
-
 import importlib
 import itertools
 import json
 import re
 import warnings
 from collections import defaultdict
 from dataclasses import dataclass
@@ -12,180 +9,125 @@
 from typing import Iterator, Optional, Union
 
 import intervaltree as ivt
 from spacy.language import Language
 from spacy.matcher import Matcher, PhraseMatcher
 from spacy.tokens import Doc, Span
 
-QUALIFIERS_ATTR = "qualifiers"
-PHRASE_MATCHER_ATTR = "TEXT"
-
-DEFAULT_CONTEXT_RULES = "psynlp_context_rules.json"
-
-
-class Qualifier(Enum):
-    """
-    A qualifier modifies an entity (e.g. negation, temporality, plausibility, etc.).
-    """
-
-    ...
+from clinlp.qualifier.qualifier import QUALIFIERS_ATTR, Qualifier, QualifierDetector
+from clinlp.util import clinlp_autocomponent
 
 
 class ContextRuleDirection(Enum):
     """
-    Direction of a Context rule, as in the original algorithm.
+    Direction of a Context rule, as in the original Context Algorithm.
     """
 
     PRECEDING = 1
     FOLLOWING = 2
     PSEUDO = 3
     TERMINATION = 4
 
 
 @dataclass
 class ContextRule:
     """
-    A Context rule, as in the original algorithm.
+    A Context rule, as in the original Context Algorithm.
 
     Args:
-        pattern: The pattern to look for in text, either a string, or a spacy pattern (list).
-        qualifier: The qualifier to modify.
-        direction: The context rule direction.
-
+        pattern: The pattern to look for in text. Either a string, or a spacy pattern (list).
+        qualifier: The qualifier to apply.
+        direction: The Context rule direction.
+        max_scope: The maximum scope (number of tokens) of the trigger, or None for using sentence boundaries.
     """
 
     pattern: Union[str, list[dict[str, str]]]
     qualifier: Qualifier
     direction: ContextRuleDirection
+    max_scope: Optional[int] = None
 
 
 class _MatchedContextPattern:
     """
-    A matched context pattern, that should be processed further.
+    A matched Context pattern, that should be processed further.
     """
 
     def __init__(self, rule: ContextRule, start: int, end: int, offset: int = 0):
         self.rule = rule
         self.start = start + offset
         self.end = end + offset
         self.scope = None
 
-    def set_initial_scope(self, sentence: Span):
-        if self.rule.direction == ContextRuleDirection.PRECEDING:
-            self.scope = (self.start, sentence.end)
-
-        elif self.rule.direction == ContextRuleDirection.FOLLOWING:
-            self.scope = (sentence.start, self.end)
-
-
-def _parse_qualifier(qualifier: str, qualifier_classes: dict[str, Qualifier]) -> Qualifier:
-    """
-    Parse a Qualifier from string.
-
-    Args:
-        qualifier: The qualifier (e.g. Negation.NEGATED).
-        qualifier_classes: A mapping of string to qualifier class.
-
-    Returns: A qualifier, as specified.
-    """
-
-    match_regexp = r"\w+\.\w+"
-
-    if not re.match(match_regexp, qualifier):
-        raise ValueError(
-            f"Cannot parse qualifier {qualifier}, please adhere to format "
-            f"{match_regexp} (e.g. NegationQualifier.NEGATED)"
-        )
-
-    qualifier_class, qualifier = qualifier.split(".")
-
-    return qualifier_classes[qualifier_class][qualifier]
-
-
-def _parse_direction(direction: str) -> ContextRuleDirection:
-    """
-    Parse a Context direction.
-
-    Args:
-        direction: The direction.
-
-    Returns: THe ContextRuleDirection.
-    """
-    return ContextRuleDirection[direction.upper()]
-
-
-def parse_rules(input_json: Optional[str] = None, data: Optional[dict] = None) -> list[ContextRule]:
-    if input_json and data:
-        raise ValueError(
-            "Please choose either input_json to load data from json, " "or provide data as dict, but not both."
-        )
+    def initialize_scope(self, sentence: Span):
+        """
+        Sets the scope this pattern ranges over, based on the sentence. This is either the window determined in
+        the `max_scope` of the rule, or the sentence boundaries if no `max_scope` is set.
+        """
 
-    if input_json:
-        with open(input_json, "rb") as file:
-            data = json.load(file)
+        max_scope = self.rule.max_scope or len(sentence)
 
-    qualifiers = {
-        qualifier["qualifier"]: Qualifier(qualifier["qualifier"], qualifier["levels"])
-        for qualifier in data["qualifiers"]
-    }
+        if max_scope < 1:
+            raise ValueError(f"max_scope must be at least 1, but got {max_scope}")
 
-    qualifier_rules = []
+        if self.rule.direction == ContextRuleDirection.PRECEDING:
+            self.scope = (self.start, min(self.end + max_scope, sentence.end))
 
-    for rule in data["rules"]:
-        qualifier = _parse_qualifier(rule["qualifier"], qualifiers)
-        direction = _parse_direction(rule["direction"])
+        elif self.rule.direction == ContextRuleDirection.FOLLOWING:
+            self.scope = (max(self.start - max_scope, sentence.start), self.end)
 
-        qualifier_rules += [ContextRule(pattern, qualifier, direction) for pattern in rule["patterns"]]
 
-    return qualifier_rules
+_defaults_context_algorithm = {
+    "phrase_matcher_attr": "TEXT",
+    "load_rules": True,
+    "rules": str(importlib.resources.path("clinlp.resources", "psynlp_context_rules.json")),
+}
 
 
 @Language.factory(
-    name="clinlp_context_matcher",
-    default_config={"phrase_matcher_attr": PHRASE_MATCHER_ATTR, "rules": None},
+    name="clinlp_context_algorithm",
     requires=["doc.sents", "doc.ents"],
+    assigns=[f"span._.{QUALIFIERS_ATTR}"],
+    default_config=_defaults_context_algorithm,
 )
-class ContextMatcher:
+@clinlp_autocomponent
+class ContextAlgorithm(QualifierDetector):
     """
-    Implements a very simple version of the context algorithm.
+    Implements the Context algorithm (https://doi.org/10.1016%2Fj.jbi.2009.05.002) as a spaCy pipeline component.
 
     Args:
         nlp: The Spacy language object to use
-        name: The name of the component
         phrase_matcher_attr: The token attribute to match phrases on (e.g. TEXT, ORTH, NORM).
-        default_rules: A filename in clinlp.resources with a set of rules to load by default
-        rules: A list of ContextRule
+        load_rules: Whether to parse any rules. Set this to `False` to use ContextAlgorithm.add_rules to
+        rules: A dictionary of rules, or a path to a json containing the rules (see clinlp.resources dir for example).
+        add ContextRules manually.
     """
 
     def __init__(
         self,
         nlp: Language,
-        name: str,
-        phrase_matcher_attr: str = PHRASE_MATCHER_ATTR,
-        default_rules: Optional[str] = DEFAULT_CONTEXT_RULES,
-        rules: Optional[list[ContextRule]] = None,
+        phrase_matcher_attr: str = _defaults_context_algorithm["phrase_matcher_attr"],
+        load_rules=_defaults_context_algorithm["load_rules"],
+        rules: Optional[Union[str | dict]] = _defaults_context_algorithm["rules"],
     ):
         self._nlp = nlp
-        self.name = name
 
         self._matcher = Matcher(self._nlp.vocab, validate=True)
         self._phrase_matcher = PhraseMatcher(self._nlp.vocab, attr=phrase_matcher_attr)
 
         self.rules = {}
 
-        if default_rules is not None:
-            self._load_default_rules(default_rules)
+        if load_rules:
+            if rules is None:
+                raise ValueError(
+                    "Did not provide rules. Set `load_rules` to False if you want to add `ContextRule` manually."
+                )
 
-        if rules:
+            rules = self._parse_rules(rules)
             self.add_rules(rules)
 
-    def _load_default_rules(self, default_rules: str):
-        with importlib.resources.path("clinlp.resources", default_rules) as path:
-            self.add_rules(parse_rules(path))
-
     def add_rule(self, rule: ContextRule):
         """
         Add a rule.
         """
         rule_key = f"rule_{len(self.rules)}"
         self.rules[rule_key] = rule
 
@@ -201,16 +143,70 @@
     def add_rules(self, rules: list[ContextRule]):
         """
         Add multiple rules.
         """
         for rule in rules:
             self.add_rule(rule)
 
-    def __len__(self):
-        return len(self.rules)
+    @staticmethod
+    def _parse_qualifier(qualifier: str, qualifier_classes: dict[str, Qualifier]) -> Qualifier:
+        """
+        Parse a Qualifier from string.
+
+        Args:
+            qualifier: The qualifier (e.g. Negation.NEGATED).
+            qualifier_classes: A mapping of string to qualifier class.
+
+        Returns: A qualifier, as specified.
+        """
+
+        match_regexp = r"\w+\.\w+"
+
+        if not re.match(match_regexp, qualifier):
+            raise ValueError(
+                f"Cannot parse qualifier {qualifier}, please adhere to format "
+                f"{match_regexp} (e.g. NegationQualifier.NEGATED)"
+            )
+
+        qualifier_class, qualifier = qualifier.split(".")
+
+        return qualifier_classes[qualifier_class][qualifier]
+
+    @staticmethod
+    def _parse_direction(direction: str) -> ContextRuleDirection:
+        """
+        Parse a Context direction.
+
+        Args:
+            direction: The direction (e.g. preceding, following, etc.).
+
+        Returns: THe ContextRuleDirection.
+        """
+        return ContextRuleDirection[direction.upper()]
+
+    def _parse_rules(self, rules: Union[str | dict]) -> list[ContextRule]:
+        if isinstance(rules, str):
+            with open(rules, "rb") as file:
+                rules = json.load(file)
+
+        qualifiers = {
+            qualifier["qualifier"]: Qualifier(qualifier["qualifier"], qualifier["values"])
+            for qualifier in rules["qualifiers"]
+        }
+
+        qualifier_rules = []
+
+        for rule in rules["rules"]:
+            qualifier = self._parse_qualifier(rule["qualifier"], qualifiers)
+            direction = self._parse_direction(rule["direction"])
+            max_scope = rule.get("max_scope", None)
+
+            qualifier_rules += [ContextRule(pattern, qualifier, direction, max_scope) for pattern in rule["patterns"]]
+
+        return qualifier_rules
 
     @staticmethod
     def _get_sentences_having_entity(doc: Doc) -> Iterator[Span]:
         """
         Return sentences in a doc that have at least one entity.
         """
         return (sent for sent in doc.sents if len(sent.ents) > 0)
@@ -225,15 +221,17 @@
     def _group_matched_patterns(matched_patterns: list[_MatchedContextPattern]) -> defaultdict:
         """
         Group matched patterns by qualifier and direction.
         """
         groups = defaultdict(lambda: defaultdict(list))
 
         for matched_rule in matched_patterns:
-            groups[matched_rule.rule.qualifier][matched_rule.rule.direction.name].append(matched_rule)
+            groups[matched_rule.rule.qualifier][matched_rule.rule.direction.name].append(
+                matched_rule
+            )  # TODO: don't use name?
 
         return groups
 
     @staticmethod
     def _limit_scopes_from_terminations(
         scopes: ivt.IntervalTree, terminations: list[_MatchedContextPattern]
     ) -> ivt.IntervalTree:
@@ -283,22 +281,19 @@
                 ivt.Interval(i.data.scope[0], i.data.scope[1], i.data) for i in qualifier_matches
             )
 
             match_scopes |= self._limit_scopes_from_terminations(qualifier_scopes, termination_)
 
         return match_scopes
 
-    def __call__(self, doc: Doc):
+    def detect_qualifiers(self, doc: Doc):
         """
-        Apply the context matcher to a doc.
+        Apply the Context Algorithm to a doc.
         """
 
-        if len(doc.ents) == 0:
-            return doc
-
         if len(self.rules) == 0:
             raise RuntimeError("Cannot match qualifiers without any ContextRule.")
 
         for sentence in self._get_sentences_having_entity(doc):
             with warnings.catch_warnings():
                 # a UserWarning will trigger when one of the matchers is empty
                 warnings.simplefilter("ignore", UserWarning)
@@ -313,21 +308,21 @@
                 # spacy Matcher handles offset differently than PhraseMatcher, when applying the matcher to a sentence
                 offset = sentence.start if isinstance(rule.pattern, list) else 0
 
                 pattern = _MatchedContextPattern(
                     rule=self._get_rule_from_match_id(match_id), start=start, end=end, offset=offset
                 )
 
-                pattern.set_initial_scope(sentence)
+                pattern.initialize_scope(sentence)
                 matched_patterns.append(pattern)
 
             match_scopes = self._compute_match_scopes(matched_patterns)
 
             for ent in sentence.ents:
-                qualifiers = set()
-
                 for match_interval in match_scopes.overlap(ent.start, ent.end):
-                    qualifiers.add(str(match_interval.data.rule.qualifier))
-
-                ent._.set(QUALIFIERS_ATTR, qualifiers)
+                    if (ent.start + 1 > match_interval.data.end) or (ent.end < match_interval.data.start + 1):
+                        self.add_qualifier_to_ent(ent, match_interval.data.rule.qualifier)
 
         return doc
+
+    def __len__(self):
+        return len(self.rules)
```

### Comparing `clinlp-0.2.0/clinlp/component/sentencizer.py` & `clinlp-0.3.0/clinlp/sentencizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from typing import Optional
 
 import spacy.tokens
 from spacy.language import Language
 
-DEFAULT_SENT_ENT_CHARS = [".", "!", "?", "\n", "\r"]
-DEFAULT_SENT_START_PUNCT = ["-", "*", "[", "("]
+from clinlp.util import clinlp_autocomponent
 
+_defaults_sentencizer = {"sent_end_chars": [".", "!", "?", "\n", "\r"], "sent_start_punct": ["-", "*", "[", "("]}
 
-@spacy.language.Language.factory(
-    "clinlp_sentencizer",
-    assigns=["token.is_sent_start", "doc.sents"],
-    default_config={"sent_end_chars": DEFAULT_SENT_ENT_CHARS, "sent_start_punct": DEFAULT_SENT_START_PUNCT},
+
+@Language.factory(
+    "clinlp_sentencizer", assigns=["token.is_sent_start", "doc.sents"], default_config=_defaults_sentencizer
 )
+@clinlp_autocomponent
 class Sentencizer:
     def __init__(
         self,
-        nlp: Language,
-        name="clinlp_sentencizer",
         sent_end_chars: Optional[list[str]] = None,
         sent_start_punct: Optional[list[str]] = None,
     ):
-        self.name = name
-
-        self.sent_end_chars = DEFAULT_SENT_ENT_CHARS if sent_end_chars is None else sent_end_chars
-        self.sent_start_punct = DEFAULT_SENT_START_PUNCT if sent_start_punct is None else sent_start_punct
+        self.sent_end_chars = _defaults_sentencizer["sent_end_chars"] if sent_end_chars is None else sent_end_chars
+        self.sent_start_punct = (
+            _defaults_sentencizer["sent_start_punct"] if sent_start_punct is None else sent_start_punct
+        )
 
         self.sent_end_chars = set(self.sent_end_chars)
         self.sent_start_punct = set(self.sent_start_punct)
 
     def _token_can_start_sent(self, token: spacy.tokens.Token) -> bool:
         """
         Determines whether a token can start a sentence
```

### Comparing `clinlp-0.2.0/clinlp/language.py` & `clinlp-0.3.0/clinlp/language.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     "wv.",
     "pol.",
     "tr.",
     "vv.",
     "mi.",
 ]
 
+CLINLP_REMOVE_ABBREVIATIONS = [
+    "ts.",
+]
+
 CLINLP_UNITS = [
     "cc",
     "CC",
     "l",
     "L",
     "ml",
     "mL",
@@ -229,15 +233,20 @@
 
 ALPHA_LOWER = "a-z"
 ALPHA_UPPER = "A-Z"
 ALPHA = "a-zA-Z"
 
 
 def _get_abbreviations():
-    return spacy.lang.nl.tokenizer_exceptions.abbrevs.copy() + CLINLP_ABBREVIATIONS
+    base = set(spacy.lang.nl.tokenizer_exceptions.abbrevs.copy())
+
+    for abbrev in CLINLP_REMOVE_ABBREVIATIONS:
+        base.remove(abbrev)
+
+    return list(base) + CLINLP_ABBREVIATIONS
 
 
 def _get_tokenizer_exceptions(
     abbreviations: list[str],
     abbrev_transforms: list[Callable[[str], str]] = None,
     keep_emoticons: bool = False,
 ):
```

### Comparing `clinlp-0.2.0/clinlp/resources/psynlp_context_rules.json` & `clinlp-0.3.0/clinlp/resources/psynlp_context_rules.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9127604166666666%*

 * *Differences: {"'qualifiers'": "{0: {'values': ['PATIENT', 'OTHER'], delete: ['levels']}, 1: {'values': "*

 * *                 "['AFFIRMED', 'NEGATED'], delete: ['levels']}, 2: {'values': ['PLAUSIBLE', "*

 * *                 "'HYPOTHETICAL'], delete: ['levels']}, 3: {'values': ['CURRENT', 'HISTORICAL'], "*

 * *                 "delete: ['levels']}}",*

 * * "'rules'": "{4: {'max_scope': 5}, 5: {'max_scope': 5}}"}*

```diff
@@ -1,38 +1,38 @@
 {
     "description": "A set of context rules based on the psynlp package, a rule-based approach somewhat tailored to information extraction from clinical text.",
     "name": "default_qualifiers",
     "qualifiers": [
         {
-            "levels": [
+            "qualifier": "Experiencer",
+            "values": [
                 "PATIENT",
                 "OTHER"
-            ],
-            "qualifier": "Experiencer"
+            ]
         },
         {
-            "levels": [
+            "qualifier": "Negation",
+            "values": [
                 "AFFIRMED",
                 "NEGATED"
-            ],
-            "qualifier": "Negation"
+            ]
         },
         {
-            "levels": [
+            "qualifier": "Plausibility",
+            "values": [
                 "PLAUSIBLE",
                 "HYPOTHETICAL"
-            ],
-            "qualifier": "Plausibility"
+            ]
         },
         {
-            "levels": [
+            "qualifier": "Temporality",
+            "values": [
                 "CURRENT",
                 "HISTORICAL"
-            ],
-            "qualifier": "Temporality"
+            ]
         }
     ],
     "rules": [
         {
             "direction": "preceding",
             "patterns": [
                 "familiair",
@@ -501,14 +501,15 @@
                 "zijzelf",
                 ","
             ],
             "qualifier": "Experiencer.OTHER"
         },
         {
             "direction": "preceding",
+            "max_scope": 5,
             "patterns": [
                 "afwezigheid van",
                 "deed geen",
                 "deed niet",
                 "geen aanwijzing voor",
                 "geen aanwijzingen voor",
                 "geen abnormale",
@@ -563,14 +564,15 @@
                 "zonder tekenen van",
                 "zonder"
             ],
             "qualifier": "Negation.NEGATED"
         },
         {
             "direction": "following",
+            "max_scope": 5,
             "patterns": [
                 "afwezig",
                 "is uitgesloten",
                 "is verdwenen",
                 "is weg",
                 "kan worden uitgesloten",
                 "laag ingeschat",
```

### Comparing `clinlp-0.2.0/PKG-INFO` & `clinlp-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
 Author: UMCU DIT Analytics
 Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: transformers
 Requires-Dist: intervaltree (>=3.1.0,<4.0.0)
-Requires-Dist: spacy (>=3.4.4,<4.0.0)
+Requires-Dist: makefun (>=1.15.1,<2.0.0)
+Requires-Dist: spacy (>=3.5.3,<4.0.0)
+Requires-Dist: transformers[torch] (>=4.30.2,<5.0.0) ; extra == "transformers"
 Description-Content-Type: text/markdown
 
 # clinlp
 
 ![clinlp](media/clinlp.png)
 
 * :hospital: `clinical` + :netherlands: `nl` + :clipboard: `NLP` = :sparkles: `clinlp`
@@ -60,15 +63,15 @@
     ]
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 
 # Qualifiers
-nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
+nlp.add_pipe('clinlp_context_algorithm', config={'phrase_matcher_attr': 'NORM'})
 
 text = (
     "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
     "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
     "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
@@ -107,15 +110,17 @@
 
 Currently, `clinlp` offers the following components, tailored to Dutch Clinical text, further discussed below: 
 
 1. [Tokenizer](#tokenizer)
 2. [Normalizer](#normalizer)
 3. [Sentence splitter](#sentence-splitter)
 4. [Entity matcher (builtin Spacy)](#entity-matcher)
-5. [Context detection](#context-detection)
+5. [Qualifier detection (=context)](#qualifier-detection)
+    - [Context Algorithm](#context-algorithm)
+    - [Transformer based negation detection](#transformer-based-negation-detection)
 
 ### Tokenizer
 
 The `clinlp` tokenizer is built into the blank model:
 
 ```python
 nlp = spacy.blank('clinlp')
@@ -170,33 +175,51 @@
 For more info, it's useful to check out these spaCy documentation pages:
 * [Rule based matching](https://spacy.io/usage/rule-based-matching)
 * [[spaCy API] Matcher](https://spacy.io/api/matcher)
 * [[spaCy API] PhraseMatcher](https://spacy.io/api/phrasematcher)
 
 Note that the `DependencyMatcher` cannot be used, and neither are part of speech tags available, as no good models for determining this information for clinical text exist (yet).  
 
-### Context detection
+### Qualifier detection
 
-After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) for this purpose. This algorithm is fairly accurate, and quite transparent and fast. Better solutions will hopefully be added to `clinlp` in the future. 
+After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002), and a [transformer-based negation detector](https://doi.org/10.48550/arxiv.2209.00470). 
 
-A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
+#### Context Algorithm
+
+The rule-based Context Algorithm is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
 
 ```python
-nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
+nlp.add_pipe('clinlp_context_algorithm', config={'phrase_matcher_attr': 'NORM'})
 ```
 
-A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows: 
+A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows:
 
 ```python
-from clinlp.component.qualifier import parse_rules
+cm = nlp.add_pipe('clinlp_context_algorithm', config={'rules': '/path/to/my_own_ruleset.json'})
+```
+
+#### Transformer based negation detection
+
+`clinlp` also includes a wrapper around the transformer based negation detector, as described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformer can be found on [huggingface](https://huggingface.co/UMCU/MedRoBERTa.nl_NegationDetection). It is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
+
+First, install the additional dependencies:
+
+```bash
+pip install "clinlp[transformers]"
+```
+
+Then add it using:
 
-cm = nlp.add_pipe('clinlp_context_matcher', config={'default_rules': None})
-cm.add_rules(parse_rules('my_custom_rules.json'))
+```python
+tn = nlp.add_pipe('clinlp_negation_transformer')
 ```
 
+Some configuration options, like the number of tokens to consider, can be specified in the `config` argument. 
+
+
 ### Where to go from here
 
 We hope to extend `clinlp` with new functionality and more complete documentation in the near future. In the meantime, if any questions or problems arise, we recommend:
 
 * Checking the source code 
 * Getting in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new))
```

