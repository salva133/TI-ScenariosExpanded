1898 - War for our World
Zwei Startszenarien zum 1. Januar 1898 fuer Terra Invicta
=========================================================
Version 1.5.0

Installation
------------
Diesen Ordner nach
  ...\Steam\steamapps\common\Terra Invicta\Mods\Enabled\WarForOurWorld\
kopieren, Spiel neu starten, im Startbildschirm unter Mods "Use Mods"
aktivieren und erneut neu starten. Das Szenario erscheint dann im
Neues-Spiel-Bildschirm unter "Szenario". Der Mod bringt zwei Eintraege mit:

  1898 - War for our World
      Das Standardszenario. Ort des Alien-Hauptquartiers bestimmt das Spiel.

  1898 - War for our World from Mars
      Gleiche Welt, aber die Invasoren kommen wie bei Wells vom Mars. Ihr
      Hauptquartier liegt auf dem Olympus Mons, ihre Station im niedrigen
      Marsorbit. Beide Szenarien teilen sich Nationen, Regionen, Armeen und
      Startzeitpunkt; sie unterscheiden sich ausschliesslich in diesen
      beiden Habitaten.

Was der Mod aendert
-------------------
Nichts an bestehenden Kampagnen. Alle Eintraege tragen den Praefix
"1898_" und werden an die Basisdaten angehaengt. Die Szenarien 2022,
2026, 2030 und 2070 bleiben unveraendert.

Inhalt
------
52 souveraene Staaten, 243 Nationen ohne eigene Staatlichkeit,
363 Regionen, 2445 bilaterale Beziehungen, 76 stehende Heere.

Das Britische Empire haelt 93 der 363 Regionen, davon 86 kolonial.
Es folgen das Russische Reich (40), Frankreich (34), das Kaiserreich
China (26), das Osmanische Reich (19) und die Vereinigten Staaten (16).

Weltwirtschaftsleistung: 2,83 Billionen statt 141,7 Billionen, also
zwei Prozent des Gegenwartsniveaus, verteilt nach den BIP-Anteilen
von 1900 nach dem Maddison-Projekt.
Weltbevoelkerung: 1,68 Milliarden.
Keine Kernwaffen, kein Raumfahrtbudget, keine Habitate, Miltech
zwischen 0,2 und 1,6 statt 4,2 bis 4,5.
Atmosphaere: 295 ppm CO2, Meeresspiegel 20 cm unter dem heutigen.

Foederationen
-------------
Dreibund: Deutsches Reich, Kaisertum Oesterreich, Koenigreich Ungarn,
  Koenigreich Italien. Die Doppelmonarchie ist als zwei Nationen
  abgebildet, weil Cisleithanien und Transleithanien 1898 getrennte
  Staatswesen mit gemeinsamer Aussenvertretung waren. Da eine Nation
  nur einer Foederation angehoeren kann, geht die Realunion im
  Dreibund auf, dem sie ohnehin als Ganzes angehoerte.
Zweiverband: Franzoesische Republik, Russisches Reich.
Schwedisch-Norwegische Union: Schweden, Norwegen.

Foederationen verpflichten zur gegenseitigen Verteidigung, teilen
Raumfahrtbudget und Boost und geben einen Bonus auf Investitionen in
die Wirtschaft. Das Deutsche Reich und Russland duerften als
autoritaer gelten, ihre Foederationen also als dunkel: Mitglieder
koennen nur mit Zustimmung der fuehrenden Nation austreten.

Grossbritannien haelt sich 1898 aus Buendnissen heraus; einzige
Ausnahme ist die alte Allianz mit Portugal. Die Allianz mit Japan
kommt erst 1902 und ist daher nicht enthalten.

Bekannte Einschraenkungen
-------------------------
- Organisationen stammen aus dem Gegenwartssatz, weil das Spiel ohne
  Organisationen nicht startet. Namen wie NASA oder CIA sind daher
  anachronistisch.
- Raete und Portraits sind der Standardsatz.
- Die drei Basistechnologien WeAreNotAlone, Skywatch und MissionToSpace
  bleiben gesetzt, damit Forschungsbaum und Oberflaeche funktionieren.
- Die Karte selbst ist unveraendert; Grenzen entsprechen den heutigen
  Regionsgrenzen, nur die Zugehoerigkeit ist die von 1898.
- Die italienische Irredenta gegen Oesterreich laesst sich nicht als
  Rivalitaet abbilden, weil Foederationsmitglieder keine Rivalen sein
  duerfen.
- Foederationsnamen werden im Spiel nicht lokalisiert; das gilt
  ebenso fuer die Foederationen des Basisspiels.
- Das Szenario nutzt nicht die zusaetzlichen Zeitsteuerungsfelder des
  Dark-Skies-DLC (alienQuietDuration_years, alienProgressionModifier und
  aehnliche). Die Aliens gehen daher im Standardtempo vor.

Aenderungen in 1.5.0
--------------------
- Zweites Szenario "1898 - War for our World from Mars". Hauptquartier und
  Station der Aliens sind Kopien der Spielvorlagen, denen ein fester Ort
  zugewiesen wurde: habSite MarsSite6 fuer die Basis, orbitTemplateName
  LowMarsOrbit fuer die Station. Im Standardszenario sind beide Felder leer,
  das Spiel waehlt den Ort dann selbst.
- Der Gegner ist in der Marsvariante von Beginn an ortsbekannt und deutlich
  naeher an der Erde. Das duerfte den Verlauf erheblich veraendern, in
  welche Richtung, muss sich im Spiel zeigen.

Aenderungen in 1.4.0
--------------------
- Das Hauptquartier der Aliens und ihre Station waren nicht enthalten. Die
  Habitatliste des Szenarios war leer, weil es 1898 keine menschlichen
  Habitate gibt; AlienHQ und AlienHQStation gehoeren aber in jedes Szenario.
  Ohne sie haetten die Aliens keine Basis gehabt.
- Die Lokalisierung folgt jetzt dem Muster des Dark-Skies-DLC. Statt eines
  eigenen Namenssatzes fuer alle 295 Nationen ueber praefixierte Aliase
  werden nur die 52 abweichenden Staaten ueber scenarioLocalizationPostfix
  ".1898" ueberschrieben. Alle uebrigen behalten ihren gewohnten Namen.
- tutorialAllowed wird ausdruecklich auf false gesetzt.

Aenderungen in 1.3.0
--------------------
- Szenario und Mod heissen jetzt "1898 - War for our World". Die internen
  Bezeichner bleiben unveraendert, damit laufende Partien weiter laden.

Aenderungen in 1.2.0
--------------------
- Die russische Besetzung von Donezk wurde entfernt. Sie stammt aus dem
  Basisspiel und beginnt erst 2014.
- Hauptstadtansprueche werden nicht mehr beschnitten. Das Feld capitalClaim
  bezeichnet die angestrebte, nicht die gehaltene Hauptstadt.
