## LaTeX- Vorlage für Bachelor- und Master-Thesen

Abfolge für komplette Kompilierung inklusive Literatur- und Abkürzungs- sowie Symbolverzeichnis (wird z. B. TeXnicCenter eingesetzt, müssen diese Einstellungen dort entsprechend gesetzt werden):

    pdflatex -shell-escape thesis-doc.tex
    bibtex thesis-doc
    makeindex -s thesis-doc.ist thesis-doc.slo -o thesis-doc.sls
    makeindex -s thesis-doc.ist thesis-doc.acn -o thesis-doc.acr
    makeindex -s thesis-doc.ist thesis-doc.glo -o thesis-doc.gls
    makeindex -s thesis-doc.ist thesis-doc.slo -o thesis-doc.sls
    pdflatex -shell-escape thesis-doc.tex
    pdflatex -shell-escape thesis-doc.tex
