# big-data-wrangling-google-ngrams

## Project Overview
The scope of this data processing and analysis report is to document the workflow involved in filtering and reducing big data of Google Ngrams down to a manageable size, and then doing some analysis locally on our machine after extracting data.  

The [Google Ngrams](https://books.google.com/ngrams/) dataset was created by Google's research team by analyzing all of the content in Google Books - these digitized texts represent approximately 4% of all books ever printed, and span a time period from the 1800s into the 2000s.
The dataset is hosted in a public S3 bucket as part of the [Amazon S3 Open Data Registry](https://registry.opendata.aws/google-ngrams/). This data has been converted to CSV and hosted on a public S3 bucket.

### Summary of steps:
1. Spin up a new EMR cluster on AWS for using Spark and EMR notebooks.
2. Copy data from S3 to HDFS.
3. Analyze and filter data using Spark.
4. Read filtered data on local machine
5. Plot the number of occurrences of the token `data` over the years.

## Project Organization
