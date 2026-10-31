> AI Assistance Declaration: ChatGPT assisted with documentation, illustrative R code, revision, and reflection drafting. Mohammad Aljarad rendered the R Markdown in RStudio and previewed the README on GitHub. Supplied HTML and screenshots were reviewed for consistency. Actual requests and review results are recorded in Appendix.md. No analytical calculations were performed.

# Synthetic Retail Sales: R Documentation Project

**Mohammad Aljarad | BDA400 | Assignment 1 | October 31, 2026**

## Overview

Create and inspect fictional retail records using R. The project displays a data structure, records, and a chart of units by product. Inputs are created internally; no external dataset or customer information is used.

## Project files

| File | Purpose |
| --- | --- |
| `README.md` | Setup, usage, dependencies, verification, and disclosure |
| `sales_preview.R` | Standalone base R script: data, console output, and chart |
| `Sales_Documentation.Rmd` | Script documentation with executable examples and an HTML table |
| `Reflection.md` | Approved reflection and three proposed questions with answers |
| `Appendix.md` | Actual prompt record, review findings, and verification evidence |

## Installation

Use R and RStudio. The standalone script needs only base R. For R Markdown, install:

```r
install.packages(c("rmarkdown", "knitr"))
```

Rendering also needs Pandoc, normally supplied with RStudio. Keep the five project files in the same directory.

## Example usage

Set the working directory to the project folder. Run the standalone script:

```r
source("sales_preview.R")
```

The Console shows structure and records; RStudio's Plots pane shows the chart. To build the documented HTML report, open `Sales_Documentation.Rmd` and select Knit, or run:

```r
rmarkdown::render("Sales_Documentation.Rmd")
```

The `.Rmd` is editable source. `Sales_Documentation.html` is generated output. The R Markdown repeats the script's workflow and formats its records with `knitr::kable()`; it does not source the script.

## Synthetic input

| Field | Type | Meaning |
| --- | --- | --- |
| `product` | Character | Fictional product label |
| `units` | Numeric | Fictional units sold |
| `unit_price` | Numeric | Fictional unit price in CAD |

| Product | Units | Unit price (CAD) |
| --- | ---: | ---: |
| Notebook | 10 | 4 |
| Pen | 15 | 2 |
| Folder | 8 | 3 |
| Marker | 12 | 5 |

## Outputs and limitations

The script prints records and creates a chart in the active graphics device. The R Markdown creates HTML with explanations, code, structure output, a table, and the chart. No input files are overwritten. No totals, averages, revenue estimates, or business recommendations are calculated. The example assumes complete inputs and one record per product; production data would need additional validation.

## Verification

| Check | Result and evidence |
| --- | --- |
| R Markdown execution | Original and revised HTML supplied by the student show successful output |
| Structure | Four observations and three variables |
| Table | Every value matches the synthetic inputs above |
| Chart | Product order and bar heights match the units column |
| GitHub formatting | Supplied screenshots show headings, tables, and highlighted code; updated README preview also supplied |
| Final source consistency | All four executable R Markdown chunks preserved; stale pending-preview claims removed |
| Standalone script | Data, structure, and plotting expressions match the rendered R Markdown; uses base R `print()` for records; no separate execution claimed |

Screenshots show R 4.6.2, rmarkdown 2.32, and knitr 1.52. Evidence and review scope are recorded in [Appendix.md](Appendix.md).

## License

No open-source license has been selected; no reuse permissions are asserted.

## References

- [GitHub Markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [tidyverse/readr README](https://github.com/tidyverse/readr)
- [R Markdown introduction](https://rmarkdown.rstudio.com/lesson-1.html)

## AI Assistance Disclosure

ChatGPT helped draft and review these files. Two documentation improvements clarified the real workflow and replaced obsolete verification statements with evidence-based results. At the student's request, the final revision adds a standalone R script and three proposed reflection questions. Those questions are identified as supplementary rather than quoted from the college instructions. The student remains responsible for reviewing the submitted work.
