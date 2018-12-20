# polar-scaffold

A scaffold for pandemic for use with the "polar" recipe

## Installation

First make sure [pandemic](https://github.com/lionel-rigoux/pandemic) is installed. Next install the scaffold:

```bash
pandemic resource install scaffold https://github.com/will-hart/polar-scaffold.git
```

You may also wish to install the `polar` recipe, 

```bash
pandemic resource install recipe --as polar https://github.com/will-hart/polar.git
```

## Usage

```bash
mkdir my_new_project && cd my_new_project
pandemic scaffold polar-scaffold
```

## Structure

The folders in the scaffold are:

 - `_public` the built files go in here
 - `analysis` this folder contains data files, spreadsheets or jupyter notebooks for performing analysis
 - `figures` this folder contains multi-part figures, the recipe has inbuilt support for `it-figures`
 - `images` raw images can be saved here from the analysis
 - `results` data files are saved here, `json` files can be used in mustache style templates with `pandemic-mustache`
 
 There are two files:
 
  - `bibliography.bib` for holding the bibliography in bibtex format
  - `manuscript.md` the actual text of the document
