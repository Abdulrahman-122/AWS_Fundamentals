# Detecting+response services?

  you can respond to any security incidents:

    1.Amazon Inspector?

        - it's service that check whether or not your app is vulnerable or not
        = it's running automated security assessments For Amazon Ec2,containers,Lambda functions.
        it show you list of findings by level+how to solve them 
        you can retrieve these findings through an API.
    2.Amazon GuardDuty?
       - this services uses malicious IP,anomaly detection , ML to identify threats accurately.
       so you can use AWS Lambda funtion to remediation these automatically.
    3.Amazon Detective:
      - after detect threat -> apply this to show you more investigate about the root  cause..
      - it has interactive visualization to show you the output of the threat.
        - include resources+user interaction
    4.Security hub;
       combine multi services into a single place 
       you can see your security+compliance state in one view.
       aggregate output from some services into actionable insights.
       it can accelerate time to resolution (TTR) with automated remediation.

       note;
         -Security Hub is specifically designed for the aggregation of security 
           findings across multiple AWS services. It's a suitable choice for this 
            use case.

  What are the AWS marketplace for Security?

      there are tools in AWS:
        1.Threat detection and prevention :
              - this tool for detecting malicious things.
        2.Identity+access management tools?
          control user permissions+authentications.
        3.Data Protection tools
          - encrypt sensitive data
        4.Compliance+governance tools
          meet security regulatory requirements.
