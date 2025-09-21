#SQL-DATAWAREHOUSE-PROJECT
![DATA WAREHS](https://github.com/user-attachments/assets/17265289-dea6-4ef5-9a77-6af061e88c35)
Building a mordern sql-datawarehouse with sql, including ETL processes, data modeling and Analytics
Prior to 


PROJECT DESIGN FOR BRONZE STAGE IN SSMS
1. Creating the database and schemas
   <img width="1219" height="458" alt="d6 creating the database and schemas" src="https://github.com/user-attachments/assets/abc82bed-9068-4595-a958-90d8876de39c" />

2. Firts table created in datawarehouse from the source folder
   
   <img width="881" height="341" alt="D7 First table created in SSMS" src="https://github.com/user-attachments/assets/909e614f-f3c6-4489-998f-d9b78f791bce" />

3. DDL's have been fully created with poper naming conventions for the various tables
   
   <img width="712" height="205" alt="D8 DDL AND TABLES HAVE BEEN CREATED WITH PROPER NAMING CONVENTIONS" src="https://github.com/user-attachments/assets/fc55dbda-489e-4d40-b71e-89ce0e9fe6c5" />

4. Writing T SQL QUERY TO DROP AND RECREATE TABLE
   IF OBJECT_ID ('bronze.crm_cust_info' , 'U') IS NOT NULL
	DROP TABLE bronze.crm_cust_info;

Explanation : OBJECT_ID('bronze.erp_pz_cat_g1v2', 'U')
Returns the object ID of the table if it exists.

'U' specifies user tables (so it checks specifically for tables, not views, procedures, etc.).

IS NOT NULL
Means the table exists (because a valid object ID was found).

DROP TABLE bronze.erp_pz_cat_g1v2;
Removes the table if it exists.
