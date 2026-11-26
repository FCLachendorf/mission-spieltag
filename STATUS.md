## 0.7: Original buildings and shovel poses

Buildings preserve aspect ratio: container 288x192, garage 192x96. Shovel poses use uniform pixel scale and a body pivot of x=32; the back pose has four additional pixels on the right. No shovel walk frames required yet. Free shovel pickup in the courtyard. Deposit action and crates moved into the container material room; garage is the equipment room. Snow clearing remains a following step.

# Testversion 0.6 â€“ 26. November 2026

## Neu in 0.6

- Drei getrennte AuÃŸenbereiche von je 960Ã—704 Weltpixeln: Containerhof als Ausgangspunkt, Trainingsfeld rechts, Spieltag unten. Automatische ÃœbergÃ¤nge an den markierten Wegenden, alternativ Ã¼ber die Aktionstaste. Ankunftspunkte verhindern sofortiges ZurÃ¼ckspringen.
- Minimap rechts oben mit Figur, Wegen, GebÃ¤uden, ÃœbergÃ¤ngen und FundstÃ¼cken. Nicht erkundete Kacheln werden verdeckt; Erkundung wird getrennt pro AuÃŸenbereich und Innenraum gespeichert.
- Sechs bisherige FundstÃ¼cke liegen auf die drei Bereiche verteilt. Bereichsbezogene Aufgabenhinweise unterstÃ¼tzen die Orientierung. Drei optionale MÃ¼llbeutel bringen je einmalig 5 Taler.
- Drei Schneehaufenvarianten integriert. Schneefall mischt kleine Pixel und einfache Kreuzflocken; echte Partikelgrafiken bleiben optional. Noch keine aktive SchneerÃ¤umfunktion.
- Sammelheft auf dem Tisch im Treffpunkt: 25 vorhandene Karten aus FCLachendorf/FCLachendorf-Sammelheft, zwei pro Ansicht auf 13 Seiten. Originalbilder werden erst beim Ã–ffnen bzw. BlÃ¤ttern geladen. Das Spiel pausiert wÃ¤hrend der Ansicht. Kleine Wanddekoration mit dem vom Nutzer genannten FundstÃ¼ck.
- Alte SpielstÃ¤nde behalten Aufgaben, Tragegegenstand und Ausbauten. Alte Positionen passen nicht zur neuen Geometrie und starten deshalb im Containerhof. Neue Positionen und Erkundung bleiben erhalten.
- FlÃ¤chen fÃ¼r Verkaufsstand/Zuschauer sind vorgesehen; diese Ausbauten sind noch nicht spielbar. Echte Mannschaftsbilder stehen noch aus.

PrÃ¼fung: Gates in beide Richtungen, ungÃ¼ltige ÃœbergÃ¤nge, Erkundungsmaske/Speicherstand, Migration, einmalige MÃ¼llbelohnung, Album-Paginierung und Bewegungspause. BrowserprÃ¼fung bei 844Ã—390 fÃ¼r beide AuÃŸenÃ¼bergÃ¤nge, Innenraum und Originalkarten.

## Neu in 0.5

- Minecraftia fÃ¼r FlieÃŸtexte, RasterForge fÃ¼r Ãœberschriften; beide WOFF2-Dateien lokal. Nunito bleibt als Fallback erhalten. Beide neuen Dateien enthalten Ã¤Ã¶Ã¼Ã„Ã–ÃœÃŸ, anhand ihrer cmap-Tabellen geprÃ¼ft.
- Das gelieferte Regal (48Ã—64), zwei Pfandkisten und der Schneeschieber (je 64Ã—64) sind integriert. GrÃ¶ÃŸentabellen berÃ¼cksichtigen ihre tatsÃ¤chlichen DateimaÃŸe und transparenten RÃ¤nder.
- Nach der Container-Renovierung kann im linken Materialraum sortiert werden: sechs Teile aufnehmen, zum passenden Regal tragen, durch Halten ablegen. Falsche Regale geben Feedback und behalten den Gegenstand in der Hand. Richtige Ablagen werden am Regal sichtbar. Einmaliger Abschlussbonus: 20 Taler.
- Teilfortschritt und getragener Gegenstand werden gespeichert. Alte SpielstÃ¤nde beginnen die neue optionale Aufgabe bei null; bestehende Upgrades bleiben erhalten.
- Schneeschieber zunÃ¤chst als sichtbares Werkzeug; noch keine aktive RÃ¤umfunktion. Die Pfandvarianten sind optische Varianten desselben Gegenstandstyps.

