# Game Design Document
## "2 Mäuse in Vietnam & Thailand"
### Ein Geburtstags-Plattformer mit Herz

---

## 1. Übersicht

| Feld | Inhalt |
|------|--------|
| **Arbeitstitel** | 2 Mäuse in Vietnam & Thailand |
| **Genre** | 2D Side-Scroller / Plattformer |
| **Zielgruppe** | 1 Person (Geburtstagskind!) |
| **Anlass** | Geburtstag am 17.01 |
| **Ton** | Niedlich, warm, humorvoll, nostalgisch |
| **Technik** | HTML5 + Canvas + JavaScript (Single File) |

---

## 2. Kernkonzept

### Die Story
Eine kleine weibliche Maus namens **"Mausi"** reist durch die Stationen einer gemeinsamen Reise – von Hanoi über Hoi An, das Mekong Delta, Saigon bis zu den thailändischen Inseln. Am Ende von Level 1 befreit sie eine männliche Maus aus einem Käfig – die ebenfalls **"Mausi"** heißt.

**Der Witz:** Beide heißen Mausi. Das ist Absicht. Das ist Liebe.

### Emotionaler Kern
- Erinnerungen an eine gemeinsame Reise
- Spielerische Liebeserklärung
- Überraschung in Level 2 (der echte Gutschein!)

---

## 3. Zwei-Level-Struktur

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│  LEVEL 1: "Die große Reise"                                            │
│  ══════════════════════════                                            │
│                                                                         │
│  [Hanoi] → [Hoi An] → [Mekong] → [Saigon] → [Inseln] → [Käfig-Finale]  │
│                                                                         │
│  Ziel: Mausi befreien                                                  │
│  Sammeln: Käse + 7 Souvenirs                                           │
│  Ende: "Mausi hat Mausi befreit!" + Geburtstagsbotschaft               │
│                                                                         │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  LEVEL 2: "Bonus-Runde – Die Schatzsuche"                              │
│  ═════════════════════════════════════════                              │
│                                                                         │
│  [Therme-Zone] → [Restaurant-Zone] → [Hotel-Zone] → [Großes Finale]    │
│                                                                         │
│  Ziel: 3 goldene Geschenke erspielen                                   │
│  Beide Mäuse spielen zusammen!                                         │
│  Ende: Gutschein-Reveal mit allen 3 Geschenken                         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 4. LEVEL 1: "Die große Reise"

### Übersicht

| Aspekt | Details |
|--------|---------|
| **Spieler** | Weibliche Mausi (allein) |
| **Zonen** | 5 Reise-Zonen + Finale |
| **Ziel** | Käfig erreichen, Mausi befreien |
| **Collectibles** | Käse (∞) + 7 Souvenirs |
| **Länge** | ca. 5-8 Minuten |

---

### Zone 1.1: Hanoi – "Roller & Pho"

**Atmosphäre:** Geschäftiges Stadtleben, warm-orange Töne, Laternen

| Element | Beschreibung |
|---------|--------------|
| **Plattformen** | Hausdächer, Schilder, Stromkabel (Balancier-Seile) |
| **Deko** | Laternen, Streetfood-Stände, Pho-Schüsseln |
| **Hindernis** | Langsame Roller (vorhersehbar, Comic-Style) |
| **Gimmick** | "Pho-Dampf" – Dampfwolken als sanfter Aufwind |
| **Souvenir** | 🍜 Mini-Pho-Schüssel |

**Postkarte beim Eintritt:**
> "Hanoi – Wo Roller tanzen und Pho dampft!"

---

### Zone 1.2: Hoi An – "Lampion-Magie"

**Atmosphäre:** Romantisch, bunte Lampions, Fluss-Reflektionen

| Element | Beschreibung |
|---------|--------------|
| **Plattformen** | Holzbrücken, schwimmende Lampions |
| **Deko** | Bunte Lampions, Fluss, alte Häuser |
| **Mechanik** | Lampion-Plattformen leuchten auf beim Landen |
| **Souvenir** | 🏮 Lampion |

**Postkarte:**
> "Hoi An – Wo Wünsche leuchten!"

---

### Zone 1.3: Mekong Delta – "Boot-Abenteuer"

**Atmosphäre:** Grün, tropisch, entspannt, Wasser

