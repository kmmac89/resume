TEX = pandoc
src = template.tex resume.yml
FLAGS = --pdf-engine=xelatex

output.pdf : $(src)
	$(TEX) $(filter-out $<,$^ ) -f markdown -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm output.pdf	
