---
# Identity (stable; never change after publishing)
id: ap1-0205
slug: unterschied-switch-router

# Display
title: "Switch vs. Router – Unterschiede"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["switch", "router", "osi-modell"]
tags: ["netzwerkgeraete", "osi", "routing", "switching"]

# Flashcard payload
card:
  type: comparison
  question: "Was ist der Unterschied zwischen einem Switch und einem Router?"
  answer: "Ein Switch arbeitet hauptsächlich auf OSI-Schicht 2 und leitet Frames innerhalb eines lokalen Netzwerks anhand von MAC-Adressen weiter. Ein Router arbeitet auf OSI-Schicht 3, verbindet verschiedene Netzwerke und leitet Pakete anhand von IP-Adressen weiter."
  examples:
    - "Switch → verbindet Geräte innerhalb eines LANs"
    - "Switch → nutzt MAC-Adressen zur Weiterleitung"
    - "Router → verbindet verschiedene Netzwerke oder Subnetze"
    - "Router → nutzt IP-Adressen und Routing-Tabellen"
    - "Beispiel: Switch verbindet PCs im Büro, Router verbindet das Büro-LAN mit dem Internet"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## Unterschied Switch vs. Router

Switches und Router sind zentrale Netzwerkgeräte mit unterschiedlichen Aufgaben:

- **Switch** → verbindet Geräte innerhalb eines Netzwerks  
- **Router** → verbindet verschiedene Netzwerke  

---

## Kernerklärung

### Vergleich Switch vs. Router

| Merkmal | Switch | Router |
|---|---|---|
| OSI-Schicht | Schicht 2 (Data Link) | Schicht 3 (Network) |
| Verarbeitung | Ethernet-Frames (IEEE 802.3) | IP-Pakete |
| Adressierung | MAC-Adresse | IP-Adresse |
| Aufgabe | Weiterleitung im gleichen Netzwerk | Verbindung zwischen Netzwerken |
| Protokolle | keine Routingprotokolle | z. B. OSPF, RIP, BGP |

### Funktionsprinzip

```mermaid
flowchart LR
A[PC 1] --> Switch
Switch --> B[PC 2]

Switch --> Router
Router --> Internet
```

- Switch: interne Kommunikation  
- Router: externe Kommunikation  

---

## Praktisches Beispiel

- Büro-Netzwerk:
  - PCs sind über einen **Switch** verbunden  
  - Internetzugang erfolgt über einen **Router**  

---

## Prüfungsrelevanz (AP1)

Sehr häufig:

- OSI-Schichten zuordnen
- Unterschied MAC vs. IP verstehen
- Aufgaben von Switch und Router erklären

---

### Typische Prüfungsfragen

- Auf welcher OSI-Schicht arbeitet ein Switch?
- Welche Adresse nutzt ein Router?
- Wofür wird ein Router eingesetzt?

---

### Antworten auf die typischen Prüfungsfragen

**Switch-Schicht?**  
→ Layer 2  

**Router-Adresse?**  
→ IP-Adresse  

**Aufgabe Router?**  
→ verbindet Netzwerke  

---

## Merksatz

**Switch verbindet Geräte – Router verbindet Netzwerke.**