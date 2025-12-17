# Installation Instructions

## Installing the Data Publication Codebook Package

You can install this package directly from GitHub using Stata's `net install` command:

```stata
net install jpal_codebook, from("https://raw.githubusercontent.com/J-PAL/Data_publication_codebook/main/") replace
```

Alternatively, if you have downloaded the files locally, navigate to the directory containing the package files and run:

```stata
net install jpal_codebook, from("`c(pwd)'") replace
```

## Usage

After installation, you can use the command:

```stata
jp_codebook "path/to/your/data/directory"
```

This will create a codebook Excel file in your current working directory with two tabs:

- "Variables": Information about each variable found in the .dta files
- "Value labels": Value label mappings for encoded variables

## Files Included

- `jpal_codebook.ado` - Main program file
- `jpal_codebook.do` - Alternative do-file version
- `jpal_codebook.pkg` - Package description file
- `stata.toc` - Table of contents file
- `README.md` - Documentation
- `LICENSE` - MIT License
