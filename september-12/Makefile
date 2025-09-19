LATEXCMD = pdflatex -shell-escape -output-directory build

name=main


$(name).pdf: $(name).tex | build
	$(LATEXCMD) $(name).tex
	cp build/$(name).pdf $(name).pdf

build:
	mkdir -p build

clean:
	$(RM) build/*

