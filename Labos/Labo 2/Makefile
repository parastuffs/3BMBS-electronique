all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_labo2" Elec-3BS-3BM_labo2.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_labo2" Elec-3BS-3BM_labo2.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_labo2_correction "\def\koriG{} \input{Elec-3BS-3BM_labo2.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_labo2_correction "\def\koriG{} \input{Elec-3BS-3BM_labo2.tex}"
	
clean:
	rm -f Elec-3BS-3BM_labo2_correction.pdf rm Elec-3BS-3BM_labo2.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
