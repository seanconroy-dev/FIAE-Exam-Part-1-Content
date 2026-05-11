---
# Identity (stable; never change after publishing)
id: ap1-0269
slug: vpn-definition

# Display
title: "VPN – Virtual Private Network"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "VPN", "Sicherheit"]
tags: ["ap1", "vpn", "netzwerk", "sicherheit"]

# Flashcard payload
card:
  type: definition
  question: "Was ist ein VPN?"
  answer: "Ein VPN ist ein virtuelles privates Netzwerk. Es stellt über ein öffentliches Netzwerk, z. B. das Internet, eine sichere und verschlüsselte Verbindung her. Dadurch können Benutzer oder Standorte geschützt auf ein privates Netzwerk zugreifen."
  examples:
    - "Homeoffice: Zugriff auf das Firmennetz über das Internet"
    - "Standortverbindung: zwei Firmenstandorte werden sicher verbunden"
    - "Öffentliches WLAN: Verbindung wird zusätzlich verschlüsselt"
    - "Remote Access: Mitarbeiter verbindet sich von außen mit dem Unternehmen"
    - "Merksatz: VPN = verschlüsselter Tunnel durch ein öffentliches Netz"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## VPN – Virtual Private Network
Ein VPN (Virtual Private Network) ermöglicht es, **private Netzwerke sicher über öffentliche Netzwerke** wie das Internet zu verbinden.

## Kernerklärung

- VPN = **logisches (virtuelles) Netzwerk**
- nutzt:
  - öffentliche Netzwerke (z. B. Internet)

- Ziele:
  - **Vertraulichkeit** (Verschlüsselung)
  - **Integrität** (keine Manipulation)
  - **Authentizität** (echte Teilnehmer)

- Umsetzung durch:
  - Tunnel-Technologien  
  - Verschlüsselungsprotokolle  

- Beispiele für Protokolle:
  - IPsec  
  - SSL/TLS  
  - OpenVPN  
  - L2TP  

```mermaid
flowchart LR
A[Client] -->|verschlüsselte Verbindung| B[Internet]
B --> C[Firmennetz]
```

## Praktisches Beispiel

- Homeoffice:
  - Mitarbeiter greift sicher auf Firmennetz zu  

- Standortvernetzung:
  - zwei Firmenstandorte werden verbunden  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist ein VPN?  
- Welche Ziele hat ein VPN?  
- Nenne typische Protokolle  

### Antworten auf die typischen Prüfungsfragen
- sicheres virtuelles Netzwerk über öffentliche Netze  
- Vertraulichkeit, Integrität, Authentizität  
- IPsec, SSL/TLS, OpenVPN, L2TP  

## Merksatz
Ein VPN macht aus dem Internet ein sicheres privates Netzwerk.