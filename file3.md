# How to interact with  AWS Resources?
  
    -  you can use AWS Management console  (through web or mobile)
    -  you can use AWS CLI(this is through bash  this providee automation through scripting + reduce errors that happen in console)
    -  you can use AWS SDK (this is through varies programming language)
note this image :
  - <img width="1652" height="1475" alt="image" src="https://github.com/user-attachments/assets/c1378b49-4e52-4a87-bd72-76aeea2205fa" />
  - The customer handles the operating system, networking, and applications on the EC2 instances. AWS manages the hardware

----
What is AMI ?
  - Amazon Machine image
  -   types;
        -   you can create your  own
        -   you can use Available one
        -   you can purchase for one from third party vendor from the market place
   
          - note;
              - AMI provides repeatability through instances you are build
                by providing the same configurations,deployment.automation... for you
              -To launch an EC2 instance for a web server, configure the AMI to define the operating system and software;
                select the instance type to allocate CPU, memory, and storage; and set up storage options,
                including the type and size of the volume.
                Load balancing, permissions, and instance termination behavior are not required
                when launching a basic Amazon EC2 web server.

             - Amazon machine Image from Ec2 instances => is  a preconfigured image with os and storage and cpus... in order to ship the software that you want to deploy on  internet

----

# AWS pricing options Pause here
  types;

      1. On-Demand instances
         you just  pay for your  consuming
      2.Reserved instances;
          by commiting to 1year or 3year you will  get  a saving up to 75 percent.
          at  pridictable workloads..
      3.Spot instances
          capacity up to 90 percent off 0n demand price + flexibility will interrupted when  AWS reclaims the instance.
      4.Saving plans 
        saving up to 72 percent across  variety of instances by commiting to 1-3 years.
      5.Dedicated hosts 
        this offers  full control + ideal for workloads with  strict security+licensing needs
      6.Dedicated instances 
        offers  isolation from other AWS customers
        pay for instances runs on hardware solely to your account
  
    note;
    - Dedicated Hosts offer exclusive use of a server with full control,
      whereas Dedicated Instances provide isolation without server control.
      this is ideal for security sensitive,licensing workloads
    - Saving Plans:-> 
      offer discounts compared with on-demand-rates 
        good for Predictable workloads
        for using compute for a specified hours per year from 1 to 3 years.
        provide  flexible pricing for Ec2,Forgate,Lambda,AI stuff
        payment include All upfront,partial upfront,No upfront.

    -What is Capacity Reservations?
      - good for critical workloads  with strict capacity requirements
      - with Ec2 you can reserve instance  in a specific availability zone for your critical workloads.
      - you only pay for instances you run
      used in on-Demand rate
      - Reserved instance
        good for steady state workloads with predictable usage
        applies over 75 percent over on-demand pricing 
        applying  discount across the availability zone inside region
        once you purchased one -> AWS offers  discount for other instances inside the same family based on instance size footprint.
    
      -On-Demand instances are more expensive than other pricing options and offer no cost- 
        saving benefits for interruptible workloads
      -Spot Instances offer up to 90 percent off On-Demand pricing, making them the most  
      cost-effective option for workloads that can tolerate interruptions.
      -Savings Plans require a commitment to consistent usage, which might not be suitable 
      for a customer just starting with unpredictable usage.

     -On-Demand pricing is ideal for starting without commitment. The customer can test and
       adjust based on actual usage before committing to longer-term options.
  
