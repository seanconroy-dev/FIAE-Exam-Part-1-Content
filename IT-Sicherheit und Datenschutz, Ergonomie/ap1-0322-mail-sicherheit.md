---
# Identity (stable; never change after publishing)
id: ap1-0322
slug: "mail-sicherheit"

# Display
title: "Sicherheitsmaßnahmen bei E-Mail-Systemen"

# Classification / navigation (machine-side)
module: "IT-Sicherheit und Datenschutz, Ergonomie"
topics: ["email", "verschluesselung", "netzwerk"]
tags: ["ap1", "kommunikation", "sicherheit"]

# Flashcard payload
card:
  type: multi
  question: "Was muss beim sicheren Einsatz eines E-Mail-Systems beachtet werden?"
  answer: "Ein E-Mail-System sollte sichere Protokolle mit TLS nutzen, z. B. SMTPS, IMAPS oder POP3S. E-Mails können zusätzlich verschlüsselt und digital signiert werden, um Inhalte zu schützen und Absender zu prüfen. Außerdem sind Spam- und Virenschutz, sichere Passwörter, MFA, regelmäßige Updates und Vorsicht bei Anhängen und Links wichtig."
  examples:
    - "SMTP mit TLS: sichere Übertragung beim Versand"
    - "IMAPS: sicherer Zugriff auf das Postfach über TLS"
    - "POP3S: sicherer Abruf von E-Mails über TLS"
    - "Digitale Signatur: Empfänger kann den Absender und die Unverändertheit prüfen"
    - "E-Mail-Verschlüsselung: Inhalt kann nur von berechtigten Empfängern gelesen werden"
    - "Spam- und Virenfilter: Schutz vor Schadsoftware und Phishing"
    - "MFA: zusätzlicher Schutz für E-Mail-Konten"
    - "Merksatz: E-Mail-Sicherheit = TLS, Verschlüsselung, Signatur, Filter und vorsichtige Nutzer"

# Lifecycle
status: published       # draft | published | deprecated
created: "2026-03-28"
updated: "2026-05-12"
---

## Sicherheitsmaßnahmen bei E-Mail-Systemen
E-Mail-Systeme sind ein häufiges Ziel für Angriffe (z. B. Abhören, Manipulation).

Daher müssen beim Einsatz geeignete Sicherheitsmaßnahmen umgesetzt werden.

## Kernerklärung

### Wichtige Maßnahmen

- **Verschlüsselung & Signatur:**
  - E-Mails sollten **verschlüsselt** übertragen werden  
  - Digitale Signaturen sichern die **Authentizität**  

- **TLS/SSL einsetzen:**
  - Nutzung von sicheren Zertifikaten  
  - Schutz der Daten während der Übertragung  

### Sichere Ports

| Protokoll | Port | Sicherheit |
|----------|------|-----------|
| POP3     | 995  | SSL/TLS   |
| IMAP     | 993  | SSL/TLS   |
| SMTP     | 465 / 587 | SSL/TLS |

Unsichere (unverschlüsselte) Verbindungen sollten vermieden werden.

```mermaid
flowchart LR
    A[Client] -->|TLS/SSL| B[Mailserver]
    B -->|TLS/SSL| C[Empfänger]
```

## Praktisches Beispiel

Ein Unternehmen konfiguriert sein Mail-System:

- IMAP nur über Port 993  
- SMTP nur über Port 587  
- TLS-Zertifikate sind aktiv  

Ergebnis: Schutz vor Abhören und Manipulation von E-Mails.

## Prüfungsrelevanz (AP1)

### Typische Prüfungsfragen
- Welche Sicherheitsmaßnahmen gibt es für E-Mail-Systeme?  
- Welche Ports werden für sichere Mailprotokolle verwendet?  

### Antworten auf die typischen Prüfungsfragen
- Verschlüsselung, Signatur und TLS/SSL einsetzen  
- POP3: 995, IMAP: 993, SMTP: 465/587  

## Merksatz
**E-Mails nur verschlüsselt übertragen – sonst können sie mitgelesen werden.**