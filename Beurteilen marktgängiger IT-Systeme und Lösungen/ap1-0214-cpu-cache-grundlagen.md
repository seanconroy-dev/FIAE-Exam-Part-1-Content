---
# Identity (stable; never change after publishing)
id: ap1-0214
slug: cpu-cache-grundlagen

# Display
title: "CPU-Cache – Grundlagen"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["cpu", "speicher"]
tags: ["cache", "l1", "l2", "l3"]

# Flashcard payload
card:
  type: definition
  question: "Was versteht man unter dem Begriff CPU-Cache?"
  answer: "Der CPU-Cache ist ein sehr schneller Zwischenspeicher direkt im oder nahe am Prozessor. Er speichert häufig benötigte Daten und Befehle, damit die CPU schneller darauf zugreifen kann als auf den Arbeitsspeicher. Typische Cache-Ebenen sind L1, L2 und L3."
  examples:
    - "L1-Cache → sehr klein, aber am schnellsten"
    - "L2-Cache → größer als L1, aber etwas langsamer"
    - "L3-Cache → meist größer, aber langsamer als L1 und L2"
    - "Cache reduziert Zugriffszeiten auf häufig benötigte Daten"
    - "Merksatz: Cache = schneller Zwischenspeicher für die CPU"
# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## CPU-Cache – Grundlagen

Der **CPU-Cache** ist ein extrem schneller Speicher im Prozessor:

- dient als **Zwischenspeicher**  
- verkürzt Zugriffszeiten auf Daten  
- entlastet den Arbeitsspeicher (RAM)  

---

## Kernerklärung

Der CPU-Cache speichert häufig benötigte Daten und Befehle direkt im Prozessor, sodass diese schneller verfügbar sind als aus dem RAM.

### Cache-Level

| Level | Eigenschaften |
|---|---|
| L1 | sehr schnell, sehr klein |
| L2 | langsamer als L1, größer |
| L3 | am langsamsten, aber am größten |

- **L1-Cache**:
  - schnellster Zugriff  
  - kleinste Kapazität  

- **L2-Cache**:
  - mittlere Geschwindigkeit  
  - größere Kapazität  

- **L3-Cache**:
  - größte Kapazität  
  - langsamster Cache (aber schneller als RAM)  

---

### Funktionsprinzip

```mermaid
flowchart LR
CPU --> L1
L1 --> L2
L2 --> L3
L3 --> RAM
RAM --> Speicher
```

- Daten werden zuerst im **L1** gesucht  
- dann **L2 → L3 → RAM**  
- Ziel: möglichst selten auf langsamen RAM zugreifen  

---

## Praktisches Beispiel

- Programm startet:
  - häufig genutzte Befehle landen im Cache  
- CPU greift schneller darauf zu → höhere Performance  

---

## Prüfungsrelevanz (AP1)

Wichtig:

- Definition des CPU-Caches  
- Unterschiede der Cache-Level (L1, L2, L3)  
- Zusammenhang mit Performance  

---

### Typische Prüfungsfragen

- Was ist der CPU-Cache?
- Warum verbessert er die Leistung?
- Welche Cache-Level gibt es?

---

### Antworten auf die typischen Prüfungsfragen

**Was ist das?**  
→ schneller Zwischenspeicher in der CPU  

**Warum schneller?**  
→ kürzere Zugriffszeiten als RAM  

**Welche Level?**  
→ L1 (schnell), L2 (mittel), L3 (groß)  

---

## Merksatz

**Je näher an der CPU, desto schneller – aber auch kleiner (L1 → L3).**