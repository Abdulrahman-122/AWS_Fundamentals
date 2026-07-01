# Network and application Attacks:

  What is DOS attcks(Denial of service attack)?

      - a way where attacker flood web app with many traffic -> so these traffic must be denied 
        if the app became overloaded + can't respond.
  <img width="1045" height="264" alt="image" src="https://github.com/user-attachments/assets/ca29422e-c501-4bef-91cf-908790112530" />

What is DDOS attacks(distributed denial of servicec attack)?

    -a way where attacker send hugh traffic through many zombie bots (pcs) in order
    to send  unknowingly traffic to the app and make it send it's metadata like ; brute-forcing.
    -What happen at this case?
    AWS stop this attack across infrastructure;
      by: 1.AWS already made Security groups -> so they will ignore attacks using capacity of regions of AWS
      2.also it made ELB  => this handles traffic first before handling it off.
      3.as the capacity of AWS is hugh so the entire number of traffic will not effect AWS infrastructure.
    AWS stop this attack across services by:
      1.AWS shield(default):
         used to clear any attack at the service of the user by:
           detect , mitigate the incoming traffic.
           no cost for this (default one)
        the advanced one-> with cost + providee attack diagnostics +integrate with cloudfront+route 53,ELB
    2.AWS WAF:
      firewall =>monitor traffic that come to the app.
      it checks the coming ips if it in the Acl of ip so it will allow for it to pass
      else will deny it

  notes;
  
          - Unlike a regular DoS attack from a single source, DDoS attacks use networks 
              of compromised computers to send traffic to the target.
          - Security groups make sure only traffic from authenticated users is allowed 
             into the system, while an ELB distributes incoming traffic to prevent any 
             single frontend server from being overwhelmed. Operating at the AWS network
             level, these components leverage the full capacity of the AWS Region to help 
             absorb large-scale attacks.
            
-----
This is how encryption working?

  <img width="1356" height="715" alt="image" src="https://github.com/user-attachments/assets/aa82addf-3d0e-49b4-a80e-5dac84a34afc" />

    = you convert your sensitive info into encrypted info(randomized characters) when you need them =>apply decryption on top of them.

Types of data encryption?

  <img width="1356" height="509" alt="image" src="https://github.com/user-attachments/assets/0d70f38e-6ddc-4923-8275-b0a919be6a57" />

      - Encryption at rest -> your data encrypted at your app
      - Encryption in transit -> your data is encrypted while it's moving to the server using (SSL,TLS) certificates...

      Types of AWS Data Protection?
        1. Amazon S3;
            - this storage contain encryption at rest at the objects that is contain.
        2.Amazon EBS;
            - this storage contain encryption at rest for both snapshots,volumes that related to Amazon Ec2 instances..
        3.Amazon Dynamo DB:
           server side encryption are enabled + stored at AWS KMS(key management system)
        Services at AWS:
          1. AWS Key management Service(AWS KMS)
              this service contain and you can make keys for lock and unlock AWS servicecs like databases 
              you can also disable them .
              these keys called:crytographic keys (randomized characters represent your secret keys)
          2.Amazon Macie;
              you can monitor your sensitive data at rest to make it's safe.
              it's using ML +automation to discover your data in Amazon S3.
              it's good for meeting compliance .
          3.AWS certificate manager(ACM)
            this service is uses to make certificates(ssl,Tls) in order to make encryption in transit  while moving your data from one service to other one.
            








