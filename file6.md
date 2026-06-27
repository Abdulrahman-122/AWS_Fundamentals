There are two types of services?
  1.Managed services
  2.Unmanaged services.
  3.fully managed services(Aws manages  all the service for you except the data of your application or whatever)
  <img width="1581" height="1077" alt="image" src="https://github.com/user-attachments/assets/1f7963c2-8d61-4588-856d-01b37adc50fb" />
  <img width="1680" height="838" alt="image" src="https://github.com/user-attachments/assets/27212652-c325-441b-8a21-70fd73b9c695" />

    notes;
      With unmanaged services like Amazon EC2, you set up and manage everything: 
      the operating system, security updates, and network settings.
      AWS only takes care of the physical hardware. 
      Managed services handle most of the infrastructure for you,
      but you still need to set up things like deployment options, 
      scaling, and environment settings. With fully managed services 
      like AWS Lambda, you don’t manage any servers at all. You upload your code,
      and AWS takes care of the rest, including infrastructure, scaling, 
      and availability.
      note(serverless(fully managed service like lambda)

----

# What is Lambda?
  
    - it's a serverless compute service that runs your code without the need for provision or manage underling infrastracture 
      os management,scaling resourses based on events
      - you can purchase for the copute time consumed  
      - it handles scaling,allocation,execution
      - you can just configure the performance by making appropriate memory or whatever.

How it's working?
   - <img width="1680" height="571" alt="image" src="https://github.com/user-attachments/assets/9958b2f4-5294-48a8-b679-206c29e70d05" />
   Upload your code to run
   trigger the code using events like ; https traffic from mobilee or AWs services
   then lambda run the code once it received the  trigger
  and you only pay for consumtion
  note; lambda is serverless compute which means you don't need to make server configuration for your stuff you just put the code and it will hanlde the other processes for you
ex;
  - you can use it to handle large amount of images  that are uploaded in image processing social media app
    it's handle all the process simultanuosly
  - we can use lambda to aggregate images from multi resources  and recommendes these for each user based on user preferences
  - it can also trigger and update scores in an image based on updates ... if you build an online  game ..
   
why it's important :

      it's manage thousends of events in real time with no need to manage servers or whatever 
        it's scales with users traffic and reduce costs by running code when user interact 
        it's charges  based on time that used for processing image.

        note;
        The key components of AWS Lambda are the function, triggers, and runtimes. 
        These components handle code, respond to events, 
        and provide the language environment. Customers do not need to manage servers, 
        scaling, or operating systems. AWS takes care of all that.


What's the difference between Containers,VMs?

    - Containers ->  faster , lighter than vms as it uses  the same host machine that they work on 
    - VMs -> they have a hybervisor that runs separately from the host machine so they are less efficient than containers
  <img width="1680" height="608" alt="image" src="https://github.com/user-attachments/assets/2fbf3fb0-6706-4a56-83f7-3672ffe5e63c" />

      - so the  concept of containers made the process of deployment easy to run any application on any machin

What is ECS?

    - called: Elastic containers services
      -it's used to deploy containers on AWS like docker  with containers

Can you compare between using(ECS with EC2 and ECS with Fargate)?


    - ECS with Ec2 
      good for small -medium apps that needs to be deploye and manage their infrastructure by the team of the app  
        full control option of the servers
    - Ecs with fargate
        good for small apps where their teams don't need to manage infrastructure and they want to focus on code and data itself
        fargate will handle the configuration and servers
        serverless option.

What is EKS ?


    - Elastic kubernetes service 
      this service runs kubernetes on AWS
      it simplify deploying,managing for that service. ...

Can you compare between (EKS with EC2 ,EKS with fargate) ?

    - EKS with EC2 
      running  kubernetes on Ec2 require the team to be fully managingfor the servers and the infrastructure that runs the service
    - Eks with fargate 

      running kubernetes on fargate -> don't require teams of the service to manage and control infrastructure
  
    
What is ECR?  

    - it's Elastic container register
    - reposity like any open container initiative standards (OCI) you can 
      - push 
      - pull images on it and manage these images 
      you can access through cli commmands or whatever.

What is the Fargate?

      - it's serverless compute service for the containers 
      - works with ECS,EKS
      - you don't need to manage or configure infrastructure you just 


  to sum up:

      mazon ECS is a scalable service for orchestrating containers on AWS,
      whereas Amazon EKS helps simplify Kubernetes deployment. 
      Amazon ECR stores and manages OCI-compliant container images, 
      integrating with Amazon ECS, Amazon EKS, and Fargate. 
      Fargate is a serverless compute engine for containers, 
      removing the need to manage infrastructure and working with Amazon ECS and Amazon EKS.


      
