CSV_FILES = csdat.csv GCdat.csv KWdat.csv CS_2015_planting_data.csv \
    GC_2015_planting_data.csv KW_2015_planting_data.csv \
    KW.planting.data.final.csv
BIB_FILES = foo.bib journal-of-the-royal-statistical-society.csl

all : fixup-data.pdf realized.pdf

realized.pdf : mf.rda realized.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("realized.Rmd")'

realized_GC.pdf GC_subdatfield.rda : realized_GC.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("realized_GC.Rmd")'

realized_KW.pdf KW_subdatfield.rda : realized_KW.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("realized_KW.Rmd")'

realized_CS.pdf : realized_CS.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("realized_CS.Rmd")'

fixup-data.pdf mf.rda : fixup-data.Rmd ${CSV_FILES} ${BIB_FILES}
	Rscript -e 'rmarkdown::render("fixup-data.Rmd")'

objfun.pdf : mf.rda objfun.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("objfun.Rmd")'

objfun_CS_2015.pdf : mf.rda objfun_CS_2015.Rmd ${BIB_FILES}
	Rscript -e 'rmarkdown::render("objfun_CS_2015.Rmd")'

