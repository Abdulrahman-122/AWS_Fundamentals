# Well Architect(last module)

AWS services for specialized use cases:

    1.Development Services:
      a.AWs CodeBuild  
          - fully managed service 
          - Continuious integration =>compile source code.
          - run tests + produces software packeges.
          - scale up or down
      b.AWS codePipeline:
        - fully managed service -> manage CI/CD + automates the build.
        - deploy phases of your release process.
        - this helps devs for streamline their work+deliver new feature...
      c.AWS X-Ray;
        - performance analysis tool helps devs visualize their apps behavior
        - identify performance bottlenecks+troubleshoot issues.
      d.AWS Appsync;
          - fully managed service
          - GraphQl service
          - by using it -> you can create single GraphQl API -> to secure Access,manipulate,combine data from multi sources.
          -GraphQl -> query language for APi in order to control the data that sent to client

      e.AWS Amplify:
          - helps you streamline process of developing,deploying,managing secure,scalable full-stack app on AWs.
          - you can add features like; authentications,APIs,storage...  
    2.Business services:
            a.Amazon Connect
              Businesses can use this AI-powered contact center service to efficiently
              set up and operate a scalable customer service call center. 
              Amazon Connect provides capabilities for call routing, recording, 
              and analytics while integrating seamlessly with other AWS services.
            b.Amazon Simple Email Service (Amazon SES)
                Amazon SES is a scalable and cost-effective email service provider that
                can be integrated into any application for reliable, high-volume email
                automation. It helps businesses optimize the delivery of transactional
                and marketing emails, resulting in enhanced customer engagement.
    3.End user computing services:
         a.Amazon AppStream 2.0
           AppStream 2.0 is a fully managed service that streams applications from
           the cloud directly to any compatible device. This includes software-as-a-service (SaaS) 
           applications and applications converted from desktop to SaaS without code revisions.
           This provides instant access to powerful software without the need for high-end local
           hardware.
        b.    Amazon WorkSpaces
          WorkSpaces is a fully managed cloud-based desktop computing service.
          With WorkSpaces, employees can securely access their work environment 
          from any device with an internet connection. Employees can perform the
          same tasks as if they were on a physical office computer, while companies
          can benefit from cost-efficiency and easy administration.      
        c. Amazon WorkSpaces Secure Browser (formerly Amazon WorkSpaces Web)
            WorkSpaces Secure Browser is a fully managed remote enterprise browser.
            It provides a protected environment for employees to access private websites, 
            SaaS applications, and the public internet. With WorkSpaces Secure Browser,
            IT departments don't need to manage specialized client software,
            infrastructure, or VPN connections.
    4.IOT services:
           a. AWS IoT Core
              AWS IoT Core is a managed cloud service used to securely connect physical 
              devices with cloud applications. It helps you create efficient IoT 
              solutions by streamlining the complex process of ingesting, processing,
              and acting on device data. Device connections and data are secured with
              mutual authentication and end-to-end encryption, and you can choose from 
              several communication protocols.

           - Some IoT solutions include the following:
              Smart security cameras – Home monitoring that sends alerts to your phone
          
              Smart pet feeders – A pet feeder that you can control remotely
          
              Smart irrigation systems – A rain machine that adjusts watering
              based on weather and soil conditions
-------
Well-Architected framework:

    - Pillers of this framework:
        - Operational Excellence;
            - operation monitoring,continuous improvement.
        -Security ->protect system.
        - Reliability:
            - emphasize recovery planning+system adaptability to meet demands.
        -Performance Efficiency:
        - Cost optimization
        - sustainability
    tools;
        - AWS well-Architected Tool;
            - free service that apply these pillers on your workloads.
                - it offers ; review your workload,milestone tracking
                - integrate with AWS identity+Access management(IAM) + APIs
                - support team collaboration.
                -good for architects engineer,compliance team.
How to apply this framework on this system?
    <img width="4917" height="2877" alt="image" src="https://github.com/user-attachments/assets/c59d9a3c-a5ca-4375-9072-05526c11971e" />

        - to apply operational Excellance ;
            -use Ec2 autoscaling -> in order to avoid rush while your system increases.
        - to apply Security;
            - use encryption+IAM policies
        - to apply Reliability;
            - use: Amazon cloudWatch in order to watch the system and automate actions
        - to apply Performance Efficient;
            - AWS compute Optimizer -> in order to avoid wasting resources.
        - to apply Cost Optimization => use AWS budgets,AWS cost Explorer (to track your budgets nad take decisions..)
        - to apply sustainability -> use AWS cost,usage report in order to report your system resources...

-----

Some applications on Well-architected framework?
<img width="1680" height="525" alt="image" src="https://github.com/user-attachments/assets/7b2c0d76-54ea-4364-a771-d6873ef1a019" />

    - this application is called  serverless  web backend by X-ray
        - Amazon Api Gateway ->receives HTTP requests from the client
        - Lambda function --> process the API through the code that you store in
        - then store the resule or extract it from Amazon DynamoDB
        - all of these things are traces by AWS X-Ray.
2.
<img width="1680" height="412" alt="image" src="https://github.com/user-attachments/assets/61944820-4836-40c6-8904-84ab5e5e516d" />

        -Serverless static website with contact form;
          - in this website -> you build a static that connect to our last architecure
          - but here we use Simple Email serviice to send email that processed by it based              on lambda function .
3.<img width="1680" height="709" alt="image" src="https://github.com/user-attachments/assets/d85f860c-47ee-4bfe-8a4e-0f25ba826225" />

        - Customer support with callback option;
            - calls or texts that client send to customer support are stored inside Amazon contact servicec response then directed to Amazon connect through Amazon cloudfront.
            - then we have two ways either connect with live agent directly or
                choose chat using Lambda function that directs you either to live agent or SMS or email....
        

    
