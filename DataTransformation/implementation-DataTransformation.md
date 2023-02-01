Here is an example of transforming ingested data using Azure Data Factory (ADF) and Azure Synapse Analytics with code:

Create an Azure Data Factory: Go to the Azure portal and create a new Azure Data Factory.

Create a Data Source: In the Azure Data Factory, create a data source. This could be a file-based source like a CSV or a database like Azure SQL Database.

Create a Data Set: In the Azure Data Factory, create a data set that points to the data source created in step 2.

Create a Pipeline: In the Azure Data Factory, create a pipeline that contains a Data Transformation activity. The Data Transformation activity uses a SQL script to transform the data from the data set created in step 3.

Run the Pipeline: In the Azure Data Factory, run the pipeline created in step 4 to transform the data.

-----
TransformData.json:-
In this example, <dataSetName> is the name of the data set created in step 3, <synapseTableName> is the name of the Azure Synapse Analytics table where the transformed data will be loaded, <storedProcedureName> is the name of the stored procedure that performs the data transformation, and <parameter1> and <parameter2> are placeholders for the parameters passed to the stored procedure. The values of these parameters are specified in the storedProcedureParameters section.