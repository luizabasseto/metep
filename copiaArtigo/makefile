LATEX_FILE = artigo
PDF_FILE = $(LATEX_FILE).pdf

all: $(PDF_FILE)

$(PDF_FILE): $(LATEX_FILE).tex references.bib
	pdflatex $(LATEX_FILE)
	bibtex $(LATEX_FILE)
	pdflatex $(LATEX_FILE)
	pdflatex $(LATEX_FILE)

clean:
	rm -f *.aux *.bbl *.blg *.log *.out

.PHONY: all clean