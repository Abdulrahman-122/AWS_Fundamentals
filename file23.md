# AWS identity and Access Management?

    - which means you create access to new users to access your console but you give them what they need and nothing else according 
     to the principle of least privileges.
    - IAM means you give users,groups,.. access based on company security needs.

      so you as a root you have everything in your hand -> so you need to put as security for root (login+MFA(multi factor authentications)
      now you can also give specific users IAM rules according to your need .
How IAM works?
<img width="1525" height="675" alt="image" src="https://github.com/user-attachments/assets/a19e2b46-e065-4896-88c3-e278e726746e" />

    - you as a root have everything
      - you can put IAM user -> to allow for specific user to access your account based on permission you will add later
      - you can put  IAM groups -> to allow for specific group to access your account based on permission you will add.
       also you define some roles or you can allow for him to see some roles like s3 or whatever.
       and all of that you put a permission for it (you give them all they want but nothing else)
Additional Access management services:

    - Aws IAM Identity center: 

        - centralized identity and access management across AWS accounts.
        - this is called:federated identity management:
            it's a system that allows usr to access multi services based on single set of credentials.
     - AWS secrets Manager:
       secure way to manage your Database credentials+ rotate or retrieve them...
       or other secrets throughout their lifecycle.
        secrets-> these are privete things like password,other credentials you must know.
     - AWS System Manager:
         it's a way to show you the nodes across your organization account+region+cloud
           node include; ID,automate registery edits,security patching,your system.
    - 
      notes;
        - MFA adds an additional layer of security by requiring a password, 
          username, something only the user has on them, such as a physical token. 
          For example, a smartphone app generating a one-time code
        - An IAM role is an identity someone can assume to gain temporary access to 
          permissions. When someone assumes an IAM role, they abandon all previous 
           permissions they had under a previous role and assume the permissions of 
            the new role
        - An IAM policy is a JSON document that allows or denies permission to access 
          AWS services and resources. It can be added to IAM users, groups, and roles to
          define access to the particular S3 bucket
        
