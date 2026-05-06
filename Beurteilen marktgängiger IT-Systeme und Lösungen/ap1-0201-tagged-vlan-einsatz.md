---
# Identity (stable; never change after publishing)
id: ap1-0201
slug: tagged-vlan-einsatz

# Display
title: "Tagged VLAN – Einsatz"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["vlan", "switching"]
tags: ["vlan", "tagging", "trunk"]

# Flashcard payload
card:
  type: basic
  question: "In welchen Situationen wird ein tagged VLAN (Virtual Local Area Network) eingesetzt?"
  answer: "Ein tagged VLAN wird eingesetzt, wenn mehrere VLANs über eine gemeinsame Netzwerkverbindung übertragen werden sollen, zum Beispiel über einen Trunk-Port zwischen Switches. Dabei erhalten Ethernet-Frames ein VLAN-Tag, damit die Zugehörigkeit zum jeweiligen VLAN erkannt wird."
  examples:
    - "Trunk-Verbindung zwischen zwei Switches"
    - "Verbindung zwischen Switch und Router bei Router-on-a-Stick"
    - "Verbindung zwischen Switch und Virtualisierungsserver mit mehreren VLANs"
    - "Ein Kabel transportiert mehrere VLANs gleichzeitig"
    - "VLAN-Tag kennzeichnet, zu welchem VLAN ein Frame gehört"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## Tagged VLAN – Einsatz

Ein **tagged VLAN** wird verwendet, um **mehrere VLANs über eine einzige physische Verbindung** zu übertragen.

Typischer Einsatz:
- Verbindung zwischen Switches
- Trunk-Ports

---

## Kernerklärung

Beim tagged VLAN:

- Ethernet-Frames erhalten ein **VLAN-Tag**
- Dieses Tag enthält:
  - VLAN-ID
- Dadurch können mehrere VLANs gleichzeitig übertragen werden

### Wann notwendig?

- Wenn sich VLANs über **mehrere Switches erstrecken**
- Wenn eine Leitung **mehrere Netzwerke transportieren soll**

### Funktionsweise

| Schritt | Beschreibung |
|---|---|
| 1 | Frame wird mit VLAN-ID versehen |
| 2 | Übertragung über Trunk-Port |
| 3 | Ziel-Switch wertet Tag aus |
| 4 | Weiterleitung ins richtige VLAN |

```mermaid
flowchart LR
A[Switch 1] -->|Trunk + VLAN Tags| B[Switch 2]
B --> C[VLAN-Zuordnung]
```

---

## Praktisches Beispiel

Ein Unternehmen hat:

- VLAN 10 → Verwaltung  
- VLAN 20 → IT  

Zwischen zwei Switches:

- nur **ein Kabel**
- beide VLANs laufen darüber
- → Frames werden **getaggt**, damit sie korrekt zugeordnet werden

---

## Prüfungsrelevanz (AP1)

Wichtige Punkte:

- Unterschied **tagged vs. untagged**
- Begriff **Trunk-Port**
- Zweck von VLAN-Tags

---

### Typische Prüfungsfragen

- Wann braucht man tagged VLANs?
- Was ist ein Trunk-Port?
- Wozu dient das VLAN-Tag?

---

### Antworten auf die typischen Prüfungsfragen

**Wann tagged VLAN?**  
→ bei mehreren VLANs über eine Verbindung

**Was ist ein Trunk-Port?**  
→ Port für mehrere VLANs gleichzeitig

**Wozu das Tag?**  
→ Kennzeichnung der VLAN-Zugehörigkeit

---

## Merksatz

**Tagged VLAN = mehrere VLANs über ein Kabel dank Kennzeichnung (Tag).**