# Comparable Bot

## Project Proposal

Once the comparables set is determined in transfer pricing analysis, the transfer pricing analyst can then proceed to download the comps financial data from the FactSet/Bureau van Dijk database and do the basic comps financial analysis to compute the chosen PLI of the transfer pricing study (under the CPM/TNMM). Automation of most of the initial comps financial analysis can be implemented in a VBA macro and incorporated in the UiPath automation through the Invoke VBA activity. The analyst must then perform detailed economic and accounting adjustments to the comps financial data to improve the comparability of the comps to the tested party based on information that can only be found in the company’s annual report. When benchmarking the client with a US comparables set, the analyst must download the company’s 10-K from the SEC’s website for the entire period of analysis and go through the 10-K filing to pull the desired data.

My application will help automate the saving of the comparable company’s annual report posted on the SEC’s website and the analysis of the 10-K filing based on the analyst’s input, thus fulfilling the final part of the comparables analysis process of making detailed economic/accounting adjustments to the comps financial data and computing the arm’s length interquartile range of return of the comps set.

## User Story/Business Case

The transfer pricing analyst will want to make the following economic/accounting adjustments to the comps financial data based on information found in the Concise Comp Data Workbook created in the automation:

* **Restatement Adjustment:** Consolidated Financial Statements are always part of the generated Concise Comp Data Workbook, and the analyst can adjust the FactSet financial data based on the corresponding year in the company's 10-K published in the following year
* **Segmentation Adjustment:** Business Segment/Geographic Segment Adjustment performs segmentation of the entire company's financial data based on ratio calculated from the chosen segment's financial data
* **Acquisition/Disposition Adjustment:** Balance sheet adjustment in the year of the company's acquisition/disposition to mitigate inaccuracy arising from the averaging of the Year-Beginning and Year-End Balance Sheet
* **Income Taxes:** Detailed accounting of income taxes contains information on the company's DTA/DTL required in computing asset-based PLI, depending on the definition of the PLI
* **Intangible Assets:** Detailed accounting of intangible assets contains information on the company's non-goodwill intangible assets and their associated amortization required in computing asset-based PLI, depending on the definition of the PLI
* **R&D Adjustment:** Adjustment of R&D expense and the effect of R&D spending on the comparable company's operating profit to the level of the tested party

## In-Progress Idea List

* Form Input Validation
* Make Concise Comp Data Workbook based on keyword with RegEx

## Future Development

Design the automation to be run on the FactSet terminal itself from the very beginning to the end