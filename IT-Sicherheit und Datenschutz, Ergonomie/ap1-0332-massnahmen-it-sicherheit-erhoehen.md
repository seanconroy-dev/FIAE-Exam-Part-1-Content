---
# Identity (stable; never change after publishing)
id: ap1-0332
slug: "massnahmen-it-sicherheit-erhoehen"

# Display
title: "Maßnahmen zur Erhöhung der IT-Sicherheit"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["sicherheitsmassnahmen", "netzwerksicherheit"]
tags: ["ap1", "it-sicherheit", "schutz"]

# Flashcard payload
card:
  type: multi
  question: "Welche Maßnahmen erhöhen die Sicherheit von IT-Systemen?"
  answer: "Die Sicherheit von IT-Systemen kann durch technische und organisatorische Maßnahmen erhöht werden. Dazu gehören Verschlüsselung, Netzsegmentierung, Firewalls, Endpoint-Security, Rechtekonzepte, regelmäßige Updates, Backups, Logging, Audits, starke Authentifizierung und Mitarbeiterschulungen."
  examples:
    - "Verschlüsselung: Daten vor unbefugtem Lesen schützen"
    - "Netzsegmentierung: Bereiche z. B. durch VLANs trennen"
    - "Firewall: unerwünschten Netzwerkverkehr blockieren"
    - "Endpoint-Security: Endgeräte vor Schadsoftware schützen"
    - "Rechtekonzept: Benutzer erhalten nur notwendige Berechtigungen"
    - "Updates: Sicherheitslücken durch Patches schließen"
    - "Backups: Daten nach Ausfall oder Angriff wiederherstellen"
    - "Logging und Audits: Sicherheitsvorfälle erkennen und nachvollziehen"
    - "MFA: Anmeldung mit zusätzlichem Faktor absichern"
    - "Schulungen: Mitarbeitende für Phishing und Sicherheitsregeln sensibilisieren"
    - "Merksatz: IT-Sicherheit = schützen, trennen, aktualisieren, sichern und kontrollieren"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-28"
updated: "2026-05-12"
---

## Maßnahmen zur Erhöhung der IT-Sicherheit

IT-Sicherheit umfasst technische und organisatorische Maßnahmen, um Systeme vor Angriffen und Schäden zu schützen.

## Kernerklärung

Wichtige Maßnahmen zur Erhöhung der IT-Sicherheit:

- **Datenverschlüsselung** (z. B. Datenträger, Kommunikation)
- **Netzwerksegmentierung** (z. B. VLANs)
- **Firewall- und Endpoint-Security-Konzepte**
- **Rechte- und Rollenkonzepte** für Benutzer und Admins
- **Regelmäßige Updates und Patches**
- **Logging und Auditing** (z. B. Penetrationstests)
- **Starke Authentifizierung** (Passwortrichtlinien, MFA)
- **Organisatorische Maßnahmen** (z. B. Vier-Augen-Prinzip)
- **Mitarbeiterschulungen** zur Sensibilisierung

### Zusammenhang

```mermaid
flowchart LR
    A[Maßnahmen] --> B[IT-Sicherheit]
    B --> C[Weniger Angriffe]
    C --> D[Weniger Schäden]
```

## Praktisches Beispiel

Ein Unternehmen schützt seine IT-Systeme durch:

- Firewall + VLAN-Trennung  
- MFA für alle Benutzer  
- Regelmäßige Updates  

Ergebnis: deutlich geringeres Risiko für Angriffe

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Nenne Maßnahmen zur IT-Sicherheit  
- Warum sind Schulungen wichtig?  

### Antworten auf die typischen Prüfungsfragen
- z. B. Verschlüsselung, Firewalls, MFA, Updates  
- Mitarbeiter erkennen Bedrohungen besser und vermeiden Fehler  

## Merksatz
**IT-Sicherheit = Technik + Organisation + Mensch.**