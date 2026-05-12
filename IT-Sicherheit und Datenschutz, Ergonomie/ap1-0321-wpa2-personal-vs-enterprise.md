---
# Identity (stable; never change after publishing)
id: ap1-0321
slug: "wpa2-personal-vs-enterprise"

# Display
title: "WPA2-Personal vs. WPA2-Enterprise"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["wlan", "verschluesselung", "authentifizierung"]
tags: ["ap1", "netzwerk", "sicherheit"]

# Flashcard payload
card:
  type: comparison
  question: "Welche Vor- und Nachteile haben WPA2-Personal und WPA2-Enterprise?"
  answer: "WPA2-Personal nutzt ein gemeinsames WLAN-Passwort. Es ist einfach einzurichten und gut für kleine Netzwerke geeignet, aber bei vielen Nutzern unsicherer und ein Passwortwechsel ist aufwendig. WPA2-Enterprise nutzt eine zentrale Authentifizierung, meist über RADIUS. Es ist sicherer und besser verwaltbar, benötigt aber mehr Aufwand und zusätzliche Infrastruktur."
  examples:
    - "WPA2-Personal Vorteil: einfach einzurichten"
    - "WPA2-Personal Vorteil: gut für Heimnetzwerke oder kleine Büros"
    - "WPA2-Personal Nachteil: alle Nutzer verwenden dasselbe WLAN-Passwort"
    - "WPA2-Personal Nachteil: Passwortwechsel muss auf allen Geräten durchgeführt werden"
    - "WPA2-Enterprise Vorteil: jeder Nutzer kann eigene Zugangsdaten verwenden"
    - "WPA2-Enterprise Vorteil: zentrale Verwaltung und höhere Sicherheit"
    - "WPA2-Enterprise Nachteil: RADIUS-Server oder ähnliche Infrastruktur nötig"
    - "WPA2-Enterprise Nachteil: Einrichtung und Verwaltung sind aufwendiger"
    - "Merksatz: Personal = gemeinsames Passwort, Enterprise = zentrale Anmeldung"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-27"
updated: "2026-05-12"
---

## WPA2-Personal vs. WPA2-Enterprise
WPA2 ist ein Sicherheitsstandard für WLAN-Netzwerke.

Es gibt zwei Varianten:
- **WPA2-Personal (PSK)**
- **WPA2-Enterprise**

Beide unterscheiden sich vor allem in Sicherheit und Verwaltungsaufwand.

## Kernerklärung

### Vergleich WPA2-Personal vs. WPA2-Enterprise

| Kriterium            | WPA2-Personal (PSK)                  | WPA2-Enterprise                  |
|----------------------|-------------------------------------|----------------------------------|
| Authentifizierung     | gemeinsames Passwort                | individuelle Zugangsdaten        |
| Sicherheit            | geringer bei vielen Nutzern         | sehr hoch                        |
| Verwaltung            | einfach                             | zentral (z. B. über Server)      |
| Einsatz               | kleine Netzwerke / Zuhause          | Unternehmen / Organisationen     |

### Vorteile & Nachteile

#### WPA2-Personal
**Vorteile:**
- leicht zu implementieren  
- weit verbreitet  

**Nachteile:**
- unsicher in größeren Umgebungen (Passwort bekannt)  
- Passwortwechsel für alle Geräte aufwendig  

#### WPA2-Enterprise
**Vorteile:**
- sehr hohe Sicherheit  
- zentrale Verwaltung von Nutzern und Geräten  

**Nachteile:**
- hoher technischer Aufwand  
- zusätzlicher Server (z. B. RADIUS) notwendig  

```mermaid
flowchart LR
    A[WPA2] --> B[Personal]
    A --> C[Enterprise]
    B --> D[Ein Passwort für alle]
    C --> E[Individuelle Nutzerkonten]
```

## Praktisches Beispiel

- **WPA2-Personal:**  
  Heim-WLAN → ein gemeinsames WLAN-Passwort für alle Geräte  

- **WPA2-Enterprise:**  
  Firmen-WLAN → jeder Mitarbeiter hat eigene Zugangsdaten  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Unterschied zwischen WPA2-Personal und Enterprise?  
- Nenne Vor- und Nachteile beider Varianten  

### Antworten auf die typischen Prüfungsfragen
- Personal: einfach, aber unsicher bei vielen Nutzern  
- Enterprise: sicher, aber aufwendig (z. B. RADIUS notwendig)  

## Merksatz
**WPA2-Personal = einfach, WPA2-Enterprise = sicher.**