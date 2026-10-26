# Affiliate Marketing Growth & Tracking (Excel)

**[Download the Excel workbook (Affiliate_Tracker.xlsx)](https://github.com/AkshatRastogi-Analyst/affiliate-marketing-tracker/raw/main/Affiliate_Tracker.xlsx)** | [All project files on GitHub](https://github.com/AkshatRastogi-Analyst/affiliate-marketing-tracker)

An Excel tracker that shows which affiliate products and platforms actually get clicks and earn commission, so weak products can be dropped and the ones that convert can be kept.

**Tools:** Microsoft Excel (formulas, SUMIFS, COUNTIFS, conditional formatting, charts) | **Platforms tracked:** Meesho Creator Hub, EarnKaro, Flipkart

> **Note on the data:** the 30 rows in this repository are **sample data made up to show how the tracker works**. They are not real earnings. To use the tracker, delete the sample rows and type in your own numbers.

## The problem

When you promote affiliate products on several platforms, it is hard to tell which product or platform is worth the effort. Posts get views, some get clicks, a few lead to orders, and the commission arrives later. Without one place to compare them, time goes to products that do not earn.

## What the workbook does

You log one row per promoted product. The sheet then works out:

| Measure | Formula |
|---|---|
| Click-through rate (CTR) | Clicks / Post Views |
| Conversion | Orders / Clicks |
| Commission | Orders x Commission per order |
| Earnings per click | Commission / Clicks |

Each product gets a decision:

| Decision | Meaning |
|---|---|
| Need more data | Clicks are below the minimum, so it is too early to judge |
| Keep | Conversion and earnings per click are both at or above the targets |
| Drop | Both are below the targets |
| Watch | One is above target and one is below |

The minimum clicks and the two targets sit on the **Settings** sheet and can be changed. The starting values are my own assumptions, not industry figures.

## Sheets

- **Guide:** how to use the file and what each column means
- **Summary:** totals by platform and by category, share of commission, Keep / Watch / Drop counts, and two charts
- **Settings:** the cut-off numbers used for decisions, plus the platform and category names used in the dropdowns and on Summary
- **Tracker:** the data entry table (yellow cells with blue text are inputs; the rest are formulas, including a Data check column)

## How to use it with your own data

1. Open `Affiliate_Tracker.xlsx`.
2. On the **Tracker** sheet, delete the sample values in columns A to H (leave the formulas in columns I to M).
3. Enter your own rows: date, platform, product, category, post views, clicks, orders and commission per order. Commission is worked out for you, so it changes when you change Orders.
4. Adjust the targets on **Settings** if needed.
5. Read the **Summary** sheet and the Decision column.

The tracker has room for 300 rows. Every number on Summary and in the charts is a formula, so changing any entry on Tracker or Settings updates everything. Anything with a platform or category that is not on the Settings lists is counted in an Other row, so the totals always match the Tracker.

## Files

```
affiliate-marketing-tracker/
├── Affiliate_Tracker.xlsx   # the tracker
├── data/sample_data.csv     # the same sample rows as plain CSV
└── README.md
```

## What I practiced

- Designing a tracker that a non-technical person can fill in
- Cleaning up a messy question ("what is working?") into a few clear measures
- Formulas that recalculate when the data changes, instead of typed-in totals
- Presenting results in a short summary with charts

## Author

Akshat Rastogi | [GitHub](https://github.com/AkshatRastogi-Analyst) | akshatrastogi0425@gmail.com
