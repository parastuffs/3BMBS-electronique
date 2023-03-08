all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_ADC-DAC" Elec-3BS-3BM_exe_ADC-DAC.tex
	pdflatex -shell-escape -jobname="Elec-3BS-3BM_exe_ADC-DAC" Elec-3BS-3BM_exe_ADC-DAC.tex


correction: *.tex
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_ADC-DAC_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_ADC-DAC.tex}"
	pdflatex -shell-escape -jobname=Elec-3BS-3BM_exe_ADC-DAC_correction "\def\koriG{} \input{Elec-3BS-3BM_exe_ADC-DAC.tex}"

clean:
	rm -f Elec-3BS-3BM_exe_ADC-DAC_correction.pdf rm Elec-3BS-3BM_exe_ADC-DAC.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
