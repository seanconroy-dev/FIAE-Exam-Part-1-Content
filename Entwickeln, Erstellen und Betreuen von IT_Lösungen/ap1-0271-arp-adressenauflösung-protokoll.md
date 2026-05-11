---
# Identity (stable; never change after publishing)
id: ap1-0271
slug: arp-adressauflösung-protokoll

# Display
title: "ARP – Address Resolution Protocol"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "Protokolle", "OSI-Modell"]
tags: ["ap1", "arp", "netzwerk", "ip", "mac"]

# Flashcard payload
card:
  type: definition
  question: "Was zeigt der Befehl arp und wofür wird das ARP-Protokoll genutzt?"
  answer: "Der Befehl arp zeigt den ARP-Cache eines Geräts an. ARP steht für Address Resolution Protocol und ordnet in einem lokalen Netzwerk einer IPv4-Adresse die passende MAC-Adresse zu. Diese Zuordnung wird im ARP-Cache gespeichert."
  examples:
    - "arp -a: zeigt die gespeicherten IP-zu-MAC-Zuordnungen"
    - "ARP löst eine IPv4-Adresse in eine MAC-Adresse auf"
    - "Der ARP-Cache speichert bekannte Zuordnungen vorübergehend"
    - "Beispiel: 192.168.1.10 wird einer MAC-Adresse zugeordnet"
    - "Merksatz: ARP = IPv4-Adresse sucht MAC-Adresse"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## ARP – Address Resolution Protocol
Das **Address Resolution Protocol (ARP)** wird in Netzwerken verwendet, um **IP-Adressen in MAC-Adressen aufzulösen**.

## Kernerklärung

- ARP arbeitet zwischen:
  - **OSI-Schicht 3 (Netzwerk)** → IP-Adresse  
  - **OSI-Schicht 2 (Sicherung)** → MAC-Adresse  

- Funktion:
  1. Gerät kennt nur die IP-Adresse  
  2. ARP sendet Anfrage ins Netzwerk („Wer hat IP X?“)  
  3. Zielgerät antwortet mit seiner MAC-Adresse  
  4. Ergebnis wird im **ARP-Cache** gespeichert  

```mermaid
sequenceDiagram
    participant A as Client
    participant B as Zielgerät

    A->>Netzwerk: ARP Request (Wer hat IP?)
    B-->>A: ARP Reply (MAC-Adresse)
    A->>A: Speicherung im ARP-Cache
```

## Praktisches Beispiel

- Befehl:
  ```bash
  arp -a
  ```
- Ausgabe:
  - Liste aller bekannten IP ↔ MAC Zuordnungen  
- Nutzung:
  - Fehleranalyse im Netzwerk  
  - Überprüfung erreichbarer Geräte  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was macht ARP?  
- In welcher OSI-Schicht arbeitet ARP?  
- Was zeigt `arp -a` an?  

### Antworten auf die typischen Prüfungsfragen
- ARP löst IP-Adressen in MAC-Adressen auf  
- Zwischen Schicht 2 und 3  
- ARP-Tabelle (IP ↔ MAC Zuordnung)  

## Merksatz
ARP verbindet IP-Adresse und MAC-Adresse – ohne ARP keine Kommunikation im LAN.