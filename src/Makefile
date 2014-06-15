all: main.pdf

main.pdf: main.tex
	pdflatex main  
	bibtex main
	pdflatex main
#	pdflatex main

clean:
	@rm -f *log *aux *out *blg *bbl *toc *brf *bcf *idx main.run.xml main.fdb_latexmk main.fls
	@find . -name "*.aux" | xargs rm

pristine: clean
	@rm -f main.pdf
