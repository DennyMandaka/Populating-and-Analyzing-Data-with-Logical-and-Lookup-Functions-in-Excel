# Populating and Analyzing Data with Logical and Lookup Functions in Excel
## Project Objective
This project demonstrates the application of Excel's logical and lookup functions by populating and analyzing data within an inventory dataset. 

## Dataset(s)
- The <a href="https://github.com/DennyMandaka/Populating-and-Analyzing-Data-with-Logical-and-Lookup-Functions-in-Excel/blob/main/Logical%20and%20Lookup%20Functions.xlsx">dataset</a> was sourced from the "Excel Skills for Data Analytics and Visualization" course offered by Macquarie University on Coursera. It contains information from an inventory database, including item codes, categories, number of stocks, prices, and many more.

## Populating and Analyzing Data with Logical and Lookup Functions
- In I4 use an IF function to determine if the Num in Stock is below the minimum stock level. If it is put a "Y" otherwise leave the cell blank.
- In J4 create a calculation to check if that item is below minimum stock level and NOT on backorder. If both are true put a "Y" otherwise leave the cell blank.
- In H4 calculate the retail price. If it is a Premium item (has Y in the Premium column) add 25% to the cost price, otherwise add 18% to the cost price.
- The reorder quantities table in N9:O12 indicates how many items we need to reorder for each category. In K4 use a nested IF to calculate the reorder quantity.
- In L4 solve the same problem but using an IF and a VLOOKUP/XLOOKUP.
- In C13 we want to automatically number rows that have items. Check if D13>0, if it is add 1 to C12, otherwise leave blank. Copy the formula down to C36.
- In E12 use a VLOOKUP to look up the item description for the Item code in the Inventory table. Copy down to E36.
- Where there are no item codes you will get an N/A. Add an IFERROR to the formula to leave the cell blank if an error occurs.
- In F12 use a VLOOKUP to look up the category for the Item code in the Inventory table. Copy down to F36.
- Add an IFERROR to the formula to leave the cell blank if an error occurs.
- In H12 use a VLOOKUP/XLOOKUP to get the retail price for that item from the inventory table, again adjusting the formula to show "" instead of N/A. Copy to H36.
- In I12 use the combination of INDEX and MATCH formula to create a dynamic lookup function.

## Process
- Use an IF function to determine stock status (below minimum or not)
- Combine the use of IF function with AND and NOT to determine the reorder status.
- Use the nested IF function to calculate the retail price and reorder quantity.
- Use VLOOKUP to populate the Item Description/Details based on the Item Code.
- Use the combination of INDEX and MATCH to create a dynamic lookup.
- Use the IFNA and IFERROR to handle potential missing or error values.
- The <a href="https://github.com/DennyMandaka/Populating-and-Analyzing-Data-with-Logical-and-Lookup-Functions-in-Excel/blob/main/Inventory.png">result</a> is like this and <a href="https://github.com/DennyMandaka/Populating-and-Analyzing-Data-with-Logical-and-Lookup-Functions-in-Excel/blob/main/Customer%20Quote.png">like this</a>.

## Insights and Conclusion
- Logical functions like IF, AND, and NOT simplify decision-making by automating checks, such as identifying items below minimum stock levels or calculating retail prices
- Lookup functions (VLOOKUP, INDEX, and MATCH) enable efficient data retrieval from large tables, ensuring accurate and dynamic analysis for inventory management
- Using IFERROR and IFNA ensures that potential errors, such as missing data, are managed gracefully, improving the reliability of analysis.
