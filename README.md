# Electric Vehicle Market Analysis – Washington State

The goal of this project is to perform an exploratory data analysis (EDA) of electric vehicle registrations in Washington State. The main objective is to identify key trends by year, manufacturer, and vehicle type. The project includes three main stages: data cleaning in Excel, data analysis using SQL, and data visualization

---

 1. Data Cleaning (Excel)

The original dataset contained 246,000+ rows and 17 columns with categorical, numerical, and geolocation data. Cleaning steps included:

- No duplicates found based on VIN.
- `Vehicle Location` was split into `Latitude` and `Longitude`.
-  Missing values handled:
-  Rows with blanks in key fields like `County`, `City`, and `Base MSRP` were removed.
- `Legislative District` (540 blanks) filled with `"Unknown"`.
-  Column `Base MSRP` was dropped due to 98% missing or zero values.

These steps ensured the dataset was consistent and ready for structured analysis in SQL and visualization in Tableau.

---

2. Data Analysis (SQL)

Using SQL (PostgreSQL), I explored patterns in EV adoption:

- Top EV brands by number of registered vehicles.
- Distribution by EV type (Battery Electric, Plug-in Hybrid).
- Registrations per year to track growth over time.
- Tesla’s growth after 2020 and its yearly market share.
- Top 3 models per brand using a window function (RANK).
- Cumulative adoption trends via running totals.

---

3. Interactive Dashboard (Tableau)

Key insights were visualized in an interactive dashboard published on Tableau Public:

- EV registrations by year  
- Top brands and models  
- Distribution of EV types  
- Geo distribution by county  
- Tesla’s growth trend and market share  

View the dashboard on Tableau Public: (https://public.tableau.com/app/profile/nazar.kapto/viz/ElectricVehicleAdoptioninWashingtonState/Dashboard1)

