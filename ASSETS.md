# Texturen-Checkliste – Mission Spieltag

Stand 0.14. Dateien unter `assets/` ablegen. PNG, transparenter Hintergrund, keine weichen Skalierungsfilter. Größen sind Zeichenflächen in Pixeln; bei größerem Motiv bitte zusätzliche transparente Ränder nennen. Gebäude und große Gegenstände aus derselben leicht erhöhten Perspektive wie der Container. Bodenanker jeweils unten mittig am sichtbaren Motiv.

## Schon vorhanden – bitte nicht erneut zeichnen

- [x] Zwei Winterbäume und drei Winterbüsche (unterschiedliche Zeichenflächen unterstützt).
- [x] Drei Schneehaufen in `environment/` und fünf Schneeflocken in `particles/`.
- [x] Container-Zustände, Garage, Fenster-Minispiel mit Hammer und Lappen.
- [x] Spieler mit und ohne Schaufel, Gehbilder.
- [x] Bälle, Hütchen, Trikot, Materialkiste, Schaufel und Regal.
- [x] Leere und gefüllte grüne/gelbe Pfandkisten.
- [x] `props/line_marker.png` (96×96) und `props/training_dummy.png` (64×128). Für kommende Platzaufgaben bereit; noch keine neue Aufgabe damit umgesetzt.

## Paket 1 – Trainingsfeld vorbereiten (als Nächstes)

Mit vorhandenen Hütchen, Aufstellfigur und Kreidewagen lässt sich bereits viel programmieren. Diese Ergänzungen machen Start und fertigen Zustand klarer:

- [ ] `props/pole_bundle.png` – 64×64: gebündelte Trainingsstangen zum Abholen im Geräteraum.
- [ ] `props/training_pole.png` – 32×64: einzelne aufgestellte Stange, Fuß unten mittig.
- [ ] `props/goal_small.png` – 128×96: kleines Trainingstor, transparentes Netz; kein Hintergrundrasen.
- [ ] `props/ball_bag.png` – 64×64: Ballnetz bzw. Ballsack am Geräteraum.

Zielmarkierungen, Fortschrittsbalken und Kreidelinien werden zunächst im Code gezeichnet. Dafür brauchst du keine Einzelbilder. Spielfelder werden vor diesen Aufgaben längs ausgerichtet.

## Paket 2 – Verkaufsstand aufbauen

Erst nach Paket 1 nötig. Je Gebäudezustand gleiche Zeichenfläche und exakt gleicher Standort:

- [ ] `buildings/kiosk_worn.png` – 192×160: geschlossener, unfertiger Verkaufsstand.
- [ ] `buildings/kiosk_restored.png` – 192×160: fertiger Stand mit offener Ausgabe und Ablage.
- [ ] `props/cup_empty.png` – 32×32: leerer Becher.
- [ ] `props/cup_full.png` – 32×32: gleicher Becher gefüllt, identische Position.
- [ ] `props/sausage_plate.png` – 32×32: Bratwurst auf Pappteller, ohne Markenaufschrift.

Geplante Verwendung: Stand herrichten und eine kurze Bestellrunde spielen. Keine dauernd wiederholte Schneeschaufelpflicht.

## Paket 3 – Das fertige Lachtstadion

- [ ] `buildings/stand_worn.png` – 256×160: kleines unfertiges Tribünenelement.
- [ ] `buildings/stand_restored.png` – 256×160: gleiches Element mit fertigen Sitz-/Stehplätzen.
- [ ] `environment/floodlight_off.png` – 64×192: Flutlichtmast, Licht aus.
- [ ] `environment/floodlight_on.png` – 64×192: identischer Mast mit leuchtenden Lampen; Lichtschein macht der Code.
- [ ] `props/goal_large.png` – 192×128: großes Tor für die Stirnseite des längs liegenden Platzes.
- [ ] `props/bench.png` – 96×64: Vereinsbank, passend zu den vorhandenen Gebäuden.

## Später optional – keine Voraussetzung

- [ ] `environment/fence_horizontal.png` – 64×64: wiederholbares waagerechtes Zaunstück.
- [ ] `environment/fence_vertical.png` – 32×64: entsprechendes senkrechtes Stück.
- [ ] `props/team_photo_frame.png` – 64×48: Rahmen für Mannschaftsbilder im Container; Bildinhalt separat.
- [ ] Eigenes Sammelheft: erst Seitenformat und Bedienung gemeinsam festlegen, danach Cover und Seiten zeichnen.

## Partikel und GUI

Aktuell keine neuen Partikel erforderlich. Windrichtung, Böen und individuelle Bewegung entstehen im Code. Die fünf Schneeflocken reichen. Staub, Funken oder Schneespritzer erst ergänzen, wenn eine konkrete Aktion sie braucht.

Auch ein komplettes GUI-Paket lohnt sich erst nach den nächsten Aufgaben: Dann stehen benötigte Fenster, Symbole und Größen fest. Die vorhandenen Fonts bleiben.

## Synchronisieren

Die lokalen Quelldateien sind maßgeblich. In 0.14 wurden alle 61 Quelldateien gegen GitHub geprüft und 17 neue/geänderte Dateien übernommen. Schneehaufen liegen jetzt nur unter `assets/environment/` im Repository. Asset-URLs haben eine Versionskennung, damit geänderte Bilder neu geladen werden.
