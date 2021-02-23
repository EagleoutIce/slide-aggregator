SHELL:= /bin/bash
CONTENTS = "Super\\\\PDF" "MEGA" "PDF3" "Halloo" "And\\\\Again" "Hyper-Daiper"

default: example clean-aux

example: generate-pdfs two-example.tex
	pdflatex two-example.tex
	pdflatex two-example.tex


build-pdfs: generate-pdfs clean-aux

generate-pdfs:	pdfs-creator.tex
	@n=0; \
	for content in $(CONTENTS); do \
		pdflatex -jobname "$$n" \\def\\content{$$content}\\input{pdfs-creator.tex}; \
		let "n+=1"; \
	done

clean-aux:
	rm {0..5}.aux {0..5}.log

.PHONY: generate-pdfs clean-aux build-pdfs example all