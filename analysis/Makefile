realized_GC.pdf : realized_GC.Rmd foo.bib \
              journal-of-the-royal-statistical-society.csl
	Rscript -e 'rmarkdown::render("realized_GC.Rmd")'

realized_KW.pdf : realized_KW.Rmd foo.bib \
              journal-of-the-royal-statistical-society.csl \
              KW_2015_planting_data.csv KWdat.csv
	Rscript -e 'rmarkdown::render("realized_KW.Rmd")'
