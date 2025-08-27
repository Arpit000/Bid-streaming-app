#Bid-Streaming-App
![1_5xZQ_HlrH_nYaCnrmk94UQ](https://github.com/user-attachments/assets/f63dc10d-c7c7-4da5-9a4f-4a7b4fe6c1f9)

This is an end-to-end pipeline that fetches bid submissions from a flask website and inserts the data into a DB table and a backup file in parallel.

Mentioned below are the components,

Flask web application (producer).
Kafka topic (on Confluent-Kafka cloud).
Consumer group 1 (consumer 1 and 2) insert records into a MySQL table and Consumer group 2 (consumer 3) will backup records to a csv file.
MySQL DB table to store the bidding data.
