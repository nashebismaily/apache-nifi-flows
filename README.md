# Apach Nifi Flows

This is a collection of Apache Nifi flows using Hortonworks Data Flow

## Oracle to Hive

This flow will:  
1) Query the Oracle database for a table and load the results into a flowfile in AVRO format.  
2) Split each row of the results from Oracle into a new flowfile.  
3) Create attributes representing the Oracle table column names in each flow file.   
4) Create a HiveQL insert statement for each row from the Oracle Table.  
5) Send the HiveQL insert statement to Hive.  
