Going Globally?
  you need to take those into your consideration 
    which region you will expand your services in
    how to make your edge location in order to ship service make consistent power not limited or whatever
    Infrastructure as a code (cloudformation)

    1.which consideration you might choose in ordet to  build the servics in another  regions?
      1.Compliance -> 
        you must accept the GDPR(general data protection Regulation)-> where contenint put restriction in order to prevent shipping data to other country
          so AWS must allows these rules and doesn't try to take data to his country 

      2.Proximity
          - you need as a AWS or any cloud environment to avoid any latency when your users need your service..
      3. Future availability
          not all regions have all features on AWS as this return to GOVCloud that if you applied some rules of US you can  access all the stuff on AWS

      4.pricing => it also play a role for you as a company and a  customer 

      note;
        When working for a government agency, making sure that the selected Region
        complies with all relevant government regulations and policies is important. 
        This includes data sovereignty, privacy laws, and other compliance requirements.
        Proximity to users or data centers is also important. Close proximity reduces 
        latency and improves the performance of applications and services.

How AWS deploying in  multi regions + multi Azs around the world?

    - AWS  making global deploying or global Azs in order to make high availability:
      and this help customers around the world also
        high availability; your system will have low latency + low failure 
        Agility : the ability to change  the service to meeet the requirements of the market you are live in
            this is a pros in AWS so you can change the  service and deploy another one
       Elasticity:
           ability to scale up or down service according to the demand on it
What about Edge location?

    - it's the ability to move across the world in ordet to lower the latency...
      this service Edge location has cloudfront (CDN(content dlivery  network ,otheer services.
What about the Global infrastructure concepts?
  there are three terms;
    Regions,
    Availability zones
    Edge locations

        - Regions -> number of regions contain multi datacenters  each region contain 3 or more availability zones 
        - Availability zones -> this is zones made in order to avoid any low latency + fast connection for the services , efficient services
          each one  contain 1 or more datacenters
        - edge => locate at multi regions around the world contain CDN(cloud delivery network) designed to ship data to these regions  that  far away from availability zones
 
         Regions are physical locations around the world that contain multiple 
         data centers. Each Region contains at least three Availability Zones. 
         Each Availability Zone contains one or more data centers. 
         Edge locations are devices in areas outside of Regions. 
         These devices provide user access to frequently accessed data with low latency.

----
What is Cloud Formation?

    - it's a way you can define your infrastructure across multi regions using Infrastructure as a code
        it's template you just define your resourses in order to run your application
        to interact with AWS APIs
          1. AWS CLI or AWS SDK  
              - cli => you can write routine backups for a service (EBS elastic block store...)
              - SDK ->  you can use it to automate some services  like S3(amazon storage services) to store some data about users)
              - Amazon managment console -> includes services like  billing and amazon quicksite,naptone..
              - IAC(infrastructure as a code like cloudformation) good for CI/Cd,esablishing an  EC2 across multi regions in an  ease way.



        notes;
          cloudformation is designed to handle complex infrastructure setups. 
          It defines infrastructure as code to help make sure that deployments are 
          consistent across different environments such as development, testing, 
          and production.
        - When deciding where to place cloud resources, 
        companies must consider multiple factors.
        Compliance refers to the Region meeting legal or regulatory requirements.
        Proximity to customers helps reduce latency and improve user experience. 
        Feature availability makes sure that the required AWS services are supported
        in the chosen Region. Pricing varies by Region, 
        so cost-efficiency is also a critical factor.
        - By using multiple AWS Regions, a company can place their resources closer to their
         end users, which reduces the distance that the data must travel.
         This results in lower latency and a better user experience. 
         By using multiple Availability Zones within a Region, 
         the company enhances the fault tolerance of their applications.
         If one zone fails, their application can continue to operate from another zone,
         maintaining high availability.

         (end of the module)
         
    
