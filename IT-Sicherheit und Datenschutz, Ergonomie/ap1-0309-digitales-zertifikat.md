---
# Identity (stable; never change after publishing)
id: ap1-0309
slug: "digitales-zertifikat"

# Display
title: "Digitales Zertifikat"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["kryptografie", "zertifikate", "pki"]
tags: ["ap1", "grundlagen", "verschluesselung", "authentifizierung"]

# Flashcard payload
card:
  type: definition
  question: "Was ist ein digitales Zertifikat?"
  answer: "Ein digitales Zertifikat ist ein elektronischer Nachweis für eine digitale Identität. Es bestätigt z. B. die Identität einer Person, Webseite, Organisation oder eines Geräts und enthält den öffentlichen Schlüssel. Ausgestellt wird es meist von einer Zertifizierungsstelle, also einer CA."
  examples:
    - "HTTPS: Zertifikat bestätigt die Identität einer Webseite"
    - "E-Mail: Zertifikat kann für Signatur oder Verschlüsselung genutzt werden"
    - "VPN: Zertifikat kann zur sicheren Anmeldung verwendet werden"
    - "CA: Certificate Authority stellt Zertifikate aus"
    - "Öffentlicher Schlüssel: ist im Zertifikat enthalten"
    - "Merksatz: digitales Zertifikat = digitaler Ausweis mit öffentlichem Schlüssel"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-25"
updated: "2026-05-11"
---

## Digitales Zertifikat

Ein digitales Zertifikat ist ein zentrales Element der IT-Sicherheit und Bestandteil der PKI.

Es dient dazu, Identitäten im Internet eindeutig und vertrauenswürdig zu bestätigen.

## Kernerklärung

### Definition
- Digitaler Datensatz zur **Authentifizierung**
- Enthält einen **öffentlichen Schlüssel**
- Wird durch eine **Zertifizierungsstelle (CA)** ausgestellt  

### Eigenschaften
- Basiert meist auf dem **X.509-Standard**  
- Nutzt **asymmetrische Kryptografie**  
- Gewährleistet:
  - **Authentizität**
  - **Vertraulichkeit**
  - **Integrität**

### Aufbau (vereinfacht)

| Bestandteil            | Beschreibung                          |
|----------------------|--------------------------------------|
| Öffentlicher Schlüssel | Für Verschlüsselung/Verifikation      |
| Inhaber              | Person/Organisation/Webseite          |
| Aussteller (CA)      | Vertrauenswürdige Stelle              |
| Gültigkeit           | Zeitraum der Nutzung                  |

```mermaid
flowchart LR
    A[Zertifikat] --> B[Öffentlicher Schlüssel]
    A --> C[Inhaber]
    A --> D[CA]
    A --> E[Gültigkeit]
```

## Praktisches Beispiel
HTTPS-Webseite:

- Website besitzt ein digitales Zertifikat  
- Browser prüft dieses Zertifikat  
- Verbindung wird als sicher angezeigt (Schloss-Symbol)  

Nutzer kann sicher kommunizieren

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist ein digitales Zertifikat?
- Welche Informationen enthält es?
- Wozu wird es verwendet?

### Antworten auf die typischen Prüfungsfragen
- Datensatz zur Bestätigung von Identitäten.  
- Öffentlicher Schlüssel, Inhaber, CA, Gültigkeit.  
- Für sichere Kommunikation und Authentifizierung.

## Merksatz
**Ein Zertifikat bestätigt: „Dieser Schlüssel gehört wirklich zu dieser Identität.“**