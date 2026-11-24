# Testversion 0.4 – 24. November 2026

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
