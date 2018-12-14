OBJECTS = EDM_report_2019 EDM_report_2018
TARGETS = $(addsuffix .pdf, $(OBJECTS))
SOURCES = $(addsuffix .tex, $(OBJECTS))


all: $(TARGETS)

%.pdf: %.tex
	latexmk -pdf -pdflatex="pdflatex -interaction=nonstopmode" -use-make $<

clean:
	latexmk -c

.PHONY: clean 
