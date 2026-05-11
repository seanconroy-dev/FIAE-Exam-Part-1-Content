---
# Identity (stable; never change after publishing)
id: ap1-0287
slug: objekt-vs-klasse

# Display
title: "Objekt vs. Klasse – Unterschied"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["OOP", "Grundlagen", "Klassen"]
tags: ["ap1", "oop", "klasse", "objekt"]

# Flashcard payload
card:
  type: comparison
  question: "Worin unterscheiden sich Klasse und Objekt?"
  answer: "Eine Klasse ist ein Bauplan oder eine Vorlage. Sie beschreibt, welche Attribute und Methoden Objekte haben können. Ein Objekt ist eine konkrete Instanz dieser Klasse und besitzt echte Werte."
  examples:
    - "Klasse: Auto"
    - "Objekt: meinAuto mit Farbe rot und 150 PS"
    - "Klasse: Kunde"
    - "Objekt: kunde1 mit Name, Kundennummer und Adresse"
    - "Attribut in der Klasse: farbe"
    - "Konkreter Wert im Objekt: rot"
    - "Merksatz: Klasse = Bauplan, Objekt = konkretes Ding"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Objekt vs. Klasse – Unterschied
In der objektorientierten Programmierung beschreibt eine **Klasse** den Bauplan, während ein **Objekt** eine konkrete Ausprägung davon ist.

## Kernerklärung

### Klasse

- Vorlage / Bauplan für Objekte  
- Definiert:
  - **Attribute** (Eigenschaften)
  - **Methoden** (Funktionen)
- Kann vererbt oder erweitert werden  

### Objekt

- Konkrete **Instanz einer Klasse**  
- Enthält:
  - konkrete Werte für Attribute  
- Nutzt die Methoden der Klasse  

### Vergleich

| Merkmal     | Klasse                          | Objekt                         |
|------------|----------------------------------|--------------------------------|
| Bedeutung   | Bauplan                         | Konkretes Exemplar            |
| Inhalt      | Attribute + Methoden            | Werte + Methoden              |
| Existenz    | abstrakt                        | real im Speicher              |
| Beispiel    | Auto                            | MeinAuto (rot, 150 PS)        |

```mermaid
flowchart LR
A[Klasse: Auto] --> B[Objekt: MeinAuto]
A --> C[Objekt: Firmenwagen]
```

## Praktisches Beispiel

```java
class Auto {
    String farbe;
    int ps;
}

Auto meinAuto = new Auto();
meinAuto.farbe = "rot";
meinAuto.ps = 150;
```

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist eine Klasse?  
- Was ist ein Objekt?  
- Unterschied zwischen Klasse und Objekt?  

### Antworten auf die typischen Prüfungsfragen
- Klasse = Bauplan  
- Objekt = Instanz  
- Objekt hat konkrete Werte  

## Merksatz
Die Klasse ist der Bauplan – das Objekt ist das fertige Produkt.