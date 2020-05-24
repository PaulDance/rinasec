default: report.tex
	latex report
	bibtex report
	latex report
	pdflatex report

clean:
	find . -not -name "report.tex" -not -name "report.bib" -not -name "Makefile" -not -name ".gitignore" -delete
