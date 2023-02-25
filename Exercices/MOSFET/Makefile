all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_MOSFET" Elec-3BS-3BM_exe_MOSFET.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_MOSFET" Elec-3BS-3BM_exe_MOSFET.tex


correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_MOSFET_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_MOSFET.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_MOSFET_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_MOSFET.tex}"

clean:
	rm -f Elec-3BS-3BM_exe_MOSFET_correction.pdf rm Elec-3BS-3BM_exe_MOSFET.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
