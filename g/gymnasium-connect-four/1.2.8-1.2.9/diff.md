# Comparing `tmp/gymnasium_connect_four-1.2.8.tar.gz` & `tmp/gymnasium_connect_four-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.8.tar", last modified: Wed Aug  2 19:17:18 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.9.tar", last modified: Fri Aug  4 06:05:54 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.8.tar` & `gymnasium_connect_four-1.2.9.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.092477 gymnasium_connect_four-1.2.8/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      251 2023-08-02 19:17:18.090965 gymnasium_connect_four-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    11454 2023-07-30 17:35:07.000000 gymnasium_connect_four-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.050360 gymnasium_connect_four-1.2.8/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     9269 2023-08-02 18:59:02.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.071167 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4654 2023-07-30 16:49:29.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:19.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0      649 2023-07-30 17:27:29.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabySmarterPlayer.py
--rw-rw-rw-   0        0        0     1920 2023-07-30 16:50:55.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2248 2023-07-30 16:50:49.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3163 2023-07-30 16:49:44.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:36.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      496 2023-07-30 16:31:44.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.075350 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     4056 2023-08-02 18:56:57.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4805 2023-07-30 16:46:39.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.084500 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1166 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 19:17:18.092477 gymnasium_connect_four-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-08-02 19:17:08.000000 gymnasium_connect_four-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.089966 gymnasium_connect_four-1.2.8/test/
--rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.8/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21564 2023-08-02 19:14:09.000000 gymnasium_connect_four-1.2.8/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.8/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:05:54.312973 gymnasium_connect_four-1.2.9/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-08-04 06:05:54.312973 gymnasium_connect_four-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11454 2023-07-30 17:35:07.000000 gymnasium_connect_four-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 06:05:54.285973 gymnasium_connect_four-1.2.9/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9269 2023-08-03 20:45:59.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:05:54.300973 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-08-04 06:00:47.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-08-04 06:02:14.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-08-03 20:45:14.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0      649 2023-08-04 06:01:41.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/BabySmarterPlayer.py
+-rw-rw-rw-   0        0        0     1920 2023-08-04 06:01:27.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-08-04 06:01:03.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0     4317 2023-08-04 06:04:43.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/SelfTrained1Player.py
+-rw-rw-rw-   0        0        0     4312 2023-08-04 06:04:38.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/SelfTrained2Player.py
+-rw-rw-rw-   0        0        0     4314 2023-08-04 06:04:57.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/SelfTrained3Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-08-04 06:05:00.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-08-04 06:05:03.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-08-04 05:36:28.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:05:54.303972 gymnasium_connect_four-1.2.9/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     4331 2023-08-04 06:05:16.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     5367 2023-08-04 06:03:40.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.9/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:05:54.308973 gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-08-04 06:05:54.000000 gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2023-08-04 06:05:54.000000 gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 06:05:54.000000 gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-04 06:05:54.000000 gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-04 06:05:54.000000 gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 06:05:54.312973 gymnasium_connect_four-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-08-04 06:05:37.000000 gymnasium_connect_four-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:05:54.311973 gymnasium_connect_four-1.2.9/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.9/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-08-02 19:14:09.000000 gymnasium_connect_four-1.2.9/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.9/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.8/LICENSE` & `gymnasium_connect_four-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/README.md` & `gymnasium_connect_four-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         else:
             return self.play_single(obs)
 
     def getName(self):
         return "AdultPlayer"
 
     def getElo(self):
-        return 1666
+        return 1665
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,11 +106,11 @@
 
         return False
 
     def getName(self):
         return "AdultSmarterPlayer"
     
     def getElo(self):
-        return 1802
+        return 1792
     
     def isDeterministic(self):
         return False
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabySmarterPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/BabySmarterPlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,11 +16,11 @@
         else:
             return self.play_single(observation)
 
     def getName(self):
         return "BabySmarterPlayer"
 
     def getElo(self):
