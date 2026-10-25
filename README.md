
# eBay Sales Dashboard (Power BI)
 
An interactive Power BI dashboard analysing 12 months of sales data from a family-run eBay store selling magnetic jewellery. It was built to answer practical business questions and provide further insights into sale demographic and postage metrics.
  
## Key findings
 
- **Promoted listings drive most sales:** 90% of sales came through promoted listings.
- **Fast dispatch:** 30% of orders ship the same day, with a median of 1 day from sale to dispatch.
- **A few products dominate:** the top item sold 142 units, over 2x the next best.
- **Where customers are:** The majority of sales came from customers in east England.
## Dashboard contents
 
- **KPI cards:** revenue, orders, quantity sold, average days from sale to dispatch.
- **Top 10 products:** ranked by units sold, labelled with each item's most frequent title.
- **Promoted vs non-promoted listings:** share of sales by listing type.
- **Sales over time:** monthly trend with a month slicer to filter the whole page.
- **UK shape map:** sales by postcode area.
## How it was built
 
1. **Data cleaning (Power Query):** removed personal and identifying columns (buyer usernames, postcodes, order and transaction IDs), fixed data types, and kept only the postcode area (e.g. "BS") for the map.
2. **Modelling:** added a calendar table for time analysis.
3. **DAX measures:** examples below.
4. **Visualisation:** layout, slicers and formatting designed for quick reading, with the key numbers at the top.

 
## Data and privacy
 
The raw export is **not** included in this repository. Buyer usernames, postcodes, order numbers and transaction IDs were removed before building the report, and the screenshot contains no personally identifiable information.
 
## Tools
 
Power BI Desktop, Power Query (M), DAX

## Data sources
Many thanks for the resource hosted on the University of Edinburgh's DataShare
- Postcode area boundaries: *GB Postcode Areas* [Dataset], University of Edinburgh, Edinburgh DataShare. https://datashare.ed.ac.uk/handle/10283/2405
  Converted from ESRI Shapefile to TopoJSON for use in a Power BI shape map.
