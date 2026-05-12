---
# Identity (stable; never change after publishing)
id: ap1-0339
slug: service-level-agreement-sla-definition

# Display
title: "Service Level Agreement (SLA)"

# Classification / navigation (machine-side)
module: "auftragsabwicklung-und-leistungserbringung"
topics: ["sla", "service-management", "it-support"]
tags: ["vertrag", "servicelevel", "reaktionszeit", "it-service"]

# Flashcard payload
card:
  type: definition
  question: "Was ist ein Service Level Agreement (SLA)?"
  answer: "Ein SLA ist eine Vereinbarung zwischen Kunde und Anbieter über die Qualität und den Umfang eines IT-Services. Darin werden z. B. Verfügbarkeit, Reaktionszeiten, Lösungszeiten, Zuständigkeiten und Servicezeiten festgelegt."
  examples:
    - "Verfügbarkeit: Server ist zu 99,5 % erreichbar"
    - "Reaktionszeit: Support reagiert innerhalb von 2 Stunden"
    - "Lösungszeit: Störung wird innerhalb von 24 Stunden behoben"
    - "Servicezeit: Support ist Montag bis Freitag von 8 bis 17 Uhr erreichbar"
    - "Zuständigkeit: Anbieter ist für Betrieb und Wartung verantwortlich"
    - "Merksatz: SLA = verbindliche Vereinbarung über IT-Servicequalität"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-28"  
updated: "2026-05-12"
---

## Service Level Agreement (SLA)

Ein Service Level Agreement (SLA) ist die Grundlage für die Qualitätssicherung von IT-Dienstleistungen zwischen Anbieter und Kunde.

## Kernerklärung
SLAs legen verbindlich fest, **welche Leistungen in welcher Qualität erbracht werden müssen**.

Typische Inhalte eines SLA:

- **Vertragslaufzeit**
- **Vertragsziele** (z. B. minimale Ausfallzeiten)
- **Servicezeiten** (z. B. Mo–Fr 07:00–18:00 Uhr)
- **Verantwortlichkeiten** (Kunde & Anbieter)
- **Kommunikationswege** (z. B. Mail, Hotline)
- **Support-Level** (1st, 2nd, 3rd Level)
- **Reaktionszeiten** (z. B. Bearbeitung innerhalb 24h)
- **Sanktionen** bei Nichterfüllung

### Struktur eines SLA (vereinfacht)
```mermaid
flowchart TD
    A[SLA] --> B[Leistungsbeschreibung]
    A --> C[Servicezeiten]
    A --> D[Reaktionszeiten]
    A --> E[Support-Level]
    A --> F[Sanktionen]
```

## Praktisches Beispiel
Ein Unternehmen betreibt einen Webshop:

- SLA garantiert:
  - **99,5 % Verfügbarkeit**
  - **Reaktionszeit: 2 Stunden bei Störungen**
  - **Supportzeiten: Mo–Fr 08:00–18:00**

→ Bei Verstoß (z. B. längerer Ausfall) erhält der Kunde eine **Gutschrift**.

## Prüfungsrelevanz (AP1)
Sehr häufiges Thema im Bereich **IT-Service und Verträge**.

### Typische Prüfungsfragen
- Was ist ein SLA?
- Welche Inhalte gehören in ein SLA?
- Welche Bedeutung haben Reaktionszeiten?

### Antworten auf die typischen Prüfungsfragen
- SLA = vertraglich definierte Servicequalität
- Enthält u. a.:
  - Servicezeiten
  - Reaktionszeiten
  - Verantwortlichkeiten
- Reaktionszeiten bestimmen, **wie schnell auf Probleme reagiert werden muss**

## Merksatz
**Ein SLA legt fest: Welche Leistung, in welcher Qualität und in welcher Zeit erbracht wird.**