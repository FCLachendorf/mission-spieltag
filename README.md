# Mission Spieltag · FC Lachendorf

Mobiles 2D-Browserspiel im Querformat, Testversion 0.5. Live-Test: https://fclachendorf.github.io/mission-spieltag/

## Spielen

Smartphone: Im linken Drittel berühren und ziehen. Der Joystick erscheint am Finger. Für Aktionen nahe herangehen und Gegenstand, Tür oder Schild gedrückt halten, bis der Ring voll ist. Beim Loslassen oder Weglaufen wird abgebrochen. Desktop: WASD/Pfeiltasten, E; alternativ Objekt mit der Maus halten.

Sechs Gegenstände sammeln → Container am Ausbau-Schild herrichten (40 Taler) → Lichter (20 Taler) → Pfand an der Garage einlagern (+40 Taler) → Rasenheizung am Hauptplatz kaufen (40 Taler). Zusätzlich nach der Renovierung im linken Materialraum: sechs Materialien aufnehmen und zu den passenden Regalen tragen (+20 Taler einmalig). Beide Containertüren sind benutzbar. Noch eine frühe Testversion, kein fertiges Spiel.

## Ohne Browserleiste

Vollbild-Knopf im Spiel, soweit unterstützt. Auf iPhone in Safari über Teilen → Zum Home-Bildschirm hinzufügen und über das neue Symbol starten. Auf Android über das Browsermenü installieren/zum Startbildschirm hinzufügen. Abhängig von Gerät und Browser kann die Ansicht vom Vollbild abweichen. Die App bleibt online; es gibt keinen Offlinecache. Speicherstände können zwischen normalem Browser und Home-Bildschirm-App getrennt sein.

## Dateien und Entwicklung

Statisches HTML/CSS/JavaScript, keine externen Laufzeitabhängigkeiten. `index.html`, `style.css`, `game.js`, `manifest.webmanifest`, `assets/`. Lokal über einen statischen Server starten, z.B. `python -m http.server 8080`. Tests: `node check-mobile.cjs` und `node check-fonts.cjs`. GitHub Pages: main, /(root). Für ALL-INKL können die gleichen Laufzeitdateien hochgeladen werden.

Grafiken: Boden 32×32, Kiste 64×32, Spieler 64×96, im Spiel 32×48. Spielerdateien: player_front_s/w.png, player_back_s/w.png, player_left_s/w.png, player_right_s/w.png; _s steht, _w geht. Je Richtung wechseln die zwei Bilder. Zusätzliche Bodenvarianten und Figurenanpassung folgen erst nach der Hauptspielschleife.

Speicherung: lokal, automatischer Spielstand, Menü zum Zurücksetzen. Keine Registrierung und keine Cloud-Synchronisierung. Siehe STATUS.md für den aktuellen Entwicklungsstand und ASSETS.md für die Asset-Konventionen. Schriften: Minecraftia für Texte und RasterForge für Titel, lokal in assets/fonts. Nunito bleibt als Fallback. Die Darstellungsgrößen werden im Code festgelegt und sind unabhängig von der Pixelgröße der PNG-Dateien.
