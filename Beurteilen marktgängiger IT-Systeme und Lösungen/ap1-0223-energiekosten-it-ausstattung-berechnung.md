---
# Identity (stable; never change after publishing)
id: ap1-0223
slug: energiekosten-it-ausstattung-berechnung

# Display
title: "Energiekosten von IT-Ausstattung berechnen"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["Energieverbrauch", "Kostenberechnung", "Leistung"]
tags: ["ap1", "berechnung", "energie"]

# Flashcard payload
card:
  type: steps
  question: "Berechne die jährlichen Energiekosten einer IT-Ausstattung bei einem Strompreis von 0,30 €/kWh: 20 Arbeitsstationen à 120 W laufen 8 h pro Arbeitstag an 220 Tagen, 4 Drucker à 50 W laufen 8 h pro Arbeitstag an 220 Tagen und 2 Server à 500 W laufen 24/7."
  answer: |
    Arbeitsstationen:
    20 × 120 W = 2.400 W = 2,4 kW
    2,4 kW × 8 h × 220 Tage = 4.224 kWh

    Drucker:
    4 × 50 W = 200 W = 0,2 kW
    0,2 kW × 8 h × 220 Tage = 352 kWh

    Server:
    2 × 500 W = 1.000 W = 1 kW
    1 kW × 24 h × 365 Tage = 8.760 kWh

    Gesamtverbrauch:
    4.224 kWh + 352 kWh + 8.760 kWh = 13.336 kWh

    Energiekosten:
    13.336 kWh × 0,30 €/kWh = 4.000,80 €

    Ergebnis: Die jährlichen Energiekosten betragen 4.000,80 €.
  examples:
    - "Watt in Kilowatt umrechnen: W ÷ 1.000 = kW"
    - "Verbrauch berechnen: kW × Betriebsstunden = kWh"
    - "Kosten berechnen: kWh × €/kWh = €"
    - "24/7-Betrieb: 24 × 365 = 8.760 Stunden pro Jahr"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Energiekosten von IT-Ausstattung berechnen
Die Energiekosten von IT-Systemen werden berechnet aus:
- **Leistung (Watt)**
- **Betriebszeit (Stunden)**
- **Strompreis (€/kWh)**

Ziel: Gesamtverbrauch (kWh) → Kosten berechnen

## Kernerklärung

### Gegeben:
- 25 Arbeitsstationen: 300 W, 9 h/Tag, 206 Tage
- 3 Drucker: 200 W, 24 h/Tag, 365 Tage
- 2 Server: 500 W, fast durchgehend (−10 h Wartung/Jahr)
- Strompreis: **0,30 €/kWh**

### Berechnung

| Gerät            | Verbrauch (kWh/Jahr) |
|------------------|----------------------|
| Arbeitsstationen | 13.905 kWh           |
| Drucker          | 5.256 kWh            |
| Server           | 8.750 kWh            |
| **Gesamt**       | **27.911 kWh**       |

### Kosten
- 27.911 kWh × 0,30 € = **8.373,30 €**

## Praktisches Beispiel
Ein Unternehmen möchte seine Stromkosten senken:
- Austausch alter PCs → weniger Watt
- Server virtualisieren → weniger Geräte

➡️ Ergebnis: geringerer Energieverbrauch → niedrigere Kosten

```mermaid
flowchart LR
A[Leistung in Watt] --> B[Betriebszeit]
B --> C[Energieverbrauch kWh]
C --> D[Kosten €]
```

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Wie berechnet man kWh aus Watt?
- Wie berechnet man Energiekosten?
- Welche Faktoren beeinflussen den Verbrauch?

### Antworten auf die typischen Prüfungsfragen
- kWh = (Watt × Stunden) / 1000
- Kosten = kWh × Preis pro kWh
- Anzahl Geräte, Leistung, Laufzeit

## Merksatz
**Energiekosten = Leistung × Zeit × Preis – je länger und stärker ein Gerät läuft, desto teurer wird es.**