| Element | Beschreibung |
|---------|--------------|
| **Plattformen** | Schwimmende Boote (schaukeln leicht) |
| **Deko** | Palmen, Wasserwege, Kokosnüsse |
| **Power-Up** | 🥥 Kokosnuss-Helm = 5 Sek. Unverwundbarkeit |
| **Souvenir** | 🚣 Boot |

**Postkarte:**
> "Mekong – Treiben lassen und genießen!"

---

### Zone 1.4: Saigon – "Neon & Chaos"

**Atmosphäre:** Urban, neon-beleuchtet, dynamisch

| Element | Beschreibung |
|---------|--------------|
| **Plattformen** | Häuserdächer, Neon-Schilder, Zebrastreifen |
| **Deko** | Skyline, Neon-Reklame, Markt-Stände |
| **Hindernis** | Rollende Koffer/Kisten (Rush-Passage) |
| **Mini-Boss** | 🛺 TukTuk-Spielzeug – 2x von oben treffen ODER ausweichen |
| **Souvenirs** | 🛵 Mini-Roller + 💡 Neon-Schild |

**Postkarte:**
> "Saigon – Stadt die niemals schläft!"

---

### Zone 1.5: Thailand-Inseln – "Insel-Hopping"

**Atmosphäre:** Paradiesisch, türkis, entspannt, Strand

| Element | Beschreibung |
|---------|--------------|
| **Plattformen** | Felsen, Strandhütten, Palmen-Stämme |
| **Deko** | Strand, türkises Wasser, Muscheln |
| **Mechanik** | 🐚 Muscheln als Sprungfedern |
| **Kosmetik** | 🤿 Schnorchel-Mausi Skin (optional, lustig) |
| **Souvenirs** | 🐚 Muschel + 🥥 Kokosnuss |

**Drei Abschnitte:**
- Koh Chang (Felsen + Dschungel)
- Koh Mak (Ruhiger Strand)
- Koh Kood (Kristallwasser + Finale-Übergang)

**Postkarte:**
> "Die Inseln – Koh Chang, Koh Mak, Koh Kood – Paradies gefunden!"

---

### Zone 1.6: Finale – "Der Strandtempel"

**Atmosphäre:** Magisch, golden, emotional

| Element | Beschreibung |
|---------|--------------|
| **Setting** | Kleine Tempelruine am Strand |
| **Ziel** | Goldenen Käse-Schlüssel finden |
| **Finale** | Käfig öffnen, Mausi befreien |

**Ablauf:**
1. Heldin erreicht Tempel
2. Findet goldenen Schlüssel
3. Öffnet Käfig
4. **Cutscene:** Beide Mäuse stehen nebeneinander

---

### Level 1 Endsequenz

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  [Käfig öffnet sich mit Partikel-Effekt]                   │
│                                                             │
│  Weibliche Mausi: "Du bist frei!"                          │
│  Männliche Mausi: "Danke! Ich bin Mausi."                  │
│  Weibliche Mausi: "...Ich auch."                           │
│  Männliche Mausi: "Oh."                                    │
│                                                             │
│  [Herzen + Käse-Partikel regnen]                           │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│           🎂 HAPPY BIRTHDAY, MAUSI! 🎂                      │
│                    17.01 ❤️                                 │
│                                                             │
│          "Mausi hat Mausi befreit!"                        │
│                                                             │
│  ───────────────────────────────────────                   │
│                                                             │
│  Souvenirs gesammelt: [🍜][🏮][🚣][🛵][💡][🐚][🥥]        │
│  Käse: 47 🧀                                               │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│          "Aber warte... da ist noch mehr!"                 │
│                                                             │
│     Männliche Mausi: "Ich hab eine Überraschung für dich!" │
│                                                             │
│              → [BONUS-LEVEL STARTEN] ←                     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## 5. LEVEL 2: "Bonus-Runde – Die Schatzsuche"

### Übersicht

| Aspekt | Details |
|--------|---------|
| **Spieler** | Beide Mäuse zusammen! (visuell) |
| **Zonen** | 3 Geschenk-Zonen + Großes Finale |
| **Ziel** | 3 goldene Geschenke erspielen |
| **Collectibles** | Die 3 Gutschein-Artefakte |
| **Länge** | ca. 3-4 Minuten |
| **Ton** | Überraschend, festlich, magisch |

