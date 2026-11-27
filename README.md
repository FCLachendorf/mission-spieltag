## Test 0.15

Lappen liegt beim Reinigen sichtbar rechts neben dem Fenster. Mit Finger oder Maus greifen und auf das Fenster ziehen; beim Loslassen kehrt er an seinen Platz zurück. Pixelige Wischmaske und 100-%-Anzeige mit Resttoleranz bleiben erhalten. Fünf neue Trainingstexturen synchronisiert (noch keine Trainingsaufgabe damit implementiert).

## Test 0.14

Sechs feste Mischgruppen aus Bäumen, Büschen und Schnee statt verstreuter Einzelobjekte. Alle 61 lokalen Asset-Dateien abgeglichen, 17 neue/geänderte Dateien übernommen; Schneehaufen nach environment verschoben. Versionierte Bild-URLs verhindern veraltete Cache-Bilder. Priorisierte Zeichenliste in ASSETS.md und nächste Spielaufgaben in ROADMAP.md. Bestehende Aufgaben, Kollisions- und Erreichbarkeitstests bestehen.

## Test 0.13

Wintervegetation mit zwei Bäumen und drei Buschvarianten, passenden Bodenankern, Kollisionen und Verdeckung. Schneeflocken fallen mit individuellen Zufallspositionen und Bewegungen statt regelmäßiger Reihen.

## Test 0.12

Reinigungsanzeige bis 100 % mit unsichtbarer Resttoleranz. Stärkeres kontinuierliches Wackeln beim Nagelziehen. Engere seitliche Kollisionen an Garage und Container anhand der sichtbaren Wände.

## Test 0.11

93 % Reinigung mit passender Lappenmaske, korrigierte Nagelpositionen und vollständig sichtbarer Hammer. Hintere Nägel bleiben sichtbar, Ziehen dauert länger und hat eine Hebelbewegung. Schneehaufen verdecken die Figur abhängig von ihrer Position und blockieren an der Basis.

## Test 0.10

Fenster als große Nahansicht ohne Dialograhmen, korrekte Nagel-/Hammer-Ebenen und echte Lappentextur. Pixeliges Wischen mit 89-%-Ziel. Schaufel-Laufanimationen und alle fünf Schneeflocken eingebaut; Schneehaufen blockieren auch von oben.

## Test 0.9

Fenster-Minispiel mit Originaltexturen: zwei Bretter nacheinander entfernen (vier Nägel), danach 78 % des Fensters sauberwischen. Beide Türen werden getrennt freigeschaufelt. Schaufel am Geräteraum ablegbar. Schneehaufen besitzen Kollisionen; fertige alte Spielstände bleiben erhalten.

## Test 0.8

Restaurierung mit zwei einmaligen Minispielen: Nägel am Fenster ziehen und den Eingang mit der Schaufel freiräumen. Danach hilft Jörg im Spiel beim Herrichten (40 Materialtaler); Weihnachtsdeko kostet weitere 20 Taler. Größere Garage, 10 % näherer Blick und stärkerer Schneefall.

# Mission Spieltag Â· FC Lachendorf

Mobiles 2D-Browserspiel im Querformat, Testversion 0.6. Live-Test: https://fclachendorf.github.io/mission-spieltag/

## Bereiche und Orientierung

Containerhof: Vereinsbasis, zwei ContainerrÃ¤ume und Garage. Dem Weg nach rechts folgen, um ins Trainingsfeld zu wechseln; dem Weg nach unten folgen, um zum Spieltag zu gelangen. Training fÃ¼hrt links zurÃ¼ck, Spieltag oben zurÃ¼ck. Die Wege mÃ¼ssen bis zum Kartenrand verfolgt werden. Die Minimap zeigt nur erkundetes GelÃ¤nde. Kartenfortschritt und Bereich werden lokal gespeichert. Bei Ãœbernahme Ã¤lterer SpielstÃ¤nde bleibt der Fortschritt bestehen, der Standort beginnt im neuen Containerhof.