-        return 1060
+        return 1058
 
     def isDeterministic(self):
         return False
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         valid_moves = [c for c in range(7) if observation[0, c] == 0]
         return np.random.choice(valid_moves)
 
     def getName(self):
         return "ChildPlayer"
     
     def getElo(self):
-        return 1272
+        return 1266
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         else:
             return self.play_single(observation)
 
     def getName(self):
         return "ChildSmarterPlayer"
 
     def getElo(self):
-        return 1571
+        return 1584
 
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         else:
             return self.play_single(obs)
 
     def getName(self):
         return "TeenagerPlayer"
 
     def getElo(self):
-        return 1655
+        return 1657
 
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         else:
             return self.play_single(obs)
 
     def getName(self):
         return "TeenagerSmarterPlayer"
 
     def getElo(self):
-        return 1658
+        return 1663
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,36 @@
     BabySmarterPlayer,
     ChildPlayer,
     ChildSmarterPlayer,
     TeenagerPlayer,
     TeenagerSmarterPlayer,
     AdultPlayer,
     AdultSmarterPlayer,
+    SelfTrained1Player,
+    SelfTrained2Player,
+    SelfTrained3Player,
 )
 
 class EloLeaderboard:
     def __init__(self):
         # Initialize the list of players
         self.playersWithEloFixed = [
             BabyPlayer(),
             BabySmarterPlayer(),
             ChildPlayer(),
+            SelfTrained1Player(),
             ChildSmarterPlayer(),
             TeenagerPlayer(),
             TeenagerSmarterPlayer(),
             AdultPlayer(),
             AdultSmarterPlayer(),
+            SelfTrained2Player(),
+            SelfTrained3Player(),
+
+            
         ]
 
     def update_elo(self, player_elo, opponent_elo, player_won, k_factor=32, draw=False):
         # Calculate the expected outcome based on the current Elo ratings
         expected_outcome = 1 / (1 + math.pow(10, (opponent_elo - player_elo) / 400))
         # Set the actual outcome based on whether the player won, lost, or drew
         if draw:
@@ -47,15 +55,16 @@
 
     def play_rounds(self, player, actualElo, num_matches):
         gamePlayed = 0
         match_results = []
         for _ in range(num_matches):
             closest_opponents = self.get_closest_opponents(actualElo, num_opponents=2)
             random.shuffle(closest_opponents)
-            scores = self.get_scores(player, closest_opponents)
+            scores =[True,True]# self.get_scores(player, closest_opponents)
+            # scores = self.get_scores(player, closest_opponents)
             for opponent, score in zip(closest_opponents, scores):
                 player_won = score > 0
                 draw = score == 0
                 match_results.append((player_won, draw, opponent.getElo()))
                 k_factor = 400 / (1 + (gamePlayed))
                 actualElo = self.update_elo(actualElo, opponent.getElo(), player_won, k_factor, draw)
                 gamePlayed += 1
@@ -96,10 +105,10 @@
         return scores
 
 
 if __name__ == "__main__":
     import time
     elo_leaderboard = EloLeaderboard()
     start_time = time.time()
-    print(elo_leaderboard.get_elo(BabySmarterPlayer(), num_matches=20))
+    print(elo_leaderboard.get_elo(SelfTrained3Player(), num_matches=500))
     end_time = time.time()
-    print(f"Time elapsed: {end_time - start_time} seconds")
+    print(f"Time elapsed: {end_time - start_time} seconds")
```

### Comparing `gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.9/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,35 @@
     BabySmarterPlayer,
     ChildPlayer,
     ChildSmarterPlayer,
     TeenagerPlayer,
     TeenagerSmarterPlayer,
     AdultPlayer,
     AdultSmarterPlayer,
