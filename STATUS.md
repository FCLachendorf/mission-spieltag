# Testversion 0.6 – 26. November 2026

## Neu in 0.6

- Drei getrennte Außenbereiche von je 960×704 Weltpixeln: Containerhof als Ausgangspunkt, Trainingsfeld rechts, Spieltag unten. Automatische Übergänge an den markierten Wegenden, alternativ über die Aktionstaste. Ankunftspunkte verhindern sofortiges Zurückspringen.
- Minimap rechts oben mit Figur, Wegen, Gebäuden, Übergängen und Fundstücken. Nicht erkundete Kacheln werden verdeckt; Erkundung wird getrennt pro Außenbereich und Innenraum gespeichert.
- Sechs bisherige Fundstücke liegen auf die drei Bereiche verteilt. Bereichsbezogene Aufgabenhinweise unterstützen die Orientierung. Drei optionale Müllbeutel bringen je einmalig 5 Taler.
- Drei Schneehaufenvarianten integriert. Schneefall mischt kleine Pixel und einfache Kreuzflocken; echte Partikelgrafiken bleiben optional. Noch keine aktive Schneeräumfunktion.
- Sammelheft auf dem Tisch im Treffpunkt: 25 vorhandene Karten aus FCLachendorf/FCLachendorf-Sammelheft, zwei pro Ansicht auf 13 Seiten. Originalbilder werden erst beim Öffnen bzw. Blättern geladen. Das Spiel pausiert während der Ansicht. Kleine Wanddekoration mit dem vom Nutzer genannten Fundstück.
- Alte Spielstände behalten Aufgaben, Tragegegenstand und Ausbauten. Alte Positionen passen nicht zur neuen Geometrie und starten deshalb im Containerhof. Neue Positionen und Erkundung bleiben erhalten.
- Flächen für Verkaufsstand/Zuschauer sind vorgesehen; diese Ausbauten sind noch nicht spielbar. Echte Mannschaftsbilder stehen noch aus.

Prüfung: Gates in beide Richtungen, ungültige Übergänge, Erkundungsmaske/Speicherstand, Migration, einmalige Müllbelohnung, Album-Paginierung und Bewegungspause. Browserprüfung bei 844×390 für beide Außenübergänge, Innenraum und Originalkarten.

## Neu in 0.5

- Minecraftia für Fließtexte, RasterForge für Überschriften; beide WOFF2-Dateien lokal. Nunito bleibt als Fallback erhalten. Beide neuen Dateien enthalten äöüÄÖÜß, anhand ihrer cmap-Tabellen geprüft.
- Das gelieferte Regal (48×64), zwei Pfandkisten und der Schneeschieber (je 64×64) sind integriert. Größentabellen berücksichtigen ihre tatsächlichen Dateimaße und transparenten Ränder.
- Nach der Container-Renovierung kann im linken Materialraum sortiert werden: sechs Teile aufnehmen, zum passenden Regal tragen, durch Halten ablegen. Falsche Regale geben Feedback und behalten den Gegenstand in der Hand. Richtige Ablagen werden am Regal sichtbar. Einmaliger Abschlussbonus: 20 Taler.
- Teilfortschritt und getragener Gegenstand werden gespeichert. Alte Spielstände beginnen die neue optionale Aufgabe bei null; bestehende Upgrades bleiben erhalten.
- Schneeschieber zunächst als sichtbares Werkzeug; noch keine aktive Räumfunktion. Die Pfandvarianten sind optische Varianten desselben Gegenstandstyps.

Prüfung: check-mobile.cjs prüft zusätzlich Tragen, falsche/richtige Ablage, Speicherstand und einmalige Belohnung. check-fonts.cjs prüft die deutschen Glyphen direkt aus beiden WOFF2-Dateien.

## Korrekturen in 0.4

- Kameraziel: Fußpunkt bei 60 % der Bildschirmhöhe, damit der sichtbare Körper leicht unter der Mitte liegt. An Kartenrändern wird die Kamera weiterhin begrenzt.
- Spieler um 5 % vergrößert. Pro Gehbild ein gemessener Fußpunkt (10–14 Pixel transparenter Rand), gemeinsam mit passendem kleinerem Bodenschatten.
- Gegenstände werden unabhängig von ihrer PNG-Zeichenfläche skaliert: Fußball 10×10, Trikot 16×16, Kiste 56×28 Weltpixel. Interaktionsflächen bleiben für Touch großzügig.
- Nunito lokal in assets/fonts, inklusive OFL-Lizenz. Oberfläche und Canvas-Beschriftung verwenden dieselbe Schrift. Deutsche Glyphen in der tatsächlichen Fontdatei geprüft.
- JavaScript verwendet Unicode-Escapes, HTML Zeichenreferenzen. Frische Versionsparameter für JS und CSS verhindern das Wiederverwenden früher beschädigter Beschriftungen.
- Noch kein zusätzliches Minispiel. Nächste Priorität ist eine aktive Sortieraufgabe im Materialraum; ASSETS-NEXT.md enthält den kleinen Grafikbedarf.

## Funktioniert

- Acht vom Nutzer gelieferte PNGs: Stand/Gang für vorne, hinten, links, rechts.
- Frei platzierter Touchstick im linken Bildschirmdrittel. Ein zweiter Finger verschiebt ihn nicht.
- Direkte Halteinteraktionen auf nahen Gegenständen, Türen und Schildern. Fortschrittsring, Abbruch beim Loslassen, Wegziehen oder Weglaufen. Desktop zusätzlich WASD/E.
- Winterkarte nach grober Referenz: Container/Garage oben, Hauptplatz südwestlich, Trainingsplätze rechts. Zwei getrennte Eingangstüren. Größerer begehbarer 2D-Innenraum.
- Dezenter Schneefall nur draußen, bei reduzierter Bewegung deaktiviert.
- Einmaliger Pfandauftrag: +40 Taler. Rasenheizung: 40 Taler, Hauptplatz wird grün. Trainingsflächen bleiben verschneit.
- Alte 0.2-Speicherstände werden übernommen. Ungültige Positionen werden korrigiert. Kein Konto nötig.
- Vollbild auf unterstützten Browsern; Home-Bildschirm-Metadaten und Manifest mit eigenen App-Icons. Keine Offline-Zusage und kein Service Worker, damit Testupdates nicht in alten Caches hängen.

## Prüfung

`node check-mobile.cjs`: Touchbereich, Pointer-Zuordnung, abgebrochene Halteaktionen, vollständige Ausbaureihenfolge, doppelte Belohnungen, beide Eingänge, Speichern/Laden, Richtungswechsel, alte Spielstände, Manifest-Icons.

Browserprüfung bei 844×390: Laden aller Grafiken, Bewegung, Gegenstand mit gehaltenem Mauszeiger einsammeln, Menü. Dies ersetzt keinen echten Mehrfinger-Test auf iPhone/Android.

## Offen

Eigentliche Platzpflege-Minispiele und Elfmeterschießen, Finale, Abschlusskarte, Audio, individuell angepasste Figur. Gebäude sind weiterhin gezeichnete Platzhalter nach den Referenzfotos. Rasenheizung ist ein spielerisch vereinfachtes Upgrade. Noch kein vollständiges 10–20-Minuten-Spiel.
