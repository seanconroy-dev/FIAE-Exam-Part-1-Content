---
# Identity (stable; never change after publishing)
id: ap1-0170
slug: usv-klassen

# Display
title: "USV-Klassen nach IEC 62040-3"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["Hardware", "Stromversorgung", "Rechenzentrum"]
tags: ["prüfungsrelevant", "definition"]

# Flashcard payload
card:
  type: multi
  question: "Welche drei USV-Klassen gibt es nach IEC 62040-3?"
  answer: |
    - **VFD (Voltage and Frequency Dependent)**: Spannung und Frequenz hängen vom Stromnetz ab. Bei Stromausfall wird auf Batterie umgeschaltet. Das ist die einfache Offline-USV.
    - **VI (Voltage Independent)**: Die Ausgangsspannung wird stabilisiert, die Frequenz bleibt aber vom Stromnetz abhängig. Das entspricht meist einer Line-Interactive-USV.
    - **VFI (Voltage and Frequency Independent)**: Ausgangsspannung und Frequenz sind unabhängig vom Stromnetz. Das ist die Online-USV mit dem höchsten Schutz.
  examples:
    - "VFD → einfache Offline-USV für einzelne PCs"
    - "VI → Line-Interactive-USV für kleine Server oder Netzwerkschränke"
    - "VFI → Online-USV für Serverräume oder Rechenzentren"
    - "Merksatz: Je mehr Buchstaben unabhängig sind, desto höher der Schutz"

# Lifecycle
status: published
created: "2026-03-12"
updated: "2026-05-06"
---

## USV-Klassen nach IEC 62040-3

Eine **Unterbrechungsfreie Stromversorgung (USV)** schützt IT-Systeme vor Problemen in der Stromversorgung, z. B.:

- Stromausfall  
- Unterspannung  
- Überspannung  
- Spannungsschwankungen  

Nach der **Norm IEC 62040-3** werden USV-Systeme in **drei Klassen** eingeteilt.

---

## Die drei USV-Klassen

| Klasse | Bedeutung | Eigenschaften |
|---|---|---|
| **VFI** | Voltage and Frequency Independent | Ausgangsspannung und Frequenz vollständig vom Stromnetz entkoppelt |
| **VI** | Voltage Independent | Spannung wird geregelt, Frequenz bleibt abhängig vom Netz |
| **VFD** | Voltage and Frequency Dependent | Spannung und Frequenz folgen dem Netz |

---

## Funktionsprinzip

```mermaid
flowchart LR
A[Stromnetz] --> B[USV-System]
B --> C[IT-Systeme / Server]
B --> D[Batterie]
```

Bei einem **Stromausfall** übernimmt die **Batterie der USV** kurzfristig die Versorgung der angeschlossenen Geräte.

---

## Unterschiede im Detail

### Klasse 1 – VFI (Online-USV)

- vollständige Entkopplung vom Stromnetz  
- schützt vor:
  - Stromausfall
  - Unterspannung
  - Überspannung
  - Frequenzschwankungen
  - Oberschwingungen  
- höchste Schutzklasse  
- typischer Einsatz: **Rechenzentren**

---

### Klasse 2 – VI (Line-Interactive)

- schützt vor:
  - Stromausfall
  - Unterspannung
  - Überspannung  
- Spannung wird stabilisiert  
- Frequenz bleibt abhängig vom Netz  
- Einsatz: **Serverräume, Netzwerkschränke**

---

### Klasse 3 – VFD (Offline-USV)

- grundlegender Schutz vor Stromausfall  
- Umschaltzeit bis etwa **10 ms**  
- Spannung und Frequenz abhängig vom Stromnetz  
- Einsatz: **Einzel-PCs, Arbeitsplätze**

---

## Prüfungsrelevanz (AP1)

Typische Prüfungsfragen:

- **USV-Klassen nennen**
- Unterschiede zwischen **VFI, VI und VFD**
- Einsatzbereiche der verschiedenen USV-Typen

**Merksatz**

> Je unabhängiger eine USV vom Stromnetz arbeitet, desto höher ist die Schutzklasse.

---