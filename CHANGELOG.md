# SalesTracker – Change Log

## Version 3.0.0 – 2026/02/13
### Added
- Persistent JSON Storage: Introduced inventory.json file handling. Data is now saved to the hard drive and loaded automatically on startup.
- Main Menu Loop: Added a navigation menu that allows the user to perform multiple actions without restarting the program.
- Restock System: Added a new feature to increase stock levels of existing items without changing their price or original entry.
- Delete Function: Added the ability to permanently remove items from the inventory list.
- Input Validation: Implemented a check for numerical inputs to prevent the program from crashing if a user types letters or symbols into price/stock fields.
- Low Stock Alerts: Added a (!) in the sales report to notify users when an item has 5 or fewer units remaining.
### Changed
- Improved Logic: The user can now search items to record a sale
- Formatted Reporting: Updated the report output layout for better readability
- Capitalization Handling: Items are now capitalized to ensure consistensy (ex. apple and Apple are treated the same)

### Fixed
- Stock Over-selling: Fixed a bug where the user can sell more units that there were actually in stock.
---

## Version 2.0.0 – 2025/08/19
### Added
- Introduced multiple product support.
- Implemented functions for adding items, processing sales, and showing reports.
- Tracks remaining stock and number of items sold.
- Generates a detailed itemized sales report.

### Changed
- Improved program structure with modular functions (`add_item`, `sell_item`, `show_report`).
- Reorganized logic for easier readability.

---

## Version 1.0.0 – 2025/08/15
### Initial Release
- Created the basic program structure.
- Added ability to input product names, prices, and quantities.
- Program automatically calculates total sales.
- Displays itemized receipt with product totals.
