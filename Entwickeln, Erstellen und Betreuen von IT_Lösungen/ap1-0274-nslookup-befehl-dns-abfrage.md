---
# Identity (stable; never change after publishing)
id: ap1-0274
slug: nslookup-befehl-dns-abfrage

# Display
title: "nslookup – DNS-Abfrage"

# Classification / navigation (machine-side)
module: "Entwickeln, Erstellen und Betreuen von IT_Lösungen"
topics: ["Netzwerk", "DNS", "Diagnose"]
tags: ["ap1", "nslookup", "dns", "netzwerk"]

# Flashcard payload
card:
  type: definition
  question: "Mit welchem Kommando prüft man DNS-Informationen?"
  answer: "Mit nslookup können DNS-Informationen abgefragt werden. Der Befehl zeigt z. B., welche IP-Adresse zu einem Domainnamen gehört. Er kann auch helfen zu prüfen, ob ein DNS-Server richtig antwortet."
  examples:
    - "nslookup google.de"
    - "Domainname wird in eine IP-Adresse aufgelöst"
    - "Prüfung, ob ein DNS-Server erreichbar ist"
    - "Fehlersuche bei Namensauflösungsproblemen"
    - "Reverse Lookup: IP-Adresse kann einem Namen zugeordnet werden"
    - "Merksatz: nslookup = DNS-Abfrage über die Kommandozeile"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-18"
updated: "2026-05-11"
---

## nslookup – DNS-Abfrage
Der Befehl **nslookup** wird verwendet, um **DNS-Abfragen** durchzuführen und die Namensauflösung zu testen.

## Kernerklärung

- nslookup dient zur:
  - **Auflösung von Domainnamen → IP-Adressen**
  - **Auflösung von IP-Adressen → Domainnamen**
- Nutzt einen **DNS-Server** (z. B. Router oder externer DNS)
- Ausgabe zeigt:
  - verwendeten DNS-Server  
  - abgefragte Adresse  
  - Ergebnis der Namensauflösung  

```mermaid
flowchart LR
A[Client] --> B[DNS Anfrage]
B --> C[DNS Server]
C --> D[IP-Adresse]
D --> A
```

## Praktisches Beispiel

```bash
nslookup fritz.box
```

Ergebnis:
- DNS-Server: z. B. 192.168.0.1  
- Rückgabe:
  - Name: fritz.box  
  - Address: 192.168.0.1  

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Wofür wird nslookup verwendet?  
- Was ist DNS?  
- Welche Informationen liefert nslookup?  

### Antworten auf die typischen Prüfungsfragen
- Zur Überprüfung der Namensauflösung  
- DNS übersetzt Namen in IP-Adressen  
- Server, Name und IP-Adresse  

## Merksatz
nslookup fragt den DNS – Name rein, IP raus.