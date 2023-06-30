# Comparing `tmp/ezregex-1.1.0.tar.gz` & `tmp/ezregex-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezregex-1.1.0.tar", last modified: Mon May  1 20:56:02 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ezregex-1.1.0.tar` & `ezregex-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1059 2023-01-01 23:18:10.000000 ezregex-1.1.0/LICENSE
--rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 21:53:36.000000 ezregex-1.1.0/LICENSE-APACHE
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 21:53:36.000000 ezregex-1.1.0/LICENSE-MIT
--rw-r--r--   0 leonard   (1000) leonard   (1000)       77 2023-04-20 21:53:36.000000 ezregex-1.1.0/MANIFEST.in
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4215 2023-05-01 20:56:02.082066 ezregex-1.1.0/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3164 2023-04-21 23:10:33.000000 ezregex-1.1.0/README.md
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/ezregex/
--rw-r--r--   0 leonard   (1000) leonard   (1000)      277 2023-04-21 00:07:40.000000 ezregex-1.1.0/ezregex/EZRegexFunctionCall.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     7433 2023-04-21 23:16:41.000000 ezregex-1.1.0/ezregex/EZRegexMember.py
--rw-------   0 leonard   (1000) leonard   (1000)     6928 2023-05-01 20:54:57.000000 ezregex-1.1.0/ezregex/__init__.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      152 2023-04-21 23:14:52.000000 ezregex-1.1.0/ezregex/_escapeChars.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    11233 2023-04-21 23:15:12.000000 ezregex-1.1.0/ezregex/invert.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/ezregex.egg-info/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4215 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)      337 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/SOURCES.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/dependency_links.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        8 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/top_level.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)      448 2023-05-01 20:55:15.000000 ezregex-1.1.0/pyproject.toml
--rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-05-01 20:56:02.082066 ezregex-1.1.0/setup.cfg
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2136 2023-04-20 22:21:57.000000 ezregex-1.1.0/setup.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/tests/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3537 2023-04-21 23:01:44.000000 ezregex-1.1.0/tests/tests.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.2.1/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.2.1/MANIFEST.in
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 ezregex-1.2.1/README.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ezregex-1.2.1/requirements.txt
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ezregex-1.2.1/setup.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ezregex-1.2.1/todo.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.2.1/tox.ini
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 ezregex-1.2.1/ezregex/EZRegexMember.py
+-rw-r--r--   0        0        0    14264 2020-02-02 00:00:00.000000 ezregex-1.2.1/ezregex/__init__.py
+-rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 ezregex-1.2.1/ezregex/invert.py
+-rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 ezregex-1.2.1/tests/tests.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ezregex-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.2.1/LICENSE
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ezregex-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ezregex-1.2.1/PKG-INFO
```

### Comparing `ezregex-1.1.0/LICENSE` & `ezregex-1.2.1/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 Copyright (c) 2023 Copeland Carter
 
+MIT License
+
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ezregex-1.1.0/ezregex/invert.py` & `ezregex-1.2.1/ezregex/invert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,223 +1,197 @@
-from dataclasses import dataclass
-from random import randint, choice, choices
 import re
-from ._escapeChars import escapeChars
-
-# from Cope import debug, todo, percent; todo('remove this')
+from copy import copy
+from dataclasses import dataclass
+from random import choice, choices, randint
 
 def unsanitize(string):
-    for part in escapeChars:
-        string = re.sub(r'\\' + part, part[1], string)
-    return string
+    return re.sub(r'\\([' + re.escape(')([]{}+*$^-\\?| ,') + r'])', '\g<1>', string)
 
 def randbool():
     return bool(randint(0, 1))
 
 def _randWord(randomlyGenerate=False):
     if randomlyGenerate:
         return ''.join(choices(_letters + '_', k=randint(1, _alot)))
     else:
         return 'word'
 
-_prevThingRegex = r'(\\?\w+)\Z'
-def _prevThing(cur):
-    try:
-        return re.search(_prevThingRegex, cur).group()
-    except AttributeError:
-        return ''
-
 # Inverting helpers
 _alot         = 6
 _digits       = '0123456789'
 _letters      = 'abcdefghijklmnopqrstuvwxyz'
 _letters     += _letters.upper()
