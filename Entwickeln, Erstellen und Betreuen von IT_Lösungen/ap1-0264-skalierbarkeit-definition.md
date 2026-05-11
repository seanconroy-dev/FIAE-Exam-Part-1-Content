---
# Identity (stable; never change after publishing)
id: ap1-0264
slug: skalierbarkeit-definition

# Display
title: "Skalierbarkeit – Bedeutung im Rechenzentrum"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Rechenzentrum", "Infrastruktur", "Betrieb"]
tags: ["ap1", "skalierbarkeit", "cloud", "infrastruktur"]

# Flashcard payload
card:
  type: definition
  question: "Was bedeutet Skalierbarkeit im Rechenzentrumsbetrieb?"
  answer: "Skalierbarkeit bedeutet, dass ein IT-System bei steigender Last erweitert werden kann. Dafür können z. B. mehr CPU, RAM, Speicherplatz oder zusätzliche Server bereitgestellt werden."
  examples:
    - "Mehr RAM oder CPU für eine virtuelle Maschine"
    - "Mehr Speicherplatz für einen Dateiserver"
    - "Zusätzliche Server bei steigenden Nutzerzahlen"
    - "Cloud-Systeme können Ressourcen flexibel erhöhen"
    - "Merksatz: Skalierbarkeit = System kann mitwachsen"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Skalierbarkeit – Bedeutung im Rechenzentrum
Skalierbarkeit beschreibt die Fähigkeit eines Systems, sich **flexibel an steigende oder sinkende Anforderungen anzupassen**, ohne die Funktionalität zu verlieren.

## Kernerklärung

- System bleibt **funktionsfähig bei Laständerung**  
- Anpassung erfolgt durch:
  - mehr CPU-Leistung  
  - mehr Arbeitsspeicher  
  - mehr Speicherplatz  

- Ziel:
  - stabiler **24/7-Betrieb**  
  - bedarfsgerechte Ressourcennutzung  

### Arten der Skalierung

| Art                | Beschreibung                              |
|--------------------|------------------------------------------|
| Vertikal (Scale-Up)| mehr Leistung für ein System              |
| Horizontal         | mehrere Systeme parallel einsetzen        |

```mermaid
flowchart LR
A[Last steigt] --> B[Ressourcen erhöhen]
B --> C[System bleibt stabil]
```

## Praktisches Beispiel

- Virtuelle Maschine:
  - mehr RAM oder CPU-Kerne zuweisen  

- Storage:
  - Speicherplatz dynamisch erweitern  

- Cloud:
  - automatische Skalierung je nach Nutzung  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was bedeutet Skalierbarkeit?  
- Nenne Beispiele für Skalierung  
- Unterschied vertikal vs. horizontal  

### Antworten auf die typischen Prüfungsfragen
- Anpassungsfähigkeit bei Laständerung  
- CPU/RAM erhöhen, Systeme hinzufügen  
- vertikal = stärker, horizontal = mehr Systeme  

## Merksatz
Skalierbarkeit bedeutet: Leistung flexibel anpassen, ohne dass das System ausfällt.