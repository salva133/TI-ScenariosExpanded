# Scenarios Expanded

Three start scenarios for Terra Invicta, each built on the world as it actually
stood on the day it begins — sovereignty, colonies, economies, alliances and
occupations taken from the historical record rather than reskinned from the
present.

The mod adds scenarios and changes nothing in existing campaigns. Every record
carries a scenario prefix and is appended to the base data, so the 2022, 2026,
2030 and 2070 scenarios — and the Dark Skies scenarios — remain untouched.

**Version 2.3.0** · Terra Invicta 1.0.51

## Installation

Copy this folder to:

```
...\Steam\steamapps\common\Terra Invicta\Mods\Enabled\ScenariosExpanded\
```

Restart the game, enable **Use Mods** on the start screen, then restart once
more. All three scenarios then appear under **Scenario**.

## The scenarios

| Scenario | Starts | Landing site |
| --- | --- | --- |
| 1898 — War for our World | 1 January 1898 | random |
| 1898 — War for our World from Mars | 1 January 1898 | random, but the aliens are based on Olympus Mons |
| 1947 — Roswell | 8 July 1947 | New Mexico |

---

### 1898 — War for our World

The year H. G. Wells published *The War of the Worlds*. 52 sovereign states,
243 nations without statehood, a fully colonial map.

| Power | Regions | of which colonial |
| --- | ---: | ---: |
| British Empire | 93 | 86 |
| Russian Empire | 40 | — |
| French Republic | 34 | 26 |
| Great Qing | 26 | — |
| Ottoman Empire | 19 | — |
| United States | 16 | — |

World economic output is two percent of the present-day figure, distributed by
the 1900 GDP shares from the Maddison Project. World population 1.68 billion. No
nuclear weapons, no space budget, no human habitats. Miltech runs 0.2 to 1.6
instead of 4.2 to 4.5. 295 ppm of CO₂, sea level 20 cm below today's.

Spain still holds Cuba, Puerto Rico and the Philippines: the start date is
1 January, three months before the Spanish-American War breaks out.

**Federations.** Triple Alliance (German Empire, Empire of Austria, Kingdom of
Hungary, Kingdom of Italy), Franco-Russian Alliance, Union of Sweden and Norway.
Austria-Hungary is modelled as two nations because Cisleithania and
Transleithania were separate states sharing a foreign policy and army. Britain
keeps to its splendid isolation; its only alliance is the old one with Portugal.

Russia is coloured green and Portugal purple, as in the colonial atlases of the
period. The base game has those two the other way round.

### 1898 — War for our World from Mars

The same world, but the invaders come from Mars as in Wells: headquarters on
Olympus Mons, station in low Mars orbit. The enemy is known from the start and
far closer to Earth than usual. Both 1898 scenarios share nations, regions,
armies and start time, and differ only in their habitat group.

### 1947 — Roswell

The day Roswell Army Air Field reported recovering a flying disc. The disc comes
down over New Mexico, which is the `RockyMountains` region.

67 sovereign states. The Cold War is four weeks past the Marshall Plan
announcement and India is five weeks from independence — on 8 July it is still
British, and so are Pakistan, Bangladesh, Burma, Ceylon and Malaya.

| Power | Regions | of which colonial |
| --- | ---: | ---: |
| British Empire | 79 | 73 |
| Soviet Union | 42 | 3 |
| French Republic | 38 | 30 |
| Republic of China | 26 | — |
| United States | 25 | 8 |
| Netherlands | 11 | 9 |

World economic output is five percent of the present-day figure; the United
States alone holds close to a quarter of it. World population 2.46 billion,
growing fast. Only the United States has nuclear weapons — the Soviet test is
two years away. Space funding exists only as captured German rocket programmes.

**The spoils of war.** Germany, Austria, Japan and Korea do not exist as states
in 1947. Their territory belongs to the victors and is held as colonies:

| Region | Held by |
| --- | --- |
| Germany (Bremen, Hamburg, Lower Saxony, North Rhine-Westphalia) | Britain |
| Bavaria (the American and French zones in the south) | United States |
| EastGermany (Berlin, Brandenburg, Mecklenburg, Saxony) | Soviet Union |
| Vienna (all of Austria) | Soviet Union |
| Hokkaido, North Honshu, South Honshu, Kyushu and Shikoku | United States |
| Ryukyus (Okinawa) | United States |
| SouthKorea | United States |
| NorthKorea | Soviet Union |

The four names remain defined, so if any of them re-emerges during a campaign it
is called Germany, Austria, Japan or Korea rather than something occupied. Their
economic weight is counted towards whoever holds the ground. Garrisons of the
respective victor stand in each region.

