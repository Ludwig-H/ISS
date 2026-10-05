all: Percolia_Elaia_2026-10-06.pdf

LATEXCMD=xelatex
TEXENV=TEXINPUTS=.:theme//:latex-inria-fonts//:

main.pdf: main.tex
	$(TEXENV) $(LATEXCMD) -file-line-error -halt-on-error main.tex
	$(TEXENV) $(LATEXCMD) -file-line-error -halt-on-error main.tex

Percolia_Elaia_2026-10-06.pdf: main.pdf
	cp main.pdf $@

clean:
	@rm -f main.aux main.log main.nav main.out main.snm main.toc main.pdf main.fls main.fdb_latexmk main.xdv
