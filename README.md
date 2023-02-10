# LaTex Script zum rendern der Satzung und Ordnungen als Pdf

## LaTex installieren

sudo apt install latexmk texlive-latex-extra texlive-fonts-extra

## Pdf Rendern

### Dieses Repository lokal clonen

```sh
git clone ...
```

### Satzungs und Ordnungstexte im submodule aus dem externen Repository aktualisieren

```sh
git submodule update --remote --merge
```

### Pdf erzeugen

Um das Inhaltsverzeichnis und die Seitenzahlen korrekt zu erstellen, sollten die Befehle nach Änderungen in den Texten doppelt ausgeführt werden.

```sh
pdflatex --shell-escape ./renderSatzung.tex
```

oder

```sh
pdflatex --shell-escape ./renderOrdnungen.tex
```
