all: simple.tex simple.bib
	pdflatex simple
	bibtex simple
	pdflatex simple
	pdflatex simple

compress: simple.pdf
	gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dNOPAUSE -dQUIET -dBATCH -sOutputFile=tmp.pdf simple.pdf
	mv tmp.pdf simple.pdf
