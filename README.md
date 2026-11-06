# Rubric

Weighted ranking workbench. Options are rows, criteria are columns, and the page ranks the options and writes down how it reached the ranking.

## What it does

- Data: paste a table from a spreadsheet or edit cells directly, and add options and criteria.
- Criteria: set a unit and a description for each criterion and choose how a raw value becomes points. There are twelve value functions: linear, fixed range, decay, logistic, target band, target (soft), step, log-linear, percentile, categorical, boolean and a custom equation. A criterion can also be calculated from other criteria, and each one has a rule for missing values.
- Weights: four ways to set them, which are a direct budget with sliders and locks that keeps the total at 100, equal weights, rank order and pairwise comparison.
- Rank: scoring by weighted sum, geometric mean, harmonic mean, TOPSIS closeness or a custom equation, with a choice of tie-break. Click a row for its arithmetic, or pin two rows to compare them.
- Stress: shows how close the answer is to flipping, and the point at which each criterion would change the winner.
- Record: the decision written out. Copy it, print it, download the model as `.json` or a workbook as `.xlsx`, or import a model `.json`.
- Starts from a blank model or one of four examples: care routing, supplier selection, hiring shortlist and site selection. Undo, redo and a dark theme are built in.

## What it does not do

- It does not choose for you. It ranks from the criteria and weights you enter, and the Stress tab shows how sensitive that ranking is.
- It has no accounts or sync. It autosaves to `localStorage` (`rubric.autosave`), keeps named saves under `rubric.save.*`, and keeps the theme under `rubric.theme`.
- The examples use invented data.

## Network and install

No network calls. Files stay in the tab. Not installable; no service worker.

## Built with

One HTML file, with no build step, no framework and no libraries. The `.xlsx` workbook is written by the page itself.

## Run locally

Open `index.html` in a browser, or serve the folder with any static file server.
