---
title: "ares debug"
date: 2025-01-26
---

qin2's elo dropped below 1500.

map EphemeronAIE win rate ~10%

downloaded some replay, noticed that it stuck in the beginning

tested local, got the following error

2025-01-26 15:29:11.390 | INFO | ares.behaviors.macro.tech_up:execute:110 - 00:41 Building UnitTypeId.GATEWAY for UnitTypeId.STALKER

2025-01-26 15:29:11.393 | INFO | ares.managers.placement_manager:request_building_placement:459 - 00:41: No available BuildingSize.THREE_BY_THREE found anywhere on map, giving up.

The base terrain is too small. need to find a way to walk around.

the issue is in sturcture_to_building_size.py, where the size is hard coded:

"UnitID.GATEWAY: BuildingSize.THREE_BY_THREE,"

most of the protoss building map to 3x3.

Update: so a quick fix is add @ ramp for the first pylon.

in this way, there will always be available placements.

tried changing size of the building, that will make building stuck from the beginning, for any map.
