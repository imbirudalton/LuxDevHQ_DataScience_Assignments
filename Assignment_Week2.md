# Power BI Project: Electronics Sales Data

## Objective
This project is designed to guide you through the entire Power BI workflow for a real-world scenario involving dirty sales data. You’ll be tasked with cleaning, analyzing, and modeling the data to create a comprehensive dashboard and a detailed report that includes key business insights.

The dataset includes various real-world challenges such as inconsistent data, missing values, and currency discrepancies. Your goal is to transform this data into something useful for decision-making in an electronics retail business.

---

## Instructions

## Step 1: Data Cleaning
Data cleaning is often the most time-consuming part of any analytics project. It's essential to ensure that your data is both accurate and consistent.

### 1. Ensure Consistency in Data Types
Some columns might have inconsistent data types.
- `OrderDate` → should be a date  
- `SalesAmount` → should be numeric  
Check for any text values that don't match the expected format.

### 2. Check for Spelling Errors
Look for inconsistencies in:
- Product names
- Country names
- Customer emails  

Example:
- "Samsung Galaxy S21"
- "Samsung GAlaxy S21"

**Tip:** Use filters to standardize values.

### 3. Missing or Incomplete Data
Check for empty or missing values in:
- Profit  
- SalesAmount  
- ShippingCost  

Decide whether to:
- Remove  
- Impute  
- Fill missing values  

### 4. Pseudonyms and Invalid Entries
Handle entries like:
- "Anonymous"
- "N/A"

Example:
- A row with `CustomerName = "N/A"` in a paid transaction should be flagged.

### 5. Ensure Correct Data Formats
Standardize:
- Dates (`OrderDate`, `DeliveryDate`)
- Currency (`USD`, `EUR`, etc.)

Example:
- Convert `"usd"`, `"US Dollar"` → **"USD"**

---

## Step 2: Data Analysis
After cleaning, extract insights using DAX measures.

### 1. Calculate Total Sales
Create a measure to sum `SalesAmount`.

### 2. Profit Margin Calculation
Formula:
Profit Margin = (Profit / SalesAmount) × 100


Create measures for:
- Transaction level
- Product level
- Region level
- Time period

### 3. Currency Conversion
- Research exchange rates (USD, EUR, GBP, etc.)
- Convert all currencies into a single currency (e.g., USD)

Example:
- EUR → USD = 1.1

### 4. Handle Missing/Incorrect Values
Consider:
- Excluding rows  
- Adjusting values  

**Questions:**
- Should you remove extreme values?
- Should you adjust them based on business logic?

---

## Step 3: Data Modeling
Structure your data for efficient analysis.

### 1. Create Dimension Tables
Examples:
- Customer
- City
- Product Categories
- Sales Reps
- Time  

Example:
- **Product Dimension:** `ProductName`, `Category`

### 2. Fact Table
Contains:
- OrderID  
- SalesAmount  
- Profit  
- Quantity  
- Discount  

Create relationships with dimension tables.

**Question:**
- How does the fact table relate to customers, products, and time?

### 3. Time Dimension
Include:
- Year  
- Quarter  
- Month  
- Week  
- Day  
- Date  

Used for:
- Trends  
- Time-based analysis  

---

## Step 4: Building the Dashboard
Create an interactive dashboard.

### 1. Key Visualizations
Use only necessary visuals:

- **KPI Cards:** Total Sales, Total Profit, Profit Margin  
- **Bar/Column Chart:** Sales by product, region, category  
- **Line Chart:** Sales trends over time  
- **Pie Chart:** Sales distribution  
- **Map Visual**

### 2. Slicers
Add filters for:
- Region  
- Customer  
- Time period  
- Product category  

Example:
- Year slicer

---

## Step 5: Creating the Report

### 1. Executive Summary
Include:
- Sales performance  
- Top products  
- Profitability  

### 2. Detailed Analysis
Breakdown of:
- Sales by region  
- Profit margins by product  
- Trends over time  

### 3. Visual Insights
Answer questions like:
- What are the top-performing products?  
- Which region has the highest profit margin?  
- How are sales trending?  

### 4. Recommendations
Examples:
- Promote high-performing products  
- Improve low-profit regions  

---

## Analysis Questions
- How do exchange rates affect sales?
- How do repeat customers impact analysis?
- Should missing values be removed or filled?

---

## Power BI Report Structure

### 1. Pages
- Reports can have multiple pages (like slides)
- Each page focuses on a specific analysis

### 2. Main Page (Dashboard)
- KPI cards  
- Slicers  
- Key visuals  

### 3. Additional Pages
Examples:
- Page 1: Overview  
- Page 2: Product Performance  
- Page 3: Geographic Analysis  
- Page 4: Customer Insights  

### 4. Navigation
- Use tabs or buttons
- Add "Next Page" / "Back" buttons

---

## Steps to Organize Pages

### 1. Create New Page
- Click "+" in Power BI
- Rename appropriately

### 2. Design Dashboard Page
- Add KPIs  
- Add charts  
- Add slicers  

### 3. Create Additional Pages
- Focus on one analysis per page  

### 4. Add Interactivity
- Buttons for navigation  
- Drill-down features  

### 5. Final Structure
- Page 1: Overview  
- Other pages: Detailed insights  

---

## Navigation
- Use page tabs  
- Add navigation buttons  

---

## Conclusion
This project covers the full Power BI workflow:
- Data cleaning  
- Data modeling  
- DAX calculations  
- Dashboard creation  

By the end, you will have a complete Power BI dashboard and report that provides meaningful insights into an electronics sales business.
