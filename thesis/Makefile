FILENAME=thesis

all: clean thesis.pdf

thesis.pdf: $(FILENAME).tex
	xelatex $^
	bibtex $(FILENAME)
	xelatex $^
	xelatex $^

edit:
	texmaker $(FILENAME).tex &

clean:
	@rm -f *.bcf *.lot *.fls *.toc *.lof *.fdb_latexmk \
	*.dvi *.aux *.log *.ps *.pdf *.out $(FILENAME).bbl \
	$(FILENAME).blg *.gz
