# Scaling_Amazone_Ec2

    - Scalability -> system potential to grow over time
      - you add scaling out to the system by adding new machines
      - you adding scaling up to the system by make power of machine hight
  <img width="1680" height="860" alt="image" src="https://github.com/user-attachments/assets/afc5bfea-0152-46c1-b374-77473d9bdcd8" />

    - elasticity -> dynamic + on demand adjustment of resources.
      - you just make scaling up or down 
        scaling up during period of high demand
        scaling down during the period of low demand
        this make cost efficient+optimal resources
        look at this:
  <img width="1632" height="1059" alt="image" src="https://github.com/user-attachments/assets/a785ebc1-7ea1-4751-b5ed-1340141142ff" />

----

# What is Amazon  Ec2 auto scaling?

    - Amazon vary or adjust number of Ec2 based on demand:
      -   this provide  better availability
      -   offers two approaches;
      -     Dynamic scaling adjusts in real time to fluctuations in demand.
      -     Predictive scaling -> by predict the number of instances based on anticipated demand
  ex;
    you can adjust your Ec2 instances dynamically based on  demand 
    also you add auto-scaling groups (collections of Ec2)
    - how to define auto-scaling groups?
       1. Minimum Capacity
          - minimum number of Ec2 instances to  keep the application running
          - <img width="1680" height="1245" alt="image" src="https://github.com/user-attachments/assets/7355d9eb-197e-487e-9a7f-dee4d8a53e7a" />
      2.Desierd capacity;
          - ideal num of instances that are enough for your current workload which auto-scaling aims to maintain.
          - if you didn't provide it it will return to minimum number by default.
     3.Maximum Capacity:
          - upper  limit of instances that can be launched 
          - this type you will use when you see high demand on your service 
          - we use it in order to scale out at increasing in demand.


      notes;
          - By deploying instances across multiple Availability Zones,
            businesses can avoid service disruption in
            the event of an Availability Zone failure
          - The AWS scalability and elasticity features automatically adjust resources 
            to meet demand, resulting cost-efficiency and performance.


-----------

# What is the  Elastic Load Balancing(ELB)?
    - it's a single point located between frontend,backend of the system
      it's direct incoming traffic  to multi instances to ensure each one still work + high speed of the system
    - So ELB,Ec2 both work in tandem to ensure high availability...
     # Benefits of using it:
       1. Efficient Traffic distribution
           enhance traffic by preventing overloading over single instance
      2. Automatic scaling
        - it has the ability to scale up or down based on  addedd or removed instances.
      3.simplified management
        it manage all the stuff without any  manually configuration even maintainance+updates..
  # What are the routes that ElB uses to make it's operation?
    1.Round Robin
      -> direct traffic in cyclic manner in order to see available server.
  <img width="1133" height="1133" alt="image" src="https://github.com/user-attachments/assets/1483c49c-dc78-4dc7-a127-f20460b2f788" />

    2.Least connection
      -> direct traffic to the server that has least connections
    3.Ip hash 
        -> direct traffic to the correct end route that he needs.
    4.Least Response timee
        -> direct traffic to the server that has fast response 
  <img width="1680" height="796" alt="image" src="https://github.com/user-attachments/assets/831358a4-58da-4df9-81f5-e80019974673" />
  - this image explain how ELB manages the high demand by distributing the traffic on multi instances as you see.


        notes;
            -ELB improves scalability by automatically distributing traffic to the EC2
              instances with the least load, resulting in efficient traffic management.
              ELB scales elastically. This means it adjusts traffic routing based on
              demand without increasing hourly costs, which is a key benefit.
            - ELB and Auto Scaling work together to efficiently manage varying levels of demand.
              ELB is responsible for distributing incoming traffic evenly across multiple EC2 instances.
              This makes sure that no single instance becomes overwhelmed.
              It also serves as a single-entry point for traffic into an Auto Scaling group,
               directing requests to the appropriate resources.
              Meanwhile, Auto Scaling automatically adjusts the number of EC2 instances
              based on the demand. It adds or removes instances as needed for optimal
              performance and resource usage. Together,
              ELB and Auto Scaling help maintain application reliability and cost efficiency.
    
