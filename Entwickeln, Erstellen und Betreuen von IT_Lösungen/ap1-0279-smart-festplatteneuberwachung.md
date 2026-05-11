---
# Identity (stable; never change after publishing)
id: ap1-0279
slug: smart-festplattenueberwachung

# Display
title: "S.M.A.R.T. – Festplattenüberwachung"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Hardware", "Speicher", "Überwachung"]
tags: ["ap1", "smart", "festplatte", "diagnose"]

# Flashcard payload
card:
  type: definition
  question: "Was bedeutet S.M.A.R.T. bei Festplatten und SSDs?"
  answer: "S.M.A.R.T. ist ein Selbstüberwachungs- und Diagnosesystem für HDDs und SSDs. Es überwacht Zustandswerte des Laufwerks, z. B. Temperatur, fehlerhafte Sektoren, Betriebsstunden und Fehler beim Lesen oder Schreiben. Dadurch können mögliche Ausfälle frühzeitig erkannt werden."
  examples:
    - "Temperaturüberwachung einer Festplatte"
    - "Erkennung fehlerhafter Sektoren"
    - "Anzeige von Betriebsstunden"
    - "Warnung bei auffälligen Laufwerkswerten"
    - "Einsatz in Servern, PCs und NAS-Systemen"
    - "Merksatz: S.M.A.R.T. = Laufwerk überwacht seinen eigenen Zustand"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## S.M.A.R.T. – Festplattenüberwachung
**S.M.A.R.T. (Self-Monitoring, Analysis and Reporting Technology)** ist ein System zur **Selbstüberwachung von Datenträgern** wie HDDs und SSDs.

## Kernerklärung

- Zweck:
  - **Früherkennung von Defekten**
  - Vermeidung von **Datenverlust**

- Funktionsweise:
  - Datenträger sammelt kontinuierlich **Zustandsdaten**
  - Speicherung als **SMART-Attribute**
  - Auswertung durch System oder Tools

- Wichtige Attribute:
  - Temperatur  
  - Betriebsstunden (Einschaltzeit)  
  - Anzahl fehlerhafter Sektoren (Bad Blocks)  
  - Lese-/Schreibfehler  

- Besonderheit:
  - Werte sind **nicht vollständig standardisiert**
  - Interpretation erfolgt je nach Hersteller unterschiedlich  

```mermaid
flowchart LR
A[Datenträger] --> B[SMART Attribute]
B --> C[Analyse]
C --> D{Grenzwert überschritten?}
D -->|Ja| E[Warnung / Ausfallrisiko]
D -->|Nein| F[Normalbetrieb]
```

## Praktisches Beispiel

```bash
smartctl -a /dev/sda
```

- Zeigt:
  - Gesundheitsstatus  
  - SMART-Werte  
  - mögliche Warnungen  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was bedeutet S.M.A.R.T.?  
- Welche Aufgabe hat es?  
- Welche Werte werden überwacht?  

### Antworten auf die typischen Prüfungsfragen
- Selbstüberwachungssystem für Datenträger  
- Frühzeitige Fehlererkennung  
- Temperatur, Laufzeit, Fehlerwerte  

## Merksatz
S.M.A.R.T. überwacht den Zustand der Festplatte und warnt vor Ausfällen.