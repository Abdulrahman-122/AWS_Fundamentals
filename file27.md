# Pricing;

Key concepts you need to consider:

    - Pay as you go ->you just pay for what you consume
    - Save when you commit-> on compute if you take commit from 1-3 years you will take saving plans..
    - pay less by using more -> once you start scale -> your pay will be less
What are the driving factors for your pricing?

    - Compute -> this need pay per hour or per second.
    - storage -> like if you use S3 you will pay for those;Storage pricing
               - Request and data retrieval pricing
                
               - Data transfer and transfer acceleration pricing
                
               - Data management and analytics pricing
                
               - Replication pricing
                
               - The price to process your data with Amazon S3 Object Lambda
    - Transfer -> inbound data transfer -> in most cases no pay
                -> outbound data transfer -> you pay for it.

-----
- AWS Organizations

      AWS Organizations provides centralized management and governance of your AWS
      environment. Using AWS Organizations, you can create, group, and manage 
      accounts. You can also apply security policies at the account level and
      consolidate billing with multiple accounts using a single payment method.

- AWS Billing and Cost Management dashboard?

      ->centralize cost management
      ->showing current charges,usage..
      ->provides tools to manage payments,budgets.
- AWS Budgets:

      -> set custom budgets+send alerts when  your saving exceeds thresholds.
      -> so you can use to forcast future expenses based on trends.
- AWS Explorer;

      -> helps visualize,analyze costs with interactive graphes,reports,forecasts.
      ->provide insights for pattern,trends..
-AWS Pricing Calculator:

      ->you make estimate for your cost by entering the compute type+storage+transfer type
      then you will got the cost for that.
      ->so you can use to estimate costs before deployment.
      ->compare costs of services.
  -----

Types of AWS supports:

    1.Basic support
    2.Developer support
    3.Business Support.
    5. Enterprise On-Ramp support
    6.Enterprise Support
 <img width="888" height="894" alt="image" src="https://github.com/user-attachments/assets/7b8b3a11-543c-488f-a01a-fd0a95ce661b" />
   
    note; your Team Account Manager is responsible for the process of helping you to land multi-Aws services for your app..
Other support;

<img width="1471" height="301" alt="image" src="https://github.com/user-attachments/assets/f6192d30-81bf-4030-bf7c-aacc795fc882" />

-----

What is AWS Marketplace?

      - digital place that contain many of software vendors.
      - it contain;
        Saas (service as a software)
          apps,collaboration tools.

        Ml+AI
        Data analytics.
What is AWS Partner Nerwork?

    - global community that uses AWS technology,programs,experties
    - it help you to maximize your services.
    
-----
Cost Optimization:
<img width="1586" height="895" alt="image" src="https://github.com/user-attachments/assets/93af41b2-2453-4dbe-8a46-b4c63f69707f" />

      - you use compute Optimizer to rightsize your compute resources.
      - also use spot instances to optimize for cost 
          -it work well for workload that are interrupted alot.
          - it use spare Amazon Ec2 forr discount compared with on-demand instances.
      -also to optimize cost use: auto scaling 
          - it help you when demand drops
          - it remove any excess resources capacity
      - load balancing also distribute traffic routes across multi-Ec2 instances.
      -when it come to database use -> Amazon RDS 
        it   has autoscaling which remove any excessess resources.
      - Read replicas -> also help you read from multi instances and reduce instrain on primary one
      - also using Amazon ElasticCache -> reduce strain on your primary instance so it optimize for cost
      - also you can use S3 (S3 Glacier Deep Archive if you access data every year)
        - for Data has changing access patterns use S3 Intelligent Tiering.
      - you can use VPC or use VPC with S3.