### Besonderheit: Zusammen unterwegs!
- Beide Mäuse laufen nebeneinander (oder hintereinander)
- Optisch: Männliche Mausi folgt der Spielerin
- Symbolisiert: "Wir machen das zusammen!"

---

### Zone 2.1: "Die Therme-Oase" 🌊

**Atmosphäre:** Entspannt, dampfend, Spa-Feeling, blau-türkis

| Element | Beschreibung |
|---------|--------------|
| **Setting** | Fantasie-Thermenlandschaft |
| **Plattformen** | Dampfende Becken, Holzstege, Wasserfälle |
| **Deko** | Dampfwolken, Kerzen, Bambus, Steine |
| **Mechanik** | Dampf-Geysire als Sprungboost |
| **Hindernis** | Heiße Quellen (kurz warten bis Dampf nachlässt) |

**Das goldene Geschenk:**
```
┌─────────────────────────────────┐
│     🌊 GOLDENE WELLE 🌊         │
│                                 │
│  Am Ende der Zone schwebt sie   │
│  majestätisch über einem        │
│  glitzernden Pool               │
│                                 │
│  [Einsammeln mit Partikel!]    │
└─────────────────────────────────┘
```

**Kurze Einblendung nach Collect:**
> "Ein Schatz gefunden! Was könnte das bedeuten...?"

---

### Zone 2.2: "Das Restaurant der Sterne" ⭐

**Atmosphäre:** Elegant, warm, Kerzenlicht, gold-rot

| Element | Beschreibung |
|---------|--------------|
| **Setting** | Fantasie-Gourmet-Restaurant |
| **Plattformen** | Gedeckte Tische, Kronleuchter, Regale |
| **Deko** | Kerzen, Weingläser, Teller, Sterne |
| **Mechanik** | Springende Champagner-Korken als Boost |
| **Hindernis** | Rollende Käsekugeln (natürlich essbar = Bonus!) |

**Das goldene Geschenk:**
```
┌─────────────────────────────────┐
│     ⭐ GOLDENER STERN ⭐         │
│                                 │
│  Schwebt über dem schönsten     │
│  Tisch im Restaurant            │
│                                 │
│  [Einsammeln mit Sternenregen!] │
└─────────────────────────────────┘
```

**Kurze Einblendung:**
> "Noch ein Schatz! Da braut sich was zusammen..."

---

### Zone 2.3: "Das Traumhotel" 🏠

**Atmosphäre:** Gemütlich, luxuriös, warm, Abendstimmung

| Element | Beschreibung |
|---------|--------------|
| **Setting** | Fantasie-Boutique-Hotel |
| **Plattformen** | Betten (federnde!), Balkone, Treppen |
| **Deko** | Kissen, Lampen, Vorhänge, Sternenhimmel |
| **Mechanik** | Betten als Trampoline |
| **Hindernis** | Fliegende Kissen (lustig, nicht gefährlich) |

**Das goldene Geschenk:**
```
┌─────────────────────────────────┐
│     🏠 GOLDENES HAUS 🏠         │
│                                 │
│  Auf dem Balkon des             │
│  schönsten Zimmers              │
│  mit Blick auf Sterne           │
│                                 │
│  [Einsammeln mit Feuerwerk!]    │
└─────────────────────────────────┘
```

**Kurze Einblendung:**
> "Der dritte Schatz! Zeit für die große Enthüllung!"

---

### Zone 2.4: Das Große Finale – "Der Geschenke-Tempel"

**Setting:** Magischer Ort wo alle 3 Schätze zusammenkommen

```
Beide Mäuse erreichen einen leuchtenden Altar.

Die 3 goldenen Artefakte schweben empor...

[TRANSFORMATION BEGINNT]

Dramatische Pause... Licht... Partikel...

Die Artefakte transformieren sich!
```

---

## 6. Der Große Gutschein-Reveal

### Die Enthüllung (Schritt für Schritt)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Bildschirm wird golden, magische Musik]                      │
│                                                                 │
│  "Die Schätze eurer Reise enthüllen ihre wahre Bedeutung..."   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘

                              ↓

┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│     🌊 Die Goldene Welle transformiert sich...                 │
│                                                                 │
│     ════════════════════════════════════════                   │
│                                                                 │
│     🧖‍♀️  "Ein Tag in der Therme"                               │
│         Entspannung pur – nur für dich!                        │
│                                                                 │
│     ════════════════════════════════════════                   │
│                                                                 │
│                    [Weiter...]                                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘

                              ↓

┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│     ⭐ Der Goldene Stern transformiert sich...                 │
│                                                                 │
│     ════════════════════════════════════════                   │
│                                                                 │
│     🍽️  "Restaurant deiner Wahl"                               │
│         Du suchst aus – ich lade ein!                          │
│                                                                 │
│     ════════════════════════════════════════                   │
│                                                                 │
│                    [Weiter...]                                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘

                              ↓

┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│     🏠 Das Goldene Haus transformiert sich...                  │
│                                                                 │
│     ════════════════════════════════════════                   │
│                                                                 │
│     🛏️  "Eine Nacht im Hotel"                                  │
│         Zusammen – irgendwo Schönes!                           │
│                                                                 │
│     ════════════════════════════════════════                   │
│                                                                 │
│                    [Weiter...]                                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘

                              ↓

┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                    ✨ DEIN GESCHENK ✨                          │
│                                                                 │
│     ═══════════════════════════════════════════════════════    │
│                                                                 │
│       🧖‍♀️  Therme         ⭐  Restaurant         🛏️  Hotel     │
│                                                                 │
│     ═══════════════════════════════════════════════════════    │
│                                                                 │
│         Ein komplettes Verwöhn-Wochenende für Mausi!           │
│                                                                 │
│     ═══════════════════════════════════════════════════════    │
│                                                                 │
│                                                                 │
│          [Konfetti-Explosion + Herzen-Partikel]                │
│                                                                 │
│                                                                 │
│              🎂 HAPPY BIRTHDAY, MAUSI! 🎂                       │
│                       17.01 ❤️                                  │
│                                                                 │
│                                                                 │
│           Alles Liebe von deinem anderen Mausi                 │
│                                                                 │
│                                                                 │
│                    [Nochmal spielen]                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 7. Gameplay-Mechaniken

### Steuerung

| Taste | Aktion |
|-------|--------|
| ← → / A D | Links / Rechts |
| ↑ / W / Space | Springen |
| Shift (optional) | Sprint |

### Physik
- Saubere Gravitation
- Coyote Time (kurze Sprung-Toleranz nach Plattformkante)
- Große, faire Hitboxen

### Sammel-Systeme

**Level 1: Käse + Souvenirs**

| Typ | Anzahl | Anzeige |
|-----|--------|---------|
| Käse 🧀 | Unbegrenzt | Counter oben links |
| Souvenirs | 7 Stück | Icons im HUD |

**Souvenirs:**
| # | Item | Zone |
|---|------|------|
| 1 | 🍜 Pho-Schüssel | Hanoi |
| 2 | 🏮 Lampion | Hoi An |
| 3 | 🚣 Boot | Mekong |
| 4 | 🛵 Mini-Roller | Saigon |
| 5 | 💡 Neon-Schild | Saigon |
| 6 | 🐚 Muschel | Thailand |
| 7 | 🥥 Kokosnuss | Thailand |

**Level 2: Goldene Geschenke**

| # | Geschenk | Zone | Bedeutung |
|---|----------|------|-----------|
| 1 | 🌊 Goldene Welle | Therme-Oase | Therme-Einladung |
| 2 | ⭐ Goldener Stern | Restaurant | Freie Restaurantwahl |
| 3 | 🏠 Goldenes Haus | Traumhotel | Hotelübernachtung |

### Power-Ups

| Power-Up | Effekt | Level/Zone |
|----------|--------|------------|
| 🍜 Pho-Dampf | Höherer Sprung | L1: Hanoi |
| 🥥 Kokosnuss-Helm | 5 Sek. Unverwundbar | L1: Mekong |
| 🐚 Muschel-Feder | Super-Sprung | L1: Thailand |
| 🤿 Schnorchel | Kosmetisch | L1: Thailand |
| ♨️ Dampf-Geysir | Sprungboost | L2: Therme |
| 🍾 Champagner-Korken | Sprungboost | L2: Restaurant |
| 🛏️ Bett-Trampolin | Bounce | L2: Hotel |

### Gegner/Hindernisse

