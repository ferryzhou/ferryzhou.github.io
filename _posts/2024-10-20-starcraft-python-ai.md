---
title: "starcraft python ai"
date: 2024-10-20
---

yesterday night, accidentally see starcraft ai bot game on yt

and curious on how to build an sc2 ai bot

so searched and found <a href="https://youtu.be/v3LJ6VvpfgI?si=JqroLLZudEd0MIPd">https://youtu.be/v3LJ6VvpfgI?si=JqroLLZudEd0MIPd</a>

and then tried it

<a href="https://github.com/BurnySc2/python-sc2/tree/develop">https://github.com/BurnySc2/python-sc2/tree/develop</a>

download maps from <a href="https://github.com/Blizzard/s2client-proto?tab=readme-ov-file#map-packs">https://github.com/Blizzard/s2client-proto?tab=readme-ov-file#map-packs</a>

2017 Season 4

copied to C:\Program Files (x86)\StarCraft II\Maps

Edit examples/protoss/cannon_rush.py, change map name to &quot;CatalystLE&quot;

python examples/protoss/cannon_rush.py

I also added 'C:\Users\ferry\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.12_qbz5n2kfra8p0\LocalCache\local-packages\Python312\Scripts' to PATH. // on windows, search Environment Variables.

and it succeeded!

For the hard level, the strategy works. I changed from hard to very hard. now the strategy does not work, and needs improvement.

C:\Users\ferry\python-sc2&gt;python examples/protoss/cannon_rush.py
2024-10-20 09:20:22.079 | INFO | sc2.protocol:_execute:72 - Client status changed to Status.launched (was None)
2024-10-20 09:20:22.080 | INFO | sc2.controller:create_game:37 - Creating new game
2024-10-20 09:20:22.081 | INFO | sc2.controller:create_game:38 - Map: CatalystLE
2024-10-20 09:20:22.082 | INFO | sc2.controller:create_game:39 - Players: Bot CannonRushBot(Protoss), name='CheeseCannon'), Computer VeryHard(Protoss, RandomBuild)
2024-10-20 09:20:22.084 | INFO | sc2.protocol:_execute:72 - Client status changed to Status.init_game (was Status.launched)
2024-10-20 09:20:30.110 | INFO | sc2.protocol:_execute:72 - Client status changed to Status.in_game (was None)
2024-10-20 09:20:30.112 | INFO | sc2.main:_play_game:221 - Player 1 - CheeseCannon
2024-10-20 09:21:37.371 | INFO | sc2.protocol:_execute:72 - Client status changed to Status.ended (was Status.in_game)
2024-10-20 09:21:37.373 | INFO | sc2.main:_play_game:228 - Result for player 1 - CheeseCannon: Defeat
2024-10-20 09:21:38.579 | INFO | sc2.protocol:__request:48 - Cannot receive: Game has already ended.
2024-10-20 09:21:38.580 | INFO | sc2.sc2process:_close_connection:231 - Closing connection at 52102...
2024-10-20 09:21:38.580 | INFO | sc2.sc2process:kill_all:33 - kill_switch: Process cleanup for 1 processes
