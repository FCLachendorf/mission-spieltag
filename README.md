# Mission Spieltag · FC Lachendorf

Mobile Spieltest-Version 0.2, Querformat empfohlen. Eigenständiges statisches Browserspiel mit Canvas und eigenen PNG-Dateien, ohne Paketinstallation oder Build-Schritt. GitHub Pages: Settings → Pages → Deploy from a branch → main → /(root).

## Bedienung

Smartphone: Bewegungsstick links und Aktion rechts. Desktop: WASD/Pfeiltasten und E. Sammle sechs Gegenstände ein und verbessere den Container am Ausbau-Schild. Betrete den Container durch die Tür; links liegt der Materialraum, rechts der Treffpunkt. Ausrüstung und Ausbauten werden lokal gespeichert, alle 2,5 Sekunden auch die Position. Browser und Geräte teilen den Spielstand nicht. Keine Anmeldung, kein Backend.

## Grafiken

PNG in assets/tiles, assets/props und assets/characters ersetzen. Boden: 32×32; Kiste: 64×32; vorhandener Spieler: 64×96, im Spiel 32×48 dargestellt. Hütchen: cone_red.png und cone_yellow.png. Aktuell verwendet die Figur bewusst ein einzelnes Standbild. Richtungsanimationen, zusätzliche Bodenvarianten und Charakteranpassung sind noch nicht implementiert. Keine Bilddateien werden von externen Diensten geladen.

## Entwicklung

index.html: Oberfläche. style.css: Vollbild und mobile Steuerung. game.js: Welt, Bewegung, Kollision, Interaktionen und Spielstand. Lokal über einen statischen HTTP-Server ausliefern, z.B. `python -m http.server 8080`. Für ALL-INKL können diese Dateien einschließlich assets unverändert hochgeladen werden.

## Status

Fertig für Tests: Bewegung, Kamera, Touchstick, einfache Kollisionen, Container mit zwei Räumen, sechs Gegenstände, Vereinstaler, zwei Ausbauten, lokaler Spielstand und Zurücksetzen.

Offen: Phaser-Umstieg bewerten, Innenraumgrafiken, Laufanimationen, Platzpflege, Finale, Audio, Abschlusskarte, optionales Konto. Der geheime Adventshinweis ist noch nicht enthalten. Die ursprünglichen Planungsdokumente und internen Rätseldetails gehören nicht in dieses öffentliche Repository.

Auf dem echten Handy prüfen: Hoch-/Querformat, Bildschirmränder und Browserleisten, Stick und Aktion gleichzeitig, Container betreten/verlassen, Kollisionen, Reload und Fortsetzen, Menü und Zurücksetzen. Testversion ist noch kein fertiges Spiel.
