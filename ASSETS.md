## 0.7: Original buildings and shovel poses

Buildings preserve aspect ratio: container 288x192, garage 192x96. Shovel poses use uniform pixel scale and a body pivot of x=32; the back pose has four additional pixels on the right. No shovel walk frames required yet. Free shovel pickup in the courtyard. Deposit action and crates moved into the container material room; garage is the equipment room. Snow clearing remains a following step.

# Grafiken und Schriften ab Testversion 0.6

Neu: snow_pile_small.png, snow_pile_mid.png und snow_pile_big.png (je 64Ã—64) sowie trash_bag.png (64Ã—64). Sie werden unterschiedlich groÃŸ dargestellt und anhand des sichtbaren unteren Pixels am Boden verankert.

Optionale Schneepartikel: assets/particles/snowflake_01.png, snowflake_02.png, snowflake_03.png. Jeweils 16Ã—16 PNG mit transparentem Hintergrund, Flocke mittig, weiÃŸ bis leicht blÃ¤ulich. Kein Schatten, kein Leuchten und keine eingebauten Bewegungsstreifen; GrÃ¶ÃŸe, Transparenz und Bewegung Ã¼bernimmt das Spiel. Die Dateien werden noch nicht automatisch eingebunden, solange sie nicht vorhanden sind. Der aktuelle Effekt funktioniert ohne diese Grafiken.

Bodenraster 32Ã—32. DateigrÃ¶ÃŸe und GrÃ¶ÃŸe in der Spielwelt sind unabhÃ¤ngig; transparente RÃ¤nder werden im Code berÃ¼cksichtigt. Vorhandene Bilder mÃ¼ssen nicht auf ein einheitliches Exportformat gezwungen werden.

| Datei in assets/props | DateigrÃ¶ÃŸe | Darstellung in Weltpixeln |
|---|---|---|
| shelf_empty.png | 48Ã—64 | 48Ã—64 |
| deposit_crate_green.png | 64Ã—64 | 26Ã—26 |
| deposit_crate_yellow.png | 64Ã—64 | 26Ã—26 |
| snow_shovel.png | 64Ã—64 | 32Ã—32 |
| ball.png | 32Ã—32 | 10Ã—10 |
| kit.png | 32Ã—32 | 16Ã—16 |
| box.png | 64Ã—32 | 56Ã—28 |

Kistenvarianten sind gleichartige PfandgegenstÃ¤nde. Sie stehen an der Garage und nach dem Pfandauftrag im Materialraum. Regale werden bei richtiger Ablage sichtbar mit Material gefÃ¼llt. Der Schneeschieber ist dekorativ platziert; eine RÃ¤umaufgabe ist ein weiterer Entwicklungsschritt.

Keine zusÃ¤tzlichen Grafiken sind zum Testen der Sortieraufgabe nÃ¶tig. Weitere Bodenvarianten und ein kompletter GUI-Satz warten, bis die Hauptspielschleife funktioniert.

## Schriften

Vom Nutzer bereitgestellt: Minecraftia-Regular.woff2 fÃ¼r Texte, RasterForgeRegular.woff2 fÃ¼r Titel. Dateien liegen lokal in assets/fonts. Beide unterstÃ¼tzen deutsche Umlaute und ÃŸ. Nunito bleibt als Fallback und behÃ¤lt seine mitgelieferte OFL-Lizenz. Die neuen Schriften verwenden ihre normale StrichstÃ¤rke ohne kÃ¼nstliche Fettung. Canvas und HTML verwenden dieselben Familien.

Spielcode enthÃ¤lt Sonderzeichen als JavaScript-Escapes, HTML als Zeichenreferenzen. Beim VerÃ¶ffentlichen wird eine neue Version fÃ¼r CSS und JS gesetzt.
