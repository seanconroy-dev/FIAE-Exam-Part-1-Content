---
# Identity (stable; never change after publishing)
id: ap1-0300
slug: "multi-factor-authentication-mfa"

# Display
title: "Multi-Faktor-Authentifizierung (MFA)"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["mfa", "authentifizierung", "zugriffssicherheit"]
tags: ["ap1", "sicherheit", "login", "schutz"]

# Flashcard payload
card:
  type: definition
  question: "Was ist MFA und wo wird es eingesetzt?"
  answer: "MFA bedeutet Multi-Factor Authentication. Dabei werden mindestens zwei unabhängige Faktoren zur Anmeldung geprüft, z. B. Passwort plus App-Code. Dadurch wird der Zugriff sicherer, weil ein gestohlenes Passwort allein nicht ausreicht."
  examples:
    - "Wissen: Passwort oder PIN"
    - "Besitz: Smartphone, TAN-Generator oder Sicherheitsschlüssel"
    - "Sein: Fingerabdruck oder Gesichtserkennung"
    - "Online-Banking: Passwort plus TAN"
    - "Cloud-Zugang: Passwort plus Authenticator-App"
    - "Firmenkonto: Anmeldung mit Passwort und Hardware-Token"
    - "Merksatz: MFA = mindestens zwei verschiedene Nachweise für die Anmeldung"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-25"
updated: "2026-05-11"
---

## Multi-Faktor-Authentifizierung (MFA)
Multi-Faktor-Authentifizierung (MFA) erhöht die Sicherheit von Logins, indem mehrere Nachweise der Identität verlangt werden.

## Kernerklärung

### Grundprinzip
Statt nur eines Passworts werden **mindestens zwei unabhängige Faktoren** abgefragt:

| Faktor-Typ        | Beispiel |
|------------------|----------|
| Wissen           | Passwort, PIN |
| Besitz           | Smartphone, TAN per SMS/App |
| Biometrie        | Fingerabdruck, Gesichtserkennung |

Zugriff wird erst gewährt, wenn mehrere Faktoren korrekt sind.

### Vorteile
- Höhere Sicherheit gegen unbefugten Zugriff  
- Schutz vor Passwortdiebstahl  
- Standard bei sicherheitskritischen Anwendungen  

```mermaid
flowchart LR
    A[Login] --> B[Passwort prüfen]
    B --> C[Zweiter Faktor prüfen]
    C --> D[Zugriff erlaubt]
```

## Praktisches Beispiel
Login beim Online-Banking:

- Eingabe von Benutzername + Passwort  
- Zusätzlicher TAN-Code per App  

Nur bei beiden korrekten Angaben erfolgt der Zugriff

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist MFA?
- Nenne Beispiele für Faktoren.
- Warum ist MFA sicherer als ein Passwort?

### Antworten auf die typischen Prüfungsfragen
- MFA ist eine Anmeldung mit mehreren unabhängigen Sicherheitsfaktoren.  
- Wissen (Passwort), Besitz (Smartphone), Biometrie (Fingerabdruck).  
- Weil ein einzelner kompromittierter Faktor nicht ausreicht.

## Merksatz
**MFA = Mehrere Nachweise → deutlich höhere Sicherheit beim Login.**