Austria is a single region covering the whole country. Vienna itself lay in the
Soviet zone and was administered jointly by all four powers, so the Soviet Union
holds it here.

East Prussia goes to the Soviet Union, Danzig and Upper Silesia to Poland. Libya,
Eritrea and Somalia are under British military administration after Italy lost
its empire in the war.

**Blocs.** The Soviet Union, Poland, Czechoslovakia, Hungary, Romania, Bulgaria
and Albania form a federation. Because Russia is authoritarian it will read as a
dark federation: members leave only with Moscow's consent. This matches the
situation after the Prague coup of February 1948 more closely than the summer of
1947, but it is the clearest way to represent the bloc.

Yugoslavia holds Croatia, Slovenia, Bosnia, Macedonia, Montenegro and Kosovo;
Czechoslovakia holds Slovakia. The Indo-Pakistani rivalry is absent — it begins
with partition five weeks after the scenario starts.

The Soviet Union is dark red and flies the USSR flag from the base game's flag
bundle. Afghanistan and Yemen use their period flags.

## Known limitations

- Organisations, councillors and portraits come from the present-day set,
  because the game will not start without them. Names like NASA or CIA are
  anachronistic in every scenario here.
- The three base technologies `WeAreNotAlone`, `Skywatch` and `MissionToSpace`
  remain set so that the tech tree and interface keep working.
- The map itself is unchanged. Borders follow present-day region boundaries;
  only ownership differs.
- In 1898 no nation has space funding, boost capacity or mission control at all.
  Getting off the planet has to be built from nothing.
- The flag bundle holds nothing for the empires of 1898, so those nations fly
  their modern flags. Britain and Germany at least fly the union jack and the
  German tricolour rather than the flags of England and East Germany.
- Federation names are not localised. This is also true of the base game's.
- Rivalries cannot exist inside a federation, which costs the Italian irredenta
  against Austria in 1898 and the Tito-Stalin split in 1947.

## Building

`build.py` runs each scenario generator into its own folder and merges the
results, because Terra Invicta reads only one file per template type per mod. It
warns on any duplicate identifier. `checkall.py` then validates the merged mod
against the base game's templates.

## Changelog

### 2.3.0

- Nation names carry no form of government any more. Kingdom, Empire, Sultanate,
  Emirate, Republic and the like are dropped; only the country name remains, so
  Italy is Italy and not the Kingdom of Italy. Four names keep theirs because
  nothing usable is left otherwise: the Ottoman Empire, the Soviet Union, the
  United States and the Dominican Republic.
- Localisation files now list only the names that actually differ from the base
  game — 20 of 52 states in 1898, 17 of 67 in 1947. Everything else falls back
  to the standard name on its own.

### 2.2.0

- No nation switches to the flag of a future union any more. The base game has
  36 of them do that — France to the European Union, Russia to the Eurasian
  Union, China to the Pan-Asian Cooperative — none of which existed in either
  period. `unionFlagResource` now matches the national flag everywhere.
- Britain flies the union jack instead of the flag of England, Germany the
  German tricolour instead of East Germany's, and Yugoslavia its own flag
  in 1947.

### 2.1.0

- Germany, Austria, Japan and Korea no longer exist as occupied states in 1947.
  Their territory passes to the victors as colonies, zone by zone, and the four
  names are kept for the case that they re-emerge.
- The Soviet Union is dark red and flies the USSR flag.

### 2.0.0

- Renamed from *1898 — War for our World* to *Scenarios Expanded*, since the mod
  now carries more than one period.
- Added *1947 — Roswell*.
- Build pipeline reworked: each scenario is generated separately and merged into
  one mod.

### 1.7.0

- Russia green, Portugal purple, matching the colonial atlases.

### 1.6.0

- Fixed the crash in `TIFactionState.NewCampaign()`. The alien administration
  `ALN` must be listed unprefixed in the nation group; a prefixed duplicate
  lacks `initialFactionStr` and leaves the alien council without a nation.
- `GameVersion` corrected to 1.0.51.

### 1.5.0

- Added the Mars variant.

### 1.4.0

- Added `AlienHQ` and `AlienHQStation`, which were missing from the habitat list.
- Localisation switched to the Dark Skies pattern using
  `scenarioLocalizationPostfix`.

### 1.3.0

- Renamed to *1898 — War for our World*.

### 1.2.0

- Removed the Russian occupation of Donetsk, inherited from the base game.
- Capital claims are no longer trimmed; `capitalClaim` denotes the intended
  capital, not the one held.

### 1.1.0

- Added federations.

### 1.0.0

- Initial release.
