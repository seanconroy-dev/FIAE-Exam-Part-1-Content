---
# Identity (stable; never change after publishing)
id: ap1-0204
slug: mailprotokolle-imaps-smtps-pop3s-vergleich

# Display
title: "Mailprotokolle – IMAPS, SMTPS und POP3S"

# Classification / navigation (machine-side)
module: "Beurteilen marktgängiger IT-Systeme und Lösungen"
topics: ["mailprotokolle", "anwendungsprotokolle"]
tags: ["smtp", "imap", "pop3", "tls", "email"]

# Flashcard payload
card:
  type: comparison
  question: "Wie unterscheiden sich die Mailprotokolle IMAPS, SMTPS und POP3S in ihren Eigenschaften?"
  answer: "SMTPS dient dem sicheren Versand von E-Mails, typischerweise über Port 465 mit SSL/TLS. IMAPS dient dem sicheren Zugriff auf E-Mails auf dem Mailserver und synchronisiert Postfächer, typischerweise über Port 993. POP3S dient dem sicheren Abruf bzw. Download von E-Mails vom Server, typischerweise über Port 995, oft mit lokaler Speicherung."
  examples:
    - "SMTPS → E-Mails sicher senden"
    - "IMAPS → E-Mails auf dem Server lesen und synchronisieren"
    - "POP3S → E-Mails sicher vom Server abrufen"
    - "Port 465 → SMTPS"
    - "Port 993 → IMAPS"
    - "Port 995 → POP3S"
    - "Hinweis: Für SMTP-Versand wird auch Port 587 mit STARTTLS verwendet"

# Lifecycle
status: published
created: "2026-03-17"
updated: "2026-05-06"
---

## Mailprotokolle – IMAPS, SMTPS und POP3S

E-Mail-Kommunikation basiert auf verschiedenen Protokollen:

- **SMTP(S)** → Versand  
- **IMAP(S)** → Zugriff & Synchronisation  
- **POP3(S)** → Abruf & Download  

Die „S“-Varianten nutzen **SSL/TLS** für sichere Übertragung.

---

## Kernerklärung

### Vergleich der Mailprotokolle

| Protokoll | Aufgabe | Port | Besonderheit |
|---|---|---|---|
| SMTPS | Versand von E-Mails | 465 | Authentifizierung + verschlüsselte Übertragung |
| IMAPS | Zugriff auf Mails | 993 | Mails bleiben auf Server, Synchronisation |
| POP3S | Abruf von Mails | 995 | Mails werden heruntergeladen (oft lokal gespeichert) |

### Funktionsprinzip

```mermaid
flowchart LR
Client -->|"SMTP(S)"| MailServer
MailServer -->|"IMAP(S)/POP3(S)"| Client
```

- **SMTP(S)**: Client → Server (Senden)  
- **IMAP(S)/POP3(S)**: Server → Client (Empfangen)

---

## Praktisches Beispiel

- Du sendest eine Mail → **SMTP(S)**
- Du liest Mails auf mehreren Geräten → **IMAP(S)**
- Du lädst Mails lokal auf PC → **POP3(S)**

---

## Prüfungsrelevanz (AP1)

Sehr häufig geprüft:

- Unterschied **IMAP vs. POP3**
- Funktion von SMTP
- Standard-Ports und Einsatz

---

### Typische Prüfungsfragen

- Welches Protokoll wird zum Versenden von E-Mails genutzt?
- Unterschied IMAP und POP3?
- Welche Ports verwenden die sicheren Varianten?

---

### Antworten auf die typischen Prüfungsfragen

**Versand?**  
→ SMTP(S)  

**IMAP vs. POP3?**  
→ IMAP synchronisiert, POP3 lädt herunter  

**Ports?**  
→ 465 (SMTP), 993 (IMAP), 995 (POP3)  

---

## Merksatz

**SMTP sendet, IMAP synchronisiert, POP3 lädt herunter.**