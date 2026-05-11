---
# Identity (stable; never change after publishing)
id: ap1-0267
slug: wlan-sicherheitsmassnahmen

# Display
title: "WLAN-Sicherheit – Schutzmaßnahmen"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "Sicherheit", "WLAN"]
tags: ["ap1", "wlan", "sicherheit", "netzwerk"]

# Flashcard payload
card:
  type: multi
  question: "Welche Maßnahmen eignen sich zur Absicherung eines WLANs?"
  answer: "Ein WLAN kann durch WPA2- oder WPA3-Verschlüsselung, ein starkes WLAN-Passwort, sichere Authentifizierung, regelmäßige Updates und getrennte Gastnetzwerke abgesichert werden. In Unternehmen werden zusätzlich oft RADIUS-Server, Client-Zertifikate oder VPN-Verbindungen genutzt. MAC-Filter bieten nur geringen Zusatzschutz, da MAC-Adressen gefälscht werden können."
  examples:
    - "Privat: WPA2 oder WPA3 mit starkem Passwort verwenden"
    - "Privat: Router-Firmware regelmäßig aktualisieren"
    - "Privat: separates Gast-WLAN für Besucher einrichten"
    - "Unternehmen: WLAN-Anmeldung über RADIUS-Server"
    - "Unternehmen: Client-Zertifikate für Geräte verwenden"
    - "Unternehmen: VPN für zusätzliche Absicherung nutzen"
    - "Hinweis: MAC-Filter sind nur Zusatzschutz, keine starke Sicherheit"
    - "Merksatz: WLAN absichern = verschlüsseln, stark authentifizieren, aktuell halten"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## WLAN-Sicherheit – Schutzmaßnahmen
Ein WLAN muss gegen unbefugten Zugriff geschützt werden, da es **drahtlos und damit leichter angreifbar** ist als kabelgebundene Netzwerke.

## Kernerklärung

Typische Sicherheitsmaßnahmen:

- **Verschlüsselung**
  - WPA2 / WPA3  
- **Authentifizierung**
  - z. B. über RADIUS-Server  
- **Zugriffskontrolle**
  - MAC-Filter (Whitelist)  
- **Zertifikate**
  - Client-Zertifikate zur Identitätsprüfung  
- **Sichere Verbindungen**
  - Nutzung von VPN  

```mermaid
flowchart LR
A[Client verbindet sich] --> B[Authentifizierung]
B --> C[Verschlüsselung aktiv]
C --> D[Zugriff erlaubt]
```

## Praktisches Beispiel

- Unternehmen:
  - WPA3 + RADIUS für Mitarbeiter  
  - Gäste-WLAN getrennt  

- Privathaushalt:
  - WPA2/WPA3 aktivieren  
  - starkes Passwort setzen  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Nenne Maßnahmen zur WLAN-Sicherung  
- Warum ist WPA3 besser als WPA2?  
- Welche Rolle spielt RADIUS?  

### Antworten auf die typischen Prüfungsfragen
- Verschlüsselung, Authentifizierung, Zugriffskontrolle  
- höhere Sicherheit, moderner Standard  
- zentrale Benutzerverwaltung  

## Merksatz
Ein sicheres WLAN braucht Verschlüsselung, Authentifizierung und Zugriffskontrolle.