**Level 1:**
| Hindernis | Verhalten | Zone |
|-----------|-----------|------|
| 🛵 Roller | Fährt langsam hin/her | Hanoi |
| 🐟 Fisch | Springt aus Wasser | Mekong |
| 🦀 Krabbe | Läuft seitlich | Thailand |
| 🛺 TukTuk | Mini-Boss (2x treffen) | Saigon |
| 📦 Koffer | Rollen durch | Saigon |

**Level 2:**
| Hindernis | Verhalten | Zone |
|-----------|-----------|------|
| ♨️ Heiße Quelle | Timing-Hindernis | Therme |
| 🧀 Käsekugeln | Rollen (aber sammelbar!) | Restaurant |
| 🛋️ Fliegende Kissen | Lustig, nicht gefährlich | Hotel |

### Checkpoints
- Nach jeder Zone automatisch
- Visuell: kleine Flagge mit Maus-Symbol

---

## 8. Visuelle Gestaltung

### Farbpalette

**Level 1:**
| Zone | Primär | Sekundär | Akzent |
|------|--------|----------|--------|
| Hanoi | Orange | Rot | Gold |
| Hoi An | Lila/Pink | Gelb | Türkis |
| Mekong | Grün | Braun | Blau |
| Saigon | Neon-Pink | Blau | Weiß |
| Thailand | Türkis | Sand | Grün |
| Finale | Gold | Weiß | Rosa |

**Level 2:**
| Zone | Primär | Sekundär | Akzent |
|------|--------|----------|--------|
| Therme | Türkis | Weiß | Gold |
| Restaurant | Rot/Gold | Creme | Gelb |
| Hotel | Lila | Rosa | Sternenweiß |
| Gutschein-Finale | Gold | Weiß | Alle Farben |

### Charakter-Design: Die beiden Mausis

```
Basis-Design (beide):
- Runder Kopf, große Augen
- Kleine runde Ohren
- Rosa Nase
- Langer Schwanz
- Farbe: Hellgrau mit rosa Akzenten

Weibliche Mausi:
- Kleine rosa Schleife am Ohr
- Spielbare Figur

Männliche Mausi:
- Kleines blaues Halstuch
- Level 1: Gefangen im Käfig
- Level 2: Folgt der Spielerin
```

### Art-Style
- Cartoon/Pixel-Hybrid
- Klare Formen, lesbar
- Warme Farben
- Viele kleine Details als Deko

---

## 9. Audio-Konzept

### Einfache WebAudio-Sounds

| Event | Sound | Level |
|-------|-------|-------|
| Sprung | Kurzes "Boing" | Beide |
| Käse sammeln | Fröhliches "Pling" | L1 |
| Souvenir | Magisches "Shimmer" | L1 |
| Goldenes Geschenk | Episches "Gong" + Glockenspiel | L2 |
| Schaden | Sanftes "Aua" | Beide |
| Checkpoint | Melodisches "Ta-da" | Beide |
| Käfig öffnen | Triumphale Fanfare | L1 Ende |
| Geschenk-Reveal | Magische Harfe | L2 Ende |
| Finale | Party-Sounds + Konfetti | Ende |

---

## 10. UI-Elemente

### HUD Level 1

```
┌──────────────────────────────────────────────────────────┐
│ 🧀 47                              [Zone: Hoi An]        │
│                                                          │
│ Souvenirs: [🍜][🏮][  ][  ][  ][  ][  ]                 │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

### HUD Level 2

```
┌──────────────────────────────────────────────────────────┐
│                           [Bonus-Level: Die Schatzsuche] │
│                                                          │
│ Geschenke: [🌊][  ][  ]    ← Zeigt gefundene Schätze    │
│                                                          │
│ 🐭🐭 ← Beide Mäuse unterwegs!                           │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

### Startbildschirm

