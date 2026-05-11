---
# Identity (stable; never change after publishing)
id: ap1-0218
slug: maximale-leistung-steckdose-berechnen

# Display
title: "Maximale Leistung einer Steckdose berechnen"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["elektrotechnik", "leistung"]
tags: ["leistung", "spannung", "strom", "berechnung"]

# Flashcard payload
card:
  type: basic
  question: "Wie berechnet man die maximale Leistung einer Steckdose mit 230 V Spannung und 16 A Absicherung?"
  answer: |
    Die maximale Leistung wird mit folgender Formel berechnet:

    P = U × I

    P = Leistung in Watt (W)
    U = Spannung in Volt (V)
    I = Stromstärke in Ampere (A)

    Beispiel:
    230 V × 16 A = 3.680 W

    Umrechnung in Kilowatt:
    3.680 W ÷ 1.000 = 3,68 kW

    Ergebnis: Eine Steckdose mit 230 V und 16 A kann maximal etwa 3.680 W bzw. 3,68 kW liefern.
  examples:
    - "Formel: P = U × I"
    - "230 V × 16 A = 3.680 W"
    - "3.680 W = 3,68 kW"
    - "Merksatz: Volt mal Ampere ergibt Watt"

# Lifecycle
status: published
created: "2026-03-18"
updated: "2026-05-11"
---

## Maximale Leistung einer Steckdose berechnen

Die maximale Leistung einer Steckdose ergibt sich aus:

- **Spannung (U)** und  
- **Stromstärke (I)**  

👉 Grundlage: **P = U · I**

Typischer Wert in Deutschland:

- 230 Volt  
- 16 Ampere  

---

## Kernerklärung

Formel:

- **P = U · I**

Einsetzen:

- **P = 230 V × 16 A = 3.680 W**
- entspricht **3,68 kW**

👉 Bedeutung:

- Das ist die **maximale Dauerleistung**, die eine Steckdose liefern kann  
- Wird sie überschritten → **Überlast / Sicherung fliegt**

---

### Zusammenhang

```mermaid
flowchart LR
U[Spannung 230V] --> P[Leistung 3680W]
I[Strom 16A] --> P
```

---

## Praktisches Beispiel

Mehrfachsteckdose:

- angeschlossene Geräte:
  - PC: 500 W  
  - Monitor: 100 W  
  - Drucker: 300 W  

→ Gesamt:

- **900 W** → unkritisch  

Aber:

- Heizlüfter (2000 W) + weitere Geräte → schnell nahe Grenze  

---

## Prüfungsrelevanz (AP1)

Wichtig:

- Standardwerte kennen: **230 V / 16 A**  
- Formel sicher anwenden  
- Ergebnis in **Watt und kW** angeben können  

---

### Typische Prüfungsfragen

- Wie hoch ist die maximale Leistung einer Steckdose?
- Welche Formel wird verwendet?
- Was passiert bei Überlast?

---

### Antworten auf die typischen Prüfungsfragen

**Maximale Leistung?**  
→ 3.680 W (3,68 kW)  

**Formel?**  
→ P = U · I  

**Überlast?**  
→ Sicherung löst aus  

---

## Merksatz

**230 V × 16 A = 3.680 W → maximale Steckdosenleistung.**