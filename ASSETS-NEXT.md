# Nächste Grafiken und feste Maßstäbe

Stand: Testversion 0.4. Die vorhandenen Texturen reichen für die nächsten grundlegenden Spielmechaniken. Keine weiteren Bodenvarianten und kein GUI-Komplettsatz nötig.

## Maßstab

Bodenraster 32×32. Die Bilddatei legt nicht die Größe in der Welt fest: transparente Ränder und Darstellungsgröße werden im Code berücksichtigt. Spielerbilder bleiben unverändert 64×96. Sichtbare Figurenhöhe etwa 40 Weltpixel. Fußball etwa 9 Weltpixel Durchmesser, gefaltetes Trikot etwa 14×13, Materialkiste etwa 35×25 sichtbare Pixel. Touchflächen bleiben unabhängig von kleinen Grafiken groß.

## Nächste Aufgabe: Materialraum sortieren

Als nächsten Entwicklungsschritt ein echtes Sortier-Minispiel planen: Materialien aufnehmen und in passende Regalbereiche bringen. Falsche Ablage wird zurückgewiesen, richtige Ablage verändert sichtbar das Regal. Es soll die bisherige reine Sammelschleife ergänzen. Noch nicht implementiert.

Die vorhandenen Bälle, Hütchen, Trikots und die Kiste reichen zum Prototypenbau. Wenn du parallel zeichnen möchtest, haben diese Dateien Vorrang:

| Datei | Zeichenfläche | Verwendung |
|---|---|---|
| assets/props/shelf-empty.png | 64×64 px | Leeres Materialregal, gleiche Perspektive wie die Figur |
| assets/props/deposit-crate.png | 32×32 px | Pfandkiste, vom Sportmaterial unterscheidbar |
| assets/props/snow-shovel.png | 32×32 px | Schneeschieber für eine spätere aktive Winteraufgabe |

PNG, transparenter Hintergrund, gleicher Lichteinfall. Gegenstände innerhalb der Zeichenfläche mittig; möglichst konsistenter Abstand zur Unterkante. Gebäude und Bodenvarianten erst ergänzen, wenn die erste Aufgabe Spaß macht. Für ein Mäh-/Schneeräum-Minispiel legen wir die benötigten Ansichten des Werkzeugs vorab fest.

## Schrift und Text

Nunito liegt inklusive OFL-Lizenz in assets/fonts. Oberfläche und Weltbeschriftungen verwenden dieselbe Schrift. Keine externen Font-Aufrufe. JavaScript enthält Unicode-Escapes für Sonderzeichen; HTML enthält Zeichenreferenzen. Das verhindert, dass eine fehlerhafte Terminal-Zeichenkodierung Umlaute beim Übertragen zerstört. Dateien bleiben UTF-8. Bei Veröffentlichung beide Dateiversionen in index.html aktualisieren.
