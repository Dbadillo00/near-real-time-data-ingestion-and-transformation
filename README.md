# near real-time data ingestion and transformation

I wanted to create a near real-time data ingestion for Ecommerce transactions. Data about purchases, product views, or shopping cart interactions, used for tracking customer behavior and real-time marketing strategies can be extremely useful for e-commerce businesses. 

Kinesis Data Streams are designed for real-time data streaming, allowing applications to consume and process the data with very low latency.

Kinesis Data Firehose prepares and loads the data continuously in near real-time to a predefined destination.

In this project, I: 

•Deployed a solution to Ingest Ecommerce transaction data
•Modified a Lambda function to parse .csv data and convert each row into a JSON object
•Sent each JSON object as a separate record to the Kinesis Data Stream
•Configured a Kinesis Data Firehose delivery stream to read from a Kinesis Data stream 
•Loaded the converted data into Amazon S3 as the final storage
