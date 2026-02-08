## Inventory Alert Automation (UiPath)
This is a simple inventory alert program built with basic RPA knowledge using UiPath Studio. It was my first try at making an inventory tool, so the focus is on clear logic, not on complex features.

## How it works
1. I first created a sample Excel file with part numbers, current stock, and safety stock values.​

2. UiPath Studio reads this Excel file into a DataTable.

3. Inside a For Each Row loop, the workflow uses if statements to check the stock level for each item:
 * If Current_Stock == 0, it sends a critical stock-out email to the person in charge.
 * Else if Current_Stock < Safety_Stock, it sends a warning email about low stock.
​
4. All emails are sent automatically, without manual checks.

## Email requirement
For real use, the project needs a business (enterprise) email account connected to Microsoft 365 / Outlook.
Free personal email accounts can have security limits, so they may block automatic sending from UiPath.

If you want, you can tell me your current UiPath or RPA level, and this README can be adjusted to match your experience.
