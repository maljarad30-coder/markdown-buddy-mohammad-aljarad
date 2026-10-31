> AI Assistance Declaration: ChatGPT assisted with documentation, illustrative R code, revision, and reflection drafting. Mohammad Aljarad rendered the R Markdown in RStudio and previewed the README on GitHub. Supplied HTML and screenshots were reviewed for consistency. Actual requests and review results are recorded in Appendix.md. No analytical calculations were performed.

# Appendix: prompts, review, and verification

**Mohammad Aljarad | BDA400 Assignment 1 | October 31, 2026**

## Actual request record

The following are English translations or concise translations of actual Arabic requests. Response summaries describe work performed, rather than invented prompt exchanges.

| Stage | Request | Response and outcome |
| --- | --- | --- |
| Initial draft | Let us start completing this assignment step by step. | Prepared project documentation and guided RStudio setup, rendering, and GitHub upload. |
| Reflection | Write it yourself. | Drafted an experience paragraph; the student replied “Excellent,” approving it. |
| Review and refinement | Review the current README and R Markdown. Check formatting, suggest two clear improvements, apply them, update verification from my RStudio run and GitHub screenshots, add my approved reflection, and record the request and results in Appendix. | Clarified the actual workflow and revised verification wording; added the approved reflection and review record. |
| Final correction | I want a complete version. Propose reflection questions, add a standalone R script, and update the repository statements saying verification still needs updating. | Added `sales_preview.R`, three proposed reflection questions and answers, synchronized evidence statements, and updated the PDF and five-file package. |

## README outline and reference comparison

Outline: Overview; Project files; Installation; Example usage; Synthetic input; Outputs and limitations; Verification; License; References; AI Assistance Disclosure.

The assistant consulted the GitHub Markdown guide and the tidyverse/readr README during drafting. The readr organization of overview, installation, and usage informed this outline. This project additionally includes a data dictionary and evidence table. Independent student reading of those sources is not asserted.

## Two clear improvements applied

1. **Clarify files, dependencies, and execution.** The documentation now identifies an included `sales_preview.R` script, explains its base R dependency, and separates console/plot output from the R Markdown HTML output. The R Markdown uses the same data and plotting expressions with a formatted table.
2. **Make verification specific and current.** Obsolete statements that the revised HTML or README had not been previewed were removed. Results now identify the supplied revised HTML and GitHub screenshots, including the observed table, chart, and formatting. Source checks on the new script are distinguished from runtime evidence.

## Formatting and consistency review

- Markdown headings have a consistent hierarchy; table headers and separator rows are present.
- Code fences are paired and R Markdown chunk names are unique.
- YAML includes the title, author, date, HTML output, and table of contents.
- All four executable R Markdown chunks are preserved from the rendered version.
- The independent script reuses the data, structure, and chart expressions; `print(sales)` replaces HTML table formatting.
- File references now name included files. Deliverable prose is in English.

## Verification evidence

| Evidence | Observed result |
| --- | --- |
| Initial HTML supplied by student | Structure, table, and chart rendered |
| Revised `Sales_Documentation(1).html` supplied by student | Revised explanatory text and the same matching outputs inspected |
| Data structure | Four observations, three variables; product labels are character values and quantities/prices are numeric |
| Table | Notebook (10, 4), Pen (15, 2), Folder (8, 3), Marker (12, 5); pairs are units and unit price in CAD |
| Chart | Notebook, Pen, Folder, Marker in order; heights 10, 15, 8, 12 |
| GitHub README screenshots | Headings, tables, and code rendered; updated header and project table previewed |
| Initial repository history | Screenshot shows `ea860b9`, initial documentation draft |
| Revised repository history | Screenshot shows `8738bc8`, documentation revision, and two commits |
| Later README correction | Student reported saving the correction; no additional commit hash supplied |
| Environment screenshots | R 4.6.2; installation messages for rmarkdown 2.32 and knitr 1.52 |

The final text edits do not change the four executable R Markdown chunks. The standalone script was compared at source level with those chunks; separate execution of that new file is not claimed. A full sessionInfo record, clean-session rerun, and independent peer review are not established by the supplied evidence. No analytical calculations were required for this input-display example.

## Reflection and final package

The approved experience paragraph is retained in `Reflection.md`. Three additional questions and answers were proposed at the student's express request because the original question wording was not available in the supplied instructions. They are explicitly identified as proposed questions.

The package contains README.md, sales_preview.R, Sales_Documentation.Rmd, Reflection.md, and Appendix.md. The companion report is `Aljarad_Mohammad_CA_BDA400_A01.pdf`. This review records local file preparation and prior repository evidence; it does not assert that this final package has already been committed remotely.

## References

- [GitHub Markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [tidyverse/readr README](https://github.com/tidyverse/readr)
- [R Markdown introduction](https://rmarkdown.rstudio.com/lesson-1.html)
