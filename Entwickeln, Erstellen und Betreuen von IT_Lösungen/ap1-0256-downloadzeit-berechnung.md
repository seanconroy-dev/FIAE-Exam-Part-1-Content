---
# Identity (stable; never change after publishing)
id: ap1-0256
slug: downloadzeit-berechnung

# Display
title: "Downloadzeit berechnen – Beispiel"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "Datenübertragung", "Berechnungen"]
tags: ["ap1", "download", "bandbreite", "rechnung"]

# Flashcard payload
card:
  type: steps
  question: "Wie berechnet man die Downloadzeit für eine 2 GiB große Datei bei einer Übertragungsgeschwindigkeit von 50 Mbit/s?"
  answer: "Die Datei zuerst von GiB in Bit umrechnen und dann durch die Übertragungsgeschwindigkeit teilen. 2 GiB = 2 × 1024³ Byte × 8 = 17.179.869.184 Bit. 17.179.869.184 Bit ÷ 50.000.000 Bit/s ≈ 344 Sekunden. Das sind etwa 5 Minuten und 44 Sekunden."
  examples:
    - "Formel: Zeit = Datenmenge ÷ Übertragungsgeschwindigkeit"
    - "1 Byte = 8 Bit"
    - "2 GiB = 17.179.869.184 Bit"
    - "50 Mbit/s = 50.000.000 Bit/s"
    - "17.179.869.184 ÷ 50.000.000 ≈ 344 Sekunden"
    - "344 Sekunden ≈ 5 Minuten und 44 Sekunden"
    - "Typischer Fehler: Mbit/s nicht mit MB/s verwechseln"
# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Downloadzeit berechnen – Beispiel
Die Downloadzeit ergibt sich aus:

- **Dateigröße (in Bit)**
- **Übertragungsrate (in Bit/s)**

Formel:
- Zeit = Datenmenge / Geschwindigkeit

## Kernerklärung

### Schrittweise Berechnung

1. **GiB → Byte**
   - 2 GiB × 1024 = 2048 MiB  
   - 2048 MiB × 1024 = 2.097.152 KiB  
   - 2.097.152 KiB × 1024 = 2.147.483.648 Byte  

2. **Byte → Bit**
   - 2.147.483.648 Byte × 8 = 17.179.869.184 Bit  

3. **Zeit berechnen**
   - 17.179.869.184 Bit / 50.000.000 Bit/s  
   = 343,6 Sekunden  

4. **Umrechnung in Minuten**
   - 343,6 s ≈ 5 Minuten 44 Sekunden  

```mermaid
flowchart LR
A[2 GiB] --> B[Byte]
B --> C[Bit]
C --> D[Division durch Bandbreite]
D --> E[Zeit in Sekunden]
E --> F[Minuten + Sekunden]
```

## Praktisches Beispiel

- Download einer großen Datei:
  - ISO-Image (z. B. Linux)  
  - Geschwindigkeit abhängig von Leitung  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Wie berechnet man Downloadzeiten?  
- Warum muss man in Bit umrechnen?  
- Welche Rolle spielt die Bandbreite?  

### Antworten auf die typischen Prüfungsfragen
- Zeit = Datenmenge / Bandbreite  
- weil Bandbreite in Bit/s angegeben ist  
- höhere Bandbreite → kürzere Zeit  

## Merksatz
Für Downloadzeiten immer: Daten in **Bit umrechnen** und durch **Bit/s teilen**.