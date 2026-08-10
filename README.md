# Scenarios Expanded

Two start scenarios for Terra Invicta, each built on the world as it actually
stood on the day it begins — sovereignty, colonies, economies, alliances and
occupations taken from the historical record rather than reskinned from the
present.

The mod adds scenarios and changes nothing in existing campaigns. Every record
carries a scenario prefix and is appended to the base data, so the 2022, 2026,
2030 and 2070 scenarios — and the Dark Skies scenarios — remain untouched.

**Version 2.7.0** · Terra Invicta 1.0.51

## Installation

Copy this folder to:

```
...\Steam\steamapps\common\Terra Invicta\Mods\Enabled\ScenariosExpanded\
```

Restart the game, enable **Use Mods** on the start screen, then restart once
more. Both scenarios then appear under **Scenario**.

## The scenarios

| Scenario | Starts | Landing site |
| --- | --- | --- |
| 1898 — War for our World | 1 January 1898 | random |
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
nuclear weapons, no space budget, no human habitats. Miltech runs 1.0 to 2.5
instead of the 3 to 5 of the present day. 295 ppm of CO₂ and a sea level 21 cm
below today's.

Spain still holds Cuba, Puerto Rico and the Philippines: the start date is
1 January, three months before the Spanish-American War breaks out.

**Federations.** Triple Alliance (German Empire, Empire of Austria, Kingdom of
Hungary, Kingdom of Italy), Franco-Russian Alliance, Union of Sweden and Norway.
Austria-Hungary is modelled as two nations because Cisleithania and
Transleithania were separate states sharing a foreign policy and army. Britain
keeps to its splendid isolation; its only alliance is the old one with Portugal.

Russia is coloured green and Portugal purple, as in the colonial atlases of the
period. The base game has those two the other way round.

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

---

## The environment

### The atmosphere

The greenhouse gases are the annual values of the historical series the climate
models are calibrated on — Law Dome ice cores spliced to the instrumental record,
as compiled for MAGICC and later for CMIP6.

| | 1898 | 1947 |
| --- | ---: | ---: |
| CO₂ | 295.0 ppm | 310.0 ppm |
| CH₄ | 0.88 ppm | 1.13 ppm |
| N₂O | 0.28 ppm | 0.288 ppm |
| Stratospheric aerosols | 0 | 0 |

Both years are volcanically quiet. Krakatoa had cleared the stratosphere long
before 1898, and Santa María and Katmai were still to come; 1947 sits in the long
gap between Katmai and Agung. Neither start carries excess aerosols.

### The sea

The game does not measure its sea level anomaly against the present. The 2022
campaign starts at +24 cm, which is the rise since roughly 1880 — the same
baseline the tide-gauge reconstructions use. 1898 therefore starts at +3 cm and
1947 at +9 cm. Both scenarios previously carried the distance to the present day
instead, which put the water some 20 cm too low.

### Sustainability

Every nation carries a sustainability value, the divisor of its pollution
multiplier: the lower it is, the more greenhouse gas the economy emits for its
size. The base game runs from about 0 to 3; at 10 a nation would take gas back
out of the atmosphere, which nothing in these two periods comes close to.

The values here are the carbon intensity of each nation as it is actually
constituted in the scenario, colonies included. For every region a nation holds,
the fossil and land-use emissions of the modern country that region belongs to
are taken from the Global Carbon Budget for the start year, split by population,
and summed; the total is divided by the nation's GDP. That ratio is scaled
against the world figure for 2022 and compressed by a square root, because the
raw spread runs to two orders of magnitude and the game's scale does not.

The result is that the dirty nations are not the industrial ones. Britain burnt
a third of the world's coal in 1898 and still lands at 0.3, the same as Brazil,
because the measure is emissions against the size of the economy — and the
economies clearing rainforest for a fraction of Britain's output come out worse.
Colombia, Nicaragua and Bolivia sit at 0.2, the Ottoman Empire and Bulgaria at
1.6. Oman and Yemen reach the top of the band at 3.0, having neither coal to
burn nor forest to clear. The base game orders its present-day nations the same way, which is why
China and much of Africa start below the European figures.

The world averages 0.54 in 1898 and 0.53 in 1947, against roughly 1.0 today.
Together with the historical GDP figures that puts world emissions in 1898 at
about four percent of the present, which is where the fossil record has them.
The flat zero the mod shipped before meant every nation emitted at the maximum
multiplier the game allows.

## Military technology

Miltech is a single number per nation doing two jobs. The difference between two
nations decides how often they hit each other; the absolute value decides how
hard. A hit takes about a tenth of the attacker's miltech in percent of the
target's health, so two armies at 0.3 need some thirty hits apiece to settle
matters, where the present-day campaigns are done in two or three. Armies also
repair themselves out of combat, and at the bottom of the scale the repairs can
outrun the damage, at which point a war stops resolving at all.

