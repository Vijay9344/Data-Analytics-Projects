Instamart Sales Performance Dashboard

📝 Project Overview
This Power BI project analyzes **Instamart sales performance** across products, outlet types, and fat content.  
The goal is to provide clear business insights into sales contribution, outlet trends, and customer preferences.
🧹 Data Cleaning & Transformation
Raw Data Issues
•	Missing values in `Item Weight` and `Outlet Size`
•	Inconsistent labels in `Fat Content` (e.g., "LF", "low fat", "reg", "Regular")
•	Duplicate rows present
•	Unstructured outlet types
Steps Performed
1.	Removed Duplicates – ensured each transaction is unique  
2.	Handled Missing Values
•	Item Weight` → filled using mean values by item category  
•	`Outlet Size` → imputed using mode based on outlet type  
1.	Standardized Columns
•	Renamed headers to consistent format  
•	Corrected categorical spelling issues  
2.	Transformed Data
•	Normalized Fat Content → `Low Fat`, `Regular`  
•	Created `Total Sales = Item_Outlet_Sales`  
•	Grouped similar items into categories
3.	New Fields / Measures (Power BI DAX)  
•	`Total Sales = SUM(Item_Outlet_Sales)
•	`Average Sales = AVERAGE(Item_Outlet_Sales)`  
•	`Total Items = DISTINCTCOUNT(Item_Identifier)`  
•	`Average Rating` (calculated from review scores if available)  
•	📊 Dashboard Insights
KPIs
•	Total Sales → ₹1,202K  
•	Average Sales per Item → ₹141  
•	Total Items Sold → 8.5K  
•	Average Rating → 4.0 ⭐  
Key Findings
1.	Fat Content
•	Low Fat → ₹425K sales (most preferred)  
•	Regular → ₹776K sales  
2.	Item Categories
•	Fruits & Vegetables → highest sales (₹178K)  
•	Snacks & Household products follow next  
3.	Outlet Size
•	Medium outlets → ₹741K sales (major contributor)  
4.	Outlet Location
•	Tier 3 cities lead with ₹472K sales  
•	Tier 1 contributes the least  
5.	Outlet Type  
•	Supermarket Type1 dominates with ₹787K sales  
6.	Yearly Trends (2012–2022)
•	Peak in 2018 → ₹204.5K  
•	Consistent growth until 2018, slight dip afterwards  
7.	⚙️ Tools & Techniques
•	Power BI Desktop (visualization & reporting)  
•	Power Query (data cleaning & transformation)  
8.	DAX (measures & KPIs)  
•	Charts Used → KPI Cards, Donut Chart, Bar Chart, Line Chart, Matrix  

 📂 Repository Files
•	`Instamart_Dashboard.pbix` → Power BI file  
•	`Dashboard.png` → Dashboard screenshot  
•	`README.md` → Documentation  

👤 Created by: Vijay Kumar L
