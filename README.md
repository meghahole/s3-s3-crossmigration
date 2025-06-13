## Project Overview
In this project, we are using AWS S3, SNS, SQS, and Lambda to transfer a data file from an S3 bucket in the source region to an S3 bucket in the target region (your default region).

Once the data is loaded into the target region's S3 bucket, we will use SQS to send a notification to trigger Glue crawler to generate a table in the Glue catalog.

After the table is created in the Glue catalog, we will leverage AWS Athena to query the data and analyze its contents.
