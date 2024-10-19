.PHONY = all clean

all: ecfaTemplate.pdf

SOURCES := ecfaTemplate.tex preamble.tex $(wildcard sections/*.tex) $(wildcard sections/introduction/*.tex)

ecfaTemplate.pdf: $(SOURCES)
#	mkdir -p .$@.build
#	cd .$@.build && latexmk -pdf ../$< && cp $@ ../
	latexmk -pdf $<

clean:
	latexmk -C
