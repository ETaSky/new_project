Download the [latest release](https://gitlab.com/xbiome-wjc/new_project_template/-/releases) to the directory and decompress


## TITLE OF YOUR PROJECT GOES HERE

YOUR PROJECT'S ABSTRACT GOES HERE



### Overview

```
project
|- README.md        # the top level description of content (this doc)
|- CONTRIBUTING.md  # instructions for how to contribute to your project
|- LICENSE.md       # the license for this project
|- .gitignore		# the local gitignore to ignore project specific files
|
|- code/          	# any programmatic code, including bash scripts to run pipeline, setup folders, notebooks etc.
|
|- data           	# raw and primary data, are not changed once created
| |- metadata_raw/	# the original study metadata, probably in excel format, should be commited to repo
| |- raw/         	# raw data, will not be altered, should be hosted on /share/projects/Analytics/, would typically be gitignored
| |- references/  	# reference files to be used in analysis, NOTE: large reference should be hosted on server
| +- processed/   	# cleaned data, will not be altered once created; will be committed to repo
|
|- results        	# all output from workflows and analyses
| |- tables/    	# text version of tables to be rendered with kable in R
| |- figures/     	# graphs, likely designated for manuscript figures
| +- pictures/    	# diagrams, images, and other non-graph graphics
|
|- submission/
| |- study.Rmd		# executable Rmarkdown for this study, if applicable
| |- study.md    	# Markdown (GitHub) version of the *.Rmd file
| |- study.tex    	# TeX version of *.Rmd file
| |- study.pdf    	# PDF version of *.Rmd file
| |- header.tex   	# LaTeX header file to format pdf version of manuscript
| |- references.bib # BibTeX formatted references
| |- XXXX.csl     	# csl file to format references for journal XXX
|
+- Makefile       	# executable Makefile for this study, if applicable
```

Other folders that may commonly be presented in a project folder includes:
```
**/archive/		# store previous major version that are not used in final analysis should be committed
**/scratch/		# previous temporary files that will be deleted after finishing should not be committed.
**/assets/		# the folder stores the template, snippets, utility scripts etc.
renv/			# the folder that may be created by renv package for r project management
*.Rproj			# the r project configuration file
.gitattribute	# the git lfs 
.renvignore		# to ignore files so that renv won't check for packages
```