-_punctuation  = r''',./;'[] = -)(*&^%$#@!~`+{}|:"<>?'''
-_whitespace   = '\t'
+_punctuation  = "./;=-&%$#@~"
+_whitespace   = '  '
 _everything   = _digits + _letters + _punctuation + _whitespace + '_'
 
-# notEscaped = r'[^\\]'
-notEscaped = r'(?<!\\)'
-
-# namedGroup('prev', either('(' + word() + ')', '.'))
-# prevThing = fr'(?P<prev>(\(\w+\)|{notEscaped}.))'
-# namedGroup('prev', anyof('(?:' + chunk() + ')', '(' + word() + ')', raw(r'(?<!\\)') + anything()))
-prevThing = r'(?P<prev>(?:\(\?\:.+\)|\(\w+\)|(?<!\\).))'
+# notParens = matchMax(anyCharExcept('(', ')'))  # + ifNotPreceededBy(r'\\'))
+# inner = atLeastNone(either('(' + optional('?:') + notParens + ')', notParens))
+# prevThing = namedGroup('prev', anyof('(?:' + inner + ')', '(' + inner + ')', ifNotPreceededBy(r'\\') + anything))
+prevThing = r'(?P<prev>(?:\(\?\:(?:(?:\((?:\?\:)?(?:[^\(\)])+\)|(?:[^\(\)])+))*\)|\((?:(?:\((?:\?\:)?(?:[^\(\)])+\)|(?:[^\(\)])+))*\)|(?<!\\).))'
 
 tillCloseParen = r'(?P<stuff>.+)\)'
 
 @dataclass
 class _invertRegexes:
-    start        = re.compile(r'\\A')
-    end          = re.compile(r'\\Z')
+    flags        = re.compile(r"\A\(\?[aiLmsux]\)")
     word         = re.compile(r'\\w\+')
     s            = re.compile(r'\\s')
     digit        = re.compile(r'\\d')
     char         = re.compile(r'\\w')
-    any          = re.compile(notEscaped + r'\.')
+    any          = re.compile(r'(?<!\\)\.')
     newline      = re.compile(r'\\n')
     carriage     = re.compile(r'\\r')
     tab          = re.compile(r'\\t')
     vert         = re.compile(r'\\v')
     f            = re.compile(r'\\f')
+    stringStart  = re.compile(r'\\A')
+    lineStart    = re.compile(r'\^')
+    stringEnd    = re.compile(r'\\Z')
+    lineEnd      = re.compile(r'\$')
     matchExactly = re.compile(r'\^(.+)\$')  # \^stuff\$
-    matchMax     = re.compile(fr'{prevThing}\+')  # (stuff)+
+    # '[' + atLeastOne(namedGroup('start', char) + '-' + namedGroup('end', char)) + ']'
+    anyBetween   = re.compile(r'\[(?:(?P<start>.)\-(?P<end>.))+\]')
     # '(' + namedGroup('stuff', chunk()) + '){' + namedGroup('amt', number()) + '}'
     matchExactAmt = re.compile(prevThing + r'\{(?P<amt>\d+)\}')  # (stuff){3}
-    # '(' + namedGroup('stuff', chunk()) + '){' + namedGroup('min', number()) + ',' + optional(space()) + namedGroup('max', number()) + '}'
-    matchRange = re.compile(prevThing + r'\{(?P<min>\d+),( )?(?P<max>\d+)\}')  # (stuff){3,4}
     # '(' + namedGroup('stuff', chunk()) + '){' + namedGroup('min', number()) + ',' + optional(space()) + '}'
     matchMore = re.compile(prevThing + r'\{(?P<min>\d+),( )?\}')  # (stuff){3,}
