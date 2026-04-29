# FIAE-Exam-Part-1-Content (Content Repository)

This repository contains the **source learning content** (Markdown cards + assets) for AP1 exam preparation.

It is consumed by:
- the **backend API** (which reads/parses these Markdown files and exposes JSON)
- the **frontend** ([seanconroy-dev/FIAE-Exam-Part-1-Learning](https://github.com/seanconroy-dev/FIAE-Exam-Part-1-Learning)) which fetches cards from the backend endpoint:
  - `GET /api/cards/markdown`

---

## Assets

Repository assets (used by README and/or cards) live in:

- `assets/Preview_final.gif`
- `assets/FrontPage.png`

Use stable links for embedding where needed (example, pinned to a commit):

- [`https://raw.githubusercontent.com/seanconroy-dev/FIAE-Exam-Part-1-Content/<commit-sha>/assets/Preview_final.gif`](https://raw.githubusercontent.com/seanconroy-dev/FIAE-Exam-Part-1-Content/<commit-sha>/assets/Preview_final.gif)
- [`https://raw.githubusercontent.com/seanconroy-dev/FIAE-Exam-Part-1-Content/<commit-sha>/assets/FrontPage.png`](https://raw.githubusercontent.com/seanconroy-dev/FIAE-Exam-Part-1-Content/<commit-sha>/assets/FrontPage.png)

---

## Folder Structure (Modules)

Top-level folders represent AP1 modules (must match `module:` in frontmatter), for example:
- `Plannen,Vorbereiten und Durchführen von Arbeitsaufgaben/`
- `Informieren und Beraten von Kunden und Kundinnen/`
- `Beurteilen marktgängiger IT-Systeme und Lösungen/`
- `Entwickeln, Erstellen und Betreuen von IT_Lösungen/`
- `Qualitätssichernde Maßnahmen/`
- `IT-Sicherheit und Datenschutz, Ergonomie/`
- `Auftragsabschluss und Leistungenerbringen/`

---

## Frontmatter Template (Immutable)

Each learning card uses a fixed YAML frontmatter.  
This schema is stable and must not be changed after publication.

```yaml
# Identity (stable; never change after publishing)
id: ap1-0000
slug: ""

# Display
title: ""

# Classification / navigation (machine-side)
module: ""          # must match one top-level folder name exactly
topics: []          # e.g. ["Netzwerke", "OSI"]
tags: []            # e.g. ["exam-relevant", "definition"]

# Flashcard payload
card:
  type: basic       # basic | multi | steps | definition | comparison
  question: ""
  answer: ""
  examples: []      # optional

# Lifecycle
status: draft       # draft | published | deprecated
created: "2026-03-10"
updated: "2026-03-10"
```

---

## File Name Convention

Files follow a strict naming pattern:

    <module-folder>/ap1-0001-<slug>.md

Rules:
- The **ID in the filename must match the ID in the frontmatter**
- The **slug should be short, unique, and lowercase**
- Words must be separated by **hyphens**

---

## Note Style Guidelines

- Language: **German**
- Style: **precise, neutral, exam-oriented**
- No conversational tone
- Prefer **short paragraphs and bullet points**
- Use tables for **comparisons or classifications**
- Use **Mermaid diagrams** for processes and relationships
