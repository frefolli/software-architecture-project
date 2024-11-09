REPORT=main

@all: ${REPORT}.pdf

${REPORT}.pdf: ${REPORT}.tex quotes.bib images/**/*.png images/*.png
	pdflatex ${REPORT}.tex
	bibtex ${REPORT}.aux
	pdflatex ${REPORT}.tex

clean:
	rm -rf *.idx ${REPORT}.pdf *-blx.bib *.aux *.log *.run.xml *.toc *.ilg *.ind *.bbl  *.blg *.out *.nav *.snm

edit:
	nvim ${REPORT}.tex
