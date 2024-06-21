CSV_FILES = csdat.csv GCdat.csv KWdat.csv CS_2015_planting_data.csv \
            KW_2015_planting_data.csv

BIB_FILES = foo.bib journal-of-the-royal-statistical-society.csl

realized_GC.pdf : realized_GC.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("realized_GC.Rmd")'

realized_KW.pdf : realized_KW.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("realized_KW.Rmd")'

mf.rda : fixup-data.Rmd ${CSV_FILES} ${BIB_FILES}
	Rscript -e 'rmarkdown::render("fixup-data.Rmd")'
