# SQL-SSMS-Services
How does SQL Work ?

<img width="1918" height="1112" alt="Screenshot 2026-04-05 101229" src="https://github.com/user-attachments/assets/1cacf9cd-d1a3-49cb-8400-f8ff736c9d1c" />

**Database Setup Process**
Installed SQL Server and SQL Server Management Studio (SSMS).
Downloaded the sample backup database file: AdventureWorks2025.bak.
Connected to the local SQL Server instance through SSMS using Windows Authentication.
Entered the default master database.
Opened Restore Database from the Databases menu.
Selected Device as the source and provided the path to the downloaded AdventureWorks2025.bak file.
Refreshed the file location and added the backup file to the restore plan.
Restored the database under the name AdventureWorks2025.
Verified that the database was successfully loaded into SSMS and confirmed accessibility through SQL queries.

**How is an SQL database formed?**
Raw data usually begins as unstructured or semi structured information coming from sources such as Excel files, CSV files, PDFs, application forms, system exports, or user input. This source data is first cleaned and standardized so that values are consistent, duplicate records are reduced, missing fields are handled, and business attributes are clearly identified. Once the data is prepared, it is mapped into a relational structure. Each business subject is separated into its own table, such as Employee, Department, Customer, or Order. Within each table, columns are defined to represent the attributes of that entity, such as EmployeeID, JobTitle, HireDate, or DepartmentName, and each row represents one individual record stored under that structure. Related tables are then grouped under schemas such as HumanResources, Sales, or Person in order to organize them by business function. These schemas together exist inside a database, which acts as the full container for all related tables, relationships, keys, constraints, and stored records. After the database has been fully created and populated inside SQL Server, SQL Server can generate a backup file from that complete database by executing a T SQL backup command such as BACKUP DATABASE. At that point, the .bak file becomes a backup representation of the already built database, containing the organized structure and data that SQL Server can later restore as a complete database environment.
