# Comparing `tmp/bgameb-0.1.2.tar.gz` & `tmp/bgameb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgameb-0.1.2.tar", last modified: Fri Jan 27 16:57:55 2023, max compression
+gzip compressed data, was "bgameb-2.0.0.tar", last modified: Wed May 24 00:45:29 2023, max compression
```

## Comparing `bgameb-0.1.2.tar` & `bgameb-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 16:57:55.023733 bgameb-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-27 16:57:34.000000 bgameb-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-27 16:57:34.000000 bgameb-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-01-27 16:57:34.000000 bgameb-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-01-27 16:57:55.023733 bgameb-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-01-27 16:57:34.000000 bgameb-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 16:57:55.023733 bgameb-0.1.2/bgameb/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/items.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/players.py
--rw-r--r--   0 runner    (1001) docker     (123)    23706 2023-01-27 16:57:34.000000 bgameb-0.1.2/bgameb/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 16:57:55.023733 bgameb-0.1.2/bgameb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-01-27 16:57:54.000000 bgameb-0.1.2/bgameb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-27 16:57:54.000000 bgameb-0.1.2/bgameb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 16:57:54.000000 bgameb-0.1.2/bgameb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-27 16:57:54.000000 bgameb-0.1.2/bgameb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-27 16:57:54.000000 bgameb-0.1.2/bgameb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-27 16:57:34.000000 bgameb-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-27 16:57:34.000000 bgameb-0.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-27 16:57:55.023733 bgameb-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-01-27 16:57:34.000000 bgameb-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:45:29.614731 bgameb-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 00:45:09.000000 bgameb-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 00:45:09.000000 bgameb-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-24 00:45:09.000000 bgameb-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-24 00:45:29.614731 bgameb-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-24 00:45:09.000000 bgameb-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:45:29.614731 bgameb-2.0.0/bgameb/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-05-24 00:45:09.000000 bgameb-2.0.0/bgameb/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:45:29.614731 bgameb-2.0.0/bgameb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-24 00:45:29.000000 bgameb-2.0.0/bgameb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-24 00:45:29.000000 bgameb-2.0.0/bgameb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:45:29.000000 bgameb-2.0.0/bgameb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-24 00:45:29.000000 bgameb-2.0.0/bgameb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 00:45:29.000000 bgameb-2.0.0/bgameb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-24 00:45:09.000000 bgameb-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-24 00:45:09.000000 bgameb-2.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 00:45:29.614731 bgameb-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 00:45:09.000000 bgameb-2.0.0/setup.py
```

### Comparing `bgameb-0.1.2/LICENSE` & `bgameb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bgameb-0.1.2/Makefile` & `bgameb-2.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `bgameb-0.1.2/PKG-INFO` & `bgameb-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,111 @@
 Metadata-Version: 2.1
 Name: bgameb
-Version: 0.1.2
+Version: 2.0.0
 Summary: Board Game Builder
 Home-page: https://github.com/KonstantinKlepikov/BoardGameBuilder
 Author: Konstantin Klepikov
 Author-email: oformleno@gmail.com
 License: MIT
 Project-URL: Docs, https://konstantinklepikov.github.io/BoardGameBuilder/
 Project-URL: Source, https://github.com/KonstantinKlepikov/BoardGameBuilder
 Description: # BoardGameBuilder
         
-        !!! Project now is in very early stage. Dont use it in any apps :)
+        !!! Project now is in very early stage.
         
         [![Release and upload to pypi](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/release.yml/badge.svg)](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/release.yml)
         [![Deploy static content to Pages](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/build-docs.yml/badge.svg)](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/build-docs.yml)
         
         Object-oriented framework for build board game logic in python
         
         `pip install bgameb`
         
         ## Short example
         
         ```python
         from typing import Optional
         from pydantic import Field
         from bgameb import (
-            Game, Player, Steps, Step, Deck, Card, Shaker, Dice,
-            Bag, log_enable
+            Game,
+            Components,
+            Player,
+            Steps,
+            Step,
+            Deck,
+            Card,
+            Shaker,
+            Dice,
+            log_enable
                 )
         
         
         if __name__ == '__main__':
             log_enable()
         
+            # Defining a classes
+            class MyPlayer(Player):
+                deck: Deck
+        
             # Creating of the game
             class MyGame(Game):
                 steps: Steps
-                deck: Deck
                 shaker: Shaker
-                bag: Bag
-                players: list[Player] = []
+                me: MyPlayer
+                opp: MyPlayer
         
             # The Player and Game are an obstract containeers for tools and stuff.
             # Deck, Bag, Shaker and Steps are tools. Dice, Card and Step are items.
+            # Use Components to fill Game class
+            C = Components[Dice | Card | Step]()
         
             G = MyGame(
-                id='one board game',
-                steps=Steps(id='steps'),
-                deck=Deck(id='deck'),
-                shaker=Shaker(id='shaker'),
-                bag=Bag(id='bag'),
-                players=[Player(id='player1'), Player(id='player2')]
+                id="my game",
+                steps=Steps(id="game steps"),
+                shaker=Shaker(id="dice shaker"),
+                me=MyPlayer(
+                    id='Me',
+                    deck=Deck(id="my cards deck")
+                        ),
+                opp=MyPlayer(
+                    id='Opponent',
+                    deck=Deck(id="opponent cards deck")
+                        )
                     )
         
             # The tool objects must be filled by items by method add().
             # That because we use some other methods for check
             # data types and makes some operations with items inside tool.
         
             # Adding game tuns order in Steps tool
-            G.steps.add(Step(id='step0'))
-            G.steps.add(Step(id='step1', priority=1))
+            C.step0 = Step(id='step0')
+            C.step1 = Step(id='step1', priority=1)
         
             # Starting of new turn
