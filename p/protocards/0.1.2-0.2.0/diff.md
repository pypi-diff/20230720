# Comparing `tmp/protocards-0.1.2.tar.gz` & `tmp/protocards-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\protocards-0.1.2.tar", last modified: Wed Jun  5 07:09:46 2019, max compression
+gzip compressed data, was "protocards-0.2.0.tar", last modified: Thu Jul 20 19:14:36 2023, max compression
```

## Comparing `protocards-0.1.2.tar` & `protocards-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2019-06-05 07:09:46.000000 protocards-0.1.2/
--rw-rw-rw-   0        0        0     5933 2019-06-05 07:09:46.000000 protocards-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards/
--rw-rw-rw-   0        0        0     2536 2019-06-05 06:31:19.000000 protocards-0.1.2/protocards/base.py
--rw-rw-rw-   0        0        0     4319 2019-06-05 06:31:19.000000 protocards-0.1.2/protocards/cribbage.py
--rw-rw-rw-   0        0        0     3523 2019-06-05 07:06:02.000000 protocards-0.1.2/protocards/standard.py
-drwxrwxrwx   0        0        0        0 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards/tests/
--rw-rw-rw-   0        0        0     1780 2019-06-05 06:31:19.000000 protocards-0.1.2/protocards/tests/test_base.py
--rw-rw-rw-   0        0        0     4896 2019-06-05 06:31:19.000000 protocards-0.1.2/protocards/tests/test_cribbage.py
--rw-rw-rw-   0        0        0     2565 2019-06-05 06:31:19.000000 protocards-0.1.2/protocards/tests/test_standard.py
--rw-rw-rw-   0        0        0        0 2019-06-05 06:31:19.000000 protocards-0.1.2/protocards/tests/__init__.py
--rw-rw-rw-   0        0        0      118 2019-06-05 07:08:15.000000 protocards-0.1.2/protocards/__init__.py
-drwxrwxrwx   0        0        0        0 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards.egg-info/
--rw-rw-rw-   0        0        0        1 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5933 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2019-06-05 07:09:46.000000 protocards-0.1.2/protocards.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4197 2019-06-05 06:39:51.000000 protocards-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2019-06-05 07:09:46.000000 protocards-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      871 2019-06-05 07:09:23.000000 protocards-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:36.235839 protocards-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 19:14:28.000000 protocards-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-20 19:14:36.235839 protocards-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-20 19:14:28.000000 protocards-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:36.231839 protocards-0.2.0/protocards/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4334 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/cribbage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3523 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:36.235839 protocards-0.2.0/protocards/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/tests/test_cribbage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-20 19:14:28.000000 protocards-0.2.0/protocards/tests/test_standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:36.231839 protocards-0.2.0/protocards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-20 19:14:36.000000 protocards-0.2.0/protocards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 19:14:36.000000 protocards-0.2.0/protocards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:14:36.000000 protocards-0.2.0/protocards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 19:14:36.000000 protocards-0.2.0/protocards.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:14:36.235839 protocards-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-07-20 19:14:28.000000 protocards-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `protocards-0.1.2/PKG-INFO` & `protocards-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-Metadata-Version: 2.1
-Name: protocards
-Version: 0.1.2
-Summary: Basic tools for working with generic game cards in python.
-Home-page: https://github.com/relsqui/protocards
-Author: Finn Ellis
-Author-email: relsqui@chiliahedron.com
-License: MIT
-Description: ## protocards
-        
-        is a library for implementing card game logic in python. It's designed to be
-        generic enough to build unique card types with, but also implements a standard
-        poker deck for convenience. Basic usage is simple:
-        
-        ```
-        >>> from protocards.standard import make_deck
-        >>>
-        >>> deck = make_deck(shuffle=True)
-        >>> hand = deck.deal(5)
-        >>> print(hand)
-        AJ6s 2h 3c
-        >>> print(hand[0])
-        Ace of Spades
-        ```
-        
-        The cribbage module implements some example game logic using protocards.
-        
-        ```
-        >>> from protocards.standard import make_deck
-        >>> from protocards.cribbage import score_hand
-        >>>
-        >>> deck = make_deck(shuffle=True)
-        >>> hand = deck.deal(4)
-        >>> turned = deck.pop()
-        >>> print(hand)
-        Jh 8d QTc
-        >>> print(turned)
-        Six of Spades
-        >>> score_hand(hand, turned)
-        {'runs': 3, 'fifteens': 0, 'pairs': 0, 'nobs': 0, 'flush': 0, 'heels': 0}
-        ```
-        
-        ### package summary
-        
-        #### base
-        base is for abstract classes which can be used on their own in
-        simple projects or subclassed to build more complex mechanics.
-        
-        A `CardProperty` is a category a card can belong to, like "spade"
-        or "three" or "green" or "flying." This base class only has a name;
-        subclass it to add other attributes, or just to have a new type
-        for easy comparison.
-        
-        `Card` is a placeholder, which provides a basic equality test to
-        its subclasses.
-        
-        `Hand` is a container for storing cards. It behaves like a list in
-        that it can be indexed or sliced, and implements the standard list
-        methods as well as these:
-        * `.shuffle()` is the opposite of `.sort()`.
-        * `.deal(n)` removes the number of cards you specify and returns them
-          as a new `Hand`.
-        
-        
-        #### standard
-        standard implements the standard 52-card deck. It defines `Rank`
-        and `Suit` as card properties, and a list of each: `RANKS` and
-        `SUITS`. These lists define the sorting order for cards with those
-        properties. Specific ranks and suits can also be accessed as
-        constants--`TWO`, `QUEEN`, `HEART`, and so on.
-        
-        `StandardCard` is your normal playing card. It has a rank, a suit, and
-        a name. You can compare StandardCards to each other; cards with lower
-        ranks are less than cards with higher ranks, and a card with a lower
-        suit is less than a card with a higher suit and the same rank. (Aces
-        are high in the default implementation. Ascending suit order is clubs,
-        diamonds, hearts, spades, following bridge.)
-        
-        `StandardHand` is what you hold StandardCards in. To Hand it adds a
-        tidy string representation (as seen in the examples), and two more
-        methods:
-         * `.by_rank(Rank)` returns a new StandardHand containing the cards
-           from your hand which have the given rank. It does *not* remove them
-           from your hand.
-         * `.by_suit(Suit)` is the same thing but for suits.
-        
-        Finally, `make_deck()` is a top-level function which just creates a full
-        deck of cards, defined as one of each possible pair of the members of
-        RANKS and SUITS. By default, it is returned still in order; pass
-        `shuffle=True` to have it shuffled first.
-        
-        
-        #### cribbage
-        cribbage implements the hand-scoring rules of cribbage (but not the
-        play rules). Its main interface is `score_hand()`, which takes a
-        StandardHand and returns a dictionary of ("score-type": points) pairs.
-        You can also pass it `turned=StandardCard` and the boolean arguments
-        `crib` and `dealer` to cover all the scoring possibilities.
-        
-        score_hand() has a series of helper functions which can be called
-        individually with a StandardHand: `score_fifteens()` etc. return
-        integers, and `check_flush()` returns a boolean. It also has the
-        `value()` function, which takes a StandardCard and returns the point
-        value of that card (for fifteens and the play).
-        
-        
-        ___
-        
-        I originally wrote this because I wanted to know what the cribbage
-        score for a whole deck of cards was. Now I can find out!
-        
-        ```
-        >>> from protocards import standard, cribbage
-        >>>
-        >>> def score_deck():
-        ...     score = cribbage.score_hand(standard.make_deck())
-        ...     for key, value in score.items():
-        ...             if value:
-        ...                 print("{} for {:,}".format(key, value))
-        ...     print("total: {:,}".format(sum(score.values())))
-        ... 
-        >>> score_deck()
-        runs for 872,415,232
-        fifteens for 34,528
-        pairs for 156
-        total: 872,449,916
-        ```
-        
-        Plus 1-2 for heels/nobs, depending on the turned card and whether you're
-        dealing.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: protocards
+Version: 0.2.0
+Summary: Basic tools for working with generic game cards in python.
+Home-page: https://github.com/relsqui/protocards
+Author: Finn Ellis
+Author-email: relsqui@chiliahedron.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## protocards
+
+is a library for implementing card game logic in python. It's designed to be
+generic enough to build unique card types with, but also implements a standard
+poker deck for convenience. Basic usage is simple:
+
+```
+>>> from protocards.standard import make_deck
+>>>
+>>> deck = make_deck(shuffle=True)
+>>> hand = deck.deal(5)
+>>> print(hand)
+AJ6s 2h 3c
+>>> print(hand[0])
+Ace of Spades
+```
+
+The cribbage module implements some example game logic using protocards.
+
+```
+>>> from protocards.standard import make_deck
+>>> from protocards.cribbage import score_hand
+>>>
+>>> deck = make_deck(shuffle=True)
+>>> hand = deck.deal(4)
+>>> turned = deck.pop()
+>>> print(hand)
+Jh 8d QTc
+>>> print(turned)
+Six of Spades
+>>> score_hand(hand, turned)
+{'runs': 3, 'fifteens': 0, 'pairs': 0, 'nobs': 0, 'flush': 0, 'heels': 0}
+```
+
+### package summary
+
+#### base
+base is for abstract classes which can be used on their own in
+simple projects or subclassed to build more complex mechanics.
+
+A `CardProperty` is a category a card can belong to, like "spade"
+or "three" or "green" or "flying." This base class only has a name;
+subclass it to add other attributes, or just to have a new type
+for easy comparison.
+
+`Card` is a placeholder, which provides a basic equality test to
+its subclasses.
+
+`Hand` is a container for storing cards. It behaves like a list in
+that it can be indexed or sliced, and implements the standard list
+methods as well as these:
+* `.shuffle()` is the opposite of `.sort()`.
+* `.deal(n)` removes the number of cards you specify and returns them
+  as a new `Hand`.
+
+
+#### standard
+standard implements the standard 52-card deck. It defines `Rank`
+and `Suit` as card properties, and a list of each: `RANKS` and
+`SUITS`. These lists define the sorting order for cards with those
+properties. Specific ranks and suits can also be accessed as
+constants--`TWO`, `QUEEN`, `HEART`, and so on.
+
+`StandardCard` is your normal playing card. It has a rank, a suit, and
+a name. You can compare StandardCards to each other; cards with lower
+ranks are less than cards with higher ranks, and a card with a lower
+suit is less than a card with a higher suit and the same rank. (Aces
+are high in the default implementation. Ascending suit order is clubs,
+diamonds, hearts, spades, following bridge.)
+
+`StandardHand` is what you hold StandardCards in. To Hand it adds a
+tidy string representation (as seen in the examples), and two more
+methods:
+ * `.by_rank(Rank)` returns a new StandardHand containing the cards
+   from your hand which have the given rank. It does *not* remove them
+   from your hand.
+ * `.by_suit(Suit)` is the same thing but for suits.
+
+Finally, `make_deck()` is a top-level function which just creates a full
+deck of cards, defined as one of each possible pair of the members of
+RANKS and SUITS. By default, it is returned still in order; pass
+`shuffle=True` to have it shuffled first.
+
+
+#### cribbage
+cribbage implements the hand-scoring rules of cribbage (but not the
+play rules). Its main interface is `score_hand()`, which takes a
+StandardHand and returns a dictionary of ("score-type": points) pairs.
+You can also pass it `turned=StandardCard` and the boolean arguments
+`crib` and `dealer` to cover all the scoring possibilities.
+
+score_hand() has a series of helper functions which can be called
+individually with a StandardHand: `score_fifteens()` etc. return
+integers, and `check_flush()` returns a boolean. It also has the
+`value()` function, which takes a StandardCard and returns the point
+value of that card (for fifteens and the play).
+
+
+___
+
+I originally wrote this because I wanted to know what the cribbage
+score for a whole deck of cards was. Now I can find out!
+
+```
+>>> from protocards import standard, cribbage
+>>>
+>>> def score_deck():
+...     score = cribbage.score_hand(standard.make_deck())
+...     for key, value in score.items():
+...             if value:
+...                 print("{} for {:,}".format(key, value))
+...     print("total: {:,}".format(sum(score.values())))
+... 
+>>> score_deck()
+runs for 872,415,232
+fifteens for 34,528
+pairs for 156
+total: 872,449,916
+```
+
+Plus 1-2 for heels/nobs, depending on the turned card and whether you're
+dealing.
```

