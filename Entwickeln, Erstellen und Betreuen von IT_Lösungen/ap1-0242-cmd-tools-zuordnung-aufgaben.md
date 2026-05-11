---
# Identity (stable; never change after publishing)
id: ap1-0242
slug: cmd-tools-zuordnung-aufgaben

# Display
title: "CMD-Tools und ihre Aufgaben – Zuordnung"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "Diagnose", "CMD"]
tags: ["ap1", "cmd", "tools", "netzwerk"]

# Flashcard payload
card:
  type: basic
  question: "Ergänze die passenden Windows-CMD-Tools: IP-Konfiguration anzeigen -> ___, Erreichbarkeit testen -> ___, DNS pruefen -> ___, ARP-Tabelle anzeigen -> ___, erweiterte Netzwerk-/Firewall-Konfiguration -> ___."
  answer: |
    Zuordnung der Aufgaben zu den passenden CMD-Tools:

    - IP-Konfiguration anzeigen -> ipconfig
    - Erreichbarkeit testen -> ping
    - DNS pruefen -> nslookup
    - ARP-Tabelle anzeigen -> arp
    - Erweiterte Netzwerk-/Firewall-Konfiguration -> netsh
  examples:
    - "ipconfig /all → detaillierte Adapter-, IP-, DHCP- und DNS-Informationen anzeigen"
    - "ping www.google.de → Erreichbarkeit prüfen"
    - "nslookup www.google.de → DNS-Auflösung prüfen"
    - "arp -a → ARP-Tabelle anzeigen"
    - "netsh advfirewall show allprofiles → Firewall-Profile anzeigen"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## CMD-Tools und ihre Aufgaben – Zuordnung
In Windows gibt es verschiedene Kommandozeilen-Tools zur Analyse und Konfiguration von Netzwerken.

Jedes Tool hat einen spezifischen Zweck.

## Kernerklärung

### Zuordnung der Tools zu Aufgaben

| Aufgabe | Tool |
|--------|------|
| Konfiguration des Netzwerkadapters anzeigen | ipconfig |
| MAC-Adresse des eigenen PCs anzeigen | ipconfig |
| IPv4/IPv6 ermitteln | ipconfig |
| DHCP-Status prüfen | ipconfig |
| Hostname anzeigen | ipconfig |
| Erreichbarkeit prüfen | ping |
| DNS-Auflösung prüfen | nslookup |
| Status der Verbindung prüfen | ping |
| MAC-Adressen im Netzwerk ermitteln | arp |
| Firewall-Regel hinzufügen | netsh |

### Tool-Übersicht

- **ipconfig**
  - zeigt IP-Adresse, Subnetz, Gateway
  - zeigt DHCP-Informationen
- **ping**
  - testet Netzwerkverbindung
- **nslookup**
  - überprüft DNS-Auflösung
- **arp**
  - zeigt MAC-Adressen im lokalen Netzwerk
- **netsh**
  - Konfiguration von Netzwerk und Firewall

```mermaid
flowchart LR
A[Problem im Netzwerk] --> B[ipconfig prüfen]
B --> C[ping testen]
C --> D[nslookup prüfen]
D --> E[arp analysieren]
E --> F[netsh konfigurieren]
```

## Praktisches Beispiel

```bash
ipconfig /all
```
Zeigt:
- IP-Adresse
- MAC-Adresse
- DHCP-Status

```bash
ping www.t-online.de
```
- prüft Erreichbarkeit einer Website

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Welches Tool zeigt die IP-Adresse?
- Wie prüft man DNS?
- Welches Tool zeigt MAC-Adressen im Netzwerk?

### Antworten auf die typischen Prüfungsfragen
- ipconfig  
- nslookup  
- arp  

## Merksatz
ipconfig zeigt Daten, ping testet Verbindung, nslookup prüft DNS, arp zeigt MACs, netsh konfiguriert Netzwerk.