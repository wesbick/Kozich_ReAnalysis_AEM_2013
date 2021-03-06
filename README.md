Download the [latest release](https://github.com/SchlossLab/new_project/releases/latest) to the directory and decompress


## Re-Analysis of Kozich data

YOUR PAPER'S ABSTRACT GOES HERE




### Overview

	project
	|- README          # the top level description of content (this doc)
	|- CONTRIBUTING    # instructions for how to contribute to your project
	|- LICENSE         # the license for this project
	|
	|- submission/
	| |- Kozich_ReAnalysis_AEM_2016.Rmd    # executable Rmarkdown for this study, if applicable
	| |- Kozich_ReAnalysis_AEM_2016.md     # Markdown (GitHub) version of the *.Rmd file
	| |- Kozich_ReAnalysis_AEM_2016.tex    # TeX version of *.Rmd file
	| |- Kozich_ReAnalysis_AEM_2016.pdf    # PDF version of *.Rmd file
	| |- Kozich_ReAnalysis_AEM_2016.tex   # LaTeX header file to format pdf version of manuscript
	| |- references.bib # BibTeX formatted references
	| |- XXXX.csl     # csl file to format references for journal XXX
	|
	|- data           # raw and primary data, are not changed once created
	| |- references/  # reference files to be used in analysis
	| |- raw/         # raw data, will not be altered
	| |- mothur/      # mothur processed data
	| +- process/     # cleaned data, will not be altered once created;
	|                 # will be committed to repo
	|
	|- code/          # any programmatic code
	|
	|- results        # all output from workflows and analyses
	| |- tables/      # text version of tables to be rendered with kable in R
	| |- figures/     # graphs, likely designated for manuscript figures
	| +- pictures/    # diagrams, images, and other non-graph graphics
	|
	|- exploratory/   # exploratory data analysis for study
	| |- notebook/    # preliminary analyses
	| +- scratch/     # temporary files that can be safely deleted or lost
	|
	+- Makefile       # executable Makefile for this study, if applicable


### How to regenerate this repository
# reference files from https://www.mothur.org/MiSeqDevelopmentData/HMP_MOCK.fasta
# raw data from https://www.mothur.org/MiSeqDevelopmentData/StabilityWMetaG.tar


#### Dependencies and locations
* Gnu Make should be located in the user's PATH
* mothur (v1.XX.0) should be located in the user's PATH
* R (v. 3.X.X) should be located in the user's PATH
* etc.


#### Running analysis

```
git clone https://github.com/SchlossLab/LastName_BriefDescription_Journal_Year.git
make write.paper
```
