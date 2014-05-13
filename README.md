# Pathfinder

Diese Programmieraufgabe wurde von [Silpion IT-Solutions](http://www.silpion.de/) für die [Firmenkontaktmesse 2014](http://www.fh-wedel.de/news/ansicht/artikel/firmenkontaktmesse-2014-die-aussteller/) an die Studenten der [FH-Wedel](http://www.fh-wedel.de/) gestellt. Unter allen eingesendeten Lösungen werden Sachpreise am Tag der Firmenkontaktmesse verlost. Die Aufgabe umfasst das Programmieren eines einfachen Programms um den Weg durch ein gegebenes Spielfeld zu finden.

Der Wettbewerb ist für die Firmenkontaktmesse 2014 geschlossen. Es gibt ein paar Infos zu den [Einsendungen](#Einsendungen).

## Idee

Eine überschaubare Aufgabe, keine Vorgaben der Technologie und die Möglichkeit etwas zu gewinnen :)
Die Aufgabe soll anregen, mal eine neue Programmiersprache auszuprobieren oder gelernte Algorithmen wie den [Dijkstra-Algorithmus](http://de.wikipedia.org/wiki/Dijkstra-Algorithmus) oder den [A*-Algorithmus](http://de.wikipedia.org/wiki/A*-Algorithmus) zu implementieren, oder gar [Reinforcement-Learning](http://de.wikipedia.org/wiki/Reinforcement_Learning) einzusetzen. Der Kreativität kann freien Lauf gelassen werden!

## Aufgabe

Die Aufgabe ist ein Programm zu schreiben, welches einen Weg durch ein simples Spielfeld findet. Es sind mehrere Spielfelder im Ordner `boards/` vorgegeben. Passende Lösungen sind im Ordner `solutions/` zu finden.

### Spielfeld

Das Spielfeld ist eine einfache Textdatei mit folgendem beispielhaften Inhalt:

```
XSXXX
X X E
X   X
XXXXX
```

* Das Zeichen `S` steht für den Start. Dieses Zeichen kann pro Spielfeld nur einmal vorkommen.
* Das Zeichen `X` steht für eine Wand und kann nicht beschritten werden.
* Das Leerzeichen steht für einen Weg und kann beschritten werden.
* Das Zeichen `E` steht für ein mögliches Ende. Dieses Zeichen kann mehrfach pro Spielfeld vorkommen. Es muss nicht zwingend am Rand des Spielfelds liegen.
* Jedes Spielfeld hat eine konstante Breite und Höhe, welche nicht zwingen gleich sein müssen.
* Es ist nicht möglich diagonal zu laufen. Nur direkte Wechsel nach Oben, Rechts, Unten und Links sind erlaubt.


### Ziel

Das Ziel ist die Ausgabe der Koordinaten des gefundenen Wegs.

Lösung für das beispielhafte Spielfeld:

```
1,0
1,1
1,2
2,2
3,2
3,1
4,1
```

* Der Weg muss die Koordinaten des Start- und Endpunktes enthalten.
* Es sind alle Koordinaten des Weges auszugeben.
* Das Koordinatensystem beginnen in der linken oberen Ecke mit (0, 0).
* Die X-Koordinate vergrößert sich mit jeder weiteren Spalte.
* Die Y-Koordinate vergrößert sich mit jeder weiteren Zeile.

### Schwierigkeitsstufen

Es ist denkbar Spielfelder zu konstruieren, die besondere Schwierigkeiten bergen.
Mögliche Ideen für solche wären:

* Kreise im Spielfeld
* Mehrere mögliche Wege
* Kein erreichbares Ende
* Kürzester Weg

Wer möchte kann gern eigene Spielfelder mit Lösungen mittels Pull-Request vorschlagen.

## Regeln

* Jeder Student der FH-Wedel kann Lösungen der Aufgabe bis zum **12.05.2014 um 23:59 per E-Mail** an **firmenkontaktmesse@silpion.de** einschicken.
* Eingeschickt werden muss der Quellcode des Programms oder ein Link dazu, sowie gerne eine kurze Installationsanleitung.
* Die Lösung müssen lauffähig und funktionsfähig umgesetzt sein.
* Jeder Teilnehmer kann beliebig viele Lösungen einschicken, jedoch kann pro Person kann nur ein Los bei der Verlosung gezogen werden.
* Die **Verlosung findet am [14.05.2014 am Stand 9](http://www.fh-wedel.de/fileadmin/fhw_files/Pressestelle/standplan_Messetag1_copy.pdf) um 13 Uhr** statt.
* Teilnehmer die während der Verlosung vor Ort sind, können sich ihren Preis direkt aussuchen. Alle anderen Teilnehmer werden per E-Mail kontaktiert.
* Es gilt immer die aktuellste Version dieser README.md Datei.

## Einsendungen

Es gab insgesamt 7 Einsendungen, vielen Dank dafür!
Alle 7 Einsendungen entsprechen den Regeln und sind funktionsfähig umgesetzt.

Die Aufteilung über die genutzen Programmiersprachen sieht wie folgt aus.

* 1x Delphi/Pascal
* 1x Typescript
* 1x Java
* 4x Haskell

Mehrfach wurde auch der Dijkstra-Algorithmus implementiert.

Bei 7 Einsendungen und 5 Preisen werden zwangsläufig leider 2 Teilnehmer leer ausgehen, doch für diese hätten wir kleine Trostpreise ;)
Wir freuen uns darauf die Teilnehmer während der Kontaktmesse zu treffen.

## Preise

Es können folgende Preise bei der Verlosung gewonnen werden:

* [Raspberry Pi Ultimate Starter Kit](http://www.amazon.de/Raspberry-Ultimate-Starter-Inklusive-Wesentlich/dp/B00HPZFAXA/) _(Hauptpreis)_
* [Rückwärtsuhr](http://www.getdigital.de/Rueckwaertsuhr.html)
* [Panic-Button](http://www.getdigital.de/Panic-Button.html)
* [Programmiersprachen Supertrumpf](https://www.getdigital.de/Programmiersprachen-Supertrumpf.html)
* [Sheldon's Wäschefalter](http://www.getdigital.de/Waeschefalter-aus-The-Big-Bang-Theory.html)

## Fragen

Wer Fragen oder Hinweise hat, kann gerne die [Issues](https://github.com/silpion/Pathfinder/issues) Funktion von github benutzen.
