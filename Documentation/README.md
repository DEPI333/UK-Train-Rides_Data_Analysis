## Power Query Documentation:

Extraction & schema typing: Automated data ingestion with explicit type transformations.
Text standardization: Cleaning and consolidating journey status, delay reasons, and station names.
Data consistency fixes: Correcting delay logic when scheduled and actual arrival times matched.
Missing value handling: Imputing missing railcards (No Railcard), delay reasons (No Delay), and cancelled arrival times.
Surrogate key creation: Generating composite primary/foreign keys (Ticket_ID, Route_Key).
Star Schema dimensional modeling: Splitting the flat file into Fact_Journey, Dim_Ticket, Dim_Route, and Dim_Date.

Technical Documentation: View Power Query Cleaning Documentation

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

