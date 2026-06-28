# Storage in AWS

1.What is Block storage?

    - they are persistent storage that are store data in Ec2 instances  they are attatched to it
    -  but these block storage are encrypted,backed up...
      types of Ec2;
        - Amazon Ec2 store:
            - this type is responsible for storing non-persistent data these storage are temporary
            - this type unmanaged.
        -Amazon EBS(Elastic book store)
            - that  type of storage is persistent attatched to Ec2 
            they are managed.
2.What is the Storage Object?

    - this is the object architechture that archtecht data in specific way
      they need metadate in order to make the process of  searching,accessing data very fast.
      ex; Amazon simple storage service(s3)
        fully managed data object that store and retrieve data from anywhere
3.What is the filesystem?

     - this is how AWS stores data inside it as standard filesystem and these systems can be able to share to any device
     they are fully managed
     types;
       1. Amazon Elastic file system 
           fully managed NFS system that used by cloud,on-premises services
       2.Amazon fsx:
         fully managed system for windows,ontap..



Additional Storage services??
    1. AWS Storage Gateway;

          -fully managed
          - hybrid cloud service ->provides on-premises access to cloud
  2. AWS Elastic Disaster Recovery:

         - fully managed services
         -  recover the streamline of your service that are virtually,cloud-based-service in AWS.

     notes;

       - in case of the fully managed service:
       -   <img width="762" height="604" alt="image" src="https://github.com/user-attachments/assets/952e66b6-93f0-4577-8eb5-9df631f69037" />
       - in case of the managed service :
         - <img width="764" height="610" alt="image" src="https://github.com/user-attachments/assets/941d0543-5472-4562-be4e-c136ec7facf9" />
      - in case of the  unmanaged service
        - <img width="764" height="606" alt="image" src="https://github.com/user-attachments/assets/93c65fa1-73aa-4928-9af7-f59897b59b01" />

        
