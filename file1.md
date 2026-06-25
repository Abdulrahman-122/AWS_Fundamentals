What is cloud computing?
  - on demand-delivery of IT resources over the internet with pay as  you go pricing

          - on-demand-delivery -> the service on cloud is working over 24/7
          - of II resources -> the services on cloud include( AI services, databases...)
          - over the internet -> all of these services you can access  during  the web browsers.
          - with pay as you go pricing -> that means the price is for your consumtion not anything else
Types of cloud computing?

    - cloud-based deployment -> you deploy the whole service on the cloud 
    - on-premises -> you deploy using vertualization,resource management tools (however these don't provide scalability like  cloud based 
    - Hybrid deployment -> you used both of on-premises,cloud-based in order to prevent migrate all important data to the cloud you just want to usee cloud resourses for  dynamic scaling
-----

What are the key benefits of using AWS?

    - it's costs uses variable expense not fixed one (suppose you didn't use the service for 1 day -> this one day won't cost you anything)
    - you will benefit from it as there are large economies of scale.
    - it's storage is dynamic (if you want to make scale of your resources big or small  you can manage those )
    - it increase  speed.
    - you don't need to pay for maintaing your data inside data centers or whatever Aws can do that for you.
    - if you need to run your service in  another country Aws can  make that deployment in minutes.
---
How data centers of AWS look like?

    - AWS build  their data centers according to this term(High availability)  
      - they put atleast 3 data centers at different location of each based country they centerialized at.
      - they ensure high availability and avoiding any fault at the system.
        - the data centers called; Azx(Az01,Ax02,Ax03) as you see;
  <img width="1602" height="884" alt="image" src="https://github.com/user-attachments/assets/061236cf-8ba5-4eea-82f1-a49df6cb4765" />

    - they mentioned that ; it's recommended to locatee your Azs away from each other in order to avoid any disaster or  outage of service...
----

How manage the cloud(you or AWS or both)?

<img width="1680" height="758" alt="image" src="https://github.com/user-attachments/assets/44753a83-b25c-410b-9bb2-68ea78e5a9b0" />

    - According to the image above:
      -  there are 3 things
        1. Customer responsibiliity(his data , the appearance of it...)
        2.AWS responsibiility (how Hardware stuff is  secure across thee cloud,storage..)
        3.AWS or Customer responsibility(depend on service (server side protection,network side protection)...)


---
ex;

    - suppose you want to build an ecommerce company based in Egypt
      you want customers from America
        so you go AWS Global expansion and build the services on ohaio data center
        in this case AWS will make high availability and ensure fault tolerance . manage their stuff 
        and secure their hardware for you
        suppose you have a significant customer at Asia so you deploy your services  in a data centers near to your customers.
<img width="1680" height="1120" alt="image" src="https://github.com/user-attachments/assets/21dab201-8c4d-4154-8c4e-54667e008f7b" />

----
notes;

        A Region is a geographical location that contains three or more Availability Zones.
        An Availability Zone is a distinct location within a Region that contains one or more 
        discrete data centers.

        AWS is responsible for the physical security of data centers. 
        This includes measures like access controls, surveillance,
        and environmental controls. Companies migrating to the cloud still
        have responsibilities such as security configurations and 
        data within their cloud environments.


      In the AWS Shared Responsibility Model, the customer is responsible for managing OS patches.
      AWS provides the underlying infrastructure, 
      but the customer must make sure that their OSs are up to date with the latest security patches.
      The customer is also responsible for encrypting client-side data. 
       AWS provides various services to help with encryption, 
       but it is the customer’s responsibility to implement and manage these services.
      Physical security of data centers and hardware maintenance are AWS responsibilities. 
      Updating software for compute, networking, 
      storage, and database services is also an AWS responsibility.

      where the client sends requests to the server. 
      The server processes these requests and returns the appropriate responses. 
      Cloud computing provides scalable and flexible server resources that can 
      be accessed over the internet.


      Global infrastructure typically involves distributing resources across multiple 
      data centers in different geographic locations. 
      By having redundant systems in various locations, 
      global infrastructure enhances fault tolerance.
      If one component fails, others can take over to minimize downtime and help ensure 
      high availability.
      Ease of use, compliance, and cost savings are benefits that can be achieved by 
      using cloud resources. However, in this case,
      the focus is on making resources highly available to global users.
