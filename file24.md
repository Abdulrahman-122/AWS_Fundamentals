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
            

Pause; Data encryption
