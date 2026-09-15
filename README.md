# Flutterco-Group-of-Companies-Sales-Report-2022-
This report provides a technical analysis of the Flutterco Group of Companies Sales Report for the Year 2022.  The dashboard serves as a comprehensive Business Intelligence (BI) tool designed to monitor Key Performance Indicators (KPIs), analyze regional trends, evaluate sales representative performance, and identify high-value customer segments.
The data indicates a highly seasonal sales cycle with significant dependency on the North Region and the New York market. However, technical observation reveals the dashboard is currently in a filtered state, isolating data for specific entities (Salesperson: Nancy Freehafer, Product: Chocolate Biscuit Mix, Customer: Company J), which alters the context of the visualizations from a macro-company view to a micro-segment view.

2. Dashboard Architecture & Data Model
The dashboard utilizes a standard star-schema layout, partitioned into four distinct functional zones:
Header (KPIs): Summary cards for instantaneous status checks.
Main Canvas (Visualizations): A mix of time-series, comparative, and geospatial charts.
Right Panel (Slicers): Interactive filters controlling the entire dataset.
Data Points: The dashboard tracks metrics including Revenue ($), Transaction Count, and Percentage of Total.

3. Technical Analysis of Visual Components
3.1. KPI Header Section
Peak Season: June was identified as the month with the highest sales trend.
Regional Leader: The North region dominates performance.
Geographic Leader: New York is the top-performing city and state.
Top Transaction: Recorded at $67,180.50.
Top Rep: Nancy Freehafer.
Product Insight: "Beverages" were flagged as sold out, indicating a potential supply chain constraint or stockout scenario in 2022.
3.2. Sales Trend Report (Time Series)
Visual Type: Line chart with data labels.
Observation: High volatility. The trend line exhibits a "W" shape with significant dips in June ($671.20) and November ($1,477.60), contrasting with sharp peaks in March ($1,564.00) and December ($2,922.80).
Technical Insight: The December spike suggests a Q4 seasonal push or a large bulk order (likely attributable to the "Company J" filter). The low granularity suggests daily data is being aggregated at the monthly level.
3.3. Top 6 Ship Cities (Horizontal Bar Chart)
Visual Type: Horizontal Bar Chart (Descending Sort).
Data: New York leads significantly ($67,180.50), followed by Portland ($50,208.35) and Miami ($50,145.33).
Technical Insight: There is a steep drop-off after the top 3 cities. New York constitutes a disproportionately large share of revenue compared to Milwaukee ($37,428.00), the lowest on this list.
