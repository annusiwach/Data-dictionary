# Task 1: Data Immersion & Wrangling
## Data-dictionary
The provided sales dataset consists of transactional records capturing customer dempgraphics, product details, and financial metrices. Below is the comprehensive data dictionary detailing the field definitions, data types,and business relevance for each attribute.
| Field Name | Data Type | Description | Business Relevance / Analytical Utility |
| **order_id** | Alphanumeric | Unique identifier assigned to each individual sales transaction. | Used to count total unique orders, calculate purchase frequency, and serve as a primary key for data joins.|
| **order_date** | Datetime | The exact date when the transaction took place. | Critical for time-series analysis, tracking seasonal sales trends, monitoring monthly growth, and understanding weekday vs. weekend purchasing behavior. |
| **customer_id** | Alphanumeric | Unique identification code assigned to an individual shopper. | Enables cohort analysis, tracking customer retention, calculating Customer Lifetime Value (CLV), and identifying loyal repeat buyers. |
| **customer_name**  | Alphanumeric | The full name of the customer. | Primarily used for personalized marketing campaigns or addressing specific accounts in B2B context; generally masked or omitted during statistical aggregation for privacy (PII). |
| **age** | Integer | The age of the customer in years. | Allows for demographic profiling. Crucial for understanding which generation (Gen Z, Millennials, Boomers) is buying specific products to optimize targeted ads. |
| **gender** | String | The self-identified gender of the customer (e.g., Male, Female, Non-binary). | Helps analyze purchasing preferences across different genders to tailor product development and marketing assets. |
| **city** | String | The geographic city where the customer resides / where the order was placed. | Drives regional marketing strategy, inventory allocation, expansion plans, and geographical sales distribution mapping. |
| **product** | String | The specific name or model of the item purchased. | Identifies top-performing products, slow-moving inventory, and helps track product-level stock velocity. |
| **category** | String | The broader product classification group (e.g., Electronics, Apparel, Home Decor). | Used for high-level revenue distribution analysis, cross-selling strategy, and analyzing macroeconomic category performance. |
| **quantity** | Integer | The volume or number of units of the product purchased in the single transaction. | Essential for supply chain management, determining demand elasticity, and calculating inventory turnover rates. |
| **unit_price** | Float / Decimal | The monetary price charged for a single unit of the product. | Helps monitor pricing strategy, evaluate discount impacts, and analyze margin thresholds. |
| **total_sales** | Float / Decimal | The total revenue generated from the transaction. Calculated as: quantity × unit_price. | The primary financial KPI. Used to evaluate absolute business performance, calculate overall gross revenue, and measure financial growth. |
