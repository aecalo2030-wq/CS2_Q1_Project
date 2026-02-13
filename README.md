# SalesTracker: Daily Sales Calculation

## Project Description
SalesTracker is a simple Python-based program that helps small businesses, shops, or individual sellers calculate total sales, track inventory, and generate sales reports.  
The program allows users to input product names, prices, stock quantities, and the number of items sold. It then calculates revenue, updates stock levels, and displays an itemized report.

## Features
- Input multiple product names, prices, and stock quantities.
- Record sales for each product.
- Automatically calculate total sales.
- Track remaining stock after purchases.
- Display a clear sales report with itemized totals.
- (Planned) Support for discounts, sales tax, and data saving.
- Persistent Storage: Saves all data to a JSON file so information is not lost when the program closes.
- Menu-Driven Interface: Includes options to record sales, restock items, add new products, and delete entries.
- Low Stock Alerts: Automatically flags any item with 5 or fewer units remaining.
- Input Validation: Prevents the program from crashing if a user enters invalid text or negative numbers.
- Detailed Reporting: Displays a formatted table showing prices, units sold, stock levels, and total revenue.

## How to Run the Program
1. Install Python (version 3.7 or later recommended).
2. No External libraries required  
3. Clone or download this repository.  
4. Open the program file (`sales_tracker.py`) in VS Code or your IDE of choice.  
5. Run the program:
   - In Codespaces: click **Run ▶** or use the terminal with  
     ```bash
     python sales_tracker.py
     ```
   - In IDE's: Copy the code and click **Run** to activate the code
5: How to use:
   - Add items: Use option 3 to add items to your store with products and       prices.
   - Record Sales: Use option 1 to subract stock and increase sold counts,       this also counts the money earned.
   - Restock: Use option 4 to add more units/stocks to an existing item.
   - View Report: Use option 2 to see your total earnings and current            inventory status.
6. File Structure:
   - main.py: This is the core of the program
   - inventory.json: This is where the files of your items are saved
### Note: If you close the program in some IDE's, it does not save the files as it has no external database to save it to.

### PREVIEW:
Step 1: Running the code
When you start the script, it checks for inventory.json. If it's the first time, it starts empty.

 MINI STORE V3.0.0 
1. Record Sale      4. Restock Item
2. View Report      5. Delete Item
3. Add New Item     6. Exit

Select Option: 3
Step 2: Adding an item
You enter the details for a new product.

Enter item name: Coke
Enter price of Coke: PHP 25
Enter starting stock: 10
Item Coke added successfully.
Step 3: Making a sale
Now, let's say a customer buys 2 bottles.

Select Option: 1

Item being sold: Coke
Quantity (Available: 10): 2
Sale recorded: PHP 50.00
Step 4: Viewing the report
The system calculates the math and shows you the current status.

Plaintext
Select Option: 2

ITEM NAME       | PRICE      | SOLD   | STOCK    | SALES     

Coke            | PHP 25.00     | 2      | 8        | PHP 50.00     

GRAND TOTAL REVENUE: PHP 50.00
Note: Items marked with '!' have low stock (5 or less).

Step 5: Closing and Reopening
If you select Option 6 (Exit), the program stops. If you open your folder, you will see inventory.json. When you run the script again tomorrow and press Option 2, that table will look exactly the same and the 2 sales and 8 remaining stock are preserved.

## Contributors
- **Student 1:** Aldrin Edrian C. Calo  
- **Student 2:** Azziah Glyre C. Alfeche  
- **Student 3:** Gianna Olivia L. Dy