-    optional  = re.compile(prevThing + r'\?(?![\:P\<\!])')  # (stuff)?
-    max       = re.compile(prevThing + r'\*')  # (stuff)*
-    either    = re.compile(r'\((\w+)\|(\w+)\)')  # (stuff|things)
+    # optional  = re.compile(prevThing + r'\?(?![\:P\<\!])')  # (stuff)?
+    optionalGreedy  = re.compile(prevThing + r'\?(?![\:P\<\!])')  # (stuff)?
+    optionalNonGreedy  = re.compile(prevThing + r'\?\?(?![\:P\<\!])')  # (stuff)??
+    atLeastNoneGreedy       = re.compile(prevThing + r'\*')  # (stuff)*
+    atLeastNoneNonGreedy       = re.compile(prevThing + r'\*\?')  # (stuff)*?
+    atLeastOneGreedy     = re.compile(fr'{prevThing}\+')  # (stuff)+
+    atLeastOneNonGreedy     = re.compile(fr'{prevThing}\+\?')  # (stuff)+?
+    # '(' + namedGroup('stuff', chunk()) + '){' + namedGroup('min', number()) + ',' + optional(space()) + namedGroup('max', number()) + '}'
+    matchRangeGreedy = re.compile(prevThing + r'\{(?P<min>\d+),( )?(?P<max>\d+)\}')  # (stuff){3,4}
+    matchRangeNonGreedy = re.compile(prevThing + r'\{(?P<min>\d+),( )?(?P<max>\d+)\}\?')  # (stuff){3,4}?
+    # either('(?:', '(') + group(atLeast1(notParens, greedy=False)) + '|' + group(atLeast1(char, greedy=False)) + ')'
+    either    = re.compile(r'(?:\(\?\:|\()((?:(?:[^\(\)](?<!\\))+)+?)\|(.+?)\)')  # (stuff|things)
     notWhitespace = re.compile(r'\\S')
     notDigit      = re.compile(r'\\D')
     notWord       = re.compile(r'\\W')
-    # This matches basically anything in square brackets that's not ^
-    anyChars    = re.compile(r'(\[([^\^]\,?)+\])')  # [s,t]
-    notAnyChars = re.compile(r'\[\^(.\,?)+\]')  # [^s,t]
-    #
-    # anyOf = re.compile(r'\((((.+)\|){1,}(.+))+\)') # (stuff|things)
-    #! NOTE: This matches passive groups: (?:sequence) but I don't think its a problem, so long as the sequence doesn't contain a |
-    #  TODO: this probably needs to be fixed at some point
-    # todo('debugging this regex is where I left off. it needs to require at least 1 | in order to work properly -- fixing the problem in the above line')
+    # '[' + ifNotFollowedBy('^') + group(atLeastOne(anyCharExcept(','))) + ']'
+    anyChars    = re.compile(r'\[(?!\^)((?:[^\,])+)\]')  # [st]
+    anyChars2    = re.compile(r'\[(?!\^)((?:.(?:\,)?)+)\]')  # [s,t]
+    # '[' + ifFollowedBy('^') + group(atLeastOne(char)) + ']'
+    notAnyChars = re.compile(r'\[(?=\^)(.+)\]')  # [^s,t]
     # group(either(ifPrecededBy('(?:'), ifPrecededBy('(')) + matchMax(anyCharExcept(r'|\)')) + '|' + matchMax(anyCharExcept(r'|\)')) + optional('|') + ifFollowedBy(')'))
-    anyOf = re.compile(r'((?:(?<=\(\?\:)|(?<=\())(?:[^\|\)])+\|(?:[^\|\)])+(?:\|)?(?=\)))')  # (stuff|things|otherThings)
-    # hex     = re.compile(r'\\(\d+)') # \\67
-    # oct     = re.compile(r'\\x(\d+)') # \x67
+    anyOf = re.compile(r'((?:(?<=\(\?\:)|(?<=\())(?:.\|)+.(?=\)))')  # (stuff|things|otherThings)
     ifThing = re.compile(r'\(\?\=' + tillCloseParen)  # (?=stuff)
     ifNotThing       = re.compile(r'\(\?!' + tillCloseParen)  # (?!stuff)
     ifPrecededBy     = re.compile(r'\(\?\<\=' + tillCloseParen)
     ifNotPrecededBy  = re.compile(r'\(\?\<\!' + tillCloseParen)
     ifNotPrecededBy2 = re.compile(r'\(\?\!\=' + tillCloseParen)
-    passiveGroup     = re.compile(r'\(\?\:([^\)\(\?]+)\)')  # (?:stuff)
+    # '(?:' + group(matchMax(notAnyChars(')', '(', '?'))) + ')'
+    passiveGroup     = re.compile(r'\(\?\:((?:[^\(\?])+)\)')  # (?:stuff)
     group = re.compile(r'\((?!\?)([^\)\(\?]+)\)')  # (stuff)
-    notGroup = re.compile(r'\(\?:(.+)\)')  # (?:stuff)
     namedGroup = re.compile(r'\(\?P\<(?P<name>\w+)\>(?P<stuff>.+)\)')  # (P?<name>stuff)
 