```
┌──────────────────────────────────────────────────────────┐
│                                                          │
│           🐭  2 MÄUSE IN VIETNAM & THAILAND  🐭          │
│                                                          │
│                    [SPIELEN]                             │
│                                                          │
│               ─────────────────                          │
│               Ein Spiel für Mausi                        │
│                    17.01 ❤️                              │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

### Level-Auswahl (nach erstem Durchspielen)

```
┌──────────────────────────────────────────────────────────┐
│                                                          │
│   [Level 1: Die große Reise]     ← Immer verfügbar      │
│                                                          │
│   [Level 2: Bonus-Runde]         ← Nach L1 freigeschaltet│
│                                                          │
└──────────────────────────────────────────────────────────┘
```

---

## 11. Easter Eggs & Gimmicks

### Pflicht-Features

| # | Feature | Beschreibung | Level |
|---|---------|--------------|-------|
| ✅ | Namenswitz | "Ich bin Mausi" - "Ich auch" - "Oh" | L1 Ende |
| ✅ | Postkarten | 5 Postkarten nach jeder L1-Zone | L1 |
| ✅ | Souvenirs | 7 sammelbare Erinnerungen | L1 |
| ✅ | Konfetti | Partikel-Explosion beim Finale | L2 Ende |
| ✅ | Geschenk-Reveal | Dramatische Gutschein-Enthüllung | L2 Ende |
| ✅ | Zusammen spielen | Beide Mäuse in Level 2 | L2 |

### Optionale Extras

| Gimmick | Beschreibung |
|---------|--------------|
| Geheimweg | Versteckter Pfad zu Bonus-Käse in L1 |
| Sound-Design | WebAudio Töne |
| Schnorchel-Skin | Kosmetisches Power-Up |
| 50+ Käse Bonus | Extra-Konfetti wenn viel gesammelt |

---

## 12. Technische Umsetzung

### Dateistruktur
```
index.html          ← Alles in einer Datei
├── HTML            ← Canvas-Container
├── CSS             ← Inline-Styles
└── JavaScript      ← Game-Logic
    ├── Game Loop
    ├── Physics
    ├── Rendering (beide Level)
    ├── Level Data (L1 + L2)
    ├── Collision
    ├── UI + Cutscenes
    └── Audio
```

### Level-Speicherung
- LocalStorage speichert: "Level 1 abgeschlossen"
- Ermöglicht direkten Zugang zu Level 2 beim nächsten Besuch

---

## 13. Personalisierung

### Leicht anpassbare Werte

```javascript
// === PERSONALISIERUNG ===
const BIRTHDAY_NAME = "Mausi";
const BIRTHDAY_DATE = "17.01";

// Die 3 Geschenke
const GIFT_1 = {
    name: "Therme",
    icon: "🧖‍♀️",
    title: "Ein Tag in der Therme",
    subtitle: "Entspannung pur – nur für dich!"
};

const GIFT_2 = {
    name: "Restaurant",
    icon: "🍽️",
    title: "Restaurant deiner Wahl",
    subtitle: "Du suchst aus – ich lade ein!"
};

const GIFT_3 = {
    name: "Hotel",
    icon: "🛏️",
    title: "Eine Nacht im Hotel",
    subtitle: "Zusammen – irgendwo Schönes!"
};

const FINAL_MESSAGE = "Alles Liebe von deinem anderen Mausi";
```

---

## 14. Spielzeit-Schätzung

| Teil | Geschätzte Zeit |
|------|-----------------|
| Level 1 komplett | 5-8 Minuten |
| Level 1 Endsequenz | 1 Minute |
| Level 2 komplett | 3-4 Minuten |
| Gutschein-Reveal | 1-2 Minuten |
| **Gesamt** | **~10-15 Minuten** |

Perfekt für ein Geburtstags-Überraschungsspiel!

---

## 15. Zusammenfassung

### Was macht dieses Spiel besonders?

1. **Zwei-Akt-Struktur:**
   - Level 1 = Emotionale Reise + Befreiung
   - Level 2 = Überraschung + echtes Geschenk

2. **Zusammen-Spielen:**
   - In Level 2 laufen beide Mäuse zusammen
   - Symbolisiert die Beziehung

3. **Der Twist:**
   - Man denkt, das Spiel ist nach Level 1 vorbei
   - Aber es gibt noch mehr!

4. **Das echte Geschenk:**
   - Therme + Restaurant + Hotel
   - Wird spielerisch "erspielt"
   - Epischer Reveal am Ende

### Der Moment der Wahrheit:

> Nach Level 1: "Oh wie süß, Mausi hat Mausi befreit!"
>
> Nach Level 2: "WARTE, das ist ein ECHTES Geschenk?!"
>
> Das ist der Moment. ❤️

---

*Erstellt mit Liebe für Mausi – 17.01*
