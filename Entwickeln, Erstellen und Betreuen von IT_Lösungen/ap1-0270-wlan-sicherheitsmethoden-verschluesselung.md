---
# Identity (stable; never change after publishing)
id: ap1-0270
slug: wlan-sicherheitsmethoden-verschluesselung

# Display
title: "WLAN – Sicherheitsmethoden und Verschlüsselung"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "WLAN", "Sicherheit"]
tags: ["ap1", "wlan", "wpa2", "wpa3", "verschluesselung"]

# Flashcard payload
card:
  type: multi
  question: "Welche Sicherheitsmethoden eignen sich für ein Unternehmens-WLAN?"
  answer: "Für ein Unternehmens-WLAN eignen sich vor allem WPA2-Enterprise oder WPA3-Enterprise mit zentraler Authentifizierung über einen RADIUS-Server. Als sichere Verschlüsselung wird AES verwendet. WPA, WEP und TKIP gelten als veraltet oder unsicher und sollten nicht mehr eingesetzt werden."
  examples:
    - "WPA2-Enterprise: Anmeldung über RADIUS-Server"
    - "WPA3-Enterprise: moderner Standard für Unternehmens-WLANs"
    - "AES: sichere Verschlüsselung bei WPA2/WPA3"
    - "SAE: modernes Authentifizierungsverfahren bei WPA3-Personal"
    - "WPA2-Personal: eher für Heimnetzwerke oder kleine Umgebungen"
    - "Unsicher: WEP, altes WPA und TKIP vermeiden"
    - "Merksatz: Unternehmen = WPA2/WPA3-Enterprise + RADIUS + AES"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## WLAN – Sicherheitsmethoden und Verschlüsselung
Für sichere WLANs müssen geeignete **Authentifizierungs- und Verschlüsselungsverfahren** eingesetzt werden, um unbefugten Zugriff zu verhindern.

## Kernerklärung

### Sicherheitsmethoden

| Methode              | Bewertung / Einsatz                 |
|---------------------|-----------------------------------|
| WPA                 | veraltet, unsicher                 |
| WPA2-Personal       | Standard im Heimnetz               |
| WPA2-Enterprise     | mit RADIUS, Unternehmen           |
| WPA3-Personal       | moderner Standard                 |
| WPA3-Enterprise     | höchste Sicherheit, mit RADIUS    |

---

### Verschlüsselungsstandards

| Standard | Beschreibung                     |
|----------|---------------------------------|
| AES      | sicherer Standard               |
| TKIP     | veraltet, unsicher              |
| SAE      | moderner Authentifizierungsmechanismus (WPA3) |

```mermaid
flowchart LR
A[WLAN Zugriff] --> B[Authentifizierung WPA2/WPA3]
B --> C[Verschlüsselung AES/SAE]
C --> D[Sicherer Zugriff]
```

## Praktisches Beispiel

- Unternehmen:
  - WPA3-Enterprise + RADIUS-Server  
- Zuhause:
  - WPA2/WPA3-Personal mit starkem Passwort  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Welche WLAN-Standards sind sicher?  
- Unterschied WPA2 vs. WPA3  
- Welche Verschlüsselung wird verwendet?  

### Antworten auf die typischen Prüfungsfragen
- WPA2 und WPA3 (WPA unsicher)  
- WPA3 = moderner und sicherer  
- AES (modern), TKIP (veraltet), SAE (WPA3)  

## Merksatz
WPA2/WPA3 mit AES (und SAE bei WPA3) sorgen für ein sicheres WLAN.