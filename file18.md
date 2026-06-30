# Databases(module7):
  types;

        - fully managed database
        - managed database
        - unmanaged database

= Fully managed services;
<img width="762" height="604" alt="image" src="https://github.com/user-attachments/assets/b9ef3615-9849-47b3-8a64-39e26271ed46" />

= managed services -> you are responsible for database configurations,query optimizations,...
<img width="764" height="610" alt="image" src="https://github.com/user-attachments/assets/d0d20c56-d951-4d05-af96-9408c4eee6bf" />

=unmanaged services => you are responsible for -> installation,configuration,patching,security,backups,high availability setup;
<img width="764" height="606" alt="image" src="https://github.com/user-attachments/assets/b583712f-f279-4b59-a7b9-6c7513052a46" />


----

# What is relational database?

    -it's way to store data inside tuples in a table 
      by using structured query language called:sql 
      by this we can restore data whatever time we want
look at this table:
<img width="1363" height="305" alt="image" src="https://github.com/user-attachments/assets/22ecd332-8d60-4673-858d-0381fe806fe6" />

      note;
        AWS can handle many of databases and also store it at many Azs especially at disasters.
-----
# what is Amazon Relational Database(RDS)?

    - service responsible for managing,patching,take backups from the database.
      it's also support multi  database instances class types that optimize memory ,I/O
    - offers Multi-Az deployment+backups 
    - it's fullybackups for the entire system -> this is good for point-in-time recovery or data archiving goal.
    - include security purposes  -> encryption in transit or at rest
What are the engines that it supports?

    - Amazon  Aurora
    - Mysql
    - oracle
    - Microsoft SQL
    - POstgresql
    - Mariadb...
ex; webapps,e-commerce platform,..

    Benefits:
        - cost-effective+automation for proning tasks like; patching,backups
        - deploy database across multi-Azs
        -  it's performance is high->provide real-time monitoring...
        - Adding security stuff to the system (protection,encryption...)

-----
# What is Amazon Aurora?

    -relational database that helps to remove redundant I/O operations  from the database 
    - it's support Mysql,postgresql  
    - can  deploy database acrosss multi-Azs
    - enhance durability ,fault tolerance.
    - it also make backups for the system.
  ex;

      good at gaming,real time analytics.

Benefits:

      -5x performance than Mysql
      3x performance than postgresql.
      -it's storage from 10GB to 128TB
        making backup for the system based on Amazon  s3 service
      - it's availability is high -> provide 6 copies of data
           it's availabililty 99.99% 
        automatically detects database failure +redirect traffic to healthy replica .

- notes;

       -Multi-AZ deployments provide enhanced availability and durability by automatically
        creating database replicas in different Availability Zones. In case of
        infrastructure failure, Amazon RDS performs an automatic failover to the
        standby instance, thus ensuring that the database remains accessible with minimal
        disruption.
      -The Aurora distributed storage architecture offers up to five times
        the throughput of standard MySQL while maintaining compatibility.
        It was specifically designed to handle high transaction workloads by distributing
        I/O across multiple storage nodes.
      - Aurora provides comparable performance to high-end commercial databases but at one-         tenth the cost, which makes it ideal for organizations looking to reduce database           costs without sacrificing performance.
----

NoSQL databases

      NoSQL databases are sometimes referred to as non-relational databases because their          structures are different than relational databases like Amazon RDS. Instead of row          and column relationships, NoSQL databases build a structure for the data that they          contain using key-value pairs instead. With key-value pairs, data is organized into          items identified by unique keys.
      
      Each key has one or more associated attributes, or values, that represent various           characteristics of the data. You can think of a key as a word entry in a dictionary,        and the value as its associated definition. Not every item in the table has to have 
      the same attributes, and you can add or remove attributes at any time.

<img width="1392" height="576" alt="image" src="https://github.com/user-attachments/assets/903f91c9-d1f3-41ef-a834-0b4c62d1bfc0" />


----
Amazon DynamoDB

    - DynamoDB is a fully managed NoSQL database service that provides fast and predictable       performance for both document and key-value data structures. It's a powerful and            incredibly fast database option for use cases that require a flexible schema, and is        ideal for applications that require high performance and seamless scaling.
    
    - DynamoDB seamlessly scales alongside your data without impacting performance, which         means that you only pay for the resources that you use. It also includes built-in           security features for enhanced protection, and automatically spreads your data across       multiple servers to handle your workload.
    Use cases
    
    Some examples of practical use cases for DynamoDB are gaming platforms, financial            service applications, and mobile applications with global user bases.
------

What is in-memory cahcing?

    
    - An in-memory cache is a high-speed storage layer that temporarily stores frequently 
      accessed data in a computer's main memory, or RAM. Retrieving data from RAM provides 
      extremely fast processing and retrieval speeds, often hundreds or thousands of times 
      faster than traditional disk-based storage systems.
    
    - When applications need specific information, they first check the cache before 
      requesting it from the original data source. This reduces the load on primary               databases 
      and speeds up response times for end users. In-memory caches are ideal for storing          session data, API responses, database query results, and other information that             applications require repeatedly.
What is Amazon ElasticCache?

    =>service uses in-memory caching to fast the operation of fetching data
    use: in gaming leadboards,database enhancement
    Benefits:
      1.provide high performance for valkey,Memchached..
      2.High availability for recovering data if something happen
      3.replications across multi Azs
      4.Build encryption while moving data from nodes to users.
------
# Additional Database services:
# What is Amazon DocumentDB

      fully managed service -> handle semistructured data
      it's compatible MongoDB
      it manage JSOn-like documents with dynamic schemas.

      good for apps that require schema changes+document oriented data.
      you can iterate without relying on predefined schemas
      it can store,query,index json data effortlessly
      it can scale automatically.
      continuous backup

      Uses:
        - content management systems.
        -catalog
        -inventory management.
        -user profile...

      Benefits;
        -Compatible with Mongo-db
        -scale storage up to 64TB in 10TG increments
        - it also scale up or down 
        - increase read throughput -> by making 15 replica underhood that the share the storage.

-------
# What is Amazon Backup?

    it's a way ->to backups muulti services in AWS
    it uses EBS,NFS,centralized backup recovery. ...
    it automate process in order to pretect the services 
    make encryption,backup across multi Azs
    Benefits:
      - Centralized backup recovery -> single monitor for all AWS services to see where are the failure or whatever.
      -make backups at multi-Azs
      -centralized regulatory compliance.

----
# what is Amazon Naptune?

    =>fully managed database
    =>build-graph database that manages highly connected data sets
    => excels at understanding complex relationships.
    uses:
        user connection mapping
        fraud detection systems 
        search systems.
    Benefits:

        support Reduce description framework.
        good at relationship mapping+pattern matching apps
        it can scale up or down + store up to 64TB

      note;
        Neptune provides low-latency and high-throughput performance for both read and              write operations, making it suitable for real-time applications working with                connected data.
        -A key benefit of AWS DMS(database migration service) is that the source database remains fully operational              during migration, which minimizes downtime to applications.
