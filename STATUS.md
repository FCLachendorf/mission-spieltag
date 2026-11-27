## Test 0.15

Lappen liegt beim Reinigen sichtbar rechts neben dem Fenster. Mit Finger oder Maus greifen und auf das Fenster ziehen; beim Loslassen kehrt er an seinen Platz zurück. Pixelige Wischmaske und 100-%-Anzeige mit Resttoleranz bleiben erhalten. Fünf neue Trainingstexturen synchronisiert (noch keine Trainingsaufgabe damit implementiert).

## Test 0.14

Sechs feste Mischgruppen aus Bäumen, Büschen und Schnee statt verstreuter Einzelobjekte. Alle 61 lokalen Asset-Dateien abgeglichen, 17 neue/geänderte Dateien übernommen; Schneehaufen nach environment verschoben. Versionierte Bild-URLs verhindern veraltete Cache-Bilder. Priorisierte Zeichenliste in ASSETS.md und nächste Spielaufgaben in ROADMAP.md. Bestehende Aufgaben, Kollisions- und Erreichbarkeitstests bestehen.

## Test 0.13

- Beide Winterbäume und alle drei Buschvarianten in allen drei Außenbereichen eingebaut. Größen und Seitenverhältnisse bleiben erhalten; getrennte Bodenanker berücksichtigen 64×64, 96×96 und 96×64 bei den Büschen.
- Vegetation wird nach Bodentiefe mit der Figur und den Schneehaufen sortiert. Stamm- und Buschbasen blockieren, die oberen Pflanzenteile verdecken die Figur dahinter.
- Platzhalterbäume ersetzt. Pflanzen erscheinen auf der Minimap nur innerhalb bereits erkundeter Bereiche.
- Schneefall als dauerhafte Einzelpartikel mit zufälligen Startpositionen, Fallgeschwindigkeiten, seitlichen Driften, Schwingungen, Größen und Transparenzen. Sanft wechselnder Wind; kein geometrisches Reihenmuster und kein Zufallsflackern pro Bild.
- Alle Fundstücke und Bereichsübergänge bleiben erreichbar. Fortschritt und erkundete Bereiche bleiben gespeichert.

## Test 0.12

- Sichtbares Reinigungsziel 100 %, intern weiterhin 93 % als Toleranz. Die Anzeige ist auf den toleranten Abschluss normiert; beim Abschluss werden verbleibende Schmutzpixel vollständig entfernt und 100 % bestätigt.
- Kontinuierliches, stärkeres Fensterwackeln bei Kreisbewegungen statt wiederholt neugestarteter CSS-Animation. Die Bewegung wächst mit der Zugspannung und klingt kurz aus. Reduzierte Bewegung bleibt berücksichtigt.
- Seitliche Gebäudekollisionen an den sichtbaren Wandkanten ausgerichtet: Garage ab Quellpixel 18 bis 174, Container ab 17 bis 272; kleiner Fußradius statt breiter zusätzlicher Randzone. Dachüberstände bestimmen die seitliche Wandkollision nicht.
- Aufgaben, Wege, Überdeckung der Schneehaufen und Speichern bleiben erhalten.

## Test 0.11

- Reinigungsschwelle 93 %. Wischmaske aus den tatsächlich sichtbaren Pixeln von cloth.png; transparente Ränder reinigen nicht. Lappen größer, weiterhin eckige Wischspuren.
- Nagelpositionen nach den Markierungen korrigiert. Hintere Nägel von Anfang an sichtbar, aber erst nach dem vorderen Brett greifbar. Richtige Zeichenebenen verdecken überlagerte Nägel natürlich.
- Hammer rechts gespiegelt und aus der Fensterbeschneidung genommen. Nagel und Hammer heben sich zusammen, mit größerer Hebelbewegung.
- Ungefähr 2,5 Umdrehungen pro Nagel. Zeitbegrenzte Fortschrittsrate erlaubt keinen sofortigen Abschluss durch schnelle Fingerkreise; bei maximalem Tempo sind mindestens etwa drei Sekunden aktive Bewegung erforderlich.
- Schneehaufen: feste Bodenfläche mit Tiefensortierung statt Kollision an der gesamten sichtbaren Höhe. Die Figur wird hinter den Haufen verdeckt und davor wieder vollständig gezeichnet. Alle Türen und Fundstücke bleiben erreichbar.
- Bestehende abgeschlossene Aufgaben bleiben gespeichert.

## Test 0.10