### Comparing `protocards-0.1.2/protocards/base.py` & `protocards-0.2.0/protocards/base.py`

 * *Files identical despite different names*

### Comparing `protocards-0.1.2/protocards/cribbage.py` & `protocards-0.2.0/protocards/cribbage.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     if check_flush(hand):
         if turned and hand[0].suit == turned.suit:
             score["flush"] = len(hand) + 1
         elif not turned or not crib:
             score["flush"] = len(hand)
 
-    if turned and dealer and turned.rank == standard.JACK:
+    if (not crib) and turned and dealer and turned.rank == standard.JACK:
         score["heels"] = 2
     elif turned and standard.StandardCard(standard.JACK, turned.suit) in hand:
         score["nobs"] = 1
 
     return score
```

### Comparing `protocards-0.1.2/protocards/standard.py` & `protocards-0.2.0/protocards/standard.py`

 * *Files identical despite different names*

### Comparing `protocards-0.1.2/protocards/tests/test_base.py` & `protocards-0.2.0/protocards/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `protocards-0.1.2/protocards/tests/test_cribbage.py` & `protocards-0.2.0/protocards/tests/test_cribbage.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,20 @@
         self.assertEqual(score["flush"], 0)
         turned = self.spades.pop()
         score = cribbage.score_hand(hand, turned=turned, crib=False)
         self.assertEqual(score["flush"], 5)
         score = cribbage.score_hand(hand, turned=turned, crib=True)
         self.assertEqual(score["flush"], 5)
 
+    def test_score_crib_heels(self):
+        hand = self.deck.by_rank(standard.FIVE)
+        turned = self.deck.by_rank(standard.JACK).pop()
+        score = cribbage.score_hand(hand, turned=turned, crib=True, dealer=True)
+        self.assertEqual(score["heels"], 0)
+
     def test_score_dealer_noturn(self):
         self.assertEqual(cribbage.score_hand(self.deck, dealer=True),
                          self.dscore)
         self.assertEqual(cribbage.score_hand(self.spades, dealer=True),
                          self.sscore)
 
     def test_score_heels(self):
```

