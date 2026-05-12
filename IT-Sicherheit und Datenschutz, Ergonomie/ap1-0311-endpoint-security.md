---
# Identity (stable; never change after publishing)
id: ap1-0311
slug: "endpoint-security"

# Display
title: "Endpoint Security"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["netzwerksicherheit", "endpoint", "schutzmassnahmen"]
tags: ["ap1", "grundlagen", "sicherheit", "endgeraete"]

# Flashcard payload
card:
  type: definition
  question: "Was bedeutet Endpoint-Security?"
  answer: "Endpoint-Security umfasst Maßnahmen zum Schutz von Endgeräten, die mit einem Netzwerk verbunden sind. Dazu gehören z. B. PCs, Laptops, Smartphones, Tablets oder Server. Ziel ist der Schutz vor Schadsoftware, unbefugtem Zugriff und Datenverlust."
  examples:
    - "Antivirus- oder Anti-Malware-Software"
    - "Firewall auf dem Endgerät"
    - "Regelmäßige Updates und Sicherheitspatches"
    - "Festplattenverschlüsselung auf Laptops"
    - "Zugriffsschutz durch Passwort, PIN oder MFA"
    - "Mobile Device Management für Firmen-Smartphones"
    - "Merksatz: Endpoint-Security = Schutz der Endgeräte im Netzwerk"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-25"
updated: "2026-05-11"
---

## Endpoint Security

Endpoint Security schützt einzelne Endgeräte innerhalb eines Netzwerks.

Dazu gehören z. B. PCs, Laptops, Smartphones oder Server.

## Kernerklärung

### Definition
- Schutzmaßnahmen für **Endgeräte (Endpoints)**  
- Verhindert:
  - unbefugte Zugriffe  
  - Schadsoftware  
  - Angriffe von außen  

### Typische Maßnahmen
- Anwendungssperren (z. B. für E-Mail/Office)  
- Überwachung von Systemen  
- Kontrolle externer Datenträger (USB etc.)  
- Whitelisting von erlaubten Programmen  

```mermaid
flowchart LR
    A[Endgerät] --> B[Endpoint Security]
    B --> C[Schutz vor Angriffen]
    B --> D[Zugriffskontrolle]
```

## Praktisches Beispiel
Unternehmen setzt Richtlinien:

- USB-Sticks nur eingeschränkt erlaubt  
- Nur freigegebene Programme dürfen laufen  
- E-Mails werden gefiltert  

Endgeräte bleiben geschützt

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist Endpoint Security?
- Welche Maßnahmen gehören dazu?
- Warum ist sie wichtig?

### Antworten auf die typischen Prüfungsfragen
- Schutz von Endgeräten im Netzwerk.  
- Überwachung, Zugriffskontrolle, Whitelisting.  
- Schutz vor Angriffen und Datenverlust.

## Merksatz
**Endpoint Security schützt jedes einzelne Gerät im Netzwerk.**