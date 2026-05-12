---
# Identity (stable; never change after publishing)
id: ap1-0346
slug: cloud-computing-iaas-paas-saas

# Display
title: "Cloud-Computing: IaaS, PaaS und SaaS"

# Classification / navigation (machine-side)
module: "auftragsabwicklung-und-leistungserbringung"
topics: ["cloud-computing", "it-architektur", "services"]
tags: ["iaas", "paas", "saas", "cloud"]

# Flashcard payload
card:
  type: comparison
  question: "Wie unterscheiden sich IaaS, PaaS und SaaS?"
  answer: "IaaS stellt IT-Infrastruktur bereit, z. B. virtuelle Server, Speicher und Netzwerke. PaaS stellt eine Plattform für Entwicklung und Betrieb von Anwendungen bereit. SaaS stellt fertige Software bereit, die direkt genutzt werden kann."
  examples:
    - "IaaS: virtuelle Maschine, Speicherplatz oder Netzwerk in der Cloud"
    - "IaaS: Kunde verwaltet Betriebssystem und Anwendungen selbst"
    - "PaaS: Plattform zum Entwickeln und Bereitstellen von Anwendungen"
    - "PaaS: Anbieter verwaltet Infrastruktur und Laufzeitumgebung"
    - "SaaS: fertige Anwendung im Browser nutzen"
    - "SaaS: Beispiele sind Microsoft 365, Google Workspace oder Webmail"
    - "Merksatz: IaaS = Infrastruktur, PaaS = Plattform, SaaS = Software"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-28"
updated: "2026-05-12"
---

## Cloud-Computing: IaaS, PaaS und SaaS

Cloud Computing stellt IT-Ressourcen als Services bereit. Dabei unterscheidet man drei grundlegende Service-Modelle.

## Kernerklärung
Die drei Cloud-Service-Modelle bauen logisch aufeinander auf:

### IaaS (Infrastructure as a Service)
- Bereitstellung von:
  - Servern
  - Speicher
  - Netzwerken
- Ersatz für klassische Rechenzentren
- Nutzer verwaltet Betriebssystem und Anwendungen selbst

### PaaS (Platform as a Service)
- Bereitstellung von:
  - Entwicklungsumgebungen
  - Laufzeitumgebungen
- Entwickler können Anwendungen erstellen, ohne sich um Infrastruktur zu kümmern

### SaaS (Software as a Service)
- Bereitstellung fertiger Software
- Nutzung über Internet (z. B. Browser)
- Keine Installation notwendig

### Vergleich der Modelle

| Modell | Was wird bereitgestellt? | Nutzer kümmert sich um |
|--------|--------------------------|------------------------|
| IaaS   | Infrastruktur            | OS, Anwendungen        |
| PaaS   | Plattform                | Anwendungen            |
| SaaS   | Software                | Nutzung                |

### Schichtenmodell
```mermaid
flowchart TD
    A[IaaS] --> B[PaaS]
    B --> C[SaaS]
```

## Praktisches Beispiel
Ein Unternehmen nutzt Cloud-Dienste:

- **IaaS**: Virtuelle Server bei einem Anbieter  
- **PaaS**: Entwicklungsplattform für Webanwendungen  
- **SaaS**: E-Mail-Dienst im Browser  

## Prüfungsrelevanz (AP1)
Sehr häufiges Thema im Bereich **Cloud & IT-Infrastruktur**.

### Typische Prüfungsfragen
- Was ist der Unterschied zwischen IaaS, PaaS und SaaS?
- Wer ist für welche Aufgaben verantwortlich?
- Welche Vorteile bietet Cloud Computing?

### Antworten auf die typischen Prüfungsfragen
- IaaS = Infrastruktur, PaaS = Plattform, SaaS = Software  
- Verantwortung nimmt von IaaS → SaaS ab  
- Vorteile:
  - Skalierbarkeit
  - Kostenersparnis
  - Flexibilität

## Merksatz
**IaaS = Hardware, PaaS = Plattform, SaaS = fertige Software**