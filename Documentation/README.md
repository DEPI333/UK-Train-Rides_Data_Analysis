## Analytical Questions & Business Scope Documentation:

Sales & Revenue Performance: Revenue trends (daily/weekly/MoM), route profitability, top-10 route Pareto analysis, and railcard pricing dynamics.
Customer Purchasing Behavior: Online vs. station split, payment preferences, booking lead-time analysis, and peak transaction hours.Ticket & Product Mix: Class distribution (First vs. Standard), volume vs. revenue contribution, and railcard utilization across ticket types.
Route & Station Network: Busiest network hubs, route pairing balance ($A \to B$ vs. $B \to A$), and high-volume commercial bottlenecks.Punctuality & Delay Analysis: On-time rates, delay distributions, root-cause clustering (signals, staffing, weather), and peak-hour operational impacts.
Refunds & Operational Impact: Refund request rates across delay severity brackets, revenue at risk, and delay-reason correlation.


## Power Query Documentation:

Extraction & schema typing: Automated data ingestion with explicit type transformations.
Text standardization: Cleaning and consolidating journey status, delay reasons, and station names.
Data consistency fixes: Correcting delay logic when scheduled and actual arrival times matched.
Missing value handling: Imputing missing railcards (No Railcard), delay reasons (No Delay), and cancelled arrival times.
Surrogate key creation: Generating composite primary/foreign keys (Ticket_ID, Route_Key).
Star Schema dimensional modeling: Splitting the flat file into Fact_Journey, Dim_Ticket, Dim_Route, and Dim_Date.

## Database Documentation:

The project uses a MySQL relational database hosted on FreeSQLDatabase.com, containing three dimension tables and one central fact table.

The database consists of 31,886 records across four tables and is integrated with Power BI for data modeling and analytical reporting.

Database Documentation includes:
- Database architecture and table definitions.
- Column names and data types.
- Primary keys and logical relationships.
- Database record counts.
- SQL validation and data integrity queries.
- Power BI database integration.

