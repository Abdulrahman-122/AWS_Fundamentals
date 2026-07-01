# AWS Migration Process:
<img width="1680" height="683" alt="image" src="https://github.com/user-attachments/assets/c6c42eda-dd3a-49e1-948e-e87ea95a5201" />

    framework:
      1.Asses -> you see whether your are ready to start migerate or not.
      2.Mobilize -> you start mobilize the resources.
      3.Migrate and modernize ->you apply your rules and start your system.

---
How to Adopt to Cloud ?

    - Amazon CAF:
      ->it's a tool used to help companies to migrate their work to cloud.
      ->Benefits: AWS CAF provides benefits for migrations to reduce business 
        risk and improve sustainability and corporate transparency. Companies can 
        grow revenue by creating new products and services in their cloud 
        transformation. They can also reduce operational costs, increase 
        productivity, and improve customer experience in their new cloud environment.
      Uses:
        you can use it to migrate legacy apps and infrastrucure.
   Keys of AWS CAF:
       <img width="1050" height="304" alt="image" src="https://github.com/user-attachments/assets/327d3f4b-aa5a-4636-82f7-6d413ffaafd4" />

          - Business-> IT needs aliens with business neads.
              - these are business roles;
                 Business managers
                 Finance managers
                 Budget owners
                 Strategy stakeholders
          - People -> ask people about the gaps + try to evaluate it.
             - these are people roles;
                 The following are common People perspective roles:
                Human resources        
                Staffing
                People managers
         - Governance-> the roles of governance helps you maximize business value + align with IT startegy.
                     -The following are common Governance perspective roles:                   
                            Chief information officer (CIO)                   
                            Program managers                    
                            Enterprise architects                
                            Business analysts                     
                            Portfolio managers

         - Platform -> apply solutions for cloud on-premises stuff 
                
                The following are common Platform perspective roles:
                    Chief technology officer (CTO)
                    IT managers
                    Solutions architects
          - Security -> choose security solution to meat your agility,control,audit..
              use CAF to implement these solutions.
              The following are common Security perspective roles:
                    Chief information security officer (CISO)            
                    IT security managers          
                    IT security analysts

          - Operations -> this helps you to run,enablee,operate,recover IT settings to make aggrement with your business stakeholders.
              use CAF to do these ;
              The following are common Security perspective roles:
                    The following are common Operations perspective roles:
                      IT operations managers
                      IT support managers

-----

what are the Seven Migrations?
<img width="1680" height="657" alt="image" src="https://github.com/user-attachments/assets/57b84b21-2d16-486f-b85d-56c3710a8d1a" />

    1.Relocate -> changing the hosting to the cloud.
    2. Rehost -> lift and shift (moving app without changes)
    3.Replatform -> (lift,tinker,shift) optimize to realize a tangible benefit.
    4.Refactor -> to add new features to improve performance (Rearchitecting)
    5.Repurchase -> move from customer service to Software as a service(Saas)
    6.Retain -> keep app running .
    7.Retire -> stop from removing the application.
-----
What is the tools in  Asses phase at the above framework?

      - Migration Evaluator:
          - migration assessment helps you 
              - create a business case for AWS cloud planning + migration.
              - analyse your current state+target state -> developing a migration readiness with cloud costs.
            Benefits;
                -remove guesswork when migrating
                - give you multi cost effective migrations .
                - gives you insight about reusing certain software licensing..
            Use cases: You can use Migration Evaluator to conduct broad-based 
               discovery, take a snapshot of your current on-premises footprint 
               to fine-tune licensing, view server dependencies, and gain 
               visibility into multiple migration scenarios. You can also 
               use it to estimate and reduce your cloud costs
      -Mobilize phase:
          - Application Discovery service:
              gather info about on-promises server 
                configurations+performance for servers+databases to create detailed migration plan.
           -Benefits:
            -you can get snapshots about on-premises inventory
            - integrate discovery data with services like; Migration hub.
           uses:
            -conduct discovery+inventory
            -create migration plan.
        -Migration Hub:
            -centralized hub -> take you from discovery ,planning => provide tools,automated migrate your app.
          Benefits;
            no cost 
            one place to monitor your migration.
  <img width="1680" height="489" alt="image" src="https://github.com/user-attachments/assets/564079ee-f2a7-466d-a9a2-fc9bb5b5262b" />

        -Migrate and Modernize:
           -Application migration service:
             tool help your on-premises and cloud apps => helps you migrate fast(expedite)
             reduce cost
          Benefits;
            - migrate from any supported Os
            - you cam maintain business operation during migration process.
            -reduce cost
          uses; for on-premises app running on servers or infrastructure or local cloud
              - modernize apps

----
Migration Database:


      - suppose you want to move from one type of DB to other one but they support the same data(this is easy to do called Homogenous DB)
      - while converting from one to another that doesn't support the first one -> called Hetrogenous DB Hard one
      AWS support the both and contain some tools for that:
        1. AWS DMS 
            - Database migration service
              =help you to migrate live databases,data warehouses.
              =it migrate DB with maintaining High availability+low latency during migration.
              =support homo,heterogenous migrations
              =suport migrate high size DB with low cost.
            uses; move managed databases + remove licensing costs , replicate onging changes in your database.
      2.AWS SCT(schema code tool)
          -convert schema from one engine to another 
          you can use it to convert from commercial DB to open source DB.
          Migrate large data like warehouse data...

-----
Transfering Data to and from the cloud?

       - when confirm the process of migration of database you need;
         -security
         -data validation
         - scheduling.
         - bandwidth
        Tools do these steps for you:

          1.AWS DataSync:
            -automate+accelerate data transfer
            - accelerate moving data transfer between on-premises+cloud storage like S3
            -it automates many aspects of the transfer like running instances....
           -use it when you want to archive your data+migrate also.
        2.AWS Transfer Family:
          - support input + output files 
          - fully managed for files that goes over FTP,SFTP,FTPS...
          - helps you transfer files from S3,EFS...
        3. Direct connect 
            -create private connection between VPC , Private network.
            so you can transfer data.
            this reduce network costs+increase bandwidth.

-----
How to migrate data offline?

    - suppose you in a place that contain poor network how to transfer data;
      use: Snowball Edge Storage Optimized device?
        this is good for high data migration on on-premises services in poor locations of network..
        - it include high compute+high performance with high storagee in offline workloads.
    
