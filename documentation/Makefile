
all: rs.pdf iwsn.pdf snaa.pdf

rs.pdf:rs/rs-documentation.pdf
	cp $< $@

iwsn.pdf:iwsn/apis.pdf
	cp $< $@

snaa.pdf:snaa/snaa-documentation.pdf
	cp $< $@
	
%.pdf:%.tex 
	cd $(<D)  && pdflatex $(<F) && pdflatex $(<F) 

rs/rs-documentation.pdf:rs/*.tex
iwsn/apis.pdf:iwsn/*.tex
snaa/snaa-documentation.pdf:snaa/*.tex


clean:
	$(RM) */*.aux */*.log  */*.pdf

proper: clean
	$(RM) *.pdf



