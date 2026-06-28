# Networking in Cloud

  <img width="1680" height="875" alt="image" src="https://github.com/user-attachments/assets/c61b3e9e-d1c2-40c6-bcf3-4b972366c6af" />
         
          key concepts  from  this image;
           1.Region -> this  is the region that near from you in order to avoid more latency.
           2. VPC -> virtual private cloud this is a private segment from the cloud that helps you to define 
                     network and services
          3. Available Azs -> as you see multi Azs this helps you to avoid  any failure if one  Azs fails
            Az contain one or more data center each datacenter contain redundant data,networking...
          4.Subnets -> pieces of Vps contain range of ips  
          5.Private subnets ->>contain data that public can't see like  data  in database or whatever.
          6.Public subnets -> contain data about public stuff like Ec2 instances,graphical interface..
      
          notes;
            Subnets are used to organize resources, share resources publicly,
            or isolate resources to keep them private.

What we use VPC?

    - it helps you esablish connection,restrict access ,make virtual network for you compared with on-premises servers
<img width="1680" height="440" alt="image" src="https://github.com/user-attachments/assets/a03fc71b-a54a-4531-85a7-2ff2df386247" />

What is the VPC gateway?

    - internet gateway
    -it's the enterence of your vpc no one can  access vpc without it
<img width="1680" height="561" alt="image" src="https://github.com/user-attachments/assets/b50de896-8ff0-4528-8b37-90ae62751db3" />

What is the private gateway?

    - it's a private gateway  connected with private vpc(virtual private cloud) like databases or instances   you don't need anyone to see it
    - so  this gateway access only any vpn(virtual private  network) access as the data that coming from these are encrypted.
<img width="1680" height="576" alt="image" src="https://github.com/user-attachments/assets/5a8baf56-2c8f-4552-9267-3bce5c2df96c" />


    notes;
        1.Amazon Virtual Private Cloud
          Amazon VPC is used to establish boundaries around your AWS resources.
        2.Virtual private gateway
          A virtual private gateway allows protected internet traffic to enter into the VPC.
        3.Virtual private network
          A VPN encrypts your internet traffic, helping protect it from anyone who might try to intercept or monitor it.

-----
What are the four  ways that you can connect anyone with  cloud?

    1.AWS Client VPN
    2.AWS site to site  vpn
    3.AWS Privatelink
    4.AWS Direct link


    AWS Client VPN?
      - it's a client service that you use in order to connect your remote  workers  or on-premises workers to the  cloud
      - fully managed you don't need to build the infrastructure or  whatever else.
      - this service scale up or down based on demand
      - in order to accept client you need to make authentications for  him and see whether he is authenticated or not.

    AWS site to site vpn?
      - it's fully managed service in order if you as a  company wants to make private network between your datacenter and your VPC on cloud
        so site to site vpn is so encrypted ,secure,accelerates applications.
        it uses for application migration+secure communication  between remote locations
<img width="1680" height="778" alt="image" src="https://github.com/user-attachments/assets/b275fc6f-5851-4ead-9181-80c349397e5f" />

    AWS PrivateLink?  
      - it's a scalable way to connect you VPC with other services or resources on the cloud without using any Gateway or ips or ...
      - you control the sites,services from your vpc as you used Privatee link
      - helps you secure your traffic + connect with simplified management rules.


    AWS Direct Connect?
      - you connect your network directly with cloud
      - this reduces  network costs+increases amount of bandwidth
  <img width="1680" height="676" alt="image" src="https://github.com/user-attachments/assets/c578a54d-651b-4a8c-a421-e6ba80ff6a41" />

      some benefits  of using Direct connect:
        - it's a good way for low latency apps + video  streaming + high performance apps
        - establish reliable data transfers at massive scale,data backups...
        -  you can connect your on-premises networks with  cloud in order to build high  performance apps..

  Additional AWS Gateway?

      - AWS transit Gateways;
        - this  gateway connect your on-premises and vpc on  cloud   through center-hub in order to expand globally.
      -Nat Gateway;
        - these Gateway within it -> some instances can connect to external vpcs but the opposite can't be.
      - API Gateway;
        - this reponsible for connection with API inside AWS


    to sum up:
      - AWS Client vpn:
          connect remote workers or on-premises to vpn
      - AWS site to site;
          encrypted network with your  vpcs
          encrypted communication with  remote locations..
      - AWS PrivateLink:
          connect services with vpc as though they were  in  your vpc
      - AWS direct  connect:
          dedicated network to your  cloud 
        
