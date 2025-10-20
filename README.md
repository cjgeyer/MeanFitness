We are now on Zenodo!
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17093287.svg)](https://doi.org/10.5281/zenodo.17093287)
This repo contains supplementary material for a paper currently titled

 * Realization of ongoing evolutionary adaptation in the field

by the following authors in some order, not necessarily this order,

 * Charles J. Geyer, University of Minnesota, geyer@umn.edu
 * Mason W. Kulbaba, St. Mary's University, mason.kulbaba@stmu.ca
 * Seema N. Sheth, North Carolina State University, ssheth3@ncsu.edu
 * Rachel E. Pain, University of Minnesota, repain@umn.edu
 * Vincent M. Eckhart, Grinnell College, eckhart@grinnell.edu
 * Ruth G. Shaw, University of Minnesota, shawx016@umn.edu

Most of the contents of this repo are a mess of blind alleys and failed
attempts.  The two output files that are current and the supplementary
material for the paper are in the `analysis` subdirectory.

 * analysis/fixup-data.pdf
 * analysis/realized.pdf

The former is just about data wrangling.  The latter has the biology and
statistics.

To reproduce the results, do
```
cd analysis
make
```

Since the PDF files listed above are committed to the repo, one does not
need to remake them to read them.  But they are fully reproducible.
