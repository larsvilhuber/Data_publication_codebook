# Data_publication_codebook

 Stata program to make a codebook for a directory that contains stata datasets. 
 
 ## Contents:

 This repo a command `jpal_codebook` via [`jpal_codebook.ado`](jpal_codebook.ado). 
 
 ## Use:
 
 - Install the ado file (you can remove it later if you don't want to keep it).
 - run the command `jp_codebook path_to_dir`, where `path_to_dir` is a string containing the path of the directory you would like to make a codebook for.
 
 ## Output:
 
 - The program outputs an excel file containing a codebook to the current working directory. The excel file has two tabs:
  - "Variables" contains each distinct variable found in the .dta datasets in the specified folder, along with information about it, including but not limited to label, value label, # of distinct values, and mean, median, etc. for numeric variables
  - "Value labels" contains the value labels used in encoded variables in the dataset, and maps their numbers to the underlying values.

## Installation Instructions

You can install this package directly from GitHub using Stata's `net install` command:

```stata
global githubbase "https://raw.githubusercontent.com/"
net install jpal_codebook, from("$githubbase/J-PAL/Data_publication_codebook/main/") replace
```

Alternatively, if you have downloaded the files locally, navigate to the directory containing the package files and run:

```stata
net install jpal_codebook, from("`c(pwd)'") replace
```
## De-installation (optional)

To uninstall the package, you can use the following command in Stata:

```stata
ado uninstall jpal_codebook
```

## Files Included

- `jpal_codebook.ado` - Main program file
- `jpal_codebook.do` - Alternative do-file version
- `jpal_codebook.pkg` - Package description file
- `stata.toc` - Table of contents file
- `README.md` - Documentation
- `LICENSE` - MIT License