-def invertRegex(regex:str, colors=True, groupNames=True, explicitConditionals=False) -> str:
-    """ 'Inverts' a regex expression. Gives an example of something that would match the given regex """
-    defaultColor   = (204, 204, 204)
-    notGroupColor  = (220, 0, 0)
-    groupNameColor = (34, 111, 157)
-
-    if explicitConditionals:
-        _proceedOpen = '   <if followed by> { '
-        _notProceedOpen = '   <if not followed by> { '
-        _preceedOpen = '   <if preceeded by> { '
-        _notPreceedOpen = '    <if not preceeded by> { '
-        _optionalClose = ' }   '
-    else:
-        _proceedOpen = _notProceedOpen = _preceedOpen = _notPreceedOpen = _optionalClose = ''
+
+def invertRegex(regex:str, tries=10) -> str:
+    """ 'Inverts' a regex expression.
+        Gives an example of something that would match the given regex
+        If tries is positive, it's guarenteed to return an expression that
+        correctly matches the given expression, or raise an Error
+    """
+    # So we can compare later and make sure it works
+    original = copy(regex)
 
     # So you can pass in an EasyRegex chain
     regex = str(regex)
-    # Because I hate everyone and this is a stupid bug and it makes NO sense
-    regex = re.sub(r'\\(?![AZbBcsSdDwWx0QEnrtvfox])', r'\\\\', regex)
 
-    def randColor():
-        return (randint(0, 255) % 20, randint(0, 255) % 20, randint(0, 255) % 20)
-
-    def color(s, c, fg=False):
-        if colors:
-            return f'\0{"3" if fg else "4"}3[48;2;{c[0]};{c[1]};{c[2]}m{s}\033[38;2;{defaultColor[0]};{defaultColor[1]};{defaultColor[2]}m'
-        else:
-            return s
+    # Because I hate everyone and this is a stupid bug and it makes NO sense
+    regex = re.sub(r'\\(?![AZbBcsSdDwWx0\|QEnrtvfox])', r'\\\\', regex)
 
     #* The order of these matter
-    regex = _invertRegexes.start.sub('', regex)  # TODO
-    regex = _invertRegexes.end.sub('', regex)  # TODO
+
+    # Very first thing, remove any flags at the beginning
+    # TODO: keep track of what flags are asserted. It's probably important?
+    regex = _invertRegexes.flags.sub('', regex)
+
+    regex = _invertRegexes.stringStart.sub('', regex)  # TODO
+    regex = _invertRegexes.stringEnd.sub('', regex)  # TODO
+    regex = _invertRegexes.lineEnd.sub('', regex)  # TODO
 
     # Single Characters
     regex = _invertRegexes.word.sub(_randWord(), regex)
     regex = _invertRegexes.s.sub(_whitespace, regex)
     regex = _invertRegexes.digit.sub(choice(_digits), regex)
     regex = _invertRegexes.char.sub(choice(_letters + '_'), regex)
-    # regex = re.sub(r'\x',  choice(_digits + 'ABCDEF'), regex)
-    # regex = re.sub(r'\O',  choice(_digits[:8]), regex)
     regex = _invertRegexes.any.sub(choice(_everything), regex)
 
     # Explicit Characters
     regex = _invertRegexes.newline.sub('\n', regex)
     regex = _invertRegexes.carriage.sub('\r', regex)
     regex = _invertRegexes.tab.sub('\t', regex)
     regex = _invertRegexes.vert.sub('\v', regex)
     regex = _invertRegexes.f.sub('\f', regex)
 
     # Matching
     regex = _invertRegexes.matchExactly.sub(r'\1', regex)
 
     # Amounts
