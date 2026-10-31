> AI Assistance Declaration: I used ChatGPT for documentation structure, wording, illustrative R examples, and revision guidance. English translations of my prompts and response summaries are recorded in Appendix.md. I rendered the original R Markdown document in RStudio and previewed the README on GitHub; ChatGPT checked the HTML and screenshots I supplied. No analytical calculations were performed. I am responsible for reviewing the accuracy and originality of this work.

# Synthetic Retail Sales: R Documentation Project

**Mohammad Aljarad | BDA400 | Assignment 1**

> Documentation revised on October 31, 2026. Original execution and GitHub preview evidence are recorded in Appendix.md; the revised files still require a new preview.

## Overview

This small R project demonstrates how to document the creation and inspection of fictional retail sales records. Its purpose is to make the input, workflow, and outputs understandable to a new reader. It does not use real customer data or produce business recommendations.

## Project files

| File | Purpose |
| --- | --- |
| `README.md` | Project overview, setup, and usage |
| `Sales_Documentation.Rmd` | Self-contained workflow, explanations, and executable R chunks |
| `Reflection.md` | Approved experience paragraph and reflection scope note |
| `Appendix.md` | AI record, README outline, references, and verification checklist |

The executable workflow is contained in `Sales_Documentation.Rmd`: create a fictional data frame, display its structure, format its records as a table, and draw a units chart. There is no separate `sales_preview.R` file in this repository. The README example below is a short console preview; the R Markdown document contains the full workflow.

## Installation

Use R with RStudio or Posit Cloud. Base R provides data creation, structure inspection, console printing, and plotting. The R Markdown table uses `knitr`; document rendering uses `rmarkdown`, `knitr`, and Pandoc (normally available through RStudio).

Run once in the R Console if needed:

```r
install.packages(c("rmarkdown", "knitr"))
```

Keep all four documentation files in the same project folder. No external dataset is required.

## Synthetic input

| Field | Meaning | Type |
| --- | --- | --- |
| `product` | Fictional product label | Character |
| `units` | Fictional units sold for that record | Numeric |
| `unit_price` | Fictional price in CAD | Numeric |

These values are illustrative inputs, not measured observations. No totals, revenue estimates, or averages are supplied as verified results.

## Example usage

The following console example creates the same synthetic inputs used in the R Markdown document:

```r
sales <- data.frame(
  product = c("Notebook", "Pen", "Folder", "Marker"),
  units = c(10, 15, 8, 12),
  unit_price = c(4, 2, 3, 5)
)
str(sales)
print(sales)
```

To render the complete report, open `Sales_Documentation.Rmd` in RStudio, save it, and select **Knit**. Open the resulting `Sales_Documentation.html` to inspect the output. Alternatively, run this from the project folder:

```r
rmarkdown::render("Sales_Documentation.Rmd")
```

## Outputs and limitations

The original document was rendered in RStudio on October 31, 2026. The supplied `Sales_Documentation.html` contains the input table, data structure, and a labelled chart of units by product. The `.Rmd` is the editable source; the `.html` is the generated report. The current revision changes documentation text only and must be knitted again to refresh that report.

The example assumes complete numeric inputs and one record per product. A chart of units is not a revenue comparison. Real-world data would require additional checks for missing values, duplicates, and invalid prices.

## Verification

| Check | Evidence and result |
| --- | --- |
| Original R Markdown render | Student-supplied HTML and RStudio screenshots show a rendered report with code and outputs. |
| Data structure | The HTML reports a data frame with four observations and three variables. |
| Table values | Notebook: 10 units, CAD 4; Pen: 15 units, CAD 2; Folder: 8 units, CAD 3; Marker: 12 units, CAD 5. These match the source inputs. |
| Chart | Labels follow Notebook, Pen, Folder, Marker; heights match 10, 15, 8, 12. |
| Original GitHub preview | Screenshots show rendered headings, tables, links, and highlighted R code. Link appearance does not confirm every destination works. |
| Revised files | R code chunks are unchanged; re-knit and preview this revision after uploading it. |

These are observations from the submitted evidence, not a claim that every possible input has been tested. See Appendix.md for remaining assignment requirements.

## License

No open-source license has been selected. This is an academic documentation exercise; no reuse permissions are asserted.

## References

- [GitHub Markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [tidyverse/readr README](https://github.com/tidyverse/readr)
- [R Markdown introduction](https://rmarkdown.rstudio.com/lesson-1.html)

## AI Assistance Disclosure

ChatGPT drafted the structure and explanatory text and suggested the initial illustrative R code. My main requests were to work through the assignment, review the README and R Markdown, apply two clarity improvements, update verification using my RStudio and GitHub evidence, and add the reflection paragraph I approved. The prompt record in Appendix.md contains English translations of the original Arabic requests.

This revision makes two improvements: (1) it identifies the actual executable file and distinguishes source from output, and (2) it replaces obsolete pending-execution statements with specific evidence and verification limits. ChatGPT applied these edits; they are not presented as unaided student writing. The original code chunks were retained. The reflection paragraph was drafted by ChatGPT and approved by me. The exact three assigned reflection questions remain unavailable in the supplied material.
