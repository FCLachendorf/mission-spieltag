# Testversion 0.3 – 24. November 2026

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