-    regex = _invertRegexes.matchMax.sub(r"\g<prev>" * randint(1, _alot), regex)
-    regex = _invertRegexes.matchExactAmt.sub(lambda m: m.group('prev') * int(m.group('amt')), regex)
-    regex = _invertRegexes.matchRange.sub(lambda m: m.group('prev') * randint(int(m.group('min')), int(m.group('max'))), regex)
+    regex = _invertRegexes.matchRangeNonGreedy.sub(lambda m: m.group('prev') * randint(int(m.group('min')), int(m.group('max'))), regex)
+    regex = _invertRegexes.matchRangeGreedy.sub(lambda m: m.group('prev') * randint(int(m.group('min')), int(m.group('max'))), regex)
+
+    regex = _invertRegexes.atLeastOneNonGreedy.sub(r"\g<prev>" * randint(1, _alot), regex)
+    regex = _invertRegexes.atLeastOneGreedy.sub(r"\g<prev>" * randint(1, _alot), regex)
+    regex = _invertRegexes.matchExactAmt.sub(lambda m: m.group('prev') * randint(int(m.group('amt')), int(m.group('amt'))), regex)
     regex = _invertRegexes.matchMore.sub(lambda m: m.group('prev') * randint(int(m.group('min')), int(m.group('min')) + _alot), regex)
 
     # Not Chuncks
     regex = _invertRegexes.notWhitespace.sub(choice(_digits  + _letters + _punctuation + '_'), regex)
     regex = _invertRegexes.notDigit.sub(choice(_letters + _whitespace  + _punctuation + '_'), regex)
-    regex = _invertRegexes.notWord.sub(choice(_punctuation + _whitespace), regex)  # I guess digits are counted as word chars?
+    regex = _invertRegexes.notWord.sub(choice(_punctuation + _whitespace), regex)
 
     # Conditionals
-    regex = _invertRegexes.ifThing.sub(_proceedOpen + r'\g<stuff>' + _optionalClose, regex)
-    regex = _invertRegexes.ifNotThing.sub(_notProceedOpen + r'\g<stuff>' + _optionalClose, regex)
-    regex = _invertRegexes.ifPrecededBy.sub(_preceedOpen + r'\g<stuff>' + _optionalClose, regex)
-    regex = _invertRegexes.ifNotPrecededBy.sub(_notPreceedOpen + r'\g<stuff>' + _optionalClose, regex)
-    regex = _invertRegexes.ifNotPrecededBy2.sub(_notPreceedOpen + r'\g<stuff>' + _optionalClose, regex)
+    regex = _invertRegexes.ifThing.sub(r'\g<stuff>', regex)
+    regex = _invertRegexes.ifNotThing.sub(r'\g<stuff>', regex)
+    regex = _invertRegexes.ifPrecededBy.sub(r'\g<stuff>', regex)
+    regex = _invertRegexes.ifNotPrecededBy.sub(r'\g<stuff>', regex)
+    regex = _invertRegexes.ifNotPrecededBy2.sub(r'\g<stuff>', regex)
 
     # Optionals
-    regex = _invertRegexes.max.sub(r'\g<prev>' * randint(0, _alot), regex)
+    regex = _invertRegexes.atLeastNoneNonGreedy.sub(r'\g<prev>' * randint(0, _alot), regex)
+    regex = _invertRegexes.atLeastNoneGreedy.sub(r'\g<prev>' * randint(0, _alot), regex)
     regex = _invertRegexes.either.sub(r'\g<1>' if randint(0,1) else r'\g<2>', regex)
-    # anyBetween    = EasyRegexSingleton(lambda cur, input, and_input: cur + r'[' + input + r'-' + and_input + r']') # TODO
-    # Alright, so the regex matches basically anything in square brackets that's not a ^, including the square brackets. This gets that,
-    #   drops the square brackets (with [1:-1]), and splits them along commas and chooses a random one
-    regex = _invertRegexes.notAnyChars.sub(lambda m: choice(list(set(_everything).difference(m.groups()[0][1:-1].split(',')))), regex)
-    regex = _invertRegexes.anyChars.sub(lambda m: choice(m.groups()[0][1:-1].split(',')), regex)
-    # regex = _invertRegexes.anyOf.sub(lambda m: choice(m.groups()[0].split('|')), regex)
+    # TODO: This isn't wrong, but it also isn't right. It only uses the start or the end, instead of the range
+    regex = _invertRegexes.anyBetween.sub(r'\g<start>' if randint(0,1) else r'\g<end>', regex)
+    regex = _invertRegexes.notAnyChars.sub(lambda m: choice(list(set(_everything).difference(list(m.group(1))))), regex)
+    regex = _invertRegexes.anyChars.sub(lambda m: choice(list(m.group(1))), regex)
+    regex = _invertRegexes.anyChars2.sub(lambda m: choice(m.groups()).replace(',', ''), regex)
+
+    regex = _invertRegexes.lineStart.sub('', regex)  # TODO
 
     def tmp(m):
-        # debug(m.groups())
-        # debug(m.groups()[0])
-        # debug(m.group())
         options = m.groups()[0].split('|')
