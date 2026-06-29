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
----
Amazon DynamoDB -> pause here
        
