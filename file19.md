# AI/ML (module8)

    AI -> science build humanlike tasks in order to mimics human being.
    ML -> Train AI by find a pattern then build a model in order to make AI learn it and perform it later based on some rules.
  <img width="1194" height="355" alt="image" src="https://github.com/user-attachments/assets/fe366720-ac12-4300-9525-9556815957d0" />



How ML help AWS ?

    -ML predict
      - trends
      - decisions
      -detect anomalies.
What are the AI/ML stack inside AWS?
<img width="1162" height="229" alt="image" src="https://github.com/user-attachments/assets/76bf6c8e-d512-4871-9305-cab2c5aebc3c" />

    - AI services:
        pre built models that are trained to perform specific tasks

    - ML services;
        Own ML models with fully managed infrastructure.
    - ML frameworks and infrastructure:
        custome approach to build models with purpose chips that integrate with ML frameworks.


------
# AWS AI/ML in detail 
Tier 1
1. Pre-built AWS AI-services:

       1.Language service:
           AWS uses models for this type.
           1.Amazon Comprehend
             this type extract key-insights + sentiments from the language ,compliance sentences...
           2.Amazon Polly;
             this type convert text -> speech
             good at assistent,e-learning...
           3.Amazon Transcribe:
             this type convert speech into text
             support multi language
             good for transcription,subtitling,metadata.
           4.Amazon Translate
             translate from language to others.
       2.computer vision+search engines:
           good for answering questions + gathering insights from videos,other stuff.
           Models:
               1.Amazon Kendra
                  use NLP (natural language processing) to search for a keyword or object within bunch of hugh data
                 uses: intelligent search,chatbots,search .
               2.Amazon Rekognition
                  - identify objects,texts witin images,videos stored in Amazon simple storage service (S3)
                  - uses;identity varifications,media analysis
               3.Amazon Textract
                 - extract handwritten text found in forms,tables.
                 good at healthcare,government...
       3.Conversational AI,Personalization services:
             - you want users to interact with your app
             - also you want to recommend some interests for them this is good for that
             Models;
               1. Amazon Lex;
                   this interact with user through conversation by using Natural language understanding , automated speech recognition
                   good for : Assistent helping,application bots.
               2.Amazon Personalize
                 -you build recommendation based on interests and historical data

Tier2
2. ML service:

      - this is more suitable if you want to control ML model without manage infrastructure.
       Models:
           - SegaMaker AI
               this model enable you to build your custom model and train it using Segamaker AI integerated development environment(IDE)
               by using this Ai you can debug,visualize data,
               offers access to hunderds of pre-trained model that you can deploy in fast way.

            Benefits:
              - this tool is free for any kind of work like , analyst,business..
              - fully managed infrastructure
              - Repeatable ML workflows.

Tier3

3.ML workflows and infrasturcture:

    these are custom frameworks especially for organizations that needs training process.
    -ML workflows:
      software library or tool that provide experienced ML environment to practice on it for ML practioners
      provide pre-built componant to help practitioners in their learning process
      AWS frameworks like; pytorch,Tenserflow..
    -AWS ML infrastructure:
      -ML-optimized Elastic compute cloud,EMR,Emazon Elastic container service -> these tools provide high performance,flexibility for ML workloads.
      
              
