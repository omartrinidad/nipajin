# (c) 2009-2016 by Markus Leupold-Löwenthal
# This file is released under CC BY-SA 4.0. Please do not apply other licenses one-way.

PDF_NAME="NIPAJIN"
TEX_NAME="nipajin"

default: de

all: de pl en es

setup:
	mkdir -p out

de: setup
	ln -sf ../content.de.tex out/content.tex
	xelatex -output-driver="xdvipdfmx -V 5 -z 9" -jobname=${PDF_NAME}-de -output-directory out ${TEX_NAME}

en: setup
	ln -sf ../content.en.tex out/content.tex
	xelatex -output-driver="xdvipdfmx -V 5 -z 9" -jobname=${PDF_NAME}-en -output-directory out ${TEX_NAME}

es: setup
	ln -sf ../content.es.tex out/content.tex
	xelatex -output-driver="xdvipdfmx -V 5 -z 9" -jobname=${PDF_NAME}-es -output-directory out ${TEX_NAME}

pl: setup
	ln -sf ../content.pl.tex out/content.tex
	xelatex -output-driver="xdvipdfmx -V 5 -z 9" -jobname=${PDF_NAME}-pl -output-directory out ${TEX_NAME}

clean:
	rm -rf out/*
