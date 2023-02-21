all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_BJT" Elec-3BS-3BM_exe_BJT.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_BJT" Elec-3BS-3BM_exe_BJT.tex


correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_BJT_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_BJT.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_BJT_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_BJT.tex}"

clean:
	rm -f Elec-3BS-3BM_exe_BJT_correction.pdf rm Elec-3BS-3BM_exe_BJT.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
