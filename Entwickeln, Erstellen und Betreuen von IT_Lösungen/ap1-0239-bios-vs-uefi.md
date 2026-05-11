---
# Identity (stable; never change after publishing)
id: ap1-0239
slug: bios-vs-uefi

# Display
title: "BIOS vs. UEFI – Vergleich"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Hardware", "Systemstart", "Firmware"]
tags: ["ap1", "bios", "uefi"]

# Flashcard payload
card:
  type: comparison
  question: "Worin unterscheiden sich BIOS und UEFI?"
  answer: "BIOS ist die ältere Firmware-Schnittstelle zum Starten eines Computers und arbeitet meist mit MBR-Partitionierung. UEFI ist der moderne Nachfolger, unterstützt grafische Oberflächen, Mausbedienung, GPT-Partitionierung, Secure Boot und das Booten von großen Laufwerken über 2 TB. BIOS ist einfacher und stärker eingeschränkt, UEFI bietet mehr Funktionen und bessere Unterstützung moderner Hardware."
  examples:
    - "BIOS → älteres Startsystem, häufig mit MBR"
    - "UEFI → moderner Nachfolger von BIOS"
    - "UEFI unterstützt GPT und große Laufwerke über 2 TB"
    - "UEFI kann Secure Boot unterstützen"
    - "Neue PCs nutzen meist UEFI"
    - "Merksatz: BIOS = alt/MBR, UEFI = modern/GPT/Secure Boot"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## BIOS vs. UEFI – Vergleich
BIOS und UEFI sind Firmware-Systeme, die den Start eines Computers steuern.

- BIOS = älteres System  
- UEFI = moderner Nachfolger  

## Kernerklärung

### Vergleich BIOS vs. UEFI

| Merkmal | BIOS | UEFI |
|--------|------|------|
| Bedienung | Tastatur | Maus + grafisch |
| Bootverfahren | MBR | GPT |
| Maximale Laufwerksgröße | bis 2 TB | > 2 TB |
| Architektur | 16-Bit | 32-/64-Bit |
| Erweiterbarkeit | eingeschränkt | modular (Treiber nachladbar) |
| Zusatzfunktionen | kaum | Netzwerk, VM-Start möglich |

### Eigenschaften im Detail

**BIOS:**
- keine Mausbedienung möglich  
- startet über Master Boot Record (MBR)  
- begrenzt auf Laufwerke bis 2 TB  

**UEFI:**
- grafische Benutzeroberfläche  
- Mausbedienung möglich  
- unterstützt große Laufwerke (> 2 TB)  
- nutzt GPT-Partitionsschema  
- 64-Bit-Unterstützung ab Werk  
- Treiber modular nachladbar  

```mermaid
flowchart LR
A[BIOS] -->|alt| B[UEFI]
B -->|modern| C[Mehr Funktionen]
```

## Praktisches Beispiel

- Alter PC mit BIOS:
  - Installation nur auf kleinen Festplatten möglich  
- Neuer PC mit UEFI:
  - große SSDs, schnellerer Start, moderne Features  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Unterschied BIOS und UEFI?
- Was ist GPT vs. MBR?
- Warum ist UEFI moderner?

### Antworten auf die typischen Prüfungsfragen
- UEFI bietet mehr Funktionen und unterstützt moderne Hardware  
- GPT erlaubt größere Laufwerke als MBR  
- UEFI ist flexibel und erweiterbar  

## Merksatz
BIOS ist alt und eingeschränkt, UEFI ist modern und leistungsfähig.