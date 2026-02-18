Hospital_db

This project creates a relational hospital database in MySQL to facilitate data extraction and analysis of hospitals, doctors, patients and prescriptions.
- Database design using ERD and pseudocode;
- Creation of relational tables using primary and foreign keys;
- Importing data from CSV files;
- Writing SQL queries to retreive and analyse data;
- Use of GitHub for version control.

There are four relational tables:
Hospitals,
Doctors,
Patients,
Prescriptions.

Hospitals, which employ many doctors, who treat many patients, who receive many prescriptions. In turn, prescriptions are prescribed by one doctor for one patient, patients are assigned to one doctor and a doctor works at one hospital.
Hospitals and doctors are linked for the Hospital_ID; doctors and patients are linked via the Doctor_ID (references Doctors as Person_ID), and prescriptions are linked to both doctors and patients via their Person_ID (Doctor/Patient_ID). Therefore, these foreign keys enforce relational integrity.
The primary keys were chosen based on the ID of each entity. This ensures data uniqueness, as each ID must be different.

ERD.png and Pseudocode show the entity relationship diagram and pseudocode (respectively) that were created during the planning of this project. 
1_createtables is the script used to create the database, move into it, create all 4 tables and set with primary and foreign keys.
2_loaddata is the script used to load data from the CSV files into these tables.
3_queries is the script used to extract and manipulate data, also ensuring all previous steps worked seamlessly.
Database.sql is the final, exported database.

The queries demonstrate filtering, ordering, aggregation and JOIN usage.
