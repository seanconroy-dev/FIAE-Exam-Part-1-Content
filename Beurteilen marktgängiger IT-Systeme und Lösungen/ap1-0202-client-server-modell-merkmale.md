---
# Identity (stable; never change after publishing)
id: ap1-0202
slug: client-server-modell-merkmale

# Display
title: "Client-Server-Modell – typische Merkmale"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["client-server", "architektur"]
tags: ["client-server", "netzwerkmodelle"]

# Flashcard payload
card:
  type: basic
  question: "Was sind typische Merkmale des Client-Server-Modells?"
  answer: "Beim Client-Server-Modell stellen Server Dienste oder Ressourcen bereit, die von Clients angefordert und genutzt werden. Die Kommunikation erfolgt über Netzwerkprotokolle. Ein Server kann mehrere Clients bedienen, und ein System kann je nach Aufgabe gleichzeitig Client und Server sein."
  examples:
    - "Webserver stellt Webseiten bereit, Browser ist der Client"
    - "Datenbankserver stellt Daten bereit, Anwendung fragt diese Daten ab"
    - "Dateiserver stellt Dateien für mehrere Clients bereit"
    - "Kommunikation erfolgt z. B. über HTTP, SMB oder SQL-Protokolle"
    - "Ein Rechner kann gleichzeitig Client und Server sein"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## Client-Server-Modell – typische Merkmale

Das **Client-Server-Modell** ist ein grundlegendes Konzept in Netzwerken.

- **Server** → bieten Dienste an  
- **Clients** → nutzen diese Dienste  

---

## Kernerklärung

### Typische Merkmale

| Merkmal | Beschreibung |
|---|---|
| Dienstebereitstellung | Server stellen Services bereit |
| Anfrageprinzip | Clients senden Anfragen |
| Kommunikation | erfolgt über definierte Protokolle |
| Mehrbenutzerfähigkeit | ein Server bedient mehrere Clients |
| Entkopplung | Funktionen sind nicht an Hardware gebunden |
| Rollenflexibilität | Systeme können Client und Server zugleich sein |

### Grundprinzip

- Client → Anfrage (Request)
- Server → Antwort (Response)

```mermaid
sequenceDiagram
Client->>Server: Anfrage (Request)
Server-->>Client: Antwort (Response)
```

---

## Praktisches Beispiel

Beim Surfen im Internet:

- Browser (Client) sendet Anfrage an Webserver
- Webserver liefert Webseite zurück

→ klassisches **Client-Server-Prinzip**

---

## Prüfungsrelevanz (AP1)

Sehr häufig gefragt:

- Rollen von Client und Server
- typische Merkmale aufzählen
- Beispiele nennen

---

### Typische Prüfungsfragen

- Was macht ein Server im Client-Server-Modell?
- Welche Rolle hat der Client?
- Nenne typische Merkmale dieses Modells.

---

### Antworten auf die typischen Prüfungsfragen

**Was macht der Server?**  
→ stellt Dienste bereit  

**Was macht der Client?**  
→ fordert Dienste an  

**Typische Merkmale?**  
→ Anfrage/Antwort, Protokolle, mehrere Clients, flexible Rollen  

---

## Merksatz

**Client fragt – Server antwortet.**