# FUTURE_DS_01 - Business Sales Performance Analytics

Future Interns, Data Science & Analytics track - Task 1.

## Objective
Analyse business sales data to find revenue trends, top-selling products, high-value categories and regional performance, and turn the results into recommendations.

## Data
- **Source:** "Sample - Superstore" public sample dataset (Kaggle).
- **Size:** 9,994 order lines, 21 columns, orders from January 2014 to December 2017.
- **Quality checks:** no missing values and no duplicate rows. Order and ship dates were stored as text and converted to real dates. The Data sheet was checked against the original CSV: row count, sales and profit totals all match.

## Tools
Microsoft Excel (formulas and summary tables).

## Method
1. Converted date columns and added helper columns: Year, Month, Profit Margin and Discount Band.
2. Built summary tables with `SUMIFS` formulas by year, month, category, sub-category, region, segment, discount band, state and product.
3. Added discount tables (average discount, share of lines discounted above 20%, and profit below and above the 20% line) by region, state, category and sub-category.
4. Wrote up the findings and recommendations on the Insights sheet, each with the numbers that support it.
5. Compared sales with profit throughout, since high sales do not always mean high profit.

## Key KPIs
| KPI | Value |
|---|---|
| Total sales | about $2.30M |
| Total profit | about $286K |
| Profit margin | about 12.5% |

## Key findings
1. **Growth:** sales rose from about $484K (2014) to $733K (2017), with a dip in 2015. Margin improved from 10.2% to 13.4% in 2016, then slipped to 12.7% in 2017.
2. **Top products:** the top 10 products bring in $245K of sales and $43K of profit. The Canon imageCLASS 2200 copier leads ($61.6K sales, $25.2K profit), but the Cisco TelePresence EX90 and GBC DocuBind P400 are top sellers that lose money.
3. **Furniture** earns a 2.5% margin, against 17.4% for Technology and 17.0% for Office Supplies.
4. **Tables and Bookcases** are the loss-making sub-categories (about -$17.7K and -$3.5K). They also have the highest average discounts in Furniture (26.1% and 21.1%).
5. **Discounts above 20%** are linked to losses. The 1,393 order lines sold above a 20% discount lost about $135K in total, and the 50%+ band loses about $76.6K.
6. **Central region** has the lowest margin (7.9%) against West (14.9%), and the heaviest discounting (average 24.0% against 10.9%).
7. **Texas, Ohio and Pennsylvania** are sizeable markets that lose money, and all three have average discounts of 32-37%.
8. Discounting is not the whole story: its effect differs by product (for example Binders are heavily discounted but still profitable overall).

## Recommendations
- Cap discounts at around 20%, with approval needed above that, and review the orders sold at 50% or more first.
- Review pricing and costs on Furniture, especially Tables and Bookcases.
- Investigate discounting in the Central region and in Texas, Ohio, Pennsylvania and Illinois.
- Check why several top-selling products make no profit, and rank products by profit as well as sales.
- Track margin monthly, not only sales.

## Files
- `FUTURE_DS_01_Superstore_Analysis.xlsx` - Data, Analysis and Insights sheets.
- `Sample - Superstore.csv` - original dataset.

## Limitations
The data does not include costs or reasons for discounting, so the analysis shows association, not proof of cause. Findings describe 2014-2017 only.

## Note on tools
An AI assistant (Claude) was used to help build the workbook and draft the write-up. I reviewed the numbers and the findings myself.
