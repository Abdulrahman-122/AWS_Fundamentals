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
AWS pricing options Pause here
