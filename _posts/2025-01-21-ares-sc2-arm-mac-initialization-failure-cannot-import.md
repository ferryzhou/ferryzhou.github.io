---
title: "ares-sc2 arm mac initialization failure cannot import"
date: 2025-01-21
---

ImportError: numpy.core.multiarray failed to import

ModuleNotFoundError: No module named 'mapanalyzerext'

ModuleNotFoundError: No module named 'sc2_helper.sc2_helper'

So download 12PoolBot from <a href="https://aiarena.net/bots/357/">https://aiarena.net/bots/357/</a>

unzip

and copy all the binary files for

map_analyzer/cext

ares-sc2/sc2_helper

also remember on mac, to zip, not zip the bot folder, but select all the files in bot folder and compress. otherwise it will report errors.

note that when uploading a bad zip to an existing bot, it will not report any error. it just silently fails. the last updated time will keep the same. that can indicate errors.
