default: report.tex
	pdflatex report
	bibtex report
	pdflatex report
	pdflatex report

clean:
	find . -not -name "*.png" -not -name "report.tex" -not -name "report.bib" -not -name "Makefile" -not -name ".gitignore" -delete
