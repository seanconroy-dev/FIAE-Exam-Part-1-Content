---
# Identity (stable; never change after publishing)
id: ap1-0266
slug: pay-per-use-modell

# Display
title: "Pay-per-use Modell – Nutzung nach Verbrauch"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Cloud", "Kostenmodelle", "Infrastruktur"]
tags: ["ap1", "pay-per-use", "cloud", "kostenmodell"]

# Flashcard payload
card:
  type: definition
  question: "Was bedeutet Pay-per-use?"
  answer: "Pay-per-use bedeutet, dass man nur für die tatsächlich genutzten Leistungen oder Ressourcen bezahlt. Typisch ist dieses Modell bei Cloud-Diensten, z. B. für Rechenleistung, Speicherplatz, Datenverkehr oder Nutzungsdauer."
  examples:
    - "Cloud-Server wird nach Laufzeit abgerechnet"
    - "Speicherplatz wird nach genutzten GB bezahlt"
    - "Rechenleistung wird nach Verbrauch abgerechnet"
    - "Datenverkehr kann nach übertragenem Datenvolumen berechnet werden"
    - "Merksatz: Pay-per-use = bezahlen nach tatsächlicher Nutzung"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Pay-per-use Modell – Nutzung nach Verbrauch
Das Pay-per-use Modell ist ein **verbrauchsabhängiges Abrechnungsmodell**, das vor allem in der Cloud und modernen IT-Infrastrukturen genutzt wird.

## Kernerklärung

- Zahlung erfolgt **nur bei tatsächlicher Nutzung**
- keine:
  - hohen Anschaffungskosten  
  - langfristige Kapitalbindung  

- Vorteile:
  - hohe Flexibilität  
  - gute Skalierbarkeit  
  - immer aktuelle Software  

- Abrechnung:
  - zeitbasiert (z. B. Stunden)  
  - nutzungsbasiert (z. B. GB, CPU)  

```mermaid
flowchart LR
A[Nutzung von Ressourcen] --> B[Messung Verbrauch]
B --> C[Abrechnung nach Nutzung]
```

## Praktisches Beispiel

- Cloud-Anbieter:
  - virtuelle Maschinen nach Stunden abrechnen  
  - Speicher nach GB  

- Unternehmen:
  - zahlen nur für tatsächlich genutzte Rechenleistung  
  - können Lastspitzen flexibel ausgleichen  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was bedeutet Pay-per-use?  
- Welche Vorteile hat das Modell?  
- Wo wird es eingesetzt?  

### Antworten auf die typischen Prüfungsfragen
- Bezahlung nach tatsächlicher Nutzung  
- flexibel, skalierbar, keine Anfangsinvestition  
- vor allem in Cloud-Umgebungen  

## Merksatz
Pay-per-use bedeutet: Zahlen nur für das, was man wirklich nutzt.