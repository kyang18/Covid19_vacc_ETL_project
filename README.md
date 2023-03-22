# Covid19_vacc_ETL_project

Our team's objective is to create clean datasets that can be used to compare various variables and their relationship with Covid vaccine rollouts worldwide.

Members:
William Powell,
Jungkyu Kim,
Kaixin Yang,
Hannah Slay,
Alex Gainer.

We obtained the original data sources from Kaggle, including Covid World Vaccination Progress, World Happiness Data, and UN Country Statistics, which were all in CSV format. We used pandas to read the CSV files and dropped unnecessary columns. We also retrieved the most recent date from each dataset using the .max() function and merged the most recent date dataframe with individual datasets to isolate the latest date. We set the index to country and formatted erroneous records using .replace().

We created an ERD using Quick DB Diagrams and created tables and relationships in Postgres. The cleaned tables were loaded into Postgres using .to_sql in our Jupyter Notebook. We chose this method for loading the final database, tables, and collections because it is efficient and allows for easy querying and analysis of the data.
