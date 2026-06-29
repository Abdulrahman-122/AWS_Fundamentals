# Amazon simple storage service(s3)?

    - it's  fully managed.
    - highly available object storage  -> store ,retrive data  as objects
      it's durability ->99.999999999%
        data  is highly  protected without loss.
        it  contain features  like versioning,lifecycle management 
    - it store objects in buckets(directory)  
      object 5TB

Can you explain what is the objects?

    - object -> your data(files,videos...)  stored in with metadate and key(object  name)
      object are differ by  their key
      it's size  up to  5TB
  <img width="1601" height="533" alt="image" src="https://github.com/user-attachments/assets/e0503ead-96d7-44a3-bc9f-8b0814f33a44" />
- What is the bucket?

      container that hold unlimited objects
      it's differ from other objects  by it's  name
      also when you creating a  bucket -> specify the region  where it  will be access there.


Benefits  of using S3?


      1.unlimited storage.
      2.you can use automatic setup to store,move data  across it through its life cycle.
      3.it's uses  with  cloud,on-premises workloads.
        used for hosting static websites+delevering media  files+content distribution
          good at archiving,data lakes ,compliance driven data retention.


Can you define Security rules that you need in order use S3?

    - this service is  private so you can make it public by modifing the permission of  it's settings

        1.Bucket policies
            each bucket has its policies
              whether its allowed  or denied  for the  object  on the bucket.

        2.Identity-based policies;
            these are policies that are  put for users,groups... who want to use these policies
            on each bucket
        3.Encryption
          - encryption secure data at S3 buckets
            by preventing unautherized access
          - also it make data save whenever it  travel to or from S3 to any location.

      notes;

        Amazon S3 is designed for scalable object storage that can efficiently store
        and serve various content types. It's ideal for mobile applications that 
        need to store and distribute user-generated content like photos and videos.
          

-----

# Amazon S3 classes +  use cases?


    - S3 -> has variety of  classes with specific performance,access,cost requirements.
      in order to address residence of data,delete them at specific period or whatever.
    Types  of classes;
      1.S3
          it's a class for storing data on cloud like storing; dynamic content,mobile ,gaming apps
            big data analytics..
          if  you  didn't determine which class  this is the default one for your storage.
    2. S3 intelligent tier
        - store data based on unknown ,changing access patterns
        - it store objects in 3 tiers
          1.a  frequent access tier
          2. an infrequent access tier
          3.archive instant access tier
        this S3 moves your data to the most-effective tier based on frequency access tier
    3.S3 standard infraquent access(standard IA)
        -used for data that is accessed less frequently +it requires repid accesss when needed.
          has high durability+high  throughput
          good if you want to restore backups,disaster recovery files...
          uses; 3 Azs
    4.S3 one zone infrequent access(one zone-IA)
        stores data in single Az
        it's  cost is lower
        this class is used for accessing data that is not high availability 
        good for storing second backups,easily recreatable data.
    5.S3   standard one  zone:
      used in one Az
      used to deliver sensitive +lower latency data.
      it's cost is 80% lower than and it's speed 10x faster than S3 standard.
    6.S3 Glacier instant retrieval;
         this  is used to store data that is rarely accesssed.
          and requires millisecond to retrieve
          it's cost  saving up to 68%  of standard S3
          it has the same latency+throuput like standard S3
    7.S3 Glacier Flexiable retrieval:
      low cost storage for archive data that is accessed 1-2 years
      your  data can be accessed from 1-5 min
      request bulk retrieval from 5-12 hours with no additional cost
      good for backups,data recovery,....
      good for acessing data  in minutes.
    8.S3 Glacier deep archive:
      -  the most  lower archive classs in AWS
      - support long term retention of data 
      - can restore data in about 12 hours
      - good for data that you can retrieve 1 or 2 per year.
      - good for retain data in 7 years or above.
      - used in financial services , health care..

    9, S3 outposts;
        -  deliver data to on-premises AWS outposts.
        -serve workloads with local data residency .
        - good to maintain high performance if data will be near to the on-premises services.

S3 Lifecycle :

    - this type we use it to automate our objects instead of manually update or doing other stuff with them using two type of actions:
        - Transition actions🤸 :  objects transit  to another storage class.
        - Expiration actions: objects expire + permanently deleted.
        
<img width="803" height="232" alt="image" src="https://github.com/user-attachments/assets/084a5f92-a94c-4b9c-bfa0-826fed504557" />

    - after 30 days -> object moves from S3 Standard Storage =>Amazon S3 IA storage class.
    
    - After 60 days in Amazon S3 IA storage -> object moves to Amazon S3 Glacier instant Retrieval class without  being accessed
    - After spending  365 days in Amazon S3 Glacier instant Retrieval storage -> object will be deleted.

ex;

        - you may need to remove data from the bucket after specific time so we use S3 lifecycle.
        - you may access data   after storing it after a long period of time so this is good for s3 lifecycle .


    notes;

        Amazon S3 Lifecycle is used create rules that automate the transition of objects  
        between storage classes. It can set expiration dates for objects based on defined  
        criteria, optimizing storage costs while maintaining access to data based on its          
        changing value over time.
          

          
