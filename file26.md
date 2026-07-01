# Monitoring:

  so this is the workflow that you will work on it:
  <img width="1177" height="577" alt="image" src="https://github.com/user-attachments/assets/7ac826b8-6cbc-4971-8c84-c8b11bd0c2f2" />

    - after=>Security => ptotect whole system from unauthorized access.
    - Monitor=> observe system activity,network traffic...
    - Audit => review and see whether you stick with your policies or not
    - Comply with the settings of the company and make this standard for other services ..

----
What are the importance of monitoring?

<img width="1680" height="440" alt="image" src="https://github.com/user-attachments/assets/a2011edb-7126-4653-a456-51486fa75ece" />

     -this way allow you to detect,obsorve your system and ensuring securiy,avilability.performance...
----

What is CloudWatch?

    -it's manage your entire services on AWS and make you monitor it at the same tim
      it gives you some features;
        1.Monitoring
        2.matrics => collect all your matrices that runs on all your services even on-premises.
        3.alarms ==>this send notifications to your employees based on a matrix you put.
        4.dashboard =>one page you can monitor your resources.
        5.logs==> centralize the logs from all resources .


    Benefits:
      - used in troubeshoot infrastructure.

---
Why we use CloudTrail?
<img width="1680" height="796" alt="image" src="https://github.com/user-attachments/assets/8ca7c89c-8dca-4130-9070-aded15251f6f" />

    - to ensure every logging to our services.
      it store all the logs to your system
      Benefits;
        = auditing,security,monitoring,operational troubleshooting
        = helps you improve compliance,security posture.

      How is it working?
        - collect Apis,calls,activities in consoles ,downloadable.... this is called:CloudTrail Events
        history of the last 90 days with no cost.
        - it collect all the logs and send it to S3 bucket to ensure whether it prove compliance with regulations 
          ex: payment card,ensurance cards.. (this is called: CloudTrail Logs)
        - CloudTrail insights -> this analyse every API that come to you and detect anomalous..
          
----

What are the benefits of Compliance with AWS?

    - AWS helps you meet compliance goals and requirements in the following ways:
      Inheriting the latest security controls that AWS uses on its own infrastructure
       Third-party validation for thousands of global requirements
        Streamlining and automating compliance
        On-demand compliance reports
    - 


    -Some Services that help you achive Complaince?
        - AWS Artifact:
           - it contain many reports about artifacts 
           - it helps you access third party security and compliance.
        -types:
          - AWS artifact Agreements:
                - you can manage agreements for all your accounts in AWS organizations.
                Different agreement are offered to some addresses that has specific regulations like
                  Health insurance Portability and Accountability (HIPAA)
          - AWS artifact Reports
                - this report contain all the stuff about agreements..

----
What is AWS Config?

    - service you uses to audit,evaluate the configurations of your AWS resources.
    - evaluate configuration against desired state,resource config chagnes,fix
    - audit security monitoring 
    - it assess and audit+evaluate the configuration of the team
What about AWS Audit manager?
<img width="1680" height="428" alt="image" src="https://github.com/user-attachments/assets/f5586a5a-9a93-4c0a-8360-212d0cc7f0ce" />

    - service audit your Aws usage+ simplify risks+ compliance assessment.
    - collect evidence + mange data.
    - save time by make automation for auditing across teams + help integrity of audits.
    - used to automate evidence collection+deploy internal risk assessments.
    - it doesn't evaluate configurations.
----
What is AWS Organizations?

    - it's an organization that helps you govern your account and resources
    - it helps you manage policies.
    - helps you automate your account
    Benefits:
      -it helps you scale your resources
      - simplify permissions through SCPS ,optimize costs...
This is how the Hierarchecy of the AWS looks like?
  <img width="1680" height="838" alt="image" src="https://github.com/user-attachments/assets/68623f22-5194-4e79-a0b8-bfd2f2957653" />

        - AWS organization-> central unit that contain root member that control everything
        - management account -> account manage every other accounts and give roles for them
        - OUs (organizational units ) -> members through the accounts.
        - SCP -> service control policy that you put on even account of user or OUs ...
        - Member account ->members that have needs that don't overlap with other OUs .
        
        
        - notes;
          - In AWS Organizations, you can apply SCPs to the organization root, 
          an individual member account, or an OU. An SCP affects all IAM users, groups,
          and roles within an account, including the AWS account root user.
          You can apply IAM policies to IAM users, groups, or roles. 
          You cannot apply an IAM policy to the AWS account root user.

----

Governance:

What are the types of Awc Governance?  
 1.AWS Control Tower:

      - service you use to enforce+manage governance rules for security across all the organization.
    Benefits:
      - uses preconfigured controls
      - help you set up multi-account environments
      -automation with built-in governance + integration of third-party at scale.
      -uses to deploy apps
-How is it working?
    - <img width="1680" height="388" alt="image" src="https://github.com/user-attachments/assets/8f7eeba0-1f2d-41e8-968b-d34add25f4a2" />

          - it see the provisioned accounts+see policy enforcement+can help you detect noncompliant resources.
          -then we have AWS Control Tower Factory->standardizes template that prrovisioning new accounts.
          - then we have control -> provide governance for all AWS environment
          - then we have landing zone that contain all the stuff about AWS account like;users,OUS ,

2.AWS service Catalog?

    -create ,share from a curated catalog of AWS resources.
    - you can deploy security tools for new AWS accounts so you govern it.
    -it helps you stay agile while perfoming governance across multi-accounts.
    uses:
      - provion access control across multi accounts.
      -applay access control+CI/CD.
3.AWS License Manager:

    -helps you manage your software licenses.
    - fine-tuning your licensing costs.
    uses;Use it to streamline license management and to simplify the Microsoft            License Mobility through Software Assurance experience. You can also use it to        automate the distribution and activation of software entitlements across AWS          accounts for end user
    
    
to rap up:

    - AWS Control Tower:
      -   service uses to govern a secure multi-account in AWS
    - AWS Service Catalog:service uses to share,organize Aws services from curated catalog that you define.
    - AWS License Manager; service helps you manage your software License.
-----

AWS Health:

    - AWS Health Dashboard:
      service shows you your account health ,..
      using AWS Health API
      -gives you time for events.actions..
      -manage service health.
<img width="1680" height="414" alt="image" src="https://github.com/user-attachments/assets/2f3d1549-ea31-43c5-a7b0-93ea8236207a" />

-----

What is AWS Trusted Advisor?
<img width="1680" height="504" alt="image" src="https://github.com/user-attachments/assets/8f382e57-2f02-430f-baec-3fb44dbbdf42" />

    -using this you evaluate your AWS account and look for best practice checks across all services.
    - All of your plans will be checked.
    -helps you optimize your account at scale.
    -used to optimize cost+efficiency,security...

What is AWS IAM access Analyzer?

     -checks your fine grained of your IAM roles.   
     - it varify , refine permissions by analyzing external access 
     - varify that your policies match your standards.
     Benefits:
       - Modify permissions.
       - Validating IAM ploicies.
       - meet your least privilege goals.
       - anything related to accessing your service is responsible for it lke:varify who can accesss...
