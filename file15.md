# Amazon Elastic File system (EFS)

      - fully managed file storage service with AWS cloud services+on-premises resources.
      - operates using  Linux Network file system  (NFS) protocol.
      - it scale up or down according to the files you added  or whatever.
      - can be accessed by multiple Ec2 simultaneously.

      Benefits:
        1. store data  in multi Azs in a region for high  availability -> in order to  avoid
           failure
        2.it support hugh of NFS -> so that many instances can access the same file system simultaneously.
        3. it's cost effective  as  it scale up or down according to the  storage you added to it.

Amazon EFS Storage Classes?

    1. Standard Storage Classes:
        it's called EFS standard or EFS standard infrequent Access:
            it's durability is high and it's availability is  high also.
            it's cost  is high  due to it's  durability.
            save data in multi Azs
    2.One Zone Storage Classes:
        work in one Az
        called:EFS one zone or EFS One zone infrequent Access
        it's cost is lower than standard one
    3.Archive storage class;
      it's cost effective
      data stored in  it accessed a few times of year
      it's cost is 50% of infrequant  access 
      

----

# what is EFS data lifecycle?

    you may ask is there a way to move data between these classes in order to  provide cost effective..
    in this case you can write  your  lifecycle policies to make it
    this operation is autemated inside EFS -> so in this case you can provide cost effective

    how  lifecycle policies works:

        1.(transition to  IA)you need to move data to EFS IA -> if the  data was accesssed one or two per quarter
        so data moves to IA after 30 days in Standard Storage.
        2. (transition to Archive) move data from IA to Arcive is  you didn't access it for about 90 days.
        3. (transition back to standard)  -> once  data  is accessed it will be transitioned to  standard EFS
        

    note:  

        Amazon EFS is designed for concurrent shared access from multiple EC2 instances 
        across different Availability Zones with consistent performance. 
        This makes it possible for global teams to collaborate on the same files.

-----

# what is Amazon  Fsx?

    - fully managed system
    - high performance file system.
    - supports high performance workloads , instances
    - supports many protocols (lustre,windows..) unlike EFS which support NFS just  
    - built on the latest AWS compute,storage,networking..
    - it's  cost is lower(lower total cost of ownership)

    Benefits:
      - supports  many  of protocols -> support migerations
      - manage infrastructure + delivering  features of  traditional  filesystem.
      - scalable  storage dynamically.
      - cost-effective.

Types;

      - Amazon  fsx for windows file server:
          fully  managed
          allow for any type of windows filesytem to store  data ,access...
          benefits:
            Migarate windows  to AWS
            Accelerate hybrid workloads.
            Reduce Sql server deployment.
            streamline virtual disktop+streaming.

      - Amazon fsx  for NetApp (OnTAP) protocol
          fully  managed 
            allow data access for ontap or netapp

          benefits:
            - Migrate workloads to AWS
            - Build applications
      - Amazon FSX for openZFS:  
        fully managed
        allow share files,access it for ZFS protocol.
        benefits:
          Migrate workloads to AWS
          Accelerate  content management.
      - Amazon FSX for Lustre:
          fully  managed
          allow sharing data for lustre
          benefitss:
            - Accelerate ML 
            - Accelerate  HPC
            - Big data  Analytics.
            ...
            
          
            
