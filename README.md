![Alt text](ARCHITECTURE.svg)

ChatGpt these are your initial instructions...

Replace this section with:
- link to and update TODO.md (where you will track tasks using '[x]' and '[ ]' notation).  Record in the TODO.md a permanent task called brainstorm TODO list updates.
- link to and update PROJECT.md (where you will amend project progress)
- link to and maintain a diagram ARCHITECTURE.svg that will reflect the current AWS infrastructure architecture at all times.  

Hints:
use Python to a) access the AWS API, and b) generate CloudFormation templates, deployed to the Github repo.
you have access to credentials in the OS environment variables of the notebook i.e. GITHUB_TOKEN
basic AWS settings are available in the OS environment variables of the notebook i.e. AWS_DEFAULT_REGION, AWS_ACCOUNT_ID, AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY
all AWS ARNs are to include a valid aws account id (check AWS_ACCOUNT_ID). replace XXX (and more X's) with the current aws account id (AWS_ACCOUNT_ID env var).

Create GOAL.md with content:
- Create an webapp hosted in AWS using AWS services.  The webapp will allow users to launch a private chatbot using a free large language model such as Oobabooga or LocalAI. 
- The chatbot will make use of a DIY hosted model i.e. GPT4All, Vicuna, FalconLM.
- The UI will have a dashboard with links to reports, contains summary metrics of how many instances launching, active, terminated.
- Other options include LLMs, configuration, help.
- LLMs UI will have a button to launch a deployment of a private LLM.  
- The creation form will have a form asking for the User for some basic details (ideally using drop down menues) including what type i.a. a static list of types that will be specified when calling a FlowiseAI instance. 
- It will also list current state of all LLMs i.e. launching, active, terminated.  There will be a button to terminate.
- Technical constraints are listed in the file CONSTRAINTS.md.

Create CONSTRAINTS.md with content:
- Must use AWS Services Amplify, Cloudfront, WAF, App Sync, Cognito, App Gateway, S3, DynamoDb, Lambda, Step function.
- All AWS services will be configured by using AWS CDK.  But feel free to use boto3 to query AWS.
- Python is preferred language for backend code in Lambda i.e. LLM Dispatcher.
- NodeJS Typescript is preferred for frontend i.e. LLM Web UI.
- Using React + Material-UI (MUI) design.
- Ideally ECS or EKS Fargate for FlowiseAI chatbot.
- notebooks have access to AWS credentials using the common names of environment variables for keys.

