---
# Identity (stable; never change after publishing)
id: ap1-0206
slug: standby-offline-usv

# Display
title: "Standby-/Offline-USV – Bedeutung"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["stromversorgung", "usv"]
tags: ["usv", "stromausfall", "hardware"]

# Flashcard payload
card:
  type: definition
  question: "Erkläre den Begriff Standby- oder Offline-USV."
  answer: "Eine Standby- oder Offline-USV versorgt angeschlossene Geräte im Normalbetrieb direkt aus dem Stromnetz. Erst bei Stromausfall schaltet sie mit kurzer Verzögerung auf Batteriebetrieb um. Sie bietet grundlegenden Schutz, aber nur begrenzten Schutz gegen Spannungsschwankungen."
  examples:
    - "Geeignet für einzelne PCs oder einfache Arbeitsplätze"
    - "Umschaltzeit typischerweise wenige Millisekunden"
    - "Günstigste und einfachste USV-Variante"
    - "Entspricht meist der USV-Klasse VFD"
    - "Nicht ideal für besonders kritische Server oder Rechenzentren"
    - "Merksatz: Standby-USV = einfach, günstig – aber nur begrenzter Schutz"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## Standby-/Offline-USV – Bedeutung

Eine **USV (unterbrechungsfreie Stromversorgung)** schützt IT-Systeme vor Stromausfällen.

Die einfachste Variante ist die:

- **Standby- bzw. Offline-USV**

---

## Kernerklärung

### Eigenschaften der Standby-/Offline-USV

- Normalbetrieb:
  - Geräte werden **direkt vom Stromnetz** versorgt  
- Bei Stromausfall:
  - Umschaltung auf **Batteriebetrieb**  
- Umschaltzeit:
  - ca. **4–10 ms**  

### Einschränkungen

- schützt nur gegen:
  - Stromausfälle  
  - kurze Spannungsschwankungen  
- schützt **nicht zuverlässig** gegen:
  - Unterspannung  
  - Überspannung  
  - Spannungsspitzen  

### Funktionsprinzip

```mermaid
flowchart LR
Netz -->|Normalbetrieb| Verbraucher
Netz --> USV
USV -->|bei Ausfall| Verbraucher
```

---

## Praktisches Beispiel

- Heim-PC mit günstiger USV:
  - Bei Stromausfall bleibt der PC kurzzeitig an  
  - Zeit zum **sicheren Herunterfahren**  

---

## Prüfungsrelevanz (AP1)

Wichtig:

- Unterschied zwischen **Offline-, Line-Interactive- und Online-USV**
- Umschaltzeit verstehen
- Einschränkungen kennen

---

### Typische Prüfungsfragen

- Wie funktioniert eine Offline-USV?
- Wie lange dauert die Umschaltung?
- Welche Schutzwirkung hat sie?

---

### Antworten auf die typischen Prüfungsfragen

**Funktionsweise?**  
→ Netzbetrieb + Umschaltung auf Batterie  

**Umschaltzeit?**  
→ ca. 4–10 ms  

**Schutz?**  
→ begrenzt (v. a. gegen Stromausfall)  

---

## Merksatz

**Offline-USV: einfach, günstig – aber nur begrenzter Schutz.**