THESIS_FILE=thesis
THESIS_COVER=outer_cover
EXAMPLE=example

all: thesis.pdf

$(THESIS_FILE).pdf: $(THESIS_FILE).tex
	xelatex $^
	bibtex $(THESIS_FILE)
	xelatex $^
	xelatex $^

cover: $(THESIS_COVER).pdf

$(THESIS_COVER).pdf: $(THESIS_COVER).tex
	xelatex $^

example: $(EXAMPLE).pdf

$(EXAMPLE).pdf: $(EXAMPLE).tex
	xelatex $^
	bibtex $(EXAMPLE)
	xelatex $^
	xelatex $^

edit:
	texmaker $(THESIS_FILE).tex &

clean:
	@rm -f *.bcf *.lot *.fls *.toc *.lof *.fdb_latexmk \
	*.dvi *.aux *.log *.ps *.pdf *.out *.bbl *.blg *.gz