- Fensterreparatur als große Nahansicht ohne Dialogkasten; Spiel-HUD währenddessen ausgeblendet. Nägel an den dunklen Endstellen der Bretter, Hammer hinter den Nagelköpfen und an die Fenstergröße angepasst.
- Echte Lappentextur aus props/cloth.png. Kantiges Putzen in Originalpixel-Blöcken, 89 % einzigartige Fläche als Abschluss. Keine runden Wischkanten.
- Alle vier Schaufel-Laufbilder eingebaut. Gleichbleibender Körpermaßstab und Fußanker; nur das hintere Standbild hat eine 68-Pixel-Zeichenfläche.
- Alle fünf gelieferten Schneeflockenvarianten werden draußen mit unterschiedlicher Größe und Bewegung gezeichnet. Transparente Ränder werden beim Zeichnen ausgespart; reduzierte Bewegung bleibt berücksichtigt.
- Schneekollisionen erfassen die gesamte sichtbare Höhe der Haufen statt nur deren unteren Bereich. Nordseitige Annäherung und Karten-Erreichbarkeit geprüft.
- Keine weiteren Texturen erforderlich, bevor diese Änderungen auf dem Handy erprobt sind. Kreidewagen, Aufstellfigur und Stangen bleiben für spätere, noch nicht umgesetzte Aufgaben vorgesehen.

## Test 0.9

- Originale Fensterebenen: zwei Nägel pro Brett, vorderes Brett zuerst. Anschließend Fenster mit Finger oder Maus reinigen; 78 % einzigartige Fläche reichen. Wiederholtes Wischen derselben Stelle zählt nicht mehrfach.
- Gezogene Nägel, fertige Fenster und beide einzeln freigeschaufelten Eingänge werden gespeichert. Unfertige Wischflächen starten beim Wiederöffnen neu.
- Schaufel am Geräteraum aufnehmen und ablegen.
- Alle Schneehaufen blockieren an ihrer Bodenfläche. Fundstücke und Übergänge bleiben erreichbar; neue Hindernisse verschieben überlappende alte Spielerpositionen sicher an den Start.
- Alte restaurierte Container bleiben fertig. Alte gemeinsame Schneeräum-Abschlüsse bleiben als beide freie Türen erhalten.
- Freies Schippen anderer Schneehaufen bleibt offen.

## Test 0.8

- Weltansicht um 10 % vergrößert; Figur und Umgebung wachsen gemeinsam.
- Garage 384×192 Weltpixel, Container 360×240; sichtbare Gebäudehöhen ähnlich, ohne das Seitenverhältnis zu verzerren. Hofpositionen und Kollisionen angepasst.
- 90 deutlichere Schneepartikel statt 45; reduzierte Bewegung bleibt berücksichtigt.
- Einmalige Fensterreparatur: drei Nägel auswählen und je eine volle Kreisbewegung; Knopf als Alternative. Leichtes Wackeln nur bei erlaubter Bewegung.
- Einmaliges Räumen der Container-Eingänge: Schaufel zuerst aufnehmen; drei Haufen mit Wischgesten entfernen, Enter als Alternative.
- Beide Vorbereitungen plus sechs Fundstücke und 40 Materialtaler sind Voraussetzung für die Restaurierung über den fiktiven Jörg-Anruf im Spiel. Kein echter Anruf.
- Danach 20 Taler für Weihnachtsdekoration mit vorhandener neuer Textur.
- Erledigte Reparaturen werden gespeichert; bereits restaurierte alte Spielstände bleiben fertig. Abgebrochene Teilversuche starten neu und kosten keine Taler.
- Freies Schippen anderer Haufen und Wegblockaden zwischen Sektionen sind noch offen. Minispielgrafiken zunächst Platzhalter.

## 0.7: Original buildings and shovel poses

Buildings preserve aspect ratio: container 288x192, garage 192x96. Shovel poses use uniform pixel scale and a body pivot of x=32; the back pose has four additional pixels on the right. No shovel walk frames required yet. Free shovel pickup in the courtyard. Deposit action and crates moved into the container material room; garage is the equipment room. Snow clearing remains a following step.

# Testversion 0.6 Ã¢â‚¬â€œ 26. November 2026

## Neu in 0.6

