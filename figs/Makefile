all: translator-pet.mmd.pdf translator-polly.mmd.pdf
	latexmk *.tex

%.mmd.pdf: %.mmd
	mmdc -i $< -o $@ --pdfFit

clean:
	latexmk -c *.tex

cleanall:
	latexmk -C *.tex
	rm *.mmd.pdf