PrÃ¼fung: check-mobile.cjs prÃ¼ft zusÃ¤tzlich Tragen, falsche/richtige Ablage, Speicherstand und einmalige Belohnung. check-fonts.cjs prÃ¼ft die deutschen Glyphen direkt aus beiden WOFF2-Dateien.

## Korrekturen in 0.4

- Kameraziel: FuÃŸpunkt bei 60 % der BildschirmhÃ¶he, damit der sichtbare KÃ¶rper leicht unter der Mitte liegt. An KartenrÃ¤ndern wird die Kamera weiterhin begrenzt.
- Spieler um 5 % vergrÃ¶ÃŸert. Pro Gehbild ein gemessener FuÃŸpunkt (10â€“14 Pixel transparenter Rand), gemeinsam mit passendem kleinerem Bodenschatten.
- GegenstÃ¤nde werden unabhÃ¤ngig von ihrer PNG-ZeichenflÃ¤che skaliert: FuÃŸball 10Ã—10, Trikot 16Ã—16, Kiste 56Ã—28 Weltpixel. InteraktionsflÃ¤chen bleiben fÃ¼r Touch groÃŸzÃ¼gig.
- Nunito lokal in assets/fonts, inklusive OFL-Lizenz. OberflÃ¤che und Canvas-Beschriftung verwenden dieselbe Schrift. Deutsche Glyphen in der tatsÃ¤chlichen Fontdatei geprÃ¼ft.
- JavaScript verwendet Unicode-Escapes, HTML Zeichenreferenzen. Frische Versionsparameter fÃ¼r JS und CSS verhindern das Wiederverwenden frÃ¼her beschÃ¤digter Beschriftungen.
- Noch kein zusÃ¤tzliches Minispiel. NÃ¤chste PrioritÃ¤t ist eine aktive Sortieraufgabe im Materialraum; ASSETS-NEXT.md enthÃ¤lt den kleinen Grafikbedarf.

## Funktioniert

- Acht vom Nutzer gelieferte PNGs: Stand/Gang fÃ¼r vorne, hinten, links, rechts.
- Frei platzierter Touchstick im linken Bildschirmdrittel. Ein zweiter Finger verschiebt ihn nicht.
- Direkte Halteinteraktionen auf nahen GegenstÃ¤nden, TÃ¼ren und Schildern. Fortschrittsring, Abbruch beim Loslassen, Wegziehen oder Weglaufen. Desktop zusÃ¤tzlich WASD/E.
- Winterkarte nach grober Referenz: Container/Garage oben, Hauptplatz sÃ¼dwestlich, TrainingsplÃ¤tze rechts. Zwei getrennte EingangstÃ¼ren. GrÃ¶ÃŸerer begehbarer 2D-Innenraum.
- Dezenter Schneefall nur drauÃŸen, bei reduzierter Bewegung deaktiviert.
- Einmaliger Pfandauftrag: +40 Taler. Rasenheizung: 40 Taler, Hauptplatz wird grÃ¼n. TrainingsflÃ¤chen bleiben verschneit.
- Alte 0.2-SpeicherstÃ¤nde werden Ã¼bernommen. UngÃ¼ltige Positionen werden korrigiert. Kein Konto nÃ¶tig.
- Vollbild auf unterstÃ¼tzten Browsern; Home-Bildschirm-Metadaten und Manifest mit eigenen App-Icons. Keine Offline-Zusage und kein Service Worker, damit Testupdates nicht in alten Caches hÃ¤ngen.

## PrÃ¼fung

`node check-mobile.cjs`: Touchbereich, Pointer-Zuordnung, abgebrochene Halteaktionen, vollstÃ¤ndige Ausbaureihenfolge, doppelte Belohnungen, beide EingÃ¤nge, Speichern/Laden, Richtungswechsel, alte SpielstÃ¤nde, Manifest-Icons.

BrowserprÃ¼fung bei 844Ã—390: Laden aller Grafiken, Bewegung, Gegenstand mit gehaltenem Mauszeiger einsammeln, MenÃ¼. Dies ersetzt keinen echten Mehrfinger-Test auf iPhone/Android.

## Offen

Eigentliche Platzpflege-Minispiele und ElfmeterschieÃŸen, Finale, Abschlusskarte, Audio, individuell angepasste Figur. GebÃ¤ude sind weiterhin gezeichnete Platzhalter nach den Referenzfotos. Rasenheizung ist ein spielerisch vereinfachtes Upgrade. Noch kein vollstÃ¤ndiges 10â€“20-Minuten-Spiel.