- Drei getrennte AuÃƒÅ¸enbereiche von je 960Ãƒâ€”704 Weltpixeln: Containerhof als Ausgangspunkt, Trainingsfeld rechts, Spieltag unten. Automatische ÃƒÅ“bergÃƒÂ¤nge an den markierten Wegenden, alternativ ÃƒÂ¼ber die Aktionstaste. Ankunftspunkte verhindern sofortiges ZurÃƒÂ¼ckspringen.
- Minimap rechts oben mit Figur, Wegen, GebÃƒÂ¤uden, ÃƒÅ“bergÃƒÂ¤ngen und FundstÃƒÂ¼cken. Nicht erkundete Kacheln werden verdeckt; Erkundung wird getrennt pro AuÃƒÅ¸enbereich und Innenraum gespeichert.
- Sechs bisherige FundstÃƒÂ¼cke liegen auf die drei Bereiche verteilt. Bereichsbezogene Aufgabenhinweise unterstÃƒÂ¼tzen die Orientierung. Drei optionale MÃƒÂ¼llbeutel bringen je einmalig 5 Taler.
- Drei Schneehaufenvarianten integriert. Schneefall mischt kleine Pixel und einfache Kreuzflocken; echte Partikelgrafiken bleiben optional. Noch keine aktive SchneerÃƒÂ¤umfunktion.
- Sammelheft auf dem Tisch im Treffpunkt: 25 vorhandene Karten aus FCLachendorf/FCLachendorf-Sammelheft, zwei pro Ansicht auf 13 Seiten. Originalbilder werden erst beim Ãƒâ€“ffnen bzw. BlÃƒÂ¤ttern geladen. Das Spiel pausiert wÃƒÂ¤hrend der Ansicht. Kleine Wanddekoration mit dem vom Nutzer genannten FundstÃƒÂ¼ck.
- Alte SpielstÃƒÂ¤nde behalten Aufgaben, Tragegegenstand und Ausbauten. Alte Positionen passen nicht zur neuen Geometrie und starten deshalb im Containerhof. Neue Positionen und Erkundung bleiben erhalten.
- FlÃƒÂ¤chen fÃƒÂ¼r Verkaufsstand/Zuschauer sind vorgesehen; diese Ausbauten sind noch nicht spielbar. Echte Mannschaftsbilder stehen noch aus.

PrÃƒÂ¼fung: Gates in beide Richtungen, ungÃƒÂ¼ltige ÃƒÅ“bergÃƒÂ¤nge, Erkundungsmaske/Speicherstand, Migration, einmalige MÃƒÂ¼llbelohnung, Album-Paginierung und Bewegungspause. BrowserprÃƒÂ¼fung bei 844Ãƒâ€”390 fÃƒÂ¼r beide AuÃƒÅ¸enÃƒÂ¼bergÃƒÂ¤nge, Innenraum und Originalkarten.

## Neu in 0.5

- Minecraftia fÃƒÂ¼r FlieÃƒÅ¸texte, RasterForge fÃƒÂ¼r ÃƒÅ“berschriften; beide WOFF2-Dateien lokal. Nunito bleibt als Fallback erhalten. Beide neuen Dateien enthalten ÃƒÂ¤ÃƒÂ¶ÃƒÂ¼Ãƒâ€žÃƒâ€“ÃƒÅ“ÃƒÅ¸, anhand ihrer cmap-Tabellen geprÃƒÂ¼ft.
- Das gelieferte Regal (48Ãƒâ€”64), zwei Pfandkisten und der Schneeschieber (je 64Ãƒâ€”64) sind integriert. GrÃƒÂ¶ÃƒÅ¸entabellen berÃƒÂ¼cksichtigen ihre tatsÃƒÂ¤chlichen DateimaÃƒÅ¸e und transparenten RÃƒÂ¤nder.
- Nach der Container-Renovierung kann im linken Materialraum sortiert werden: sechs Teile aufnehmen, zum passenden Regal tragen, durch Halten ablegen. Falsche Regale geben Feedback und behalten den Gegenstand in der Hand. Richtige Ablagen werden am Regal sichtbar. Einmaliger Abschlussbonus: 20 Taler.
- Teilfortschritt und getragener Gegenstand werden gespeichert. Alte SpielstÃƒÂ¤nde beginnen die neue optionale Aufgabe bei null; bestehende Upgrades bleiben erhalten.
- Schneeschieber zunÃƒÂ¤chst als sichtbares Werkzeug; noch keine aktive RÃƒÂ¤umfunktion. Die Pfandvarianten sind optische Varianten desselben Gegenstandstyps.

PrÃƒÂ¼fung: check-mobile.cjs prÃƒÂ¼ft zusÃƒÂ¤tzlich Tragen, falsche/richtige Ablage, Speicherstand und einmalige Belohnung. check-fonts.cjs prÃƒÂ¼ft die deutschen Glyphen direkt aus beiden WOFF2-Dateien.

## Korrekturen in 0.4

