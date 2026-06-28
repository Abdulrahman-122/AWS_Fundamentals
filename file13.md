#  storage;

  1.EC2 instance storage:

      - this type of  storage is temporary
      - attatched to Ec2
      - used to store buffers,caches,scratch data..  
  <img width="636" height="232" alt="image" src="https://github.com/user-attachments/assets/d3b0bb30-6d23-41fb-84e2-7b2df663e6b3" />

  Benefits:

        - Automatically available storage ->  as it come with Ec2  + you don't pay  for it+high performance for  I/O data 
        - As you don't pay for it so it doesn't provide any fees 
          - it's ideal for services  that don't need to store high important data
        - it's performance  is good  .
2.What is EBS(Amazone elastic  Block store)

    - another way to store data but in persistent way
    - it's work for many Ec2 instances 
    - stores data inside databases,filesystems
    - it's high performance  storage service+ low latency.
  how it's working:
  <img width="636" height="232" alt="image" src="https://github.com/user-attachments/assets/4227d7cb-5f70-4694-8675-91d39c621de3" />

    - EC2 is running while EBS  store data in 
    - once Ec2 stopped -> then EBS will still contain data mybe other Ec2 needs it so it provide that data to it
  Benefits:

    - Provide snapshots in order to use it in another Azs 
    - you can connect it with  different instances.
    - it ensure that the data is recoverable and found into another Az  especially at disastars.
    - it' cost is effective
    - performance tuning ;you can change it's volume type on the fly in order to match the application requirements (IOPs input output per second) .

to sum up;

    -EC2 instance store is directly attached to the host, 
      offering extremely low latency and high I/O performance for applications 
      that need temporary storage with fast access.

    - Amazon EBS ensures data protection through automatic replication within 
      the same Availability Zone. This provides the high availability and 
      durability needed for financial applications with critical data.

------
# EPS snapshots;

  What is  the EBS snapshots?

      -it's a copy of EBS data in order to avoid any crashing or disaster  or whatever
        -  they  are stored inside redundant Azs using Amazon S3
        -note; you as customer responsible for managing these snapshots  as it take storage so be aware of what you do

    How are snapshots working?
      - when you take snapshot for specific day
      - then you take the anoher one the day after -> only the new data added to 
        the new snapshot this called; incremental
        snapshots.
    Benefits of EBS?
      - it's enable fast data recovery from corruption  by taking a  backup for it
      - operational flexibility -> sharing  data across AWS account
      - reduce backup time ,cost as it usess incremental starategy(only new data will be added)

But in case you need to update thousands of snapshots?

    - in this case;
        you need to use Amazon life cycle manager
          this manager -> enables you to automate the entire work instead of proning or whatever 

    = Benefits:
      - it's helps you to set a compliance requirements  by schedule regular backups
  how to make Amazon life cycle manager?

      - create snapshot policy.
      - create EBS volume
      - determine the data that you want
      - automate the creation,deletion  of EBS by schedule.
      - Add  additional features like tags,snapshot archiving...

      note;
        Amazon Data Lifecycle Manager defines lifecycle policies that automate snapshot 
        management based on schedules. This eliminates the need for manual snapshot 
        management
      

      


      
