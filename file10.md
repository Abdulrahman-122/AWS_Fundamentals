How you access the public resourses on AWS?
  <img width="1680" height="381" alt="image" src="https://github.com/user-attachments/assets/3479c22c-dc9a-4089-83ff-efeee1e8a2f2" />

      - you send your  packets to AWS Gateway
      - AWS Gateway allow for packets
      - but before it enter to public vpcs that contain public instances
      - Network ACls(Access control list) see whether these packets of that user allowed or not
        by check the permission  whether you as user has a credentials or not if you have -> allow to get the instances .

This is a good  metaphor to remember:

      - by default when you build a vpc it's default ACL pass all inbound,outbound packets as it's default rules  allow  anything  
  <img width="1680" height="699" alt="image" src="https://github.com/user-attachments/assets/541941a7-e0b4-4437-ad31-3773684b911d" />

        - Howerever  you must add your  rules to check whether  these packets are accept your or not
  <img width="1680" height="685" alt="image" src="https://github.com/user-attachments/assets/63f52643-de2e-40c8-b0a2-a480773f8e6b" />

      -  Network ACls (virtual firewalls that controll traffic)

      note; 
        - Network Acls are stateless -> they don't remember any inbound,outbound it just check every packet acress through it
  <img width="1680" height="685" alt="image" src="https://github.com/user-attachments/assets/dd5bba0c-ad88-4310-b821-c5300080c6a0" />

What is the security group?

    - it's a virtual firewall that  checks inbound,outbound packets 
      it's default rules  -> checks inbound packets whether it's on the list or  not 
        if  not ->deny it
        however it's allow any outbound  packets to go out of the system
      you  can  add your custom rules
        to allow inbound,outbound packets 
          you  may deny specific packets
          but  if you allow to access specific one  -> you also allow it to go  outbound without checks

look at  this mataphor:
<img width="1680" height="981" alt="image" src="https://github.com/user-attachments/assets/9155b184-ca32-4cdc-8c9f-c19fdf9ddce7" />
<img width="1680" height="990" alt="image" src="https://github.com/user-attachments/assets/ac2daf3c-980a-43ea-9f96-8dd2710eae15" />

      note; 
        security group is statful -> if it has alist of packets that are allowed -> every time these packets  came to  it no need for check it will be  passed through it.
<img width="1680" height="716" alt="image" src="https://github.com/user-attachments/assets/588e7de3-3be5-4432-8c45-0ccddb8fc9e6" />


to sum up:

<img width="1102" height="706" alt="image" src="https://github.com/user-attachments/assets/51f06fb0-576a-4678-84d4-f565eb5596d3" />
<img width="1353" height="721" alt="image" src="https://github.com/user-attachments/assets/9765db39-d16c-4b1d-9789-838ac2faa6a9" />




