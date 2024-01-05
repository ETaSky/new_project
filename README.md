Download the [latest release](https://gitlab.com/xbiome-wjc/new_project_template/-/releases) to the directory and decompress


## TITLE OF YOUR PROJECT GOES HERE

YOUR PROJECT'S ABSTRACT GOES HERE



### Overview
```
project
|- README.md          # the top level description of content (this doc)
|- CONTRIBUTING    # instructions for how to contribute to your project
|- LICENSE         # the license for this project
|- DESCRIPTION     # list some required package
|- .gitignore	   # the local gitignore to ignore project specific files
|- .gitattributes	   # to set behavior for file types, such as diff behavior
|
|- data/           # raw and primary data, are not changed once created
|  |-references/   # reference files to be used in analysis
|  |-processed/    # cleaned data, will not be altered once created;
|                  # will be committed to repo
|  +-raw/          # raw data, will not be altered
|
|- code/          # any programmatic code, including bash scripts to run pipeline, setup folders, etc.
|  |-archive/     # Codes that not been used or updated, but can be informative
|
|- outputs/	      # any direct outputs from running analysis, using sub-directory to separate analysis
|                  # contents in this folder may be gitignored
|
+- results/        # all created figs, tbls, etc. from workflows and analyses, but no direct output

```

Other folders that may commonly be presented in a project folder includes:
```
**/archive/		# store previous major version that are not used in final analysis, should be committed
**/scratch/		# previous temporary files that will be deleted after finishing, should not be committed.
**/assets/		# the folder stores the template, snippets, utility scripts etc, should be committed
renv/			# the folder that may be created by renv package for r project management
*.Rproj			# the r project configuration file
.renvignore		# to ignore files so that renv won't check for packages
```
