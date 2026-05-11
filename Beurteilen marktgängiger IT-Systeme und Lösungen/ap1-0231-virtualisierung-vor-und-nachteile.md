---
# Identity (stable; never change after publishing)
id: ap1-0231
slug: virtualisierung-vor-und-nachteile-cloud

# Display
title: "Vor- und Nachteile der Virtualisierung (inkl. Cloud)"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["Virtualisierung", "Cloud Computing"]
tags: ["Vorteile", "Nachteile", "Server", "Kosten", "Skalierung"]

# Flashcard payload
card:
  type: basic
  question: "Was sind die Vor- und Nachteile der Virtualisierung von Servern und Desktops, auch unter Berücksichtigung von Cloud-Angeboten?"
  answer: "Vorteile: bessere Hardwareauslastung, Strom- und Platzersparnis, schnelle Bereitstellung neuer Systeme, einfachere Skalierbarkeit, bessere Möglichkeiten für Redundanz und zentrale Verwaltung sowie geringere Anfangsinvestitionen bei Cloud-Angeboten. Nachteile: Abhängigkeit von Infrastruktur oder Cloud-Anbieter, mögliche Latenzen, laufende Kosten im 24/7-Betrieb, eingeschränkte Individualisierung, höherer Administrationsaufwand und mögliche Verfügbarkeits- oder Datenschutzrisiken."
  examples:
    - "Servervirtualisierung: mehrere virtuelle Server laufen auf einem physischen Host"
    - "Desktopvirtualisierung: Benutzer arbeiten auf virtuellen Desktops, z. B. per VDI"
    - "Cloud-Vorteil: Ressourcen können schnell hinzugebucht werden"
    - "Cloud-Nachteil: laufende Kosten können bei Dauerbetrieb hoch werden"
    - "Risiko: Fällt der Virtualisierungshost aus, können mehrere virtuelle Systeme betroffen sein"
    - "Merksatz: Virtualisierung spart Hardware und macht flexibler, erhöht aber Abhängigkeit und Verwaltungsaufwand"

# Lifecycle
status: published
created: "2026-03-29"
updated: "2026-05-11"
---

## Virtualisierung: Vor- und Nachteile (inkl. Cloud)

Virtualisierung ermöglicht es, mehrere virtuelle Systeme auf einer physischen Hardware zu betreiben. In Kombination mit Cloud-Angeboten wird Infrastruktur flexibel, skalierbar und oft kosteneffizient bereitgestellt.

## Kernerklärung

### Vorteile
- **Stromersparnis** durch bessere Hardwareauslastung  
- **Skalierbarkeit**: Ressourcen flexibel anpassbar  
- **Redundanz / Ausfallsicherheit** durch verteilte Systeme  
- **Schnelle Bereitstellung** (Provisionierung) von Servern  
- **Kaum Kapazitätsgrenzen** in der Cloud  
- **Kostenvorteile** durch Pay-as-you-go-Modelle  
- **Keine Anfangsinvestitionen** (Cloud statt eigener Hardware)  
- **Verlängerung der Lebensdauer alter Software** durch virtuelle Umgebungen  

### Nachteile
- **Nicht immer günstiger im Dauerbetrieb (24/7)**  
- **Höhere Latenzen** durch Virtualisierungsschichten oder Cloud-Zugriff  
- **Eingeschränkte Kontrolle** (z. B. bei Cloud-Anbietern)  
- **Nicht vollständige Selbstadministration möglich**  
- **Individuallösungen eingeschränkt**  
- **Abhängigkeit vom Anbieter / Verfügbarkeit je nach Region**

### Vergleichstabelle

| Aspekt            | Virtualisierung lokal        | Cloud-Lösung                  |
|------------------|-----------------------------|-------------------------------|
| Kosten           | Hohe Anfangsinvestition     | Pay-as-you-go                 |
| Skalierbarkeit   | Begrenzt durch Hardware     | Nahezu unbegrenzt             |
| Kontrolle        | Hoch                        | Eingeschränkt                 |
| Verfügbarkeit    | Eigenverantwortung          | Anbieterabhängig              |
| Wartung          | Eigenleistung               | Oft durch Anbieter übernommen |

## Praktisches Beispiel
Ein Unternehmen betreibt früher 10 physische Server.  
Durch Virtualisierung laufen alle Systeme auf 2 leistungsstarken Hosts.

Zusätzlich werden Lastspitzen über Cloud-Server abgefangen:

```mermaid
graph LR
A[Physische Server früher] --> B[Virtualisierte Hosts]
B --> C[Cloud Erweiterung]
C --> D[Flexible Skalierung]
```

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Nennen Sie Vorteile der Virtualisierung.
- Welche Nachteile entstehen durch Cloud-Nutzung?
- Warum ist Virtualisierung skalierbar?
- Wann ist Virtualisierung wirtschaftlich sinnvoll?

### Antworten auf die typischen Prüfungsfragen
- Vorteile: bessere Ressourcennutzung, Skalierbarkeit, schnelle Bereitstellung  
- Nachteile: Abhängigkeit, Latenzen, eingeschränkte Kontrolle  
- Skalierbarkeit: Ressourcen können dynamisch zugewiesen werden  
- Wirtschaftlich: besonders bei variabler Last und geringer Anfangsinvestition  

## Merksatz
**Virtualisierung spart Ressourcen und erhöht Flexibilität – Cloud verstärkt das, bringt aber Abhängigkeiten mit sich.**