---
# Identity (stable; never change after publishing)
id: ap1-0198
slug: udp-vs-tcp-vergleich

# Display
title: "UDP vs. TCP – Vergleich der Protokolle"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["protokolle", "transportprotokolle"]
tags: ["tcp", "udp", "vergleich", "netzwerkgrundlagen"]

# Flashcard payload
card:
  type: basic
  question: "Worin unterscheiden sich die Protokolle UDP und TCP?"
  answer: "UDP ist verbindungslos, schnell und hat einen kleinen Header von 8 Byte. Es bietet keine gesicherte Zustellung, keine Reihenfolgegarantie und keine erneute Übertragung verlorener Pakete. TCP ist verbindungsorientiert, hat einen größeren Header von mindestens 20 Byte und sorgt für zuverlässige Übertragung, Reihenfolge, Fehlerbehandlung und Verbindungssteuerung."
  examples:
    - "UDP → schnell, aber nicht zuverlässig garantiert"
    - "TCP → zuverlässiger, aber mit mehr Verwaltungsaufwand"
    - "UDP-Beispiele: DNS, VoIP, Streaming, Online-Gaming"
    - "TCP-Beispiele: HTTP/HTTPS, SSH, E-Mail-Übertragung"
    - "Merksatz: UDP = schnell und einfach, TCP = zuverlässig und kontrolliert"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## UDP vs. TCP – Vergleich der Protokolle

**UDP (User Datagram Protocol)** und **TCP (Transmission Control Protocol)** sind zwei zentrale **Transportprotokolle** im TCP/IP-Modell.

Sie unterscheiden sich hauptsächlich in:

- **Zuverlässigkeit**
- **Geschwindigkeit**
- **Funktionsumfang**

---

## Kernerklärung

### Vergleich UDP vs. TCP

| Eigenschaft | UDP | TCP |
|---|---|---|
| Headergröße | 8 Byte | 20 Byte |
| Geschwindigkeit | hoch | geringer |
| Paketverlusterkennung | nein | ja |
| Ende-zu-Ende-Kontrolle | nein | ja |
| Fehlerbehebung | nein | ja |
| Erkennung von Duplikaten | nein | ja |
| Flusskontrolle | nein | ja |
| Zeitüberwachung der Verbindung | nein | ja |

### Grundprinzip

- **UDP**
  - verbindungslos
  - keine Garantie für Zustellung
  - sehr schnell

- **TCP**
  - verbindungsorientiert
  - garantiert Reihenfolge und Zustellung
  - zuverlässiger, aber langsamer

```mermaid
flowchart LR
A[Transportprotokolle] --> B[UDP]
A --> C[TCP]

B --> D[Schnell, aber unzuverlässig]
C --> E[Langsamer, aber zuverlässig]
```

---

## Praktisches Beispiel

| Anwendung | Protokoll | Grund |
|---|---|---|
| Video-Streaming | UDP | Geschwindigkeit wichtiger als Perfektion |
| Online-Gaming | UDP | geringe Latenz entscheidend |
| Web (HTTP/HTTPS) | TCP | zuverlässige Übertragung notwendig |
| Dateiübertragung (FTP) | TCP | keine Datenverluste erlaubt |

---

## Prüfungsrelevanz (AP1)

Sehr häufiges Thema:

- Unterschiede **UDP vs. TCP**
- Eigenschaften zuordnen (z. B. „welches Protokoll hat Fehlerkontrolle?“)
- typische Einsatzgebiete

---

### Typische Prüfungsfragen

- Welches Protokoll ist schneller: UDP oder TCP?
- Welches Protokoll garantiert die Zustellung?
- Welche Funktionen bietet TCP, die UDP nicht hat?

---

### Antworten auf die typischen Prüfungsfragen

**Welches ist schneller?**  
→ **UDP**

**Welches garantiert Zustellung?**  
→ **TCP**

**Welche Zusatzfunktionen hat TCP?**  
→ Fehlerkontrolle, Reihenfolge, Flusskontrolle, Verbindungsüberwachung

---

## Merksatz

**UDP = schnell, aber unsicher.  
TCP = langsam, aber zuverlässig.**