3ainfo_2019.pdf:

all: 3ainfo_2019.pdf attendance.pdf

3ainfo_2019.pdf: 3atimetable_2019.tex

3atimetable.pdf: 3atimetable_2019.tex

%.tex: %.Rnw
	Rscript -e "library(knitr); knit('$*.Rnw')"
%.pdf: %.tex
	pdflatex $*
	pdflatex $*
clean:
	rm -f unnamed*
	rm -f *.{aux,tikz,out,log,blg,toc}
fresh: clean
	rm -f *.pdf
