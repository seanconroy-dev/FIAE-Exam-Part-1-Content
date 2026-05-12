---
# Identity (stable; never change after publishing)
id: ap1-0329
slug: "schutzbedarfsanalyse-kriterien-it-systeme"

# Display
title: "Schutzbedarfsanalyse von IT-Systemen"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["schutzbedarfsanalyse", "risikobewertung"]
tags: ["ap1", "it-sicherheit", "risiken"]

# Flashcard payload
card:
  type: multi
  question: "Welche Kriterien gehören zu einer Schutzbedarfsanalyse für IT-Systeme?"
  answer: "Bei einer Schutzbedarfsanalyse wird bewertet, wie stark IT-Systeme, Daten oder Prozesse geschützt werden müssen. Wichtige Kriterien sind Schutzobjekte, Schutzziele, Bedrohungen, mögliche Schadenshöhe, Eintrittswahrscheinlichkeit, Gefährdungspotenzial, passende Schutzmaßnahmen und eine Kosten-Nutzen-Betrachtung."
  examples:
    - "Schutzobjekte: Server, Datenbanken, Anwendungen oder personenbezogene Daten"
    - "Schutzziele: Vertraulichkeit, Integrität und Verfügbarkeit"
    - "Bedrohungen: Schadsoftware, Ausfall, Diebstahl oder unbefugter Zugriff"
    - "Schadenshöhe: finanzieller Schaden, Datenverlust oder Reputationsschaden"
    - "Eintrittswahrscheinlichkeit: Wie wahrscheinlich ist ein Vorfall?"
    - "Gefährdungspotenzial: Wie stark wäre das Unternehmen betroffen?"
    - "Schutzmaßnahmen: Backup, Zugriffskontrolle, Verschlüsselung oder Firewall"
    - "Kosten-Nutzen: Aufwand der Maßnahme im Verhältnis zum Risiko bewerten"
    - "Merksatz: Schutzbedarf = Was schützen, wovor schützen, wie schlimm wäre der Schaden?"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-28"
updated: "2026-05-12"
---

## Schutzbedarfsanalyse von IT-Systemen

Die Schutzbedarfsanalyse ist ein zentraler Bestandteil der IT-Sicherheit.  
Sie hilft dabei, Risiken zu erkennen und geeignete Schutzmaßnahmen abzuleiten.

## Kernerklärung

Wichtige Kriterien einer Schutzbedarfsanalyse:

- **Risikoanalyse**: Wie wahrscheinlich sind Angriffe?
- **Schutzobjekte**: Welche Systeme/Daten müssen geschützt werden?
- **Bedrohungsszenarien**: Welche konkreten Gefahren gibt es?
- **Schadensausmaß**: Wie groß wäre der mögliche Schaden?
- **Gefährdungspotenzial**: Wie stark ist die aktuelle Bedrohungslage?
- **Schutzmaßnahmen**: Welche Maßnahmen sind geeignet?
- **Kosten-Nutzen-Abwägung**: Lohnt sich die Maßnahme wirtschaftlich?

### Zusammenhang

```mermaid
flowchart LR
    A[Bedrohung] --> B[Risikoanalyse]
    B --> C[Schutzbedarf]
    C --> D[Maßnahmen]
    D --> E[IT-Sicherheit]
```

### Übersicht

| Kriterium | Bedeutung |
|----------|----------|
| Risiko | Wahrscheinlichkeit eines Angriffs |
| Schutzobjekte | Kritische Systeme/Daten |
| Bedrohungen | mögliche Angriffe |
| Schaden | Auswirkungen eines Vorfalls |
| Maßnahmen | Schutz der Systeme |
| Kosten-Nutzen | Wirtschaftlichkeit |

## Praktisches Beispiel

Ein Unternehmen analysiert seinen Webserver:

- Hohe Angriffswahrscheinlichkeit (Internet erreichbar)  
- Kritische Kundendaten betroffen  
- Maßnahmen: Firewall, Updates, Backups  

Ergebnis: Reduziertes Risiko und höhere Sicherheit

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist eine Schutzbedarfsanalyse?  
- Welche Kriterien werden betrachtet?  

### Antworten auf die typischen Prüfungsfragen
- Analyse zur Bewertung von Risiken und Schutzbedarf von IT-Systemen  
- z. B. Risiko, Bedrohungen, Schaden, Maßnahmen, Kosten-Nutzen  

## Merksatz
**Schutzbedarf = Risiko + Schaden → passende Sicherheitsmaßnahmen auswählen.**