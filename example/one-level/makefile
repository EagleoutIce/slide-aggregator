SHELL:= /bin/bash
CONTENTS = "Super\\clearpage PDF" "MEGA" "PDF3" "Halloo"

default: example clean-aux

example: generate-pdfs one-example.tex
	pdflatex one-example.tex
	pdflatex one-example.tex


build-pdfs: generate-pdfs clean-aux

generate-pdfs:	pdfs-creator.tex
	@n=0; \
	for content in $(CONTENTS); do \
		pdflatex -jobname "$$n" \\def\\content{$$content}\\input{pdfs-creator.tex}; \
		let "n+=1"; \
	done

clean-aux:
	rm {0..3}.snm {0..3}.aux {0..3}.nav {0..3}.log {0..3}.toc {0..3}.out

.PHONY: generate-pdfs clean-aux build-pdfs example all