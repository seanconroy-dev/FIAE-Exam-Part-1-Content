---
# Identity (stable; never change after publishing)
id: ap1-0268
slug: vpn-verbindungsarten

# Display
title: "VPN-Verbindungsarten"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "VPN", "Sicherheit"]
tags: ["ap1", "vpn", "netzwerk", "sicherheit"]

# Flashcard payload
card:
  type: multi
  question: "Welche 3 VPN-Verbindungsarten gibt es?"
  answer: "Die drei typischen VPN-Verbindungsarten sind End-to-Site, Site-to-Site und End-to-End. End-to-Site verbindet ein einzelnes Endgerät mit einem Firmennetz. Site-to-Site verbindet zwei Netzwerke oder Standorte miteinander. End-to-End verbindet zwei einzelne Endgeräte direkt miteinander."
  examples:
    - "End-to-Site: Mitarbeiter greift aus dem Homeoffice auf das Firmennetz zu"
    - "End-to-Site: auch Remote-Access-VPN oder Host-to-LAN genannt"
    - "Site-to-Site: zwei Firmenstandorte werden per VPN verbunden"
    - "Site-to-Site: auch LAN-to-LAN oder Gateway-to-Gateway genannt"
    - "End-to-End: zwei einzelne Rechner kommunizieren direkt verschlüsselt"
    - "End-to-End: auch Host-to-Host genannt"
    - "Merksatz: End-to-Site = Gerät zu Netz, Site-to-Site = Netz zu Netz, End-to-End = Gerät zu Gerät"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## VPN-Verbindungsarten
VPN (Virtual Private Network) ermöglicht eine **sichere Verbindung über unsichere Netzwerke** wie das Internet.

Es gibt drei grundlegende Verbindungsarten.

## Kernerklärung

### 1. End-to-Site (Remote Access VPN)
- Verbindung:
  - einzelner Client → Netzwerk (LAN)
- auch genannt:
  - Host-to-LAN  
  - Host-to-Gateway  

- Einsatz:
  - Homeoffice  
  - mobiler Zugriff  

---

### 2. Site-to-Site VPN
- Verbindung:
  - Netzwerk → Netzwerk  
- auch genannt:
  - LAN-to-LAN  
  - Gateway-to-Gateway  

- Einsatz:
  - Verbindung von Firmenstandorten  

---

### 3. End-to-End VPN
- Verbindung:
  - einzelner Host → einzelner Host  
- auch genannt:
  - Host-to-Host  
  - Remote-Desktop-VPN  

- Einsatz:
  - direkte, gesicherte Kommunikation zwischen zwei Geräten  

```mermaid
flowchart LR
A[Client] -->|End-to-Site| B[Firmennetz]
B -->|Site-to-Site| C[anderes Firmennetz]
A -->|End-to-End| D[anderer Client]
```

## Praktisches Beispiel

- End-to-Site:
  - Mitarbeiter verbindet sich von zuhause ins Firmennetz  

- Site-to-Site:
  - Hauptstandort ↔ Außenstelle  

- End-to-End:
  - sichere Verbindung zwischen zwei Rechnern  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Nenne die 3 VPN-Arten  
- Unterschied zwischen Site-to-Site und Remote Access  
- Wo wird welche Art eingesetzt?  

### Antworten auf die typischen Prüfungsfragen
- End-to-Site, Site-to-Site, End-to-End  
- Site-to-Site = Netzwerke, Remote = einzelner Nutzer  
- Homeoffice vs. Standortvernetzung  

## Merksatz
VPN verbindet entweder Nutzer, Netzwerke oder einzelne Geräte sicher über das Internet.