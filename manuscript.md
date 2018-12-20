---
title: 'WH Thesis Chapter'
author: 'You'
csl: style.csl
pandemic:
  recipe: polar
  format: pdf
  mustache: "results/vars.json"
  figures: "figures/panels.json"
---

# Introduction

This is the `polar` template. It is designed for data-rich documents. The features include:

1. use `pandemic-it-figures` to build up multi-part figures
2. use `pandemic-mustache` to substitute variables into the document from a results file
3. full support for citations with a custom style

## Citations

Variables can be included using the `mustache` / `handlebars` syntax: {{other.notmaths}}}.
If the variable contains LaTeX style mathematics, use the "unescaped" style of reference,
{{{maths}}}.

Citations are include using the `@` symbol, for instance: [@darwin1859].

## Cross references

Cross references use the `{#ID}` syntax:

![**An interesting figure**](./figures/figure1.png){#fig:id}

See figure @fig:id.

## Equations

$$ \beta = 3 $${#eq:id}

See equation @eq:id.

A reference list is automatically included at the end of the document when exported to PDF.

# References
