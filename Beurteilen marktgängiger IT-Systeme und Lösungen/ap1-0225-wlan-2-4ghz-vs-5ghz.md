---
# Identity (stable; never change after publishing)
id: ap1-0225
slug: wlan-2-4ghz-vs-5ghz

# Display
title: "WLAN: Unterschiede zwischen 2,4 GHz und 5 GHz"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["WLAN", "Funktechnik", "Frequenzen"]
tags: ["ap1", "wlan", "vergleich"]

# Flashcard payload
card:
  type: basic
  question: "Was sind die Vor- und Nachteile beim Einsatz eines 2,4-GHz- sowie eines 5-GHz-WLANs?"
  answer: "2,4 GHz bietet eine größere Reichweite und durchdringt Hindernisse besser, ist aber langsamer und störanfälliger, da viele Geräte diesen Frequenzbereich nutzen. 5 GHz bietet höhere Datenraten und meist weniger Störungen, hat aber eine geringere Reichweite und wird stärker durch Wände oder Hindernisse gedämpft."
  examples:
    - "2,4 GHz → größere Reichweite, besser durch Wände"
    - "2,4 GHz → störanfälliger durch Bluetooth, Mikrowellen oder Nachbar-WLANs"
    - "5 GHz → höhere Geschwindigkeit und weniger Überlappung"
    - "5 GHz → kürzere Reichweite und stärkere Dämpfung"
    - "2,4 GHz eher für Reichweite, 5 GHz eher für Geschwindigkeit"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## WLAN: Unterschiede zwischen 2,4 GHz und 5 GHz

WLAN (Wireless Local Area Network) nutzt hauptsächlich zwei Frequenzbereiche:

- **2,4 GHz**
- **5 GHz**


Beide haben unterschiedliche Eigenschaften hinsichtlich **Reichweite, Geschwindigkeit und Störanfälligkeit**.

## Kernerklärung

### Vergleich der Frequenzbänder

| Eigenschaft        | 2,4 GHz                         | 5 GHz                          |
|------------------|----------------------------------|--------------------------------|
| Reichweite        | hoch (bis ~300 m außen)         | geringer                       |
| Durchdringung     | gut (Wände etc.)                | schlechter                     |
| Geschwindigkeit   | geringer (bis ~600 Mbit/s)      | höher                          |
| Störungen         | hoch (viele Geräte)             | geringer                       |
| Kanäle            | wenige, überlappend             | mehr, nicht überlappend        |
| Verbreitung       | sehr hoch                       | geringer                       |

### 2,4 GHz – Vorteile
- Große Reichweite
- Gute Durchdringung von Hindernissen
- Weit verbreitet

### 2,4 GHz – Nachteile
- Störanfällig (z. B. durch andere Geräte)
- Channel Overlapping (nur wenige nutzbare Kanäle)
- Geringere Datenrate

### 5 GHz – Vorteile
- Höhere Datenraten
- Weniger Störungen
- Keine Kanalüberlappung

### 5 GHz – Nachteile
- Geringere Reichweite
- Schlechtere Durchdringung von Wänden
- Einschränkungen (z. B. DFS/TPC)

```mermaid
flowchart LR
A[WLAN Frequenz] --> B[2,4 GHz]
A --> C[5 GHz]
B --> D[Hohe Reichweite]
B --> E[Mehr Störungen]
C --> F[Hohe Geschwindigkeit]
C --> G[Geringere Reichweite]
```

## Praktisches Beispiel
- **2,4 GHz**: Einsatz in großen Gebäuden mit vielen Wänden  
- **5 GHz**: Einsatz in Büros mit hoher Datenlast (z. B. Video, große Datenmengen)

➡️ Moderne Netzwerke nutzen oft **beide Frequenzen parallel (Dual-Band)**

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Unterschiede zwischen 2,4 GHz und 5 GHz?
- Warum ist 2,4 GHz störanfälliger?
- Wann nutzt man 5 GHz?

### Antworten auf die typischen Prüfungsfragen
- 2,4 GHz = Reichweite / 5 GHz = Geschwindigkeit
- Viele Geräte nutzen 2,4 GHz → mehr Interferenzen
- 5 GHz bei hoher Bandbreite und geringeren Störungen

## Merksatz
**2,4 GHz = Reichweite, 5 GHz = Geschwindigkeit.**