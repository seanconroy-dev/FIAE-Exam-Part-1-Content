---
# Identity (stable; never change after publishing)
id: ap1-0207
slug: online-usv

# Display
title: "Online-USV – Bedeutung"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["stromversorgung", "usv"]
tags: ["usv", "stromausfall", "online-usv"]

# Flashcard payload
card:
  type: definition
  question: "Wie funktioniert eine Online-USV?"
  answer: "Eine Online-USV versorgt angeschlossene Geräte dauerhaft über einen Wechselrichter. Der Strom wird dabei ständig aufbereitet, sodass eine stabile Ausgangsspannung entsteht. Bei Netzausfall gibt es keine Umschaltzeit, weil die Batterie bereits in das System eingebunden ist."
  examples:
    - "Geeignet für Serverräume und kritische IT-Systeme"
    - "Keine Umschaltzeit bei Stromausfall"
    - "Bietet hohen Schutz gegen Stromausfall, Spannungsschwankungen und Netzstörungen"
    - "Entspricht meist der USV-Klasse VFI"
    - "Auch als Doppelwandler-USV oder Double-Conversion-USV bekannt"
    - "Merksatz: Online-USV = maximale Sicherheit ohne Unterbrechung"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## Online-USV – Bedeutung
Die **Online-USV (USV-Klasse 1)** ist die hochwertigste Form der unterbrechungsfreien Stromversorgung.

- höchste Sicherheit  
- keine Umschaltzeit  
- konstante Stromqualität  

---

## Kernerklärung

### Eigenschaften der Online-USV

- Verbraucher werden **dauerhaft über Wechselrichter** versorgt  
- Netzspannung wird:
  - gleichgerichtet → Batterie  
  - wieder in stabile Wechselspannung umgewandelt  
- **keine Umschaltzeit** bei Stromausfall  
- Batterie ist **immer aktiv eingebunden**

### Vorteile

- Schutz vor:
  - Stromausfall  
  - Unterspannung / Überspannung  
  - Spannungsschwankungen  
  - Frequenzstörungen  
  - elektromagnetischen Einflüssen  

- liefert nahezu **perfekte Sinusspannung**

### Funktionsprinzip

```mermaid
flowchart LR
Netz --> Gleichrichter --> Batterie --> Wechselrichter --> Verbraucher
```

---

## Praktisches Beispiel

- Serverraum / Rechenzentrum:
  - kritische Systeme laufen über **Online-USV**
  - kein Ausfall bei Stromproblemen  

---

## Prüfungsrelevanz (AP1)

Sehr wichtig:

- Unterschied **Offline vs. Online USV**
- Vorteil: **keine Umschaltzeit**
- Einsatzbereiche (kritische Systeme)

---

### Typische Prüfungsfragen

- Was ist der Hauptvorteil einer Online-USV?
- Gibt es eine Umschaltzeit?
- Wovor schützt sie?

---

### Antworten auf die typischen Prüfungsfragen

**Hauptvorteil?**  
→ konstante Versorgung ohne Unterbrechung  

**Umschaltzeit?**  
→ keine  

**Schutz?**  
→ umfassend (alle Störungen)  

---

## Merksatz

**Online-USV: maximale Sicherheit ohne Unterbrechung.**