+    SelfTrained1Player,
+    SelfTrained2Player,
+    SelfTrained3Player,
 )
 
 
 class EloLeaderboard:
     def __init__(self):
         # Initialize the list of players
         self.players = [
             BabyPlayer(),
             BabySmarterPlayer(),
             ChildPlayer(),
             ChildSmarterPlayer(),
             TeenagerPlayer(),
             TeenagerSmarterPlayer(),
             AdultPlayer(),
-            AdultSmarterPlayer()
+            AdultSmarterPlayer(),
+            SelfTrained1Player(),
+            SelfTrained2Player(),
+            SelfTrained3Player(),
         ]
         # Initialize the Elo rankings for each player
         self.elo_rankings = {player.getName(): player.getElo() if player.getElo() is not None else 1500 for player in self.players}
 
     def update_elo(self, player_elo, opponent_elo, player_won, k_factor=32, draw=False):
         # Calculate the expected outcome based on the current Elo ratings
         expected_outcome = 1 / (1 + math.pow(10, (opponent_elo - player_elo) / 400))
@@ -68,20 +74,21 @@
         # Add new players to the leaderboard
         self.players.extend(new_players)
         for player in new_players:
             self.elo_rankings[player.getName()] = player.getElo() if player.getElo() is not None else 1500
 
         # Play the specified number of matches
         for i in range(num_matches):
-            k_factor = 0.05 / (1 + 1 / 10)
-            self.play_round(k_factor, move_elo_already_known)
+            k_factor = 0.1 / (1 + 1 / 10)
             if display_log:
-                print(f"Elo rankings after {i+1} matches:")
+                print(f"Elo rankings after {i} matches:")
                 self.display_rankings()
                 print("\n")
+            self.play_round(k_factor, move_elo_already_known)
+            
 
         # Return the updated Elo ratings for the new players
         new_player_elos = [self.elo_rankings[player.getName()] for player in new_players]
         return new_player_elos
 
     def display_rankings(self):
         # Sort the rankings in descending order of Elo ratings
@@ -102,8 +109,23 @@
                 obs, _ = env.reset()
                 return rewards
 
 
 if __name__ == "__main__":
 
     elo_leaderboard = EloLeaderboard()
-    print(elo_leaderboard.get_elo([], num_matches=100000,display_log=True,move_elo_already_known=True))
+    print(elo_leaderboard.get_elo([], num_matches=400,display_log=True,move_elo_already_known=True))
+
+
+# Elo rankings after 233 matches:
+# 0. max 2538
+# 1. SelfTrained3Player: 2020
+# 2. SelfTrained2Player: 1944
+# 3. AdultSmarterPlayer: 1792
+# 4. AdultPlayer: 1665
+# 5. TeenagerSmarterPlayer: 1663
+# 6. TeenagerPlayer: 1657
+# 7. ChildSmarterPlayer: 1584
+# 8. SelfTrained1Player: 1385
+# 9. ChildPlayer: 1266
+# 10. BabySmarterPlayer: 1058
+# 11. BabyPlayer: 1000
```

### Comparing `gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.9/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 connect_four_gymnasium/players/BabyPlayer.py
 connect_four_gymnasium/players/BabySmarterPlayer.py
 connect_four_gymnasium/players/ChildPlayer.py
 connect_four_gymnasium/players/ChildSmarterPlayer.py
 connect_four_gymnasium/players/ConsolePlayer.py
 connect_four_gymnasium/players/ModelPlayer.py
 connect_four_gymnasium/players/Player.py
+connect_four_gymnasium/players/SelfTrained1Player.py
+connect_four_gymnasium/players/SelfTrained2Player.py
+connect_four_gymnasium/players/SelfTrained3Player.py
 connect_four_gymnasium/players/SimulatePlayer.py
 connect_four_gymnasium/players/TeenagerPlayer.py
 connect_four_gymnasium/players/TeenagerSmarterPlayer.py
 connect_four_gymnasium/players/__init__.py
 connect_four_gymnasium/tools/EloLeaderboard.py
 connect_four_gymnasium/tools/Update_bot_elo.py
 connect_four_gymnasium/tools/__init__.py
```

### Comparing `gymnasium_connect_four-1.2.8/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.9/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.9/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.8/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.9/test/test_ppo_env.py`

 * *Files identical despite different names*