-            current_steps = G.steps.deal()
+            current_steps = G.steps.deal(C)
         
             # Game steps is a priority queue, ordered by "priority" attribute
-            last = G.steps.pop()
+            last = G.steps.pops()
         
             # Adding of cards to deck. "count" parameter define how mutch
             # copies of card we must deal.
-            G.deck.add(
+            C.update(
                 Card(id='First', description='story', count=2)
                     )
-            G.deck.add(Card(id='Second', count=1))
-        
-            # All items in tools are saved in spetial object Component.
-            # Is a dict-like class. Component is predefined as attribute "c".
-            # A component usied as base for other operations with items.
-            cards_component = G.deck.c
+            C.update(Card(id='Second', count=1))
         
+            # All items in tools are saved in spetial object Components.
+            # Is a dict-like class. A component usied as base for other operations with items.
             # Any item is available in Component with dot or classic dict
             # notation. Names for that notation is transited from ids of items.
-            card = G.deck.c.first
-            card = G.deck.c['first']
+            card = C.first
+            card = C['first']
+            step = C.step0
         
             # You can get item by its id
-            card = G.deck.c.by_id('First')
+            card = C.by_id('First')
         
             # If you relocate some bult-in attrs, inherite from stuff classes,
             # then define aliases for attributes. In this example we use two
             # different solution: Field aliase and config.
             # Dont forget use G.dict(by_alias=True) to get aliases.
             # More infoshere:
             # https://docs.pydantic.dev/usage/model_config/#alias-generator
@@ -102,36 +118,36 @@
                 class Config(Card.Config):
                     fields = {'is_revealed': 'is_open'}
         
                 @property
                 def my_calculated_field(self) -> str:
                     return self.some_text.upper()
         
-            G.deck.add(
+            C.update(
                 MyCard(id='Thierd', description='story', count=3)
                     )
         
-            # Use default counters of any objects - counters not added to schema output
-            G.deck.c.first._counter['yellow'] = 12
-            G.deck.c.second._counter['banana'] = 0
+            # Use default counters of any objects - counters not added to schema
+            G.me.deck._counter['yellow'] = 12
+            G.me.deck._counter['banana'] = 0
         
             # Dealing and shuffling of deck
-            G.deck.deal().shuffle()
+            G.me.deck.deal(C).shuffle()
         
             # Adding dices to shaker
-            G.shaker.add(
+            C.update(
                 Dice(id='dice#8', sides=8, count=10)
                     )
+            G.shaker.deal(C)
         
-            # Roll dices
-            result = G.shaker.c.dice_8.roll()
+            # You can use items from Components
+            result = C.dice_8.roll()
         
-            # Use bag as collection of any items
-            G.bag.add(Dice(id='dice'))
-            G.bag.add(Card(id='card'))
+            # Or use from tool
+            result = G.shaker.roll()
         ```
         
         ## Documentation
         
         - [docs](https://konstantinklepikov.github.io/BoardGameBuilder/)
         - [pypi](https://pypi.org/project/bgameb/)
```

### Comparing `bgameb-0.1.2/README.md` & `bgameb-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,101 @@
 # BoardGameBuilder
 
-!!! Project now is in very early stage. Dont use it in any apps :)
+!!! Project now is in very early stage.
 
 [![Release and upload to pypi](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/release.yml/badge.svg)](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/release.yml)
 [![Deploy static content to Pages](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/build-docs.yml/badge.svg)](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/build-docs.yml)
 
 Object-oriented framework for build board game logic in python
 
 `pip install bgameb`
 
 ## Short example
 
 ```python
 from typing import Optional
 from pydantic import Field
 from bgameb import (
-    Game, Player, Steps, Step, Deck, Card, Shaker, Dice,
-    Bag, log_enable
+    Game,
+    Components,
+    Player,
+    Steps,
+    Step,
+    Deck,
+    Card,
+    Shaker,
+    Dice,
+    log_enable
         )
 
 
 if __name__ == '__main__':
     log_enable()
 
+    # Defining a classes
+    class MyPlayer(Player):
+        deck: Deck
+
     # Creating of the game
     class MyGame(Game):
         steps: Steps
-        deck: Deck
         shaker: Shaker
-        bag: Bag
-        players: list[Player] = []
+        me: MyPlayer
+        opp: MyPlayer
 
     # The Player and Game are an obstract containeers for tools and stuff.
     # Deck, Bag, Shaker and Steps are tools. Dice, Card and Step are items.
+    # Use Components to fill Game class
+    C = Components[Dice | Card | Step]()
 
     G = MyGame(
-        id='one board game',
-        steps=Steps(id='steps'),
-        deck=Deck(id='deck'),
-        shaker=Shaker(id='shaker'),
-        bag=Bag(id='bag'),
-        players=[Player(id='player1'), Player(id='player2')]
+        id="my game",
+        steps=Steps(id="game steps"),
+        shaker=Shaker(id="dice shaker"),
+        me=MyPlayer(
+            id='Me',
+            deck=Deck(id="my cards deck")
+                ),
+        opp=MyPlayer(
+            id='Opponent',
+            deck=Deck(id="opponent cards deck")
+                )
             )
 
     # The tool objects must be filled by items by method add().
     # That because we use some other methods for check
     # data types and makes some operations with items inside tool.
 
     # Adding game tuns order in Steps tool
-    G.steps.add(Step(id='step0'))
-    G.steps.add(Step(id='step1', priority=1))
+    C.step0 = Step(id='step0')
+    C.step1 = Step(id='step1', priority=1)
 
     # Starting of new turn
-    current_steps = G.steps.deal()
+    current_steps = G.steps.deal(C)
 
     # Game steps is a priority queue, ordered by "priority" attribute
-    last = G.steps.pop()
+    last = G.steps.pops()
 
     # Adding of cards to deck. "count" parameter define how mutch
     # copies of card we must deal.
-    G.deck.add(
+    C.update(
         Card(id='First', description='story', count=2)
             )
-    G.deck.add(Card(id='Second', count=1))
-
-    # All items in tools are saved in spetial object Component.
-    # Is a dict-like class. Component is predefined as attribute "c".
-    # A component usied as base for other operations with items.
-    cards_component = G.deck.c
+    C.update(Card(id='Second', count=1))
 
+    # All items in tools are saved in spetial object Components.
+    # Is a dict-like class. A component usied as base for other operations with items.
     # Any item is available in Component with dot or classic dict
     # notation. Names for that notation is transited from ids of items.
-    card = G.deck.c.first
-    card = G.deck.c['first']
+    card = C.first
+    card = C['first']
+    step = C.step0
 
     # You can get item by its id
-    card = G.deck.c.by_id('First')
+    card = C.by_id('First')
 
     # If you relocate some bult-in attrs, inherite from stuff classes,
     # then define aliases for attributes. In this example we use two
     # different solution: Field aliase and config.
     # Dont forget use G.dict(by_alias=True) to get aliases.
     # More infoshere:
     # https://docs.pydantic.dev/usage/model_config/#alias-generator
@@ -92,36 +108,36 @@
         class Config(Card.Config):
             fields = {'is_revealed': 'is_open'}
 
         @property
         def my_calculated_field(self) -> str:
             return self.some_text.upper()
 
-    G.deck.add(
+    C.update(
         MyCard(id='Thierd', description='story', count=3)
             )
 
-    # Use default counters of any objects - counters not added to schema output
-    G.deck.c.first._counter['yellow'] = 12
-    G.deck.c.second._counter['banana'] = 0
+    # Use default counters of any objects - counters not added to schema
+    G.me.deck._counter['yellow'] = 12
+    G.me.deck._counter['banana'] = 0
 
     # Dealing and shuffling of deck
-    G.deck.deal().shuffle()
+    G.me.deck.deal(C).shuffle()
 
     # Adding dices to shaker
-    G.shaker.add(
+    C.update(
         Dice(id='dice#8', sides=8, count=10)
             )
+    G.shaker.deal(C)
 
-    # Roll dices
-    result = G.shaker.c.dice_8.roll()
+    # You can use items from Components
+    result = C.dice_8.roll()
 
-    # Use bag as collection of any items
-    G.bag.add(Dice(id='dice'))
-    G.bag.add(Card(id='card'))
+    # Or use from tool
+    result = G.shaker.roll()
 ```
 
 ## Documentation
 
 - [docs](https://konstantinklepikov.github.io/BoardGameBuilder/)
 - [pypi](https://pypi.org/project/bgameb/)
```

### Comparing `bgameb-0.1.2/bgameb/errors.py` & `bgameb-2.0.0/bgameb/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,18 @@
     def __init__(self, name: str) -> None:
         self.message = f'Stuff with {name=} is exist in ' + \
                         'Component class instance or wrong name of stuff.'
         super().__init__(self.message)
 
 
 class ComponentClassError(CustomRuntimeError):
-    """Given class can't be a part of component.
+    """Given class can't be a part of components.
     """
-    def __init__(self, obj_, logger: Logger) -> None:
-        self.message = f'Given: {obj_} cant be used as part of Component.'
-        logger.exception(self.message)
+    def __init__(self, obj_) -> None:
+        self.message = f'Given: {obj_} cant be used as part of Components.'
         super().__init__(self.message)
 
 
 class StuffDefineError(AttributeError):
     """Bad definition of item.
     """
     def __init__(self, message: str, logger: Logger) -> None:
```

### Comparing `bgameb-0.1.2/bgameb/items.py` & `bgameb-2.0.0/bgameb/items.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Game dices, coins, cards and other items
 """
 import random
 from typing import Optional, NoReturn, Any, cast
 from pydantic import PositiveInt, NonNegativeInt, ConstrainedInt
-from bgameb.base import Base
+from bgameb.base import BaseItem
 from bgameb.errors import StuffDefineError
 
 
-class BaseItem(Base):
-    """Base class for game items (like dices or cards)
-    """
-
-
 class Step(BaseItem):
     """Game steps or turns
 
     ..
         Attr:
 
             priority (NonNegativeInt): priority queue number. Default to 0.
     """
-    #: priority queue number. Default to 0.
     priority: NonNegativeInt = 0
 
     def __eq__(self, other: 'Step') -> bool:  # type: ignore[override]
         return self.priority == other.priority
 
     def __lt__(self, other: 'Step') -> bool:
         return self.priority < other.priority
@@ -40,16 +34,20 @@
 
     def __ge__(self, other: 'Step') -> bool:
         return self.priority >= other.priority
 
 
 class Sides(ConstrainedInt):
     """Int subtipe to define sides of dices
+
+    ..
+        Attr:
+
+            gt (int): greate than 1 constraint.
     """
-    #: greate than 1 constraint
     gt = 1
 
 
 class Dice(BaseItem):
     """Rolling or tossed objects, like dices or coins.
 
     .. code-block::
@@ -76,24 +74,18 @@
 
             _range (list[PositiveInt]): range of roll, started from 1.
 
         Raises:
 
             StuffDefineError: mapping keys is not equal of roll range.
     """
-    #: Count of dices.
     count: PositiveInt = 1
-    #:  Sides of dice or coin.
     sides: Sides = cast(Sides, 2)
-    #: Optional mapping of roll result
-    #: Mapping must define values for each side.
     mapping: dict[PositiveInt, Any] = {}
-    #: Last roll values
     last_roll: list[PositiveInt] = []
-    #: Last mapped roll values
     last_roll_mapped: list[Any] = []
     _range: list[PositiveInt] = []
 
     def __init__(self, **data):
         super().__init__(**data)
         self._range = list(range(1, self.sides + 1))
 
@@ -121,15 +113,15 @@
     def __ge__(self, other: 'Dice') -> bool:
         return self.sides >= other.sides
 
     def roll(self) -> list[PositiveInt]:
         """Roll and return result
 
         Returns:
-            List[PositiveInt]: result of roll
+            list[PositiveInt]: result of roll
         """
         self.last_roll = [
             random.choices(self._range, k=1)[0] for _
             in list(range(self.count))
                 ]
         return self.last_roll
 
@@ -162,21 +154,17 @@
 
     .. code-block::
         :caption: Example:
 
             card = Card(id='unique_card')
             card.tap(side='left')
     """
-    #: Count of cards.
     count: PositiveInt = 1
-    #: Is card oppened.
     is_revealed: bool = False
-    #: Is card is_active.
     is_active: bool = True
-    #: The side of tap.
     side: Optional[str] = None
 
     def flip(self) -> 'Card':
         """Face up or face down the card regardles of it condition
 
         Returns:
             Card
```

### Comparing `bgameb-0.1.2/bgameb/tools.py` & `bgameb-2.0.0/bgameb/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,314 +2,88 @@
 """
 import random
 from pydantic import Field, PositiveInt
 from collections import deque
 from collections.abc import KeysView
 from heapq import heappop, heappush
 from typing import Optional, Iterable, Union, Any
-from bgameb.base import Base, Component
-from bgameb.items import Card, Dice, Step, BaseItem
-from bgameb.errors import ArrangeIndexError, ComponentClassError
+from bgameb.base import BaseTool, BaseToolExtended, Components
+from bgameb.items import Card, Dice, Step
+from bgameb.errors import ArrangeIndexError
 
 
-class BaseTool(Base):
-    """Base class for game tools
-    """
-    #: The basis of tool. Contains items.
-    c: Component[str, BaseItem] = Field(
-        default_factory=Component, exclude=True, repr=False
-            )
-    #: Current items representation of tool
-    #: like dealed and shuffled deck of csrd.
-    #: This making from Component items.
-    current: list[BaseItem] = []
-    #: Last item removed from current.
-    last: Optional[BaseItem] = None
-
-    class Config(Base.Config):
-        json_encoders = {
-            Component: lambda c: c.to_json()
-                }
-
-    @property
-    def current_ids(self) -> list[str]:
-        """Get ids of current objects
-
-        Returns:
-            List[str]: list ids of current
-        """
-        return [item.id for item in self.current]
-
-    @property
-    def last_id(self) -> Optional[str]:
-        """Get id of last
-
-        Returns:
-            Optional[str]: id
-        """
-        if self.last is not None:
-            return self.last.id
-        return None
-
-    def get_items(self) -> dict[str, BaseItem]:
-        """Get items from Component
-
-        Returns:
-            dict[str, BaseItem]: items mapping
-        """
-        return {item.id: item for item in self.c.values()}
-
-    def _item_replace(self, item: BaseItem) -> BaseItem:
-        """Get item replaced copy
-
-        Returns:
-            Item (BaseItem): an item object
-        """
-        return item.__class__(**item.dict())
-
-    def by_id(self, id: str) -> list[BaseItem]:
-        """Get item from current by its id
-
-        Args:
-            id (str): item id
-
-        Returns:
-            list[BaseItem]: items
-        """
-        return [item for item in self.current if item.id == id]
-
-    def clear(self) -> None:
-        """Clear the current and last
-        """
-        self.current.clear()
-        self.last = None
-        self._logger.debug('Current and last clear!')
-
-    def append(self, item: BaseItem) -> None:
-        """Append item to current
-
-        Args:
-            item (Item): appended items
-        """
-        item = self._item_replace(item)
-        self.current.append(item)
-        self._logger.debug(f'To current is appended item: {item.id}')
-
-    def count(self, item_id: str) -> int:
-        """Count the number of current items with given id.
-
-        Args:
-            item_id (str: an item id
-
-        Returns:
-            int: count of items
-        """
-        count = self.current_ids.count(item_id)
-        self._logger.debug(f'Count of {item_id} in current is {count}')
-        return count
-
-    def extend(self, items: Iterable[BaseItem]) -> None:
-        """Extend the current by appending items
-        started from the left side of iterable.
-
-        Args:
-            items (Iterable[Item]): iterable with items
-        """
-        items = [self._item_replace(item) for item in items]
-        self.current.extend(items)
-        self._logger.debug(
-            f'Current are extended by {[item.id for item in items]} from right'
-                )
-
-    def index(
-        self,
-        item_id: str,
-        start: int = 0,
-        end: Optional[int] = None
-            ) -> int:
-        """Return the position of item in the current
-        (after index start and before index stop).
-        Returns the first match or raises ValueError if not found.
-
-        Args:
-            item_id (str): an item id
-            start (int): start index. Default to 0.
-            end (int, optional): stop index. Default to None.
-
-        Returns:
-            int: index of the the first match
-        """
-        names = self.current_ids
-        ind = names.index(item_id, start) if end is None \
-            else names.index(item_id, start, end)
-        self._logger.debug(f'Index of {item_id} in current is {ind}')
-        return ind
-
-    def insert(self, item: BaseItem, pos: int) -> None:
-        """Insert item into the current at given position.
-
-        Args:
-            item (Item): an item object
-            pos (int): position
-        """
-        item = self._item_replace(item)
-        self.current.insert(pos, item)
-        self._logger.debug(f'To current is inserted {item.id} on {pos=}')
-
-    def pop(self) -> BaseItem:
-        """Remove and return an item from the current.
-        If no items are present, raises an IndexError.
-
-        Returns:
-            Item: an item object
-        """
-        self.last = self.current.pop()
-        self._logger.debug(f'{self.last.id} is poped from current')
-        return self.last
-
-    def remove(self, item_id: str) -> None:
-        """Remove the first occurrence of item from current.
-        If not found, raises a ValueError.
-        Args:
-            item_id (str): an item id
-        """
-        ind = self.index(item_id)
-        item = self.current[ind]
-        self.current.remove(item)
-        self._logger.debug(f'Is removed from current {item_id}')
-
-    def reverse(self) -> None:
-        """Reverse the items in the current.
-        """
-        self.current.reverse()
-        self._logger.debug('Current is reversed')
-
-
-class Bag(Base):
-    """Bag object
-
-    ..
-        Attr:
-
-            c (Component(BaseItem)):
-                The basis of tool. Contains items.
-    """
-    #: The basis of tool. Contains items.
-    c: Component[str, BaseItem] = Field(
-        default_factory=Component, exclude=True, repr=False
-            )
-
-    class Config(Base.Config):
-        json_encoders = {
-            Component: lambda c: c.to_json()
-                }
-
-    def add(self, stuff: BaseItem) -> None:
-        """Add stuff to Bag component
-
-        Args:
-            stuff (BaseItem): game stuff
-        """
-        if issubclass(stuff.__class__, BaseItem):
-            self.c.update(stuff)
-            self._logger.info(
-                f'Component updated by stuff with id="{stuff.id}".'
-                    )
-        else:
-            raise ComponentClassError(stuff, self._logger)
-
-
-class Shaker(BaseTool):
+class Shaker(BaseToolExtended[Dice]):
     """Shaker object
 
     ..
         Attr:
 
-            c (Component[Dice]): the basis of shaker. Contains dices.
-
-            current (Deque[Dice]): current dice list.
+            current (list[Dice]): Current dices representation of shaker.
+                                  This making from Components items.
 
             last (Dice), optional: last dice removed from current.
 
             last_roll (dict[str, list[PositiveInt]), optional:
                 last roll result.
 
             last_roll_mapped (dict[str, list[Any]]), optional:
                 last mapped roll result.
     """
-    #: The basis of shaker. Contains dices.
-    c: Component[str, Dice] = Field(  # type: ignore
-        default_factory=Component, exclude=True, repr=False
-            )
-    #: Current dices representation of shaker.
-    #: This making from Component items.
-    current: list[Dice] = []  # type: ignore
-    #: Last dice removed from current.
-    last: Optional[Dice] = None
-    #: Last roll result
     last_roll: dict[str, list[PositiveInt]] = {}
-    #: Last mapped roll result
     last_roll_mapped: dict[str, list[Any]] = {}
 
-    def add(self, stuff: Dice) -> None:
-        """Add dice to component of shaker
-
-        Args:
-            stuff (Dice): dice object
-        """
-        if isinstance(stuff.__class__, Dice) \
-                or issubclass(stuff.__class__, Dice):
-            self.c.update(stuff)
-            self._logger.info(
-                f'Component updated by stuff with id="{stuff.id}".'
-                    )
-        else:
-            raise ComponentClassError(stuff, self._logger)
-
-    def deal(self, items: Optional[list[str]] = None) -> 'Shaker':
+    def deal(
+        self,
+        components: Components[Dice],
+        items: Optional[list[str]] = None
+            ) -> 'Shaker':
         """Deal new shaker current. The current is cleared
         before deal.
 
         Args:
-            items (Optional[List[str]]): items ids
+            components (Components): game components
+            items (Optional[list[str]]): item ids
 
         Returns:
             Shaker
         """
         self.clear()
 
         if not items:
-            for stuff in self.c.values():
-                self.append(stuff)
+            for stuff in components.values():
+                if issubclass(stuff.__class__, Dice):
+                    self.append(stuff)
         else:
             for id in items:
-                if id in self.c.ids:
-                    self.append(self.c[id])
+                if id in components.ids:
+                    comp = components.by_id(id)
+                    if issubclass(comp.__class__, Dice):
+                        self.append(comp)
 
         self._logger.debug(f'Is deal current: {self.current_ids}')
         return self
 
     def roll(self) -> dict[str, list[int]]:
         """Roll all stuff in shaker and return results
 
         Return:
-            Dict[str, list[int]]: result of roll
+            dict[str, list[int]]: result of roll
 
         .. code-block::
             :caption: Example:
 
                 {
                     "six_dice": [5, 3, 2, 5],
                     "twenty_dice": [2, 12, 4],
                 }
         """
         self.last_roll = {}
 
         for item in self.current:
-            self.last_roll[item.id] = item.roll()
+            self.last_roll[item.id] = item.roll()  # type: ignore
 
         self._logger.debug(f'Result of roll: {self.last_roll}')
 
         return self.last_roll
 
     def roll_mapped(self) -> dict[str, list[Any]]:
         """Roll all stuff in shaker and return mapped results.
@@ -317,98 +91,81 @@
 
         Returns:
             dict[str, list[Any]]: result of roll
         """
         self.last_roll_mapped = {}
 
         for item in self.current:
-            self.last_roll_mapped[item.id] = item.roll_mapped()
+            self.last_roll_mapped[item.id] = item.roll_mapped()  # type: ignore
 
         self._logger.debug(f'Result of roll: {self.last_roll_mapped}')
 
         return self.last_roll_mapped
 
 
-class Deck(BaseTool):
+class Deck(BaseToolExtended[Card]):
     """Deck object
 
     ..
         You can add cards, define it counts and deal a deck.
         Result is saved in current attr as deque object. This object
         has all methods of
         `python deque
         <https://docs.python.org/3/library/collections.html#deque-objects>`_
 
         Attr:
 
-            c (Component[Card]): the basis of deck. Contains cards.
-
-            current (Deque[Card]): current cards deque.
+            current (Deque[Card]): Current cards representation of deck.
+                                   This making from Component items.
 
             last (Card), optional: last card, removed from current.
     """
-    #: the basis of deck. Contains cards.
-    c: Component[str, Card] = Field(  # type: ignore
-        default_factory=Component, exclude=True, repr=False
-            )
-    #: Current cards representation of deck.
-    #: This making from Component items.
     current: deque[Card] = Field(default_factory=deque)  # type: ignore
-    # Last card, removed from current.
-    last: Optional[Card] = None
-
-    def add(self, stuff: Card) -> None:
-        """Add card to component
-
-        Args:
-            stuff (Card): Card object
-        """
-        if isinstance(stuff.__class__, Card) \
-                or issubclass(stuff.__class__, Card):
-            self.c.update(stuff)
-            self._logger.info(
-                f'Component updated by stuff with id="{stuff.id}".'
-                    )
-        else:
-            raise ComponentClassError(stuff, self._logger)
 
-    def _item_replace(self, item: Card) -> Card:  # type: ignore[override]
+    def _item_replace(self, item: Card) -> Card:
         """Get replaced copy of card
 
         Args:
             item (Card): a card object
 
         Returns:
-            Card: a card object
+            Card
         """
-        item = item.__class__(**item.dict())
+        item = super()._item_replace(item)
         item.count = 1
         return item
 
-    def deal(self, items: Optional[list[str]] = None) -> 'Deck':
-        """Deal new deck current. Cured is cleared
+    def deal(
+        self,
+        components: Components[Card],
+        items: Optional[list[str]] = None
+            ) -> 'Deck':
+        """Deal new deck current. Curent is cleared
         before deal.
 
         Args:
-            items (Optional[List[str]]): list of cards ids
+            components (Components): game components
+            items (Optional[list[str]]): list of cards ids
 
         Returns:
             Deck
         """
         self.clear()
 
         if not items:
-            for stuff in self.c.values():
-                for _ in range(stuff.count):
-                    self.append(stuff)
+            for stuff in components.values():
+                if issubclass(stuff.__class__, Card):
+                    for _ in range(stuff.count):
+                        self.append(stuff)
         else:
             for id in items:
-                comp = self.c.by_id(id)
-                if comp:
-                    self.append(comp)
+                if id in components.ids:
+                    comp = components.by_id(id)
+                    if issubclass(comp.__class__, Card):
+                        self.append(comp)
 
         self._logger.debug(f'Is deal current: {self.current_ids}')
         return self
 
     def shuffle(self) -> 'Deck':
         """Random shuffle current deck.
 
@@ -445,19 +202,22 @@
                 )
 
     def popleft(self) -> Card:
         """Remove and return a card from the left side of the current deck.
         If no cards are present, raises an IndexError.
 
         Returns:
-            Card: a card object
+            Card
         """
-        self.last = self.current.popleft()
-        self._logger.debug(f'{self.last.id} is poped from left of current')
-        return self.last
+        self.last = self.current.popleft()  # type: ignore
+        self._logger.debug(
+            f'{self.last.id if self.last else None} '
+            'is poped from left of current'
+                )
+        return self.last  # type: ignore
 
     def rotate(self, n: int) -> None:
         """Rotate the current deck n steps to the right.
         If n is negative, rotate to the left.
 
         Args:
             n (int): steps to rotation
@@ -492,15 +252,15 @@
         self,
         order: list[str],
         to_arrange: Union[list[str], KeysView[str]]
             ) -> None:
         """Chek is order and deque contains same elements
 
         Args:
-            order (List[str]): ordered list of cards ids
+            order (list[str]): ordered list of cards ids
             to_arrange (list[str]): list of deque ids
 
         Raises:
             ArrangeIndexError: Given card ids and deque ids not match
         """
         if set(to_arrange) ^ set(order):
             raise ArrangeIndexError(
@@ -511,15 +271,15 @@
     def reorder(
         self,
         order: list[str],
             ) -> 'Deck':
         """Reorder current deque from right side.
 
         Args:
-            order (List[str]): ordered list of cards ids
+            order (list[str]): ordered list of cards ids
             ordered from left side to right
 
         Returns:
             Deck
         """
         len_ = len(order)
         self._check_order_len(len_)
@@ -543,15 +303,15 @@
     def reorderleft(
         self,
         order: list[str],
             ) -> 'Deck':
         """Reorder current deque from left side.
 
         Args:
-            order (List[str]): ordered list of cards ids
+            order (list[str]): ordered list of cards ids
             ordered from left side to right
 
         Returns:
             Deck
         """
         len_ = len(order)
         self._check_order_len(len_)
@@ -578,15 +338,15 @@
         start: int,
             ) -> 'Deck':
         """Reorder current deque from right side started
         with given position.
 
         Args:
             start (int): start of reordering
-            order (List[str]): ordered list of cards ids
+            order (list[str]): ordered list of cards ids
             ordered from right side to left
 
         Returns:
             Deck
         """
         len_ = len(order)
         self._check_order_len(len_)
@@ -612,15 +372,15 @@
         self,
         query: dict[str, int],
         remove: bool = True
             ) -> list[Card]:
         """Search for cards in current by its id.
 
         Args:
-            query (Dict[str, int]): dict with id of searched
+            query (dict[str, int]): dict with id of searched
                                     cards and count of searching
             remove (bool): if True - remove searched cards from
                            current deck. Default to True.
 
         Return:
             List[Card]: list of find cards, equal searching count
 
@@ -629,15 +389,15 @@
 
                 game.deck1.search(
                     {'card1': 2,
                      'card2': 1 },
                     remove=False
                     )
         """
-        for_deque: deque = deque()
+        for_deque: deque[Card] = deque()
         result = []
 
         while True:
             try:
                 card = self.current.popleft()
                 if card.id in query.keys() and query[card.id] > 0:
                     result.append(card)
@@ -662,15 +422,15 @@
 
         Args:
             count (int, optional): count of random cards. Defaults to 1.
             remove (bool, optional): if True - remove random cards from
                                      current deck. Default to True.
 
         Returns:
-            List[Card]: list of random cards
+            list[Card]: list of random cards
         """
         if not self.current:
             self._logger.debug(
                 'Is empty current deck. Random cards not choosed.'
                     )
             return []
         if not remove:
@@ -690,132 +450,70 @@
                     break
             self._logger.debug(
                 f'Random choised cards with remove: {result}'
                     )
             return result
 
 
-class Steps(BaseTool):
+class Steps(BaseTool[Step]):
     """Game steps order object
 
     ..
         Attr:
 
-            c (Component[Step]): the basis of steps. Contains steps.
-
-            current (List[Tuple[int, Step]]):
-                current representation of order in steps.
+            current (list[Step]]):
+                Current representation of order in steps.
+                This making from Component items.
 
             last (Step), optional: last poped from current step.
     """
-    #: The basis of steps. Contains steps.
-    c: Component[str, Step] = Field(  # type: ignore
-        default_factory=Component, exclude=True, repr=False
-            )
-    #: Current representation of order in steps.
-    #: This making from Component items.
-    current: list[tuple[int, Step]] = []  # type: ignore
-    #: Last step, removed from current.
+    current: list[Step] = []
     last: Optional[Step] = None
 
-    @property
-    def current_ids(self) -> list[str]:
-        """Get ids of current objects
-
-        Returns:
-            List[str]: list ids of current
-        """
-        return [item[1].id for item in self.current]
-
-    def add(self, stuff: Step) -> None:
-        """Add Step to component
-
-        Args:
-            stuff (Step): Step object
-        """
-        if isinstance(stuff.__class__, Step) \
-                or issubclass(stuff.__class__, Step):
-            self.c.update(stuff)
-            self._logger.info(
-                f'Component updated by stuff with id="{stuff.id}".'
-                    )
-        else:
-            raise ComponentClassError(stuff, self._logger)
-
     def deal(
         self,
+        components: Components[Step],
         items: Optional[list[str]] = None
             ) -> 'Steps':
         """Clear current order and create new current order
 
         Args:
-            items (Optional[List[str]]): list of stuff ids
+            components (Components): game components
+            items (Optional[list[str]]): list of stuff ids
 
         Returns:
             Steps
         """
         self.clear()
 
         if not items:
-            for stuff in self.c.values():
-                self.push(stuff)
+            for stuff in components.values():
+                if issubclass(stuff.__class__, Step):
+                    self.push(stuff)
         else:
             for id in items:
-                comp = self.c.by_id(id)
-                if comp:
-                    self.push(comp)
+                if id in components.ids:
+                    comp = components.by_id(id)
+                    if issubclass(comp.__class__, Step):
+                        self.push(comp)
 
         self._logger.debug(f'Is deal current: {self.current_ids}')
         return self
 
-    def by_id(self, id: str) -> list[BaseItem]:
-        """Get items from current by its id
-
-        Args:
-            id (str): item id
-
-        Returns:
-            list[BaseItem]: items
-        """
-        return [item[1] for item in self.current if item[1].id == id]
-
     def push(self, item: Step) -> None:
         """Push Step object to current
 
         Args:
             item (Step): Step class instance
         """
-        replaced: Step = self._item_replace(item)  # type: ignore
-        heappush(self.current, (replaced.priority, replaced))
+        replaced = self._item_replace(item)
+        heappush(self.current, replaced)
 
-    def pop(self) -> Step:
-        """Pop Step object from current with lowest priority
+    def pops(self) -> Step:
+        """Pop Step object from current with smallest priority
 
         Returns:
-            Step: Step instance object
+            Step
         """
-        self.last = heappop(self.current)[1]
+        self.last = heappop(self.current)
         self._logger.debug(f'{self.last.id} is poped from current')
         return self.last
-
-    def append(self, item: BaseItem) -> None:
-        raise NotImplementedError
-
-    def extend(self, items: Iterable[BaseItem]) -> None:
-        raise NotImplementedError
-
-    def index(
-        self,
-        item_id: str,
-        start: int = 0,
-        end: Optional[int] = None
-            ) -> int:
-        raise NotImplementedError
-
-    def insert(self, item: BaseItem, pos: int) -> None:
-        raise NotImplementedError
-
-    def remove(self, item_id: str) -> None:
-        raise NotImplementedError
-
-    def reverse(self) -> None:
-        raise NotImplementedError
```

### Comparing `bgameb-0.1.2/bgameb.egg-info/PKG-INFO` & `bgameb-2.0.0/bgameb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,111 @@
 Metadata-Version: 2.1
 Name: bgameb
-Version: 0.1.2
+Version: 2.0.0
 Summary: Board Game Builder
 Home-page: https://github.com/KonstantinKlepikov/BoardGameBuilder
 Author: Konstantin Klepikov
 Author-email: oformleno@gmail.com
 License: MIT
 Project-URL: Docs, https://konstantinklepikov.github.io/BoardGameBuilder/
 Project-URL: Source, https://github.com/KonstantinKlepikov/BoardGameBuilder
 Description: # BoardGameBuilder
         
-        !!! Project now is in very early stage. Dont use it in any apps :)
+        !!! Project now is in very early stage.
         
         [![Release and upload to pypi](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/release.yml/badge.svg)](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/release.yml)
         [![Deploy static content to Pages](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/build-docs.yml/badge.svg)](https://github.com/KonstantinKlepikov/BoardGameBuilder/actions/workflows/build-docs.yml)
         
         Object-oriented framework for build board game logic in python
         
         `pip install bgameb`
         
         ## Short example
         
         ```python
         from typing import Optional
         from pydantic import Field
         from bgameb import (
-            Game, Player, Steps, Step, Deck, Card, Shaker, Dice,
-            Bag, log_enable
+            Game,
+            Components,
+            Player,
+            Steps,
+            Step,
+            Deck,
+            Card,
+            Shaker,
+            Dice,
+            log_enable
                 )
         
         
         if __name__ == '__main__':
             log_enable()
         
+            # Defining a classes
+            class MyPlayer(Player):
+                deck: Deck
+        
             # Creating of the game
             class MyGame(Game):
                 steps: Steps
-                deck: Deck
                 shaker: Shaker
-                bag: Bag
-                players: list[Player] = []
+                me: MyPlayer
+                opp: MyPlayer
         
             # The Player and Game are an obstract containeers for tools and stuff.
             # Deck, Bag, Shaker and Steps are tools. Dice, Card and Step are items.
+            # Use Components to fill Game class
+            C = Components[Dice | Card | Step]()
         
             G = MyGame(
-                id='one board game',
-                steps=Steps(id='steps'),
-                deck=Deck(id='deck'),
-                shaker=Shaker(id='shaker'),
-                bag=Bag(id='bag'),
-                players=[Player(id='player1'), Player(id='player2')]
+                id="my game",
+                steps=Steps(id="game steps"),
+                shaker=Shaker(id="dice shaker"),
+                me=MyPlayer(
+                    id='Me',
+                    deck=Deck(id="my cards deck")
+                        ),
+                opp=MyPlayer(
+                    id='Opponent',
+                    deck=Deck(id="opponent cards deck")
+                        )
                     )
         
             # The tool objects must be filled by items by method add().
             # That because we use some other methods for check
             # data types and makes some operations with items inside tool.
         
             # Adding game tuns order in Steps tool
-            G.steps.add(Step(id='step0'))
-            G.steps.add(Step(id='step1', priority=1))
+            C.step0 = Step(id='step0')
+            C.step1 = Step(id='step1', priority=1)
         
             # Starting of new turn
-            current_steps = G.steps.deal()
+            current_steps = G.steps.deal(C)
         
             # Game steps is a priority queue, ordered by "priority" attribute
-            last = G.steps.pop()
+            last = G.steps.pops()
         
             # Adding of cards to deck. "count" parameter define how mutch
             # copies of card we must deal.
-            G.deck.add(
+            C.update(
                 Card(id='First', description='story', count=2)
                     )
-            G.deck.add(Card(id='Second', count=1))
-        
-            # All items in tools are saved in spetial object Component.
-            # Is a dict-like class. Component is predefined as attribute "c".
-            # A component usied as base for other operations with items.
-            cards_component = G.deck.c
+            C.update(Card(id='Second', count=1))
         
+            # All items in tools are saved in spetial object Components.
+            # Is a dict-like class. A component usied as base for other operations with items.
             # Any item is available in Component with dot or classic dict
             # notation. Names for that notation is transited from ids of items.
-            card = G.deck.c.first
-            card = G.deck.c['first']
+            card = C.first
+            card = C['first']
+            step = C.step0
         
             # You can get item by its id
-            card = G.deck.c.by_id('First')
+            card = C.by_id('First')
         
             # If you relocate some bult-in attrs, inherite from stuff classes,
             # then define aliases for attributes. In this example we use two
             # different solution: Field aliase and config.
             # Dont forget use G.dict(by_alias=True) to get aliases.
             # More infoshere:
             # https://docs.pydantic.dev/usage/model_config/#alias-generator
@@ -102,36 +118,36 @@
                 class Config(Card.Config):
                     fields = {'is_revealed': 'is_open'}
         
                 @property
                 def my_calculated_field(self) -> str:
                     return self.some_text.upper()
         
-            G.deck.add(
+            C.update(
                 MyCard(id='Thierd', description='story', count=3)
                     )
         
-            # Use default counters of any objects - counters not added to schema output
-            G.deck.c.first._counter['yellow'] = 12
-            G.deck.c.second._counter['banana'] = 0
+            # Use default counters of any objects - counters not added to schema
+            G.me.deck._counter['yellow'] = 12
+            G.me.deck._counter['banana'] = 0
         
             # Dealing and shuffling of deck
-            G.deck.deal().shuffle()
+            G.me.deck.deal(C).shuffle()
         
             # Adding dices to shaker
-            G.shaker.add(
+            C.update(
                 Dice(id='dice#8', sides=8, count=10)
                     )
+            G.shaker.deal(C)
         
-            # Roll dices
-            result = G.shaker.c.dice_8.roll()
+            # You can use items from Components
+            result = C.dice_8.roll()
         
-            # Use bag as collection of any items
-            G.bag.add(Dice(id='dice'))
-            G.bag.add(Card(id='card'))
+            # Or use from tool
+            result = G.shaker.roll()
         ```
         
         ## Documentation
         
         - [docs](https://konstantinklepikov.github.io/BoardGameBuilder/)
         - [pypi](https://pypi.org/project/bgameb/)
```

### Comparing `bgameb-0.1.2/bgameb.egg-info/requires.txt` & `bgameb-2.0.0/bgameb.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bgameb-0.1.2/requirements-dev.txt` & `bgameb-2.0.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bgameb-0.1.2/setup.py` & `bgameb-2.0.0/setup.py`

 * *Files identical despite different names*

