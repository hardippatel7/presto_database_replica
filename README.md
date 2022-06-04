# presto_database_replica
The repo contains the .sql file of the database of the Presto mobile app. 

Open your Oracle SQL Developer and import the file on an empty schema. It will populate the strcture of the database.

--metadata--
database information:
Oracle Database 11g Express Edition Release 11.2.0.2.0 - 64bit Production
PL/SQL Release 11.2.0.2.0 - Production
"CORE	11.2.0.2.0	Production"
TNS for 64-bit Windows: Version 11.2.0.2.0 - Production
NLSRTL Version 11.2.0.2.0 - Production

--strucutre information--
list of tables:
ADDRESS
PRESTO_USER
SAVED_PAYMENT_METHOD
PRESTO_CARD
TRANSIT_SYSTEM
STOP_LOCATION
ACTIVITY
TRANSACTION

list of indexes:
ACTIVITY_USER_ID_INDEX
PRESTO_CARD_NUMBER_INDEX

list of triggers:
#To deduct balance (if applicable) on each tap
deduct_balance_on_activity


list of functions:
#Function to get total money spent by a Presto Card
get_total_spending

#Function to create a new Presto User
create_new_user

list of procedures:
#Procedure to Add New Presto Card
add_new_presto_card

#Procedure to Enable Auto Pay
enable_auto_pay

list of packages:
presto_package
