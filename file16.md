#AWS Storage Gateway;  

    it's way used to scale your local storage with AWS cloud storage 
    it's make low latency for accessing data frequently.
    it's used with on-premises services also.
    it's good for hybrid cloud storage
    use on-premises files backed by cloud .
    
    
    Benefits;
      -enables connectivity between on-premises apps and cloud + make low latency when accessing
      data
      - improve data management -> improve security,compliance,durability of data.
      - local caching -> this type  keep accessing data to ensure quick access while managing  less data in the cloud
        So when someone opens a file again:
            Read file
                ↓
            Found in cache
                ↓
            Fast response
            
            No need to download it every time.
      - cost optimization ->has cost-effective for backups,disaster recovery,archiving.
            
types of  Storage Gateway:


    1. Amazon S3 file Gateway:
        you local environment is connected with S3 
        provides on-premises applications
        provide unlimited cloud storage using familiar file protocol.
        S3 ->store,retrieve cloud objects using familiar file operations.
        you upload data to S3 gateway ->S3 take these data and stored it as objects(keys) in the cloud
          then pick a copy of frequently accessed data and put it in cache to make the operation of accessing data veryfast
    2.Volume Gateway;

      - you create virtual storage volumes
      - this type work as bridge between on-premises infrastracture and your cloud volumes and you represent data as ISCSI volumes that can be mounted by your existing apps
        types of it;
          1.cached volume mode -> stores data  in cloud and put frequently accessed  data into the cache to make low latency
          2.Stored volume mode =>keeps your dataset + Asynchronously  backing it up to the cloud as EBl snapshots.


     3.Tape Gateway;
        - replace physical tape infrastructure with virtual tape capabilities ->this achieve durability+scalability.
        - once you used it => it  presents itself to your backup app as hardware tape.
        - you can use your less frequently data to a cost-efffective storage.

        notes;
          -S3 File Gateway provides a file interface into Amazon S3 so the team can 
          store and retrieve objects using standard file protocols like NFS and SMB. 
          With S3 File Gateway, frequently accessed data is cached locally for low-latency
          access while data is stored in Amazon S3 for durability and cost-effectiveness.
          -Cached Volume mode is ideal for this scenario because it stores the most frequently 
          accessed data locally for low-latency access while maintaining the complete dataset 
          in Amazon S3. This provides both the local performance that engineers need and the
          benefits of secure cloud backup.
          
          

----


# AWS Elastic disaster Recovery

      -  replicates data or critical workloads in minimul time
      - it allows  physical,virtual servers during disruptions to  make recovery  or backup fast.
      - good at  healthcare where system availability is crucial.
      - you can use it to eliminate downtimes ,data loss while eliminating the costs associated with maiantaining secondary data centers.


        Benefits;
          1.revover workloads at disruptions.
          2.automate disaster recovery through a console -> so it will reduce  manual configurations..
          3.cost-effective => you  just need for usage +no infrastructure cost or whatever.
        Use Cases:
          1.health care.
              recover records of patients at outages ...
              by replicating their data through cloud this will  help continuiously return data when needed
          2.Financial services:
              recover data  from banking to ensure continuously retain data when needed.
          3.Manafucturing operation recovery;
              so manufucturer may use Elastic  disaster recovery to ensure that everything workwell at disasters or ...

          note;
            Elastic Disaster Recovery provides continuous block-level replication that
            maintains exact server replicas with minimal time between backup intervals, 
            enabling rapid recovery when needed.

            
            
        