### Comparing `protocards-0.1.2/protocards/tests/test_standard.py` & `protocards-0.2.0/protocards/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `protocards-0.1.2/protocards.egg-info/PKG-INFO` & `protocards-0.2.0/protocards.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-Metadata-Version: 2.1
-Name: protocards
-Version: 0.1.2
-Summary: Basic tools for working with generic game cards in python.
-Home-page: https://github.com/relsqui/protocards
-Author: Finn Ellis
-Author-email: relsqui@chiliahedron.com
-License: MIT
-Description: ## protocards
-        
-        is a library for implementing card game logic in python. It's designed to be
-        generic enough to build unique card types with, but also implements a standard
-        poker deck for convenience. Basic usage is simple:
-        
-        ```
-        >>> from protocards.standard import make_deck
-        >>>
-        >>> deck = make_deck(shuffle=True)
-        >>> hand = deck.deal(5)
-        >>> print(hand)
-        AJ6s 2h 3c
-        >>> print(hand[0])
-        Ace of Spades
-        ```
-        
-        The cribbage module implements some example game logic using protocards.
-        
-        ```
-        >>> from protocards.standard import make_deck
-        >>> from protocards.cribbage import score_hand
-        >>>
-        >>> deck = make_deck(shuffle=True)
-        >>> hand = deck.deal(4)
-        >>> turned = deck.pop()
-        >>> print(hand)
-        Jh 8d QTc
-        >>> print(turned)
-        Six of Spades
-        >>> score_hand(hand, turned)
-        {'runs': 3, 'fifteens': 0, 'pairs': 0, 'nobs': 0, 'flush': 0, 'heels': 0}
-        ```
-        
-        ### package summary
-        
-        #### base
-        base is for abstract classes which can be used on their own in
-        simple projects or subclassed to build more complex mechanics.
-        
-        A `CardProperty` is a category a card can belong to, like "spade"
-        or "three" or "green" or "flying." This base class only has a name;
-        subclass it to add other attributes, or just to have a new type
-        for easy comparison.
-        
-        `Card` is a placeholder, which provides a basic equality test to
-        its subclasses.
-        
-        `Hand` is a container for storing cards. It behaves like a list in
-        that it can be indexed or sliced, and implements the standard list
-        methods as well as these:
-        * `.shuffle()` is the opposite of `.sort()`.
-        * `.deal(n)` removes the number of cards you specify and returns them
-          as a new `Hand`.
-        
-        
-        #### standard
-        standard implements the standard 52-card deck. It defines `Rank`
-        and `Suit` as card properties, and a list of each: `RANKS` and
-        `SUITS`. These lists define the sorting order for cards with those
-        properties. Specific ranks and suits can also be accessed as
-        constants--`TWO`, `QUEEN`, `HEART`, and so on.
-        
-        `StandardCard` is your normal playing card. It has a rank, a suit, and
-        a name. You can compare StandardCards to each other; cards with lower
-        ranks are less than cards with higher ranks, and a card with a lower
-        suit is less than a card with a higher suit and the same rank. (Aces
-        are high in the default implementation. Ascending suit order is clubs,
-        diamonds, hearts, spades, following bridge.)
-        
-        `StandardHand` is what you hold StandardCards in. To Hand it adds a
-        tidy string representation (as seen in the examples), and two more
-        methods:
-         * `.by_rank(Rank)` returns a new StandardHand containing the cards
-           from your hand which have the given rank. It does *not* remove them
-           from your hand.
-         * `.by_suit(Suit)` is the same thing but for suits.
-        
-        Finally, `make_deck()` is a top-level function which just creates a full
-        deck of cards, defined as one of each possible pair of the members of
-        RANKS and SUITS. By default, it is returned still in order; pass
-        `shuffle=True` to have it shuffled first.
-        
-        
-        #### cribbage
-        cribbage implements the hand-scoring rules of cribbage (but not the
-        play rules). Its main interface is `score_hand()`, which takes a
-        StandardHand and returns a dictionary of ("score-type": points) pairs.
-        You can also pass it `turned=StandardCard` and the boolean arguments
-        `crib` and `dealer` to cover all the scoring possibilities.
-        
-        score_hand() has a series of helper functions which can be called
-        individually with a StandardHand: `score_fifteens()` etc. return
-        integers, and `check_flush()` returns a boolean. It also has the
-        `value()` function, which takes a StandardCard and returns the point
-        value of that card (for fifteens and the play).
-        
-        
-        ___
-        
-        I originally wrote this because I wanted to know what the cribbage
-        score for a whole deck of cards was. Now I can find out!
-        
-        ```
-        >>> from protocards import standard, cribbage
-        >>>
-        >>> def score_deck():
-        ...     score = cribbage.score_hand(standard.make_deck())
-        ...     for key, value in score.items():
-        ...             if value:
-        ...                 print("{} for {:,}".format(key, value))
-        ...     print("total: {:,}".format(sum(score.values())))
-        ... 
-        >>> score_deck()
-        runs for 872,415,232
-        fifteens for 34,528
-        pairs for 156
-        total: 872,449,916
-        ```
-        
-        Plus 1-2 for heels/nobs, depending on the turned card and whether you're
-        dealing.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: protocards
+Version: 0.2.0
+Summary: Basic tools for working with generic game cards in python.
+Home-page: https://github.com/relsqui/protocards
+Author: Finn Ellis
+Author-email: relsqui@chiliahedron.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## protocards
+
+is a library for implementing card game logic in python. It's designed to be
+generic enough to build unique card types with, but also implements a standard
+poker deck for convenience. Basic usage is simple:
+
+```
+>>> from protocards.standard import make_deck
+>>>
+>>> deck = make_deck(shuffle=True)
+>>> hand = deck.deal(5)
+>>> print(hand)
+AJ6s 2h 3c
+>>> print(hand[0])
+Ace of Spades
+```
+
+The cribbage module implements some example game logic using protocards.
+
+```
+>>> from protocards.standard import make_deck
+>>> from protocards.cribbage import score_hand
+>>>
+>>> deck = make_deck(shuffle=True)
+>>> hand = deck.deal(4)
+>>> turned = deck.pop()
+>>> print(hand)
+Jh 8d QTc
+>>> print(turned)
+Six of Spades
+>>> score_hand(hand, turned)
+{'runs': 3, 'fifteens': 0, 'pairs': 0, 'nobs': 0, 'flush': 0, 'heels': 0}
+```
+
+### package summary
+
+#### base
+base is for abstract classes which can be used on their own in
+simple projects or subclassed to build more complex mechanics.
+
+A `CardProperty` is a category a card can belong to, like "spade"
+or "three" or "green" or "flying." This base class only has a name;
+subclass it to add other attributes, or just to have a new type
+for easy comparison.
+
+`Card` is a placeholder, which provides a basic equality test to
+its subclasses.
+
+`Hand` is a container for storing cards. It behaves like a list in
+that it can be indexed or sliced, and implements the standard list
+methods as well as these:
+* `.shuffle()` is the opposite of `.sort()`.
+* `.deal(n)` removes the number of cards you specify and returns them
+  as a new `Hand`.
+
+
+#### standard
+standard implements the standard 52-card deck. It defines `Rank`
+and `Suit` as card properties, and a list of each: `RANKS` and
+`SUITS`. These lists define the sorting order for cards with those
+properties. Specific ranks and suits can also be accessed as
+constants--`TWO`, `QUEEN`, `HEART`, and so on.
+
+`StandardCard` is your normal playing card. It has a rank, a suit, and
+a name. You can compare StandardCards to each other; cards with lower
+ranks are less than cards with higher ranks, and a card with a lower
+suit is less than a card with a higher suit and the same rank. (Aces
+are high in the default implementation. Ascending suit order is clubs,
+diamonds, hearts, spades, following bridge.)
+
+`StandardHand` is what you hold StandardCards in. To Hand it adds a
+tidy string representation (as seen in the examples), and two more
+methods:
+ * `.by_rank(Rank)` returns a new StandardHand containing the cards
+   from your hand which have the given rank. It does *not* remove them
+   from your hand.
+ * `.by_suit(Suit)` is the same thing but for suits.
+
+Finally, `make_deck()` is a top-level function which just creates a full
+deck of cards, defined as one of each possible pair of the members of
+RANKS and SUITS. By default, it is returned still in order; pass
+`shuffle=True` to have it shuffled first.
+
+
+#### cribbage
+cribbage implements the hand-scoring rules of cribbage (but not the
+play rules). Its main interface is `score_hand()`, which takes a
+StandardHand and returns a dictionary of ("score-type": points) pairs.
+You can also pass it `turned=StandardCard` and the boolean arguments
+`crib` and `dealer` to cover all the scoring possibilities.
+
+score_hand() has a series of helper functions which can be called
+individually with a StandardHand: `score_fifteens()` etc. return
+integers, and `check_flush()` returns a boolean. It also has the
+`value()` function, which takes a StandardCard and returns the point
+value of that card (for fifteens and the play).
+
+
+___
+
+I originally wrote this because I wanted to know what the cribbage
+score for a whole deck of cards was. Now I can find out!
+
+```
+>>> from protocards import standard, cribbage
+>>>
+>>> def score_deck():
+...     score = cribbage.score_hand(standard.make_deck())
+...     for key, value in score.items():
+...             if value:
+...                 print("{} for {:,}".format(key, value))
+...     print("total: {:,}".format(sum(score.values())))
+... 
+>>> score_deck()
+runs for 872,415,232
+fifteens for 34,528
+pairs for 156
+total: 872,449,916
+```
+
+Plus 1-2 for heels/nobs, depending on the turned card and whether you're
+dealing.
```

### Comparing `protocards-0.1.2/README.md` & `protocards-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `protocards-0.1.2/setup.py` & `protocards-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="protocards",
-    version="0.1.2",
+    version="0.2.0",
     author="Finn Ellis",
     author_email="relsqui@chiliahedron.com",
     license="MIT",
     description="Basic tools for working with generic game cards in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/relsqui/protocards",
```

