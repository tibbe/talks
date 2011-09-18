TARGET = slides.pdf

all: $(TARGET)

clean:
	rm -f *.aux *.dvi *.log *.nav *.out *.snm *.toc *.pdf *.vrb *.hi *.o *.prof

distclean: clean
	rm -f $(TARGET)

pdf: all
	open $(TARGET)

%.pdf: %.tex
	xelatex -file-line-error $<

.PHONY: all clean distclean pdf
