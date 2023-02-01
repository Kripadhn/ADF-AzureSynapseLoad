Here is an example of transforming ingested data using Azure Data Factory (ADF), Azure Databricks, and Azure Synapse Analytics with code:

Create an Azure Data Factory: Go to the Azure portal and create a new Azure Data Factory.

Create a Data Source: In the Azure Data Factory, create a data source. This could be a file-based source like a CSV or a database like Azure SQL Database.

Create a Data Set: In the Azure Data Factory, create a data set that points to the data source created in step 2.

Create an Azure Databricks Workspace: In the Azure portal, create an Azure Databricks workspace.

Create a Databricks Notebook: In the Azure Databricks workspace, create a new Databricks notebook.

Write Transformation Code: In the Databricks notebook, write the code for transforming the data. This could be in Python, Scala, or SQL.

Create a Cluster: In the Azure Databricks workspace, create a Databricks cluster to run the notebook.

Create a Pipeline: In the Azure Data Factory, create a pipeline that contains a Databricks Notebook activity. The Databricks Notebook activity runs the notebook created in step 5 on the cluster created in step 7.

Run the Pipeline: In the Azure Data Factory, run the pipeline created in step 8 to run the notebook and transform the data.

-------
TransformData-Databricks.json:-
In this example, <previousActivity> is the name of the activity that runs before the Databricks Notebook activity, <dataSetName> is the name of the data set created in step 3, <synapseTableName> is the name of the Azure Synapse Analytics table where the transformed data will be loaded, <notebookPath> is the path to the Databricks notebook, and <parameter1> and <parameter2> are placeholders for parameters that can be passed to the Databricks notebook. The values of these parameters are specified in the baseParameters section.