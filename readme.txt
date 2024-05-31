our data source or data set: https://www.kaggle.com/datasets/krishd123/olympics-legacy-1896-2020
mega table or main table : Athlete.csv

Tables Creation:
We created the following relations using create.sql:

R1 (Athletes): AthleteID → Name, Gender, Age
R2 (Teams): TeamID → TeamName, NOC
R3 (Sports): SportID → SportName
R4 (Venues): VenueID → City, Country
R5 (Events):
EventID → EventName, Year, Season
SportID → EventID
VenueID → EventID
R6 (Medals): MedalID → MedalType
R7 (AthleteEvents): (AthleteID, EventID) → MedalID
R8 (TeamEvents): (TeamID, EventID) → MedalID

Database Integration
We established connections and decomposed, normalized and integrated all the tables to form a database normalize.db using a Python script file script.py.

Loading Values into Tables:
We uploaded .csv files to pdadmin (PostgreSQL) and used load.sql to insert values into respective attributes of every table.

Query Execution:
We demonstrated various queries on normalize.db through PostgreSQL.

Results and Report:
Query were analyzed,optimized and included in milestone2.pdf.

