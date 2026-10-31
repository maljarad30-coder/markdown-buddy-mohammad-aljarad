> AI Assistance Declaration (draft): ChatGPT assisted with documentation structure, wording, and illustrative code blocks on October 31, 2026. Prompts and response summaries are recorded in Appendix.md. Student review, execution, and verification are pending; this draft does not certify that they have occurred. Final calculations, if any, must be completed and checked by the student.

# Synthetic Retail Sales: R Documentation Project

**Mohammad Aljarad | BDA400 | Assignment 1**

> Review draft. Complete the checklist in Appendix.md before submission.

## Overview

This small R project demonstrates how to document the import and inspection of fictional retail sales records. Its purpose is to make the input, workflow, and outputs understandable to a new reader. It does not use real customer data or produce business recommendations.

## Project files

| File | Purpose |
| --- | --- |
| `README.md` | Project overview, setup, and usage |
| `Sales_Documentation.Rmd` | Script explanation and illustrative executable chunks |
| `Reflection.md` | Provisional reflection topics for student review |
| `Appendix.md` | AI record, README outline, references, and verification checklist |

The documented workflow is a proposed `sales_preview.R` script: create a fictional data frame, display its structure, print its records, and draw a units chart. The examples are included in the R Markdown file. The student must review and adopt or replace this script description before finalization.

## Installation

Use R with RStudio or Posit Cloud. The examples use base R. Rendering the document additionally requires `rmarkdown`, `knitr`, and Pandoc (normally available through RStudio).

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

The following is an illustrative documentation example to review and run:

```r
sales <- data.frame(
  product = c("Notebook", "Pen", "Folder", "Marker"),
  units = c(10, 15, 8, 12),
  unit_price = c(4, 2, 3, 5)
)
str(sales)
print(sales)
```

Open `Sales_Documentation.Rmd` and knit it to HTML. Alternatively, run this from the project folder:

```r
rmarkdown::render("Sales_Documentation.Rmd")
```

## Outputs and limitations

When successfully rendered, the document should display the input table, data structure, and a labelled chart of units by product. It produces `Sales_Documentation.html`. This is an expected behavior description, not an execution report.

The example assumes complete numeric inputs and one record per product. A chart of units is not a revenue comparison. Real-world data would require additional checks for missing values, duplicates, and invalid prices.

## Verification

Compare every displayed value with the input, inspect heading hierarchy and code formatting, and confirm the chart labels. Record the actual result and any corrections in Appendix.md. Review GitHub's rendered README separately from the knitted document.

## License

No open-source license has been selected. This is an academic documentation exercise; no reuse permissions are asserted.

## References

- [GitHub Markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [tidyverse/readr README](https://github.com/tidyverse/readr)
- [R Markdown introduction](https://rmarkdown.rstudio.com/lesson-1.html)

## AI Assistance Disclosure

ChatGPT drafted the structure and explanatory text and suggested illustrative R code blocks. The model identifier should be recorded from the interface if available; no specific version has been assumed. The actual user requests and response summaries appear in Appendix.md. Student edits and validation remain pending. Before submitting, replace this status with an accurate account of the edits and checks actually completed.
