# Edge Networking services:

    - Route53;
        - it's a dns resolver that route end user to the applications that provided by AWS like EC2 instances...
        - it  manage all of your domain  names within a single location.

    -Amazon CloudFront:
        -  service uses CDN(content delivery Network)
        - it stores  copies of  your  service like apps and stores it near to the users instead of accessing your service each   time your  user  wants to access your data
        so it makes the process fast and efficient.

      ex;
        -companyies  may use it to stream the videos of their apps fast even at high demand
        - shop stores use it to ship their  data when shopping or whatever.
        - ....
      how it's working?
  -<img width="1680" height="625" alt="image" src="https://github.com/user-attachments/assets/c400c071-2ae5-4609-abef-9143d50d64a0" />

      - you  as a user enter the company name 
      - Route53  -> resolve your dns name  into ips and   send you Ack
      - then you request the ip through near cloudfront
      - cloudfront ask loadbalancer for the traffic of from the  app
      - loadbalancer sends your requesst to the server that responsible for that traffic  
      - data return to you...
    Global Accelerator?

      - it's service that publish your apps globally at the same fast ,efficient 
            if something goes wrong with  your apps in one location  it uses  intellegent traffic and fastover to solve this
            and pass the traffic through private traffic network of AWS
          ex;
            companies  uses this in order to makeesure  no lag when playing a game at many locations.
            banks also uses it to makesure their services are fast even at poor area of network

    to sum up;
      - AWS Route53-> AWS DNS resolver+it makes it possible for a company to make all of their domain names in a single service
      - Amazon cloudfront->CDN service that delivers your content with low latency high speed
      - AWS Global Accelerators -> service that uses AWS global  network to improve application availability,performance,security.


----
When it's coming to connection between corporate that needs to send their data across AWS but they want secure transmission ?

    - so they can choose direct connection which is good for that stuff unlike vpn as they may send hugh data 
    so they use many direct connection with AWS edges then these edges will send thier data to the nearest Azs and store it in their vpc their.
<img width="1680" height="625" alt="image" src="https://github.com/user-attachments/assets/6bd11a88-7419-4c9a-a0e9-ac509d8128a0" />


----
Can you explain how users get to your data if their was in far country??

  <img width="1680" height="806" alt="image" src="https://github.com/user-attachments/assets/59dcf363-357a-4d07-9a8d-557d655ba0a4" />

    - user send request to the nearest route53
    - route53 will search for the closest cloudfront edge location and send their traffic to
      then route53 in this cloudfront will direct that request to the AZs  that belong to your apps or service.

  note:

      AWS Direct Connect connection would provide both the bandwidth for the 
      large data payloads and the security requirements needed for compliance.
      


    
