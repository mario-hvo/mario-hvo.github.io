---
title: _config.yml erstellen
parent: Jekyll static site generator
nav_order: 2
---

# Die _config.yml Datei erstellen und konfigurieren

Die `_config.yml` ist die **zentralste Konfigurationsdatei** in Jekyll (und damit auch bei GitHub Pages mit Just the Docs).

Sie liegt immer direkt im Root deines Repositories (nicht in einem Unterordner).

### Schritt-für-Schritt: Datei anlegen

1. Öffne dein Repository lokal oder direkt auf GitHub.
2. Erstelle eine neue Datei namens genau `_config.yml` (Achtung: Unterstrich am Anfang, .yml am Ende).
3. Füge den Inhalt ein (Beispiel unten).
4. Commit & Push → GitHub Pages baut automatisch neu (kann 1–10 Minuten dauern).

### Minimal-Beispiel für Just the Docs
remote_theme: just-the-docs/just-the-docs  
title: Meine Bulme Web-Doku  
description: Grundlagen Webentwicklung – Bulme Projekt  
search_enabled: true             # true = Suchfeld oben aktiv, false = aus  
search.button: true              # Floating-Such-Button unten rechts


### Erklärung der wichtigsten Keys (was du wirklich nutzen kannst)

- remote_theme  
  Definiert das Theme von GitHub (remote_theme statt theme, weil du kein lokales Theme hast).  
  Beispiel: `remote_theme: just-the-docs/just-the-docs`

- title  
  Der Haupt-Titel deiner Site (erscheint oben links in der Sidebar).

- description  
  Kurze Beschreibung (Meta-Description für Suchmaschinen + Subtitle).

- search_enabled  
  `true` = Suchfunktion aktiv (empfohlen).  
  `false` = Suchfeld komplett aus.

- aux_links  
  Links oben rechts in der Navigationsleiste (z. B. zu deinem GitHub-Repo).


### Beliebte remote_themes (Stand März 2026 – alle GitHub Pages kompatibel)

- just-the-docs/just-the-docs               → Sehr gut für Doku
- cotes2020/jekyll-theme-chirpy             → Blog-ähnlich, mit Tags & Profil
- mmistakes/minimal-mistakes                → Sehr flexibel, aber mehr Konfig
- vaibhavvikas/jekyll-theme-minimalistic    → Sehr schlank, mit Sidebar
- Read the Docs                             → Auch sehr gut für Doku

Beispiel-Wechsel:  
`remote_theme: cotes2020/jekyll-theme-chirpy`

### Häufige Fehler & wie du sie vermeidest

- Datei heißt `_config.yaml` statt `_config.yml` → Jekyll ignoriert sie komplett.
- Falsche Einrückung im YAML (z. B. 2 statt 4 Leerzeichen) → Build-Fehler.
- `theme:` statt `remote_theme:` → funktioniert nur bei lokal installierten Themes.
