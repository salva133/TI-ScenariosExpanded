# 1898 — War for our World

Two start scenarios for Terra Invicta set on 1 January 1898, the year H. G. Wells
published *The War of the Worlds*.

The mod adds two entries to the scenario list and changes nothing in existing
campaigns. Every record carries the `1898_` prefix and is appended to the base
data, so the 2022, 2026, 2030 and 2070 scenarios — and the Dark Skies scenarios
— remain untouched.

**Version 1.6.0** · Terra Invicta 1.0.51

## Installation

Download `WarForOurWorld-v<version>.zip` from the [releases](../../releases) and
unpack the `WarForOurWorld` folder from it into:

```
...\Steam\steamapps\common\Terra Invicta\Mods\Enabled\
```

Restart the game, enable **Use Mods** on the start screen, then restart once
more. Both scenarios then appear under **Scenario** in the new campaign screen.

Do **not** copy the whole repository there. Terra Invicta's mod manager parses
every `.json` file it finds anywhere under a mod folder and expects each one to
be a template array, so a tooling file that happens to be JSON stops the mod
from installing with *MOD MANAGER FAILED TO LOAD JSON*. The release archive
holds only `ModInfo.json`, the eleven template files and this README.

## The two scenarios

| Scenario | Alien headquarters |
| --- | --- |
| 1898 — War for our World | Placed by the game, as in every base scenario |
| 1898 — War for our World from Mars | Olympus Mons, with the station in low Mars orbit |

The Mars variant is the one closer to Wells, where the invaders explicitly come
from Mars and astronomers watch the launches through telescopes before the first
cylinder lands. The enemy is therefore known from the start and far closer to
Earth than usual.

Both scenarios share nations, regions, armies and start time. They differ only
in their habitat group, so any later change to the world applies to both.

## The world of 1898

52 sovereign states, 243 nations without statehood, 363 regions, 2,445 bilateral
relations and 76 standing armies.

| Power | Regions | of which colonial |
| --- | ---: | ---: |
| British Empire | 93 | 86 |
| Russian Empire | 40 | — |
| French Republic | 34 | 26 |
| Great Qing | 26 | — |
| Ottoman Empire | 19 | — |
| United States | 16 | — |
| German Empire | 14 | 8 |
| Kingdom of Spain | 13 | 8 |

World economic output is 2.83 trillion instead of 141.7 trillion, that is two
percent of the present-day figure, distributed according to the 1900 GDP shares
from the Maddison Project. World population is 1.68 billion.

No nuclear weapons, no space budget, no human habitats. Miltech ranges from 0.2
to 1.6 rather than 4.2 to 4.5. The atmosphere holds 295 ppm of CO₂ and sea level
sits 20 cm below today's.

Spain still holds Cuba, Puerto Rico and the Philippines: the start date is
1 January, three months before the Spanish-American War breaks out. That war
will happen during your campaign rather than before it.

## Federations

| Federation | Members |
| --- | --- |
| Triple Alliance | German Empire, Empire of Austria, Kingdom of Hungary, Kingdom of Italy |
| Franco-Russian Alliance | French Republic, Russian Empire |
| Union of Sweden and Norway | Sweden, Norway |

Austria-Hungary is modelled as two nations because Cisleithania and
Transleithania were separate states sharing a common foreign policy and army.
Since a nation can belong to only one federation, the real union is absorbed
into the Triple Alliance, which it belonged to as a whole anyway.

Federations pledge mutual defence, share space funding and boost, and grant a
bonus to Economy investment. Germany and Russia are likely to count as
authoritarian, making their federations *dark*: members may only leave with the
lead nation's consent. Italy will not walk out of the Triple Alliance cheaply.

Britain keeps to its splendid isolation. Its only alliance is the old one with
Portugal — the Anglo-Japanese Alliance does not arrive until 1902.

## Known limitations

- Organisations come from the present-day set, because the game will not start
  without them. Names like NASA or CIA are therefore anachronistic.
- Councillors and portraits are the standard set.
- The three base technologies `WeAreNotAlone`, `Skywatch` and `MissionToSpace`
  remain set so that the tech tree and interface keep working.
- The map itself is unchanged. Borders follow present-day region boundaries;
  only ownership is that of 1898.
- The Italian irredenta against Austria cannot be represented as a rivalry,
  because federation members may not be rivals.
- Federation names are not localised. This is also true of the base game's
  federations.
- The scenario does not use the Dark Skies timing fields
  (`alienQuietDuration_years`, `alienProgressionModifier` and similar), so the
  aliens advance at the standard pace.

## Changelog

### 1.6.0

- Retargeted to Terra Invicta 1.0.51.
- The scenario's nation list uses vanilla's `ALN` instead of the mod's own
  `1898_ALN` copy of the Alien Nation, which is now gone.
- Mod description rewritten in English; the German scenario descriptions carry
  real umlauts again.

### 1.5.0

- Added the second scenario, *1898 — War for our World from Mars*. The alien
  headquarters and station are copies of the game's templates with a fixed
  location: `habSite` `MarsSite6` for the base, `orbitTemplateName`
  `LowMarsOrbit` for the station. Both fields are empty in the originals, which
  is why the game picks the location itself there.

### 1.4.0

- The alien headquarters and station were missing. The scenario's habitat list
  was empty because there are no human habitats in 1898, but `AlienHQ` and
  `AlienHQStation` belong in every scenario. Without them the aliens would have
  had no base.
- Localisation now follows the Dark Skies pattern. Instead of a full name set
  for all 295 nations via prefixed aliases, only the 52 differing states are
  overridden through `scenarioLocalizationPostfix` `.1898`. Every other nation
  keeps its familiar name.
- `tutorialAllowed` is now set explicitly to false.

### 1.3.0

- Scenario and mod renamed to *1898 — War for our World*. Internal identifiers
  are unchanged so that running campaigns keep loading.

### 1.2.0

- Removed the Russian occupation of Donetsk, inherited from the base game and
  dating from 2014.
- Capital claims are no longer trimmed. The `capitalClaim` field denotes the
  intended capital, not the one currently held — Taiwan claims Shanghai, South
  Yemen claims Sanaa.

### 1.1.0

- Added federations.

### 1.0.0

- Initial release.

## Continuous integration

Every push and pull request runs the Terra Invicta mod validator from
[`salva133/My-Workflows`](https://github.com/salva133/My-Workflows). It reads the
mod the way the game does and reports what the game would swallow in silence:

* `ModInfo.json` parses, carries the fields the mod menu reads, and lists every
  template file present — a template missing from `TemplatesToConcatArrays` is a
  file the game never opens.
* Every `1898_` name a record points at resolves to a record the mod defines, so
  a mistyped region in an army or a bilateral relation is caught rather than
  quietly dropping that army or claim.
* Every nation, region, army, habitat and start time is listed in the
  `TIMetaTemplate` entry for its type. A record the meta template does not list
  is a record no scenario ever loads.
* Every localization key resolves through `scenarioPrefix` and
  `scenarioLocalizationPostfix` to a record that exists, English and German
  carry the same keys, and both files are valid UTF-8 — a `.deu` file saved as
  cp1252 reaches the game as mojibake rather than as an error.

A release is cut by bumping `Version` in `ModInfo.json` and pushing to `master`:
the checks run again, and a green run publishes `WarForOurWorld-v<version>.zip`
— a `WarForOurWorld` folder ready to drop into `Mods\Enabled` — as a GitHub
release tagged `v<version>`.