The band therefore starts at 1.0, the point where a hit takes a tenth of the
target. 1898 runs 1.0 to 2.5, 1947 runs 1.0 to 3.4. The whole band is shifted,
not stretched: every distance between two nations is the one the historical
reading gave them, so the hit chances between any two of them are untouched. The
one thing that changes with the floor is the ratio in damage between the
strongest and the weakest, which narrows — the Bhutanese army is no longer
fighting at a fortieth of the German rate, but at a sixth.

The order is the historical one. Germany and Britain lead 1898, Germany for the
general staff, the Krupp guns and the Gewehr 98, Britain for the fleet rather
than for the army that was about to embarrass itself in South Africa. France
follows with the Canon de 75 of 1897, the best field gun in the world. The
United States sits below Russia and Austria because its army in 1898 was 28,000
regulars, with volunteers still carrying black powder and an artillery park a
generation old; only the navy was new. Spain sits below the United States, which
is how that war went, and the Ottoman Empire above Greece, which is how the war
of 1897 went. China sits at 1.5, level with Portugal and Greece, three years
after the Japanese took the Beiyang fleet apart.

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

### 2.7.0

- Raised the miltech band. Damage in ground combat is proportional to the
  attacker's absolute miltech, so at the old values a battle took some ten times
  the rounds of a present-day one, and two weak nations could repair faster than
  they could hurt each other. 1898 now runs 1.0 to 2.5 and 1947 1.0 to 3.4,
  where they ran 0.1 to 1.6 and 0.2 to 2.6.
- The band is shifted, not stretched. Hit chances depend only on the difference
  between two nations, and every difference is unchanged, so no nation gained or
  lost ground against any other. The order is untouched.

### 2.6.0

- Corrected the greenhouse gases. N₂O stood at 0.29 ppm in 1898, which is the
  concentration of 1953 and also the exact threshold above which the game counts
  the gas at all; the ice cores give 0.2797 ppm for that year. CH₄ was 20 to
  25 ppb high in both scenarios. CO₂ was already right in both.
- Corrected the sea level. The game counts its anomaly from about 1880, not from
  the present day: the 2022 campaign starts at +24 cm. 1898 therefore stands at
  +3 cm and 1947 at +9 cm, where the mod had −20 and −3. The two old values were
  not even consistent with each other — they were 17 cm apart, where the
  reconstructions have the two years 6 cm apart.
- Every nation now carries a sustainability value of its own, computed from the
  fossil and land-use emissions of the ground it holds against its GDP. They ran
  a flat 0.0 before, which meant every nation on the map emitted at the highest
  pollution multiplier the game has.

### 2.5.0

- Removed the Mars variant. `TIFactionState.NewCampaign()` looks up the habitat
  templates `AlienHQ` and `AlienHQStation` by their literal names, without
  applying `scenarioPrefix`, so `1898M_AlienHQ` was never found and the method
  ran into a null reference. The orbit of the alien station is hard-coded to
  `LowNeptuneOrbit` as well. A scenario-specific alien headquarters is therefore
  not possible through templates, and the variant is gone rather than shipped
  broken. `checkall.py` now rejects any prefixed headquarters.
- The mod is back to two scenarios and 2.1 MB.

### 2.4.0

- Fixed the crash when starting the Mars variant. `AlienHQ` is hard-coded in the
  game's assembly: the alien headquarters must carry exactly that name or
  `TIFactionState.NewCampaign()` cannot find it. Renaming it to
  `1898_AlienHQMars` broke the scenario. The Mars variant now has its own prefix
  `1898M_` and defines `1898M_AlienHQ`, which the game resolves through
  `scenarioPrefix` before falling back to the base entry.
- As a consequence the two 1898 scenarios no longer share their data; each ships
  a full prefixed set. The mod grows from 2.1 to 3.1 MB.
- `build.py` now clears each generator's output folder before running, so no
  file survives from an earlier build that the generator no longer writes.

### 2.3.1

- Fixed nations taking the name of a future union. The base game gives 30 of the
  states in these scenarios a union name that applies once they hold enough
  ground: France becomes the European Union, Australia the Republic of the
  Southern Cross, Colombia Greater Colombia, Poland the Intermarium, China the
  Pan-Asian Cooperative. All union names now match the national name. Version
  2.3.0 made this worse by dropping the entries that had been masking it.

### 2.3.0

- Nation names carry no form of government any more. Kingdom, Empire, Sultanate,
  Emirate, Republic and the like are dropped; only the country name remains, so
  Italy is Italy and not the Kingdom of Italy. Four names keep theirs because
  nothing usable is left otherwise: the Ottoman Empire, the Soviet Union, the
  United States and the Dominican Republic.
- Localisation files list only the states that need their own entry: a name that
  differs from the base game, or a union name that has to be overridden.

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
