# Crowdfunding_ETL ReadMe

Overview:
In this project, we created an ETL data pipeline using Python and Pandas to 
extract and transform the data. Once the data was transformed, we created 
CSV files with the transformed data and created table schema’s in a Postgres
database.

In the attached Jupiter notebook, we used python to create 4 dataframes 
outlined below:

     -Category dataframe
        - This dataframe extracts each unique category ID and includes a 
          column to what unique category that that id corresponds to
    -Subcategory data frame
        -Similarly to the first dataframe, this dataframe extracts the 
         unique SUBcategories in the dataframe and their unique id’s
    -Crowdfunding dataframe
        -Using the provided excel data, we created a dataframe in python
         with all required columns, reformatting certain columns and 
         values to best suit the data type (ex: datetime format for launch 
         dates and float data type for numerical values in the “goal” and 
         “pledged” columns)
    -Contacts dataframe
        -Using dictionaries in Python, we created a dataframe from the 
         contacts excel provided to include the first name, last name and 
         email address of each contact id listed. We also used python to 
         split the first and last name from the data in separate columns

Finally, we created a Postgres database and schema to upload the created 
csv files into tables, keeping in mind the correct order required for foreign 
and primary keys created for the tables.
