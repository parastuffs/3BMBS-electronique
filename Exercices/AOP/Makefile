all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_aop" Elec-3BS-3BM_exe_aop.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_aop" Elec-3BS-3BM_exe_aop.tex


correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_aop_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_aop.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_aop_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_aop.tex}"

clean:
	rm -f Elec-3BS-3BM_exe_aop_correction.pdf rm Elec-3BS-3BM_exe_aop.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
