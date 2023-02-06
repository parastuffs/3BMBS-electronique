all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_diodes" Elec-3BS-3BM_exe_diodes.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_diodes" Elec-3BS-3BM_exe_diodes.tex


correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_diodes_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_diodes.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_diodes_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_diodes.tex}"

clean:
	rm -f Elec-3BS-3BM_exe_diodes_correction.pdf rm Elec-3BS-3BM_exe_diodes.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
