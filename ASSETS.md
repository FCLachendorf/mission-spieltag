## Nächste Texturen (0.8)

Die Varianten container_worn_fixed_window.png und container_restored_decoration.png sind eingebaut. Weitere Gebäudezustände werden gerade nicht benötigt.

| Priorität | Datei unter assets/ | Zeichenfläche | Zweck |
|---|---|---|---|
| 1 | minigames/wood_plank.png | 96×32 | Einzelnes verwittertes Brett, transparenter Hintergrund |
| 1 | minigames/nail.png | 16×16 | Nagelkopf von vorne, transparent |
| 1 | minigames/hammer.png | 32×32 | Klauenhammer zum Nagelziehen, transparent |
| 2 | characters/player_front_shovel_w.png | 64×96 | Zweite Bewegungsphase mit Schaufel |
| 2 | characters/player_back_shovel_w.png | 68×96 | Zweite Bewegungsphase; Körperposition wie im vorhandenen _s |
| 2 | characters/player_left_shovel_w.png | 64×96 | Zweite Bewegungsphase mit Schaufel |
| 2 | characters/player_right_shovel_w.png | 64×96 | Zweite Bewegungsphase mit Schaufel |
| 3 | props/line_marker.png | 64×64 | Kreidewagen für den Geräteraum |
| 3 | props/training_dummy.png | 32×64 | Aufstellfigur |
| 3 | props/pole_bundle.png | 32×64 | Bündel Trainingsstangen |
| 4 | particles/snowflake_01.png bis snowflake_03.png | je 16×16 | Unterschiedliche Flocken, transparent und zentriert |

Alle Maße sind Zeichenflächen, nicht die sichtbare Größe im Spiel. Die Figur innerhalb neuer Frames weder verschieben noch skalieren. Zusätzlicher Platz für Werkzeuge ist erlaubt, wenn die Seite bekannt ist. Minispiel-Grafiken und weitere Geräte sind erst nach der Lieferung verdrahtet; die aktuellen Minispiele verwenden Platzhalter und vorhandene Schneehaufen.

## 0.7: Original buildings and shovel poses

Buildings preserve aspect ratio: container 288x192, garage 192x96. Shovel poses use uniform pixel scale and a body pivot of x=32; the back pose has four additional pixels on the right. No shovel walk frames required yet. Free shovel pickup in the courtyard. Deposit action and crates moved into the container material room; garage is the equipment room. Snow clearing remains a following step.

# Grafiken und Schriften ab Testversion 0.6

Neu: snow_pile_small.png, snow_pile_mid.png und snow_pile_big.png (je 64Ãƒâ€”64) sowie trash_bag.png (64Ãƒâ€”64). Sie werden unterschiedlich groÃƒÅ¸ dargestellt und anhand des sichtbaren unteren Pixels am Boden verankert.

Optionale Schneepartikel: assets/particles/snowflake_01.png, snowflake_02.png, snowflake_03.png. Jeweils 16Ãƒâ€”16 PNG mit transparentem Hintergrund, Flocke mittig, weiÃƒÅ¸ bis leicht blÃƒÂ¤ulich. Kein Schatten, kein Leuchten und keine eingebauten Bewegungsstreifen; GrÃƒÂ¶ÃƒÅ¸e, Transparenz und Bewegung ÃƒÂ¼bernimmt das Spiel. Die Dateien werden noch nicht automatisch eingebunden, solange sie nicht vorhanden sind. Der aktuelle Effekt funktioniert ohne diese Grafiken.

Bodenraster 32Ãƒâ€”32. DateigrÃƒÂ¶ÃƒÅ¸e und GrÃƒÂ¶ÃƒÅ¸e in der Spielwelt sind unabhÃƒÂ¤ngig; transparente RÃƒÂ¤nder werden im Code berÃƒÂ¼cksichtigt. Vorhandene Bilder mÃƒÂ¼ssen nicht auf ein einheitliches Exportformat gezwungen werden.

| Datei in assets/props | DateigrÃƒÂ¶ÃƒÅ¸e | Darstellung in Weltpixeln |
|---|---|---|
| shelf_empty.png | 48Ãƒâ€”64 | 48Ãƒâ€”64 |
| deposit_crate_green.png | 64Ãƒâ€”64 | 26Ãƒâ€”26 |
| deposit_crate_yellow.png | 64Ãƒâ€”64 | 26Ãƒâ€”26 |
| snow_shovel.png | 64Ãƒâ€”64 | 32Ãƒâ€”32 |
| ball.png | 32Ãƒâ€”32 | 10Ãƒâ€”10 |
| kit.png | 32Ãƒâ€”32 | 16Ãƒâ€”16 |
| box.png | 64Ãƒâ€”32 | 56Ãƒâ€”28 |

Kistenvarianten sind gleichartige PfandgegenstÃƒÂ¤nde. Sie stehen an der Garage und nach dem Pfandauftrag im Materialraum. Regale werden bei richtiger Ablage sichtbar mit Material gefÃƒÂ¼llt. Der Schneeschieber ist dekorativ platziert; eine RÃƒÂ¤umaufgabe ist ein weiterer Entwicklungsschritt.

Keine zusÃƒÂ¤tzlichen Grafiken sind zum Testen der Sortieraufgabe nÃƒÂ¶tig. Weitere Bodenvarianten und ein kompletter GUI-Satz warten, bis die Hauptspielschleife funktioniert.

## Schriften

Vom Nutzer bereitgestellt: Minecraftia-Regular.woff2 fÃƒÂ¼r Texte, RasterForgeRegular.woff2 fÃƒÂ¼r Titel. Dateien liegen lokal in assets/fonts. Beide unterstÃƒÂ¼tzen deutsche Umlaute und ÃƒÅ¸. Nunito bleibt als Fallback und behÃƒÂ¤lt seine mitgelieferte OFL-Lizenz. Die neuen Schriften verwenden ihre normale StrichstÃƒÂ¤rke ohne kÃƒÂ¼nstliche Fettung. Canvas und HTML verwenden dieselben Familien.

Spielcode enthÃƒÂ¤lt Sonderzeichen als JavaScript-Escapes, HTML als Zeichenreferenzen. Beim VerÃƒÂ¶ffentlichen wird eine neue Version fÃƒÂ¼r CSS und JS gesetzt.
