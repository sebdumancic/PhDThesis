# Autogenerated Makefile, Mon May 21 13:31:26 CEST 2018.

MAINDIR = /Users/seb/Desktop/thesis/main

.PHONY: preface.pdf
preface.pdf: 
	( cd "$(MAINDIR)" && make chapters/preface/$@ )

.PHONY: bare preface_bare.pdf
bare: preface_bare.pdf
preface_bare.pdf: 
	( cd "$(MAINDIR)" && make chapters/preface/$@ )

.PHONY: image
image: 
	@if [ -f image/Makefile ]; then (cd image  && make); \
		else echo No Makefile found for /Users/seb/Desktop/thesis/main/image ...; fi;

.PHONY: figurelist
figurelist:
	@( cd $(MAINDIR) && make --no-print-directory $@ TEXFILE=chapters/preface/preface.tex )

.PHONY: clean
clean:
	$(RM) $(foreach ext, .toc .aux .log .bbl .blg .log .lof .lot .ilg .out .glo .gls .nlo .nls .brf .ist .glg .synctex.gz .tgz .idx .ind -blx.bib .fdb_latexmk .run.xml .bcf, $(wildcard preface*$(ext)))

.PHONY: realclean
realclean: clean
	$(RM) preface.pdf preface_bare.pdf

s:
	@echo gvim preface.tex allpapers.bib > $@
	@chmod +x $@
	@echo You can now start using ./s
