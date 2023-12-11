# APPS_csl

A Citation Style Language (csl) file for formatting citations for the journal "Applications In Plant Sciences". 

This citation styling file should work with most common reference managers including Zotero, Mendeley, and Endnote. Download the file "applications-in-plant-sciences.csl" and consult your specific software manual on how to install it.

If you are using Quarto to generate a publication, you can also use the "applications-in-plant-sciences.csl" file. Download the file and place it in the same directory as your .qmd file. Add another file to the directory with your bibtex formatted bibliography, "references.bib".  Then add the following to the YAML header in your .qmd file:

```
---
format: docx
editor: 
  markdown: 
    wrap: 72
bibliography: references.bib
csl: applications-in-plant-sciences.csl
---
```

Each reference in your "references.bib" file should start with a unique identifier, e.g: "@article{Baker2023,". To insert the reference in your text, add the unique identifier in square brackets: "[@Baker2023]". To add a formatted references to your rendered document, add the following code:
```
::: {#refs}
:::
```
For more complicated in-text references (multiple authors, suppress author, add text inside of parentheses, etc), see the [quarto guide on footnotes and citations](https://quarto.org/docs/authoring/footnotes-and-citations.html#sec-citations).

Render your .qmd to .docx and watch the magic!

