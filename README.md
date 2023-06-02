# angular-llm-manager

ChatGpt these are your initial instructions:
Update this file to include"
- link to and update TODO.md (where you will track tasks using '[x]' and '[ ]' notation).  Record in the TODO.md a permanent task called brainstorm TODO list updates.
- link to and update PROJECT.md (where you will amend project progress)
- link to and update DESIGN.md (where you will record your design decisions) 
- create GOAL.md with content:
Create an webapp hosted in AWS using AWS services.  The webapp will allow users to launch a private chatbot using a free large language model such as Oobabooga or LocalAI. 
The chatbot will make use of a DIY hosted model i.e. GPT4All, Vicuna, FalconLM.
The UI will have a dashboard with links to reports, contains summary metrics of how many instances launching, active, terminated.
Other options include LLMs, configuration, help.
LLMs UI will have a button to launch a deployment of a private LLM.  The creation form will have a form asking for the User for some basic details (ideally using drop down menues).
It will also list current state of all LLMs i.e. launching, active, terminated.  There will be a button to terminate.
Technical constraints are listed int he file CONTRAINTS.md.
- create CONSTRAINTS.md with content:
Must use AWS Services Amplify, Cloudfront, WAF, App Sync, Cognito, App Gateway, S3, DynamoDb, Lambda, Step function.
Also AWS CodeBuild, CodePipeline, CloudFormation.
Python is preferred language for backend code i.e. LLM Dispatcher.  
NodeJS Typescript is preferred for frontend i.e. LLM Web UI.
Using React + Material-UI (MUI) design.
Ideally using Sagemaker else one of ECS, EKS, EC2, Lambda.  Please advise me of anything better.
