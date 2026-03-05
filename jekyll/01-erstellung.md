---
title: Erstellung einer Seite
parent: Jekyll static site generator
nav_order: 1
---
# Was ist Markdown?

Markdown ist eine **leicht lesbare Auszeichnungssprache** (lightweight markup language), die 2004 von John Gruber entwickelt wurde.  
Ziel: Man schreibt Text fast wie normalen Fließtext, kann aber mit wenigen Zeichen Formatierungen hinzufügen, die später in HTML umgewandelt werden.

Markdown wird überall verwendet:
- GitHub (README, Issues, Pull Requests, Wikis)
- GitLab, Bitbucket
- Viele Doku-Tools (MkDocs, Jekyll, Hugo, Docusaurus)
- Editoren mit Vorschau (VS Code, Typora, Obsidian)
- Foren (Reddit, Discord, Stack Overflow)

Dateiendung: meist `.md` oder `.markdown`

## Die wichtigsten Markdown-Elemente

### 1. Überschriften

```markdown
# Überschrift Ebene 1 (H1)
## Überschrift Ebene 2 (H2)
### Überschrift Ebene 3 (H3)
#### Überschrift Ebene 4 (H4)
``` 

### 2. Textformatierung (Inline)
```
**fett**     oder     __fett__
*kursiv*    oder     _kursiv_
~durchgestrichen~~
**fett und _kursiv_ kombiniert**
```

### 3. Listen (Leerzeichen nach -+*)
- Ungeordnete Listen
```
  -Erster Punkt
  -Zweiter Punkt
    -Unterpunkt (4 Leerzeichen oder Tab einrücken)
  *Auch mit Stern möglich
  +Oder mit Plus
```

- Geordnete Listen
```
  1.Erster Punkt
  2.Zweiter Punkt
     1.Unterpunkt
  3.Dritter Punkt
```

### 4. Links
```
[GitHub Pages Dokumentation](https://docs.github.com/en/pages)

[Link mit Tooltip](https://example.com "Das ist ein Tooltip")
```

### 5. Bilder
```
![Alternativer Text](https://example.com/bild.jpg)

![Jekyll Logo](https://jekyllrb.com/img/logo-2x.png "Jekyll Logo")

![Lokales Bild](./assets/images/screenshot.png)
```

### 6. Code
- Inline
Das ist `inline code` – gut für Befehle oder Dateinamen.
  - Dies macht man mit Backticks nur eines davon, hinten und vorne von dem Wort was man möchte.

- Code-Block mit Syntax-Highlighting
```bash
  git add .
  git commit -m "Initial commit"
  git push origin main
```

### 8. Horizontale Linie
```
---
oder
***
```

