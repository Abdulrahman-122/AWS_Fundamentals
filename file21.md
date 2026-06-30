# Data Analytics:

  <img width="1680" height="412" alt="image" src="https://github.com/user-attachments/assets/42ab2106-838f-4cf4-925e-c6a403153a64" />
    
    Data pipelines for ETL(Extract,Transform,Load) process?
  
    - you gather data from different resources (Extract)
    - transform it into a consistent format for tools to consume.(Transform)
    - load it into destination system -> data warehouse.(Load)

    notes;
      - Data analytics people uses these data in order to provide it to
        -loan company to explain landing decisions.
        -Medical researcher to analyze clinical data.
        - insurance companies .
      -In the field of data analytics, analysts transform raw historical data 
        into valuable insights and trends.
  <img width="1194" height="390" alt="image" src="https://github.com/user-attachments/assets/cb3db5c3-cf3b-4ac9-be1b-c456009401c9" />

-----
# AWS data pipeline services?

    1.Data Ingestion services?
      contain;
        - moving data from source system to chosen storage.
        - use real-time ingestion if data you need it immediately.
        - use batch ingestion when some latency is tolerable.
      Services:
        1.Amazon Kinesis Data streams -> digest data from servers,sensors, apps...
          for real time ingestion of terabyte of data

        2.Amazon Data Firehose  
          move data from sources to lakes or warehouses.

    2.Data storage services: 
        this is the place where data come to
          like ; data lakes (store amount of row data)
                  warehouses for businesses intelligence.(data are structured)
          AWS services;
            Amazon S3:
              - store data lakes in it 
              - contain structured+ unstructured data.

           Amazon Redshift;
               - provide storing structured,semistructured data (warehouse data)
    3.Data Catalogin Service:
         -this is where your data + metadate are stored.
         services:
           - AWS Glue Data catlog;
               store metadata+your data in a catalog
    4.Data processing services:
      transoform data to be clean
      services:
        1.Aws Glue;
           make ETL process efficient and automated.
        2.Amazon EMR;
            used for large scale data processing -> handle infrastructure+cluster management
              Amazon EMR : support Apache Spark,Hadoop...
    5.Data analysis+visualization services?
        - visualization tools for develop insights about your data.
      services:
        1.Amazon Athena;
            analyze data in relation,non-relational data sources.
            access data hosted on S3
            or on-premises or in other cloud environments
        2.Amazon Redshift;
          run queries on massive data or parallel processing architecture to analyze those data
          it's contain columnar storage+massive parallel processing architecture.

        3.Amazon Quicksight;
          technical+non-technical people can make dashboard to report various data sources without managing infrastructure

        4.Amazon openSearch Service:
          -you can search for precise keyword matching or natural language queries.
          it also provide dashboard to monitor.


To rap up:
  consider this workflow;
  <img width="1680" height="1021" alt="image" src="https://github.com/user-attachments/assets/40a2836e-46ed-4b9a-a658-b2fead44237e" />

      - an ecommerce app that show products to customers
      - the team of this app Gather data to Amazon DynamoDB 
      - Then the team make ingestion for that data through an Amazon Kensis data stream
      - then they move data to wirehouse using Amazon firehose
      - then the team operate Lambda function to convert json format to CSV file in order to work on
      - then move to Amazon simple storage S3 
      - then move it To Catalog with metadata in order to make tables from that data using AWS Glue Data Catalog
      - then use Amazon Athena to visualize it into structured ,non structurd format
      -also don't forget we take data from Amazon S3 to Amazon SegaMaker AI in order to allow ML team to train the models on this new data.
      
            
