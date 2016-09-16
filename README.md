# Thesis

My thesis is constructed of several .tex files (and a .bib for the bibliography). 

__NG_Thesis.tex__ is the main file. It contains the preamble and other general formatting information. It refers to and inserts the other files as necessary.

__uafthesis.cls__ is the custom document class file to produce a UAF approved thesis. It was orignally written in 1996 by Curt Szuberla kludging together report.cls and ucthesis.cls. It has since been updated over the years by several other students as formatting requirements change.

__NG_abstract.tex__ contains the abstract.

__NG_intro.tex__ contains the first chapter. It is the introductory chapter contianing the problem statement and background information on microgrids and other relevant information.

__NG_bib.bib__ contains bibliographical information of each of my cited sources.

__tables__ directory contains .tex files of included tables.

There are probably several methods to generate a pdf. Here is one:
To generate a .dvi on a linux system from scratch run "latex NG_Thesis.tex" once to generate the apropirate .aux files. 
Then run "bibtex NG_Thesis.aux" to generatre appropriate bibliography files.
Finally run "latex NG_Thesis.tex" two times to generate the dvi file with appropriately linked sources. 

Additional changes that do _not_ involve citations only need a single "latex NG_Thesis.tex" execution. Changes that do involve citations require the whole process to be repeated (I believe).

The command "dvipdf NG_Thesis.dvi" can convert the dvi into a pdf.


To do this on a windows machine requires Miktex or something. I'm not really sure.
