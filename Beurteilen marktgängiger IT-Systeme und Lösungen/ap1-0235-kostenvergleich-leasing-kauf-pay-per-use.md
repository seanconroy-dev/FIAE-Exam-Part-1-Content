---
# Identity (stable; never change after publishing)
id: ap1-0235
slug: kostenvergleich-leasing-kauf-pay-per-use

# Display
title: "Kostenvergleich: Leasing vs. Kauf vs. Pay-per-use"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["Kostenvergleich", "Cloud", "Betriebsmodelle"]
tags: ["ap1", "leasing", "cloud", "kosten"]

# Flashcard payload
card:
  type: steps
  question: "Vergleiche Leasing, Kauf und Pay-per-use über 3 Jahre: Leasing kostet 4.333,33 € pro Monat, Kauf kostet 100.000 € Anschaffung plus 30.000 € Service, Pay-per-use kostet 3,22 € pro Stunde bei 24/7-Betrieb. Welche Option ist am günstigsten?"
  answer: |
    Leasing:
    4.333,33 € × 36 Monate = 155.999,88 € ≈ 156.000 €

    Kauf:
    100.000 € + 30.000 € Service = 130.000 €

    Pay-per-use:
    3 Jahre × 365 Tage × 24 h = 26.280 h
    26.280 h × 3,22 €/h = 84.621,60 €

    Ergebnis:
    Pay-per-use ist mit 84.621,60 € am günstigsten, danach Kauf mit 130.000 €, am teuersten ist Leasing mit ca. 156.000 €.
  examples:
    - "Leasing: monatliche Rate × 36 Monate"
    - "Kauf: Anschaffungskosten + Servicekosten"
    - "Pay-per-use: Stunden × Preis pro Stunde"
    - "24/7 über 3 Jahre: 3 × 365 × 24 = 26.280 Stunden"
    - "Reihenfolge: Pay-per-use < Kauf < Leasing"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Kostenvergleich: Leasing vs. Kauf vs. Pay-per-use
Beim Vergleich von IT-Betriebsmodellen werden die Gesamtkosten über einen Zeitraum (hier: **3 Jahre**) betrachtet.

➡️ Drei typische Modelle:
- Leasing  
- Kauf (On-Premises)  
- Pay-per-use (Cloud)  

## Kernerklärung

### Kostenübersicht (3 Jahre)

| Modell        | Berechnung | Gesamtkosten |
|--------------|-----------|-------------|
| **Leasing**  | 36 × 4.333,33 € | **155.999,88 €** ≈ 156.000 € |
| **Kauf**     | 100.000 € + 30.000 € Service | **130.000 €** |
| **Pay-per-use** | 3,22 €/h × 24 h × 365 d × 3 Jahre | **84.621,60 €** |

### Rangfolge

1. **Pay-per-use (günstigstes Modell)**  
2. **Kauf**  
3. **Leasing (teuerstes Modell)**  

```mermaid
flowchart LR
A[Pay-per-use<br>~84k €] --> B[Kauf<br>~130k €]
B --> C[Leasing<br>~156k €]
```

## Praktisches Beispiel

Ein Unternehmen benötigt Serverleistung:

- **Leasing:** monatliche Fixkosten  
- **Kauf:** hohe Anfangsinvestition  
- **Cloud:** nutzungsabhängige Kosten  

➡️ Bei dauerhafter Nutzung kann Kauf sinnvoll sein,  
➡️ bei flexibler Nutzung ist Pay-per-use oft günstiger  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Welche Variante ist am günstigsten?
- Wie berechnet man Pay-per-use?
- Wann lohnt sich Kauf vs. Cloud?

### Antworten auf die typischen Prüfungsfragen
- Pay-per-use ist am günstigsten  
- Preis pro Stunde × Nutzungszeit  
- Kauf bei dauerhafter Nutzung, Cloud bei Flexibilität  

## Merksatz
**Je flexibler die Nutzung, desto sinnvoller Pay-per-use – je konstanter, desto eher Kauf.**