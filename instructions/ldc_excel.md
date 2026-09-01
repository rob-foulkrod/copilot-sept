# LDC Investment Operations Demo

**Scenario:** You're a commodity trading operations analyst at Louis Dreyfus Company reviewing trade flows, book value, merchandising margin revenue, client segments, and trading-book risk signals.

## Demo Setup

Use: LDC_Commodity_Book_Insights_Demo.xlsx

NOTE: This workbook uses synthetic sample data for training.

## Copilot in Excel

### Workbook Orientation

[Worksheet: any] Summarize this workbook in 30 seconds.

[Worksheet: any] Explain this workbook as if I am a commodity trading operations director.

[Worksheet: any] What are the most important columns in this workbook?

### Data Cleanup

[Worksheet: Trade Flows] Normalize similar product line or client segment names.

[Worksheet: Trade Flows] Identify duplicate records in this table.

[Worksheet: Trade Flows] Find unusual or outlier values in Net Flows, Book Value End, or Merchandising Margin.

### Calculated Columns

[Worksheet: Trade Flows] Add a new columns to Trade Flows that labels each trade’s Counterparty Tier and Country.


[Worksheet: Trade Flows] Create a new column called Flow Impact Category based on Net Flows. Use High Inflow, Moderate Inflow, Outflow, and Stable.

[Worksheet: Risk Metrics] Create a formula to identify trading books with negative active return and tracking error above the risk threshold.

[Worksheet: Trade Flows] Explain this inherited formula in the Est. Annual Margin Revenue column.

### Trend Analysis

[Worksheet: Trade Flows] Analyze trade flow trends by month.

[Worksheet: Summary] Identify product lines with the highest estimated annual margin revenue.

[Worksheet: Summary] Create a pivot table by Region and Product Line showing Net Flows, Book Value End, and Est. Annual Margin Revenue.

[Worksheet: Summary] Create a chart showing Est. Annual Margin Revenue by Product Line.

### Risk Analysis

[Worksheet: Risk Metrics] Highlight all trading books approaching risk review status.

[Worksheet: Risk Metrics] Apply conditional formatting for books with negative active return.

[Worksheet: Risk Metrics] Identify trading books that need leadership attention and explain why.

### Executive Dashboard Challenge

[Worksheet: Summary] Create an Executive Trading Operations Dashboard from this workbook.

Include:

- Total Book Value End
- Total Net Flows
- Estimated Annual Margin Revenue
- Top Revenue Product Line
- Product Line trend
- Regional book value view
- Risk watchlist
- Executive summary with recommended actions

Use an executive-friendly layout with red, amber, and green indicators.

### Copilot Premium / Analyst

Using Python, forecast next quarter net flows and identify clusters of recurring book-level or client-segment risks. Create a clear summary, show the forecast trend, and explain which areas need leadership attention.

## Copilot in Word

Write a 150-word executive risk summary based on this workbook for LDC leadership.

## Key Takeaway

Copilot in Excel helps commodity trading teams move from raw position and trade-flow data to executive-ready insights, dashboards, risk summaries, and advanced forecasts in one connected workflow.

## Appendix: Intentional Data Issues

The Trade Flows worksheet contains several intentional data-quality issues for the cleanup demonstrations:

| Issue | Cell or range | What to look for | Expected correction |
| --- | --- | --- | --- |
| Client Segment | E8 | Food Manufacturers | Food Manufacturer |
| Duplicate record | A13:O13 | Exact duplicate of A8:O8 | Remove or flag the duplicate |
| Product Line | B15 | Grains and Oilseeds Complex | Grains & Oilseeds |
| Client Segment | E16 | Beverage Manufacturer | Beverage Producer |
| Net Flows outlier | I20 | $650M | $65M |
| Merchandising Margin outlier | K20 | 170 bps | 17 bps |
| Product Line | B22 | Grains & Oilseeds with a trailing space | Grains & Oilseeds |
| Duplicate record | A23:O23 | Exact duplicate of A16:O16 | Remove or flag the duplicate |
| Product Line | B23 | Coffees | Coffee |
| Client Segment | E24 | Biofuel and Renewable Fuel Producers | Biofuels |

## Appendix: Trade Flows Column Reference

| Column | Field |
| --- | --- |
| A | Trade Book ID |
| B | Product Line |
| C | Commodity |
| D | Region |
| E | Client Segment |
| F | Month |
| G | Contracted Volume (000 MT) |
| H | Gross Trade Value ($M) |
| I | Net Flows ($M) |
| J | Book Value End ($M) |
| K | Merchandising Margin (bps) |
| L | Est. Annual Margin Revenue ($M) |
| M | Counterparty |
| N | Merchandiser |
| O | Position Limit Utilization (%) |

Est. Annual Margin Revenue ($M) = Book Value End ($M) x Merchandising Margin (bps) / 10,000.

## Note On Synthetic Content

All companies and people in the workbook are fictitious and drawn from approved fictitious-name sources. Louis Dreyfus Company appears only as the delivery audience in the file name and title. Volumes are in thousands of metric tons; values are in USD millions.
