all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_labo1" Elec-3BS-3BM_labo1.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_labo1" Elec-3BS-3BM_labo1.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_labo1_correction "\def\koriG{} \input{Elec-3BS-3BM_labo1.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_labo1_correction "\def\koriG{} \input{Elec-3BS-3BM_labo1.tex}"
	
clean:
	rm -f Elec-3BS-3BM_labo1_correction.pdf rm Elec-3BS-3BM_labo1.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
