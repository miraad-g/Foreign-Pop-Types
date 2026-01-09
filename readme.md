# Foreign Pop Types
A mod for Europa Universalis V that adds new worker types for all foreign buildings in the game.

[![Steam Workshop](https://img.shields.io/badge/Steam%20Workshop-Subscribe-blue)](https://steamcommunity.com/sharedfiles/filedetails/?id=3640891677)

## Overview
Currently (as of version 1.0.10), the game has a bug that prevents the construction of foreign buildings in locations that already have pops of the same religion and culture.
Equally important, if a location has too many pops of the same type but different cultures/religions, the game automatically merges the smaller group into the larger one. This means that when building, for example, a Trade Office, there is a risk that all Burghers in that location will start counting as *your* Burghers. The same applies to other types of foreign buildings. This **significantly** impacts estates power, in extreme cases creating situations where your country has more foreign pops than domestic ones. Paradox has acknowledged this behavior as [WAD](https://forum.paradoxplaza.com/forum/threads/foreign-pops-counted-as-my-own-population-in-foreign-locations-where-i-built-a-trade-office.1873234/), which I strongly disagree with.

This mod solves both of these problems.

## Features
* Added 6 new foreign pop types, analogous to all existing ones except Tribesmen and Slaves. They are functionally identical to standard pops and exert the same influence on the location/country. The same modifiers apply to them.
* The worker type for all foreign buildings has been changed to their foreign counterpart.
* Slightly reworked the interface for the cards that filter buildings by worker type. By default, foreign type cards are hidden to avoid cluttering the UI. You can toggle the view by right-clicking on any of the cards.

![Cards demonstration](https://i.ibb.co/sds3w5Ht/image.png)

## Fixes Explanation
* Since foreign building workers are now a different pop type, you can construct buildings in locations with pops of the same culture and religion. The game only checks for identical pop types, so no conflict occurs.
* Foreign pop types will not merge with standard pop types, solving the "capture" issue. However, they are still counted as part of both your country and the country where the building is located. I consider this WAD, as it prevents the merging of excessively large groups that would unreasonably skew your estates power. Otherwise, it seems logical that workers residing abroad should influence both countries.

## Localization
The mod is available in the following languages:
* English
* Русский
* Português

For other languages available in the game, the mod will display in English without placeholders. The mod contains little new text, and all tooltips are identical to their vanilla counterparts.

## Compatibility
* Not compatible with Ironman.
* Fully compatible with existing saves.
* *Should be* compatible with any other mods. No vanilla files are overwritten; all changes are applied to existing objects. It is recommended to load this mod last to ensure its changes take priority.
* Slightly modifies the GUI (toggleable), but overwriting this will not break the mod.

## Known Issues
* The issue with building foreign constructions in locations of the same culture and religion may reappear if another country builds a foreign building there first. I am currently developing a separate mod to circumvent this specific issue (almost complete).
* Identical foreign pop groups will still merge when the location limit is reached (4 for same religion, 8 for different religions). However, this does not cause major problems, as their number is relatively small compared to the total population. This can be fixed by changing the limit values in 00_defines.txt, but it will likely have a significant performance impact, especially in the late game.
* Foreign pop types spawn with zero literacy. This is a known bug affecting all pop types. We are waiting for Paradox to fix it.

## Installation
Subscribe to the mod on the [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3640891677).

### Manual Installation
* Download this repository.
* Copy the contents to your Documents\Paradox Interactive\Europa Universalis V\mod\ folder.
* Enable it in the game as usual.

#### Special thanks to Conner for the inspiration! Check out his [mods](https://steamcommunity.com/workshop/filedetails/?id=3619138120) too — they're great.