HTMLS := $(patsubst %.tex,%.htm,$(wildcard *.tex))

default: touch $(HTMLS)

pdf:
	xelatex --interaction nonstopmode ladder.to.akanishta.tex

touch:
	touch *.tex

%.htm: %.tex
	hevea "$<" -o "$@"
