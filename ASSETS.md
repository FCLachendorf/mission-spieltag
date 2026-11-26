# Grafiken und Schriften ab Testversion 0.5

Bodenraster 32×32. Dateigröße und Größe in der Spielwelt sind unabhängig; transparente Ränder werden im Code berücksichtigt. Vorhandene Bilder müssen nicht auf ein einheitliches Exportformat gezwungen werden.

| Datei in assets/props | Dateigröße | Darstellung in Weltpixeln |
|---|---|---|
| shelf_empty.png | 48×64 | 48×64 |
| deposit_crate_green.png | 64×64 | 26×26 |
| deposit_crate_yellow.png | 64×64 | 26×26 |
| snow_shovel.png | 64×64 | 32×32 |
| ball.png | 32×32 | 10×10 |
| kit.png | 32×32 | 16×16 |
| box.png | 64×32 | 56×28 |

Kistenvarianten sind gleichartige Pfandgegenstände. Sie stehen an der Garage und nach dem Pfandauftrag im Materialraum. Regale werden bei richtiger Ablage sichtbar mit Material gefüllt. Der Schneeschieber ist dekorativ platziert; eine Räumaufgabe ist ein weiterer Entwicklungsschritt.

Keine zusätzlichen Grafiken sind zum Testen der Sortieraufgabe nötig. Weitere Bodenvarianten und ein kompletter GUI-Satz warten, bis die Hauptspielschleife funktioniert.

## Schriften

Vom Nutzer bereitgestellt: Minecraftia-Regular.woff2 für Texte, RasterForgeRegular.woff2 für Titel. Dateien liegen lokal in assets/fonts. Beide unterstützen deutsche Umlaute und ß. Nunito bleibt als Fallback und behält seine mitgelieferte OFL-Lizenz. Die neuen Schriften verwenden ihre normale Strichstärke ohne künstliche Fettung. Canvas und HTML verwenden dieselben Familien.

Spielcode enthält Sonderzeichen als JavaScript-Escapes, HTML als Zeichenreferenzen. Beim Veröffentlichen wird eine neue Version für CSS und JS gesetzt.
