To schedule data ingestion and transformation processes to run on a regular basis with code implementation in Azure Data Factory (ADF), you can use the "Trigger" feature in ADF. Here's an example of how you can schedule a pipeline to run on a daily basis:

Create a pipeline that contains the data ingestion and transformation activities.

Create a trigger: In the Azure Data Factory, create a trigger that will run the pipeline on a daily basis.

----------

DailyIngestionAndTransformation.json:-
In this example, <pipelineName> is the name of the pipeline that contains the data ingestion and transformation activities, Day is the frequency of the trigger, which means the pipeline will run on a daily basis, interval is the number of days between each trigger run, startTime is the date and time when the first trigger run will occur, and timeZone is the time zone in which the trigger will run.

Once you've created the trigger, you can activate it to start the daily execution of the pipeline.