AIM: 
To create and drop triggers in PL/SQL 
PROCEDURE: 
TRIGGER :A Trigger is a stored procedure that defines an action that the database 
automatically take when some database-related event such as Insert, Update or Delete occur.  
TYPES OF TRIGGERS:The various types of triggers are as follows, 
•	Before: It fires the trigger before executing the trigger statement. 
•	After: It fires the trigger after executing the trigger statement. 
•	For each row: It specifies that the trigger fires once per row. 
•	For each statement: This is the default trigger that is invoked.
It specifies that the trigger fires once per statement. 
VARIABLES USED IN TRIGGERS: 
:new :old 
These two variables retain the new and old values of the column updated in the database.
The values in these variables can be used in the database triggers for data manipulation Syntax: 
Create or replace trigger <trg_name> Before /After Insert/Update/Delete 
[of column_name, column_name….] on <table_name> [for each row] [when condition] begin ---statement end; 
Create a trigger that insert current user into a username column of an existing table Procedure
for doing the experiment: 
1.	Create a table student4 with name and username as arguments 
2.	Create a trigger for each row that insert the current user as user name into a table
3.  Execute the trigger by inserting value into the table
