Here is an example of integrating data from multiple sources into Azure Synapse Analytics using Azure Data Factory (ADF) with code:

Create an Azure Data Factory: Go to the Azure portal and create a new Azure Data Factory.

Create Data Sets: In the Azure Data Factory, create data sets for each source of data that needs to be integrated. For example, if the data is stored in Azure Blob Storage, Azure Data Lake Storage, or any other storage location, create a data set for each of those locations.

Create a Destination Table: In Azure Synapse Analytics, create the table where the integrated data will be loaded.

Create a Copy Activity: In the Azure Data Factory, create a pipeline that contains a Copy activity for each source of data. The Copy activity copies the data from each source to the destination table in Azure Synapse Analytics.

---------

LoadIntegratedData.json:-
In this example, <sourceDataSet1Name> and <sourceDataSet2Name> are the names of the data sets created in step 2, <synapseTableName> is the name of the Azure Synapse Analytics table where the integrated data will be loaded, Overwrite is the copy behavior, which means the existing data in the destination table will be overwritten, writeBatchSize is the number of rows to write in a single batch, writeBatchTimeout is the time after which a batch write operation times out, sqlWriterStoredProcedureName is the name of the stored procedure that will be used to write the data to the destination table, UnionAllSource is the type of source that will be used to perform the integration, and sources is an array of sources to be integrated.