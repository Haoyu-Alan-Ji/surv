# Overleaf package: Word-style PLOS ONE draft

Upload this entire ZIP to Overleaf and compile `main.tex` with **pdfLaTeX**.

## What changed relative to the prior LaTeX package

- Letter paper, **1-inch margins** (matching the prior Word reference document).
- Times-like text via `newtxtext`, **12 pt** body text.
- **Double spacing**, continuous line numbers, and page numbers.
- Main and subsection headings are black, bold, 12 pt, with spacing matched to the Word reference styles.
- The PLOS sample-template's narrow 5.25-inch text block, 2.75-inch left margin, date footer, and footer rule were removed.
- Tables were resized as native LaTeX tables to fit the normal 6.5-inch text block.
- The current bibliography in `main.tex` is a static rendering generated from the supplied `plos_one_vancouver.csl` and `references.bib`, in citation order. This avoids pretending that `plos2015.bst` is identical to the CSL.

## References

`plos_one_vancouver.csl` and `references.bib` are included for provenance and future regeneration. The manuscript currently compiles without BibTeX because the CSL-rendered references are embedded as `thebibliography` entries in `main.tex`.

If references are added or reordered later, regenerate the bibliography from the included CSL/BibTeX pair and update the `thebibliography` block.

## Figures

Figures are displayed in the working PDF while `\\showfigurestrue` is active. Change it to `\\showfiguresfalse` if you want a caption-only manuscript PDF and plan to upload figure files separately.
