all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_labo3" Elec-3BS-3BM_labo3.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_labo3" Elec-3BS-3BM_labo3.tex

correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_labo3_correction "\def\koriG{} \input{Elec-3BS-3BM_labo3.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_labo3_correction "\def\koriG{} \input{Elec-3BS-3BM_labo3.tex}"

clean:
	rm -f Elec-3BS-3BM_labo3.pdf Elec-3BS-3BM_labo3_correction.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk