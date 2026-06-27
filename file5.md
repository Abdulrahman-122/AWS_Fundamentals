# Messaging and Queuing

What is a single monolithic service(tightly coupled)? 

 - architecture of service contain (database logic,web application,user interface ) tightly coupled together
    if one service fail -> the entire system will fail also.
   - <img width="1680" height="861" alt="image" src="https://github.com/user-attachments/assets/6b52dca3-e95d-416f-b6ae-1c69ac65fc2b" />

What is the Microservices architechture(loosely coupled(each part is alone)?

  - the arechitechture of the system is separate at each service (each service work with itself)
    - this ensure if a service fail => the entire system still function well.
    - <img width="1680" height="851" alt="image" src="https://github.com/user-attachments/assets/a113f061-d1b8-425c-b9cd-2f5fa958126d" />
- this type is more scalable than tightly arch
There are three services at AWS to enhance communication?
  1. EventBridge
  2. Amazon SQS
  3. Amazon  SNS

  EventBridge?

         - Serverless service make communication better between parts of application like database,backend...
          ex;
             if you ordered a meal from a restaurant -> this service handle events like order placed or payment method + handle high volumes  of events during peak time

  Amazon SQS?

           - SQS -> message queuing system -> put messages into a queue + then employee will process it and dispatch it from that queue  .
  ex;<img width="1680" height="569" alt="image" src="https://github.com/user-attachments/assets/f6af3dca-8eb2-40dc-8111-aae4c9727090" />


  Amazon SNS?

      - publish-subscribe service 
        it's a service that publish messages to each user based on their interests that they subscribe to it before
        like one customer may love updates about products -> SNS send specific updates about that products
        one may love new products -> SNS is responsible for sending tailored messages to that user based on that.
  <img width="1680" height="802" alt="image" src="https://github.com/user-attachments/assets/3cb5a677-1519-45ec-820f-d83f735fffae" />


notes;

    - In tightly coupled systems, components are heavily interdependent. 
    If one component fails, it can cause cascading failures. 
    In contrast, loosely coupled systems have components that operate independently, 
    so the failure of one component does not disrupt the entire system.
    - Amazon SQS safely stores transaction details until the fraud detection service 
    can process them, preventing data loss when the service is unavailable.
(end of module2)
     
