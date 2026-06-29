# to rap up the storage module;


  1. What is EC2 store;

          -type of storage  around Ec2
           good  for temporary data
           like; buffers,caches..
           it's performance is high
           no cost
2.What is EBS(Elastic block store)


          work with multi Ec2 
          store data persistent
          store data in filesystems or databases
          low latency
          scale up or down dynamically
          cost-effective
          provide snapshots
      what is the importance of snapshots?
          -retain data at disaster
          - able to move data to another Azs
          - it make snapshots using Amazon S3

      you can automate the workflow of EBS by using; Amazon life cycle manager -> to automate where to take snapshots...
note;

      Amazon EBS provides block storage volumes that must be attached to Amazon EC2 
      instances. It cannot be directly accessed over the internet, does not support 
      URL-based file sharing, and is limited in capacity to the size of 
      provisioned volumes.


=====


What is Amazon S3?

      fully managed object storage ->provide store,retrieve data.
      has high durability ,store objectss in buckets.
      buckets => contain unlimited objects 
      unlimited storage
      store static  files,delevering media files
      good at archiving,good for delevering content like videos,mobile stuff
  security rules in S3

        Bucker policies + identity based policies+Encryption
  Classes of Amazon S3:

      -S3 -> store dynamic data +big analytics data 
      - S3 intelligent tier -> store data based on tier or time you access it
          types:
            frequent access tier
            infraquent access tier
            archive access tier
      -S3 standard infraquent access
          if you access data less => good options
          store data in 3 Azs
          high durability+high througput.
      -S3 one zone infraquent access
          store data that you access less in one zone
          it's cost 80%of previous one
      -S3 standard one zone
        used in one zone
        delever sensitive,low latency
        10x of standard IA
        cost 80% of standard 
      -S3 Glacier flexiable retrieval
        good for data that you access from 1-2years
        data are accessed  from 1-5 min
        good for backups
      -S3 Glacier Deep archive:
        good for data that you access less in 1-2 years
        access data in 12 hours
        retain data for 7 years or above
        good for financial services,health care

      - s3 outputs;
        good with on-premises AWS outposts
        server data locally on local servers
        high performance if data near to the on-premises .

    S3 lifecycle:
      data still in standard storage for 30 days=>moves to IA storage for about 60 days => moves to Glacier instant retrievel for about 356 days =>then deleted.

----

# what is Amazon Elastic File system;

      fully managed storage with AWS+on-premises service
      operates using NFS linux
      scales up or down 
      accessed by multi Ezs
      store data in multi-Azs
      support hugh of NFS ->so multi instances can access it simultaneously.
      cost effective 
    Types of classes:
      1.Efs standard + Efs standard infraquent access:
          durability high+availability high
          cost is high
          store data in multi azs
      2.One zone Storage classes:
          work in one zone
          it's cost is lower than standard
      3.Archive storage class;
          data is access a few times of year
          it's cost is effective.
      it's designed for concurrent shared access from muulti Ec2 instances across multi Azs
        so it's good for globally projects.

----

# What is Amazon FSX?


      -  Fully managed file system=>support high perfromance workloads=>support many protocols =>cost is lower
      - cost effective
      types;
        - Amazon FSX for windows file server:
          deploy windows on AWS
        - Amazon FSX for NetApp
            fully managed+allow data access for netapp.
        - Amazon FSX for openZFS:
            fully managed  =>allow openZFS to AWS
        - AWS for Lustre
            - Migrate HPC,ML,Big data analytics
----

# What is AWS Storage Gateway:

    good for hybrid cloud storage
    scale  up  or down based on storage
    low latency+access data frequently
    improves durability,security of data
    use local caching to improve access
    cost-effective

    Types:

        1.Amazon S3 file Gateway
            store data from on-premises services
            store data as objects at S3
            use local caching to speed the process of accessing data
        2.Volume Gateway;
            this type works as bridge between on-premises infrastructure+cloud
            create virtual volumes
            types:
                cached volume mode -> uses cache to access data frequently
                stored volume mode -> take snapshot from the data on your local services like (Elastic block storage
    
        3.Tape Gateway;
            = replace physical tape with virtual ones

        note;
        File Gateway provides a file interface into Amazon S3 object storage. It maintains          low-latency local access to frequently accessed data through local caching and              seamlessly integrates with existing file-based workflows.
-----

#What is Elastic disaster Recovery?

      -recover workloads at disruptions
      - cost effective 
      - used in healthcares ,financial services,Manafucturing operation recovery
        provide block level replications with minimal time between backups + enable rapid recovery when needed.
      
