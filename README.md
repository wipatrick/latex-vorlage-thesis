## LaTeX-Vorlage für Bachelor- und Master-Thesen

Abfolge für komplette Kompilierung inklusive Literatur- und Abkürzungs- sowie Symbolverzeichnis (wird z. B. TeXnicCenter eingesetzt, müssen diese Einstellungen dort entsprechend gesetzt werden):

    pdflatex -shell-escape thesis-doc.tex
    bibtex thesis-doc
    makeindex -s thesis-doc.ist thesis-doc.slo -o thesis-doc.sls
    makeindex -s thesis-doc.ist thesis-doc.acn -o thesis-doc.acr
    makeindex -s thesis-doc.ist thesis-doc.glo -o thesis-doc.gls
    makeindex -s thesis-doc.ist thesis-doc.slo -o thesis-doc.sls
    pdflatex -shell-escape thesis-doc.tex
    pdflatex -shell-escape thesis-doc.tex

## Was beinhaltet die Vorlage?
| N° | Feature       | Beschreibung                                                                                                                            |
|----|---------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| 1  | Aufbau        | Allgemeiner Aufbau einer wissenschaftlichen Arbeit                                                                                      |
| 2  | Verzeichnisse | Inhalts-, Tabellen-, Abbildungs-, Abkürzungs-, Symbol-, Literatur-VZ                                                                    |
| 3  | Tabelle       | Vorlage zur Erstellung einer Latex-Tabelle inkl. Tabellenfußnoten                                                                       |
| 4  | Abbildung     | Vorlage zum Einfügen einer Abbildung                                                                                                    |
| 5  | Pseudocode    | Vorlage zum Einfügen von Pseudo-Code                                                                                                    |
| 6  | Quelltext     | Vorlage zum Einfügen von Quelltext                                                                                                      |
| 7  | Zitieren      | Vorlage zur Referenzierung von Quellenangaben im [natdin-Stil](http://be-jo.net/2013/08/latex-welchen-bibliographystyle-wahlen/#natdin) |