Im Treffpunkt liegt ein interaktives Sammelheft mit 25 Originalkarten. Zwei Karten pro Ansicht, 13 Seiten. Die Bilder stammen aus dem Ã¶ffentlichen Vereinsarchiv im Repository FCLachendorf/FCLachendorf-Sammelheft und werden bei Bedarf von dessen Ã¶ffentlicher Bildquelle geladen. Das Spiel funktioniert ohne externe JavaScript-Bibliotheken; das Kartenheft benÃ¶tigt zusÃ¤tzlich eine Verbindung zu dieser Bildquelle.

## Spielen

Smartphone: Im linken Drittel berÃ¼hren und ziehen. Der Joystick erscheint am Finger. FÃ¼r Aktionen nahe herangehen und Gegenstand, TÃ¼r oder Schild gedrÃ¼ckt halten, bis der Ring voll ist. Beim Loslassen oder Weglaufen wird abgebrochen. Desktop: WASD/Pfeiltasten, E; alternativ Objekt mit der Maus halten.

Sechs GegenstÃ¤nde sammeln â†’ Container am Ausbau-Schild herrichten (40 Taler) â†’ Lichter (20 Taler) â†’ Pfand an der Garage einlagern (+40 Taler) â†’ Rasenheizung am Hauptplatz kaufen (40 Taler). ZusÃ¤tzlich nach der Renovierung im linken Materialraum: sechs Materialien aufnehmen und zu den passenden Regalen tragen (+20 Taler einmalig). Beide ContainertÃ¼ren sind benutzbar. Noch eine frÃ¼he Testversion, kein fertiges Spiel.

## Ohne Browserleiste

Vollbild-Knopf im Spiel, soweit unterstÃ¼tzt. Auf iPhone in Safari Ã¼ber Teilen â†’ Zum Home-Bildschirm hinzufÃ¼gen und Ã¼ber das neue Symbol starten. Auf Android Ã¼ber das BrowsermenÃ¼ installieren/zum Startbildschirm hinzufÃ¼gen. AbhÃ¤ngig von GerÃ¤t und Browser kann die Ansicht vom Vollbild abweichen. Die App bleibt online; es gibt keinen Offlinecache. SpeicherstÃ¤nde kÃ¶nnen zwischen normalem Browser und Home-Bildschirm-App getrennt sein.

## Dateien und Entwicklung

Statisches HTML/CSS/JavaScript, keine externen LaufzeitabhÃ¤ngigkeiten. `index.html`, `style.css`, `game.js`, `manifest.webmanifest`, `assets/`. Lokal Ã¼ber einen statischen Server starten, z.B. `python -m http.server 8080`. Tests: `node check-mobile.cjs` und `node check-fonts.cjs`. GitHub Pages: main, /(root). FÃ¼r ALL-INKL kÃ¶nnen die gleichen Laufzeitdateien hochgeladen werden.

Grafiken: Boden 32Ã—32, Kiste 64Ã—32, Spieler 64Ã—96, im Spiel 32Ã—48. Spielerdateien: player_front_s/w.png, player_back_s/w.png, player_left_s/w.png, player_right_s/w.png; _s steht, _w geht. Je Richtung wechseln die zwei Bilder. ZusÃ¤tzliche Bodenvarianten und Figurenanpassung folgen erst nach der Hauptspielschleife.

Speicherung: lokal, automatischer Spielstand, MenÃ¼ zum ZurÃ¼cksetzen. Keine Registrierung und keine Cloud-Synchronisierung. Siehe STATUS.md fÃ¼r den aktuellen Entwicklungsstand und ASSETS.md fÃ¼r die Asset-Konventionen. Schriften: Minecraftia fÃ¼r Texte und RasterForge fÃ¼r Titel, lokal in assets/fonts. Nunito bleibt als Fallback. Die DarstellungsgrÃ¶ÃŸen werden im Code festgelegt und sind unabhÃ¤ngig von der PixelgrÃ¶ÃŸe der PNG-Dateien.
