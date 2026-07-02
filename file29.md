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