-        # debug(options)
-        # return debug(choice(m.groups()[0].split('|')), clr=2)
-        # return debug(choice(options), clr=2)
         return choice(options)
     regex = _invertRegexes.anyOf.sub(tmp, regex)
 
-    # Sets
-    # regex = _invertRegexes.sub(r' \[A-Z\]',      choice(_letters.upper()), regex)
-    # regex = _invertRegexes.sub(r' \[a-z\]',      choice(_letters.lower()), regex)
-    # regex = _invertRegexes.sub(r'\[A-Za-z\]',    choice(_letters), regex)
-    # regex = _invertRegexes.sub(r'\[A-Za-z0-9\]', choice(_letters + _digits), regex)
-    # regex = _invertRegexes.sub(r'\[0-9\]',       choice(_digits), regex)
-    # regex = _invertRegexes.sub(r'\[0-9a-fA-F\]', choice(_digits + "ABCDEF"), regex)
-    # regex = _invertRegexes.sub(r'\[0-7\]',       choice(_digits[:8]), regex)
-    # regex = _invertRegexes.sub(r'\[:punct:\]',   choice(_punctuation), regex)
-    # regex = _invertRegexes.sub(r'\[ \t\r\n\v\f\]', choice(_whitespace), regex)
-    # # regex = _invertRegexes.sub(r'\[\x00-\x1F\x7F\]', regex)
-    # regex = _invertRegexes.sub(r'\[\\x21-\\x7E\]', choice(_everything.replace(' ', '')), regex)
-    # regex = _invertRegexes.sub(r'\[\x20-\x7E\]', choice(_everything), regex)
-    # regex = _invertRegexes.sub(r'\[A-Za-z0-9_\]', choice(_letters + _digits + '_'), regex)
-
-    # Numbers
-    # regex = _invertRegexes.hex.sub(r'0x\1',regex)
-    # regex = _invertRegexes.oct.sub(r'0o\1',regex)
-
     # Groups
-    regex = _invertRegexes.optional.sub(r'\g<prev>' if randint(0,1) else '', regex)
-    regex = _invertRegexes.notGroup.sub(color(r'\1', notGroupColor), regex)  # TODO
-    regex = _invertRegexes.namedGroup.sub((color(r'\g<name>: ', groupNameColor) if groupNames else '') + color(r'\g<stuff>', groupNameColor, True), regex)
-    regex = _invertRegexes.passiveGroup.sub(r'\1', regex)
-    regex = _invertRegexes.group.sub(color(r'\1', randColor()), regex)
+    def denest(regex, replace, current):
+        new = regex.sub(replace, current)
+        if current != new:
+            new = denest(regex, replace, new)
+        return new
+
+    regex = denest(_invertRegexes.optionalNonGreedy, r'\g<prev>' if randint(0,1) else '', regex)
+    regex = denest(_invertRegexes.optionalGreedy, r'\g<prev>' if randint(0,1) else '', regex)
+    regex = denest(_invertRegexes.namedGroup, r'\g<stuff>', regex)
+    regex = denest(_invertRegexes.passiveGroup, r'\1', regex)
+    regex = denest(_invertRegexes.group, r'\1', regex)
 
     # referenceGroup = EasyRegexSingleton(lambda cur, name:        f'{cur}(?P={name})') # TODO))
 
     # Undo what we did earlier
     regex = re.sub(r'\\\\', r'\\', regex)
-    return unsanitize(regex)
+    regex = unsanitize(regex)
 
-def testInvertRegex(regex, count=10, colors=True, groupNames=True, explicitConditionals=False):
-    for i in range(count):
-        print(invertRegex(regex, colors, groupNames, explicitConditionals))
+    # If the regex passed in isn't in what we generated, try again
+    if re.search(str(original), regex) is not None or tries < 0:
+        return regex
+    else:
+        if not tries:
+            raise NotImplementedError(f"Sorry, I can't invert the given regex. You can try again, or submit a bug report by emailing smartycope@gmail.com and including `{self}`")
+        else:
+            return invertRegex(original, tries=tries-1)
```

### Comparing `ezregex-1.1.0/setup.py` & `ezregex-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             break
     else:
         version = '0.0.1'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
-REQUIRES = []
+REQUIRES = ['rich']
 
 kwargs = {
     'name': 'ezregex',
     'version': version,
     'description': '',
     'long_description': readme,
     'author': 'Copeland Carter',
```

