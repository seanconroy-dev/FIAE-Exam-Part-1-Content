---
# Identity (stable; never change after publishing)
id: ap1-0221
slug: wlan-infrastructure-modus

# Display
title: "WLAN Infrastructure Mode: Bedeutung und Funktionsweise"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["WLAN", "Netzwerk", "Access Point"]
tags: ["ap1", "wlan", "grundlagen"]

# Flashcard payload
card:
  type: basic
  question: "Wie funktioniert ein WLAN Access Point im Infrastructure-Modus?"
  answer: "Im Infrastructure-Modus verbinden sich WLAN-Clients nicht direkt miteinander, sondern über einen Access Point. Der Access Point stellt die Verbindung zum kabelgebundenen Netzwerk her und ermöglicht den Zugriff auf Dienste wie Internet, Server oder Unternehmensnetzwerk. Die Authentifizierung erfolgt z. B. über WPA2, WPA3 oder RADIUS."
  examples:
    - "Notebook verbindet sich per WLAN mit dem Access Point"
    - "Access Point verbindet WLAN-Clients mit dem LAN"
    - "Clients kommunizieren über den Access Point, nicht direkt miteinander"
    - "In Unternehmen kann die Anmeldung über WPA2/WPA3-Enterprise mit RADIUS erfolgen"
    - "Infrastructure-Modus = WLAN mit zentralem Access Point"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## WLAN Infrastructure Mode: Bedeutung und Funktionsweise
Der **Infrastructure Mode** ist der Standardbetrieb eines WLANs.  
Dabei kommunizieren Clients **nicht direkt miteinander**, sondern immer über einen **Access Point (AP)**.

## Kernerklärung
Im Infrastructure Mode:

- Der **Access Point fungiert als zentrale Vermittlungsstelle**
- Clients verbinden sich mit dem AP
- Der AP stellt die Verbindung zu einem bestehenden Netzwerk her (z. B. LAN / Unternehmensnetz)

### Authentifizierung
Clients müssen sich anmelden:
- Benutzername/Passwort
- MAC-Adresse
- Verfahren:
  - WPA2 / WPA3
  - RADIUS (Enterprise)
  - WPS (unsicher, selten empfohlen)

### Ablauf
```mermaid
flowchart LR
A[Client] --> B[Access Point]
B --> C[Netzwerk / LAN]
C --> D[Server / Internet]
```

## Praktisches Beispiel
Ein Mitarbeiter verbindet sich mit dem Firmen-WLAN:

1. Laptop findet WLAN
2. Verbindung zum Access Point
3. Anmeldung mit Zugangsdaten
4. Zugriff auf Unternehmensnetz (z. B. Datei-Server)

➡️ Kommunikation läuft immer über den Access Point

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Was ist der Unterschied zwischen Infrastructure Mode und Ad-hoc?
- Welche Rolle hat der Access Point?
- Wie erfolgt die Authentifizierung im WLAN?

### Antworten auf die typischen Prüfungsfragen
- Infrastructure: zentral über AP / Ad-hoc: direkt zwischen Clients
- AP vermittelt zwischen WLAN und kabelgebundenem Netzwerk
- Authentifizierung über WPA2/WPA3, ggf. RADIUS

## Merksatz
**Im Infrastructure Mode ist der Access Point die zentrale Schnittstelle zwischen WLAN-Clients und dem Netzwerk.**