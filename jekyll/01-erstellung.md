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
Neue Zeile = am ende des Satze zwei Leerzeichen machen und dann ENTER
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

- Wenn Sie Github Pages + Jekyll + Kramdown + Just the Docs nutzen.
  - Kramdown unterstützt Attribute Lists: {: ... } direkt hinter dem Bild-Syntax.
- Bild größe ändern.
```
  ![ALT](./bild.jpg){:width="400" } => Breite genau 400px
  ![ALT](./bild.jpg){:height="300" } => Höhe genau 400px
  ![ALT](./bild.jpg){:width="50%" height="auto" } => 50% der Container Breite
```

- Position / Ausrichtung
```
  ![ALT](./bild.jpg){: .mx-auto .d-block } => Bild horizontal mittig
  ![ALT](./bild.jpg){: .float-right .ml-4 } => Bild fließt rechts, Text links drumherum
  ![ALT](./bild.jpg){: .float-left .mr-4 } => Bild fließt links, Text rechts drumherum
  ![ALT](./bild.jpg){: .ml-3 .mr-3 .mt-2 .mb-2 } => Margin left/right/top/bottom
  ![ALT](./bild.jpg){: .shadow .shadow-lg } => Leichter / starker Schatten
```
- Weitere nützliche Attribute
  - {: .rounded} => abgerundete Ecken
  - {: .border} => dünner Rahmen

### 6. Code
- Inline
```
Das ist `inline code` – gut für Befehle oder Dateinamen.
```

- Code-Block mit Syntax-Highlighting
````
```bash
  git add .
  git commit -m "Initial commit"
  git push origin main
```
````

- Beispiel

```python
  print("Hello World")
  for i in range(5):
    print(i)
```


### 8. Horizontale Linie
```
---
oder
***
```

