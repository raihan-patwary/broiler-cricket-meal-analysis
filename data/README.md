# Data

The workbook is not stored in this repository.

| | |
|---|---|
| File | `H Fisher Growth 22 - Open access.xlsx` |
| Source | Mendeley Data, https://doi.org/10.17632/rj5fybnzh6.1 (version 1, CC BY 4.0) |
| SHA-256 of the copy analysed | `2c0e12849a7441e66ee190f0c438d84d914ceae9d51b9b97367f64ec5737a118` |

## How to provide it

- **Google Colab:** run a notebook. It asks for the file and saves it in this folder. Each notebook has its own Colab session, so each one asks once.
- **Your own machine:** download the file from the link above and save it in this folder without renaming it.

The notebooks only read the file. They never write to it.

## Sheets and where they are used

Every sheet starts with a key to the treatment codes (rows 1 to 8). The column labels come further down, in row 12 or 13 of the spreadsheet.

This file uses spreadsheet references (row 1, column A). The notebooks count rows and columns from zero, as pandas does, so spreadsheet row 13 is row 12 there and column A is column 0.

| Sheet | Content | Rows of data | Notebook |
|---|---|---|---|
| `Growth data` | Body weight, feed intake, gain and feed:gain of each pen at each weekly weighing | 144 (24 pens x 6 weighings) | 1 and 3 (2 for the pen key) |
| `Organ weights and indices` | Body weight, six organ weights, their indices and ileal pH of sampled birds on days 13, 20 and 35 | 216 (72 birds per day) | 2 (1 for the sampling days) |
| `Meat yield, breast & liver Lab` | Breast weights and yields, liver and breast colour of birds sampled on day 35 | 72 | 2 and 3 |
| `Meat cook yield` | Raw and cooked breast weight, cooking loss | 72 | 2 |
| `Meat texture` | Force readings on raw and cooked breast, several per bird | 289 | 2 |
| `Intestinal lesion scores` | Lesion score of sampled birds on days 20 and 35 | 144 (72 birds per day) | 2 |

## Layout of `Growth data`

Spreadsheet row and column references:

- row 13: column labels
- rows 14 to 157: data
- columns A to K: weekly records, 24 pens x 6 weighings (the table analysed)
- columns O to X: the same pens summarised by feeding period
- columns AB to AK: 35-day totals

The weekly table has these columns: Pen, Treatment, Diet, Day, Period, Rep, Average weight (g), Daily feed intake (g), Daily weight gain (g/d), Feed : Gain, % Mortalities. Body weight, feed intake and gain are means per bird for each pen.
