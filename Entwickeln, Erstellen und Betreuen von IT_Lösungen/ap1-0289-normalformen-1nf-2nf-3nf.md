---
# Identity (stable; never change after publishing)
id: ap1-0289
slug: normalformen-1nf-2nf-3nf

# Display
title: "Normalformen (1NF, 2NF, 3NF) und ihr Zweck"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Normalisierung", "DB-Design"]
tags: ["ap1", "datenbank", "normalformen"]

# Flashcard payload
card:
  type: multi
  question: "Welche ersten drei Normalformen gibt es und wozu dienen sie?"
  answer: "Die ersten drei Normalformen helfen, Tabellen sauber zu strukturieren und Datenredundanzen zu vermeiden. 1NF bedeutet: Jeder Tabellenwert ist atomar, also nicht weiter sinnvoll teilbar. 2NF bedeutet: Jedes Nicht-Schlüsselattribut hängt vom gesamten Primärschlüssel ab. 3NF bedeutet: Nicht-Schlüsselattribute hängen nicht voneinander ab, sondern nur vom Schlüssel."
  examples:
    - "1NF: In einem Feld steht nur ein Wert, z. B. eine Telefonnummer statt mehrere Telefonnummern"
    - "2NF: Bei zusammengesetztem Schlüssel hängen alle anderen Felder vom ganzen Schlüssel ab"
    - "3NF: Die Postleitzahl bestimmt nicht zusätzlich den Ort in derselben Tabelle, wenn das ausgelagert werden sollte"
    - "Zweck: weniger doppelte Daten"
    - "Zweck: weniger Änderungs-, Einfüge- und Löschfehler"
    - "Merksatz: 1NF = atomar, 2NF = ganzer Schlüssel, 3NF = nur vom Schlüssel"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Normalformen (1NF, 2NF, 3NF) und ihr Zweck
Die Normalisierung ist ein zentraler Bestandteil des Datenbankdesigns und dient dazu, **Redundanzen zu vermeiden** und die Datenqualität zu verbessern.

## Kernerklärung

### Zweck der Normalisierung
- Vermeidung von **Datenredundanz**
- Verbesserung der **Datenkonsistenz**
- Vermeidung von **Anomalien** (Einfüge-, Änderungs-, Löschanomalien)

### Die ersten drei Normalformen

| Normalform | Bedingung | Ziel |
|------------|----------|------|
| 1NF        | Alle Attribute sind atomar | Keine mehrfachen Werte |
| 2NF        | Jedes Nichtschlüsselattribut ist voll funktional abhängig vom Primärschlüssel | Vermeidung partieller Abhängigkeiten |
| 3NF        | Keine transitiven Abhängigkeiten | Weitere Redundanzvermeidung |

```mermaid
flowchart LR
A[Unnormalisierte Tabelle] --> B[1NF]
B --> C[2NF]
C --> D[3NF]
```

## Praktisches Beispiel

**Vor Normalisierung:**
- Tabelle: Kunde (ID, Name, Produkt1, Produkt2)

**Nach 1NF:**
- Tabelle wird aufgeteilt → keine mehrfachen Werte mehr

**Nach 2NF:**
- Trennung von Kunden- und Produktdaten

**Nach 3NF:**
- Entfernung indirekter Abhängigkeiten (z. B. Ort abhängig von PLZ)

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist das Ziel der Normalisierung?  
- Unterschiede zwischen 1NF, 2NF und 3NF  
- Was sind transitive Abhängigkeiten?  

### Antworten auf die typischen Prüfungsfragen
- Ziel: Redundanz vermeiden  
- 1NF: atomar  
- 2NF: volle Abhängigkeit  
- 3NF: keine indirekten Abhängigkeiten  

## Merksatz
1NF: atomar – 2NF: voll abhängig – 3NF: keine indirekten Abhängigkeiten.