all: Percolia_Board_meeting_1_2026-10-02.pdf

LATEXCMD=xelatex
TEXENV=TEXINPUTS=.:theme//:latex-inria-fonts//:

main.pdf: main.tex
	$(TEXENV) $(LATEXCMD) -file-line-error -halt-on-error main.tex
	$(TEXENV) $(LATEXCMD) -file-line-error -halt-on-error main.tex

Percolia_Board_meeting_1_2026-10-02.pdf: main.pdf
	cp main.pdf $@

clean:
	@rm -f main.aux main.log main.nav main.out main.snm main.toc main.pdf main.fls main.fdb_latexmk main.xdv
