---
# Identity (stable; never change after publishing)
id: ap1-0230
slug: bluetooth-spezifikationen-reichweite-datenrate-frequenz

# Display
title: "Bluetooth: Reichweite, Datenrate und Frequenzbereich"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["bluetooth", "funktechnik"]
tags: ["ap1", "netzwerke", "drahtlos", "ism-band"]

# Flashcard payload
card:
  type: basic
  question: "Was sind typische technische Spezifikationen von Bluetooth hinsichtlich Reichweite, Datentransferrate und Frequenzbereich?"
  answer: "Bluetooth arbeitet im 2,4-GHz-ISM-Band, ungefähr von 2,402 bis 2,480 GHz. Die Reichweite hängt von der Leistungsklasse ab: Klasse 1 ca. 100 m, Klasse 2 ca. 10 m und Klasse 3 ca. 1 m. Die Datenrate hängt vom Bluetooth-Standard ab, z. B. Basic Rate ca. 1 MBit/s und Enhanced Data Rate bis ca. 2 bis 3 MBit/s."
  examples:
    - "Klasse 1 → ca. 100 m, hohe Sendeleistung"
    - "Klasse 2 → ca. 10 m, typisch für viele mobile Geräte"
    - "Klasse 3 → ca. 1 m, sehr geringe Reichweite"
    - "Frequenzbereich → 2,402 bis 2,480 GHz"
    - "Basic Rate → ca. 1 MBit/s"
    - "Enhanced Data Rate → bis ca. 2 bis 3 MBit/s"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## Bluetooth: Reichweite, Datenrate und Frequenzbereich

Bluetooth ist ein drahtloser Kommunikationsstandard im **ISM-Band**, der sich durch unterschiedliche Reichweitenklassen, Datenraten und Betriebsmodi (Classic vs. Low Energy) auszeichnet.

## Kernerklärung

### 1. Reichweite (abhängig von Sendeleistung)
| Klasse | Sendeleistung | Reichweite (typisch) |
|--------|--------------|----------------------|
| Klasse 1 | 100 mW (20 dBm) | ca. 100 m |
| Klasse 2 | 2,5 mW (4 dBm) | ca. 10 m |
| Klasse 3 | 1 mW (0 dBm) | ca. 1 m |

➡️ Höhere Leistung = größere Reichweite, aber höherer Energieverbrauch.

---

### 2. Datentransferrate
| Modus | Datenrate (brutto) |
|------|-------------------|
| Basic Rate (BR) | ca. 1 MBit/s |
| Enhanced Data Rate (EDR) | ca. 2–3 MBit/s |

➡️ EDR verbessert die Effizienz und Geschwindigkeit gegenüber BR.

---

### 3. Frequenzbereich
- **2,402 – 2,480 GHz**
- Lizenzfreies **ISM-Band**
- Nutzung von **Frequenzsprungverfahren (FHSS)** zur Störungsreduktion

---

### 4. Bluetooth-Versionen
- **Bluetooth Classic (1.x – 3.x)** → höhere Datenrate
- **Bluetooth Low Energy (BLE, ab 4.x)** → energieeffizient, geringere Datenrate

---

## Praktisches Beispiel
- **Bluetooth-Kopfhörer (Klasse 2)**  
  → Reichweite ca. 10–20 m, ausreichend für Wohnung

- **Industrieanwendung (Klasse 1)**  
  → größere Reichweite bis 100 m erforderlich

---

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Welche Reichweitenklassen gibt es bei Bluetooth?
- Welche Datenraten unterstützen BR und EDR?
- In welchem Frequenzbereich arbeitet Bluetooth?
- Warum nutzt Bluetooth das ISM-Band?

### Antworten auf die typischen Prüfungsfragen
- 3 Klassen: 1 (100 m), 2 (10 m), 3 (1 m)
- BR: 1 MBit/s, EDR: 2–3 MBit/s
- 2,402–2,480 GHz
- Lizenzfrei, weltweit nutzbar

---

## Merksatz
**Bluetooth = 2,4 GHz ISM-Band + Klassen für Reichweite + BR/EDR für Datenrate.**