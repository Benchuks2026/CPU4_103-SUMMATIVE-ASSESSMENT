README
CROWNFIELD EYE Hospital Database System
Overview

Store patient information securely.
Manage clinician and specialty records.
Record clinic locations and appointment schedules.
Track diagnoses and prescribed medicines.
Support follow-up appointments.
Reduce data redundancy through normalization.
Enforce business rules using triggers.
Support efficient retrieval of information through SQL queries.
Database Structure

The database consists of the following tables:

Patient
Specialty
Clinician
Clinic
Diagnosis
Medicine
Appointment
AppointmentMedicine 
FollowUp

Normalisation

The database was normalised to Third Normal Form (3NF):

1NF: Removed repeating groups and ensured atomic values.
2NF: Removed partial dependencies by creating separate entity tables.
3NF: Removed transitive dependencies by separating specialties, diagnoses, and medicines into independent tables.

This process improved data integrity and reduced duplication.


The database QUERRY CODES includes:

Aggregate Query using GROUP BY and HAVING
INNER JOIN across multiple related tables
LEFT JOIN to identify missing records
Common Table Expression (CTE) / Subquery
Stored Procedure with an input parameter
Trigger enforcing appointment booking rules
Security Features

To improve security and data integrity:

Access controls can be implemented using SQL GRANT and REVOKE permissions.
Foreign key constraints maintain referential integrity.
Triggers automatically enforce business rules.
Sensitive patient records can be restricted to authorised users only.
Technologies Used
MySQL Workbench
MySQL Database Server
SQL (DDL, DML, DQL)
Entity Relationship Modelling (ERD)
Sample Business Rule

A trigger was implemented to prevent a patient from being booked for more than three appointments on the same day. This ensures valid scheduling and improves data quality.

