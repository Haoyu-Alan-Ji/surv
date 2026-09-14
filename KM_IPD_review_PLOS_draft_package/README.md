# KM-to-IPD review manuscript package

Keep all files in this folder when rendering the manuscript.

## Main files

- `KM_IPD_review_manuscript.qmd`: English Sections 1-4, abstract, references, supporting-information captions, and figure insertion markers.
- `KM_IPD_review_tables.xlsx`: manuscript Tables 1-2, the full search log, and a PRISMA count audit sheet.
- `KM_IPD_review_figures.pptx`: two editable figures used in Sections 3-4.
- `references.bib`: cited references.
- `plos_one_vancouver.csl`: numbered PLOS-style citations in square brackets.
- `plos_one_reference.docx`: Word style template with Letter page size, single-column layout, double spacing, continuous line numbering, and page numbers.

## Render the Word manuscript

The QMD imports the two manuscript tables directly from the Excel workbook with `readxl` and `flextable`.

```bash
quarto render KM_IPD_review_manuscript.qmd --to docx
```

Required R packages:

```r
install.packages(c("readxl", "flextable"))
```

## Items intentionally left for final verification

- Author names, affiliations, and corresponding-author details.
- PRISMA counts currently marked `Placeholder` in the `PRISMA counts` worksheet. The draft paragraph uses the same internally consistent provisional sequence.
- The final PRISMA flow diagram (Fig 1).
- Export and insertion of Fig 2 and Fig 3 from the PowerPoint file at the marked locations in the QMD.
- Final search update, software-version freeze, and submission declarations.