- Kameraziel: FuÃƒÅ¸punkt bei 60 % der BildschirmhÃƒÂ¶he, damit der sichtbare KÃƒÂ¶rper leicht unter der Mitte liegt. An KartenrÃƒÂ¤ndern wird die Kamera weiterhin begrenzt.
- Spieler um 5 % vergrÃƒÂ¶ÃƒÅ¸ert. Pro Gehbild ein gemessener FuÃƒÅ¸punkt (10Ã¢â‚¬â€œ14 Pixel transparenter Rand), gemeinsam mit passendem kleinerem Bodenschatten.
- GegenstÃƒÂ¤nde werden unabhÃƒÂ¤ngig von ihrer PNG-ZeichenflÃƒÂ¤che skaliert: FuÃƒÅ¸ball 10Ãƒâ€”10, Trikot 16Ãƒâ€”16, Kiste 56Ãƒâ€”28 Weltpixel. InteraktionsflÃƒÂ¤chen bleiben fÃƒÂ¼r Touch groÃƒÅ¸zÃƒÂ¼gig.
- Nunito lokal in assets/fonts, inklusive OFL-Lizenz. OberflÃƒÂ¤che und Canvas-Beschriftung verwenden dieselbe Schrift. Deutsche Glyphen in der tatsÃƒÂ¤chlichen Fontdatei geprÃƒÂ¼ft.
- JavaScript verwendet Unicode-Escapes, HTML Zeichenreferenzen. Frische Versionsparameter fÃƒÂ¼r JS und CSS verhindern das Wiederverwenden frÃƒÂ¼her beschÃƒÂ¤digter Beschriftungen.
- Noch kein zusÃƒÂ¤tzliches Minispiel. NÃƒÂ¤chste PrioritÃƒÂ¤t ist eine aktive Sortieraufgabe im Materialraum; ASSETS-NEXT.md enthÃƒÂ¤lt den kleinen Grafikbedarf.

## Funktioniert

- Acht vom Nutzer gelieferte PNGs: Stand/Gang fÃƒÂ¼r vorne, hinten, links, rechts.
- Frei platzierter Touchstick im linken Bildschirmdrittel. Ein zweiter Finger verschiebt ihn nicht.
- Direkte Halteinteraktionen auf nahen GegenstÃƒÂ¤nden, TÃƒÂ¼ren und Schildern. Fortschrittsring, Abbruch beim Loslassen, Wegziehen oder Weglaufen. Desktop zusÃƒÂ¤tzlich WASD/E.
- Winterkarte nach grober Referenz: Container/Garage oben, Hauptplatz sÃƒÂ¼dwestlich, TrainingsplÃƒÂ¤tze rechts. Zwei getrennte EingangstÃƒÂ¼ren. GrÃƒÂ¶ÃƒÅ¸erer begehbarer 2D-Innenraum.
- Dezenter Schneefall nur drauÃƒÅ¸en, bei reduzierter Bewegung deaktiviert.
- Einmaliger Pfandauftrag: +40 Taler. Rasenheizung: 40 Taler, Hauptplatz wird grÃƒÂ¼n. TrainingsflÃƒÂ¤chen bleiben verschneit.
- Alte 0.2-SpeicherstÃƒÂ¤nde werden ÃƒÂ¼bernommen. UngÃƒÂ¼ltige Positionen werden korrigiert. Kein Konto nÃƒÂ¶tig.
- Vollbild auf unterstÃƒÂ¼tzten Browsern; Home-Bildschirm-Metadaten und Manifest mit eigenen App-Icons. Keine Offline-Zusage und kein Service Worker, damit Testupdates nicht in alten Caches hÃƒÂ¤ngen.

## PrÃƒÂ¼fung

`node check-mobile.cjs`: Touchbereich, Pointer-Zuordnung, abgebrochene Halteaktionen, vollstÃƒÂ¤ndige Ausbaureihenfolge, doppelte Belohnungen, beide EingÃƒÂ¤nge, Speichern/Laden, Richtungswechsel, alte SpielstÃƒÂ¤nde, Manifest-Icons.

BrowserprÃƒÂ¼fung bei 844Ãƒâ€”390: Laden aller Grafiken, Bewegung, Gegenstand mit gehaltenem Mauszeiger einsammeln, MenÃƒÂ¼. Dies ersetzt keinen echten Mehrfinger-Test auf iPhone/Android.

## Offen

Eigentliche Platzpflege-Minispiele und ElfmeterschieÃƒÅ¸en, Finale, Abschlusskarte, Audio, individuell angepasste Figur. GebÃƒÂ¤ude sind weiterhin gezeichnete Platzhalter nach den Referenzfotos. Rasenheizung ist ein spielerisch vereinfachtes Upgrade. Noch kein vollstÃƒÂ¤ndiges 10Ã¢â‚¬â€œ20-Minuten-Spiel.
