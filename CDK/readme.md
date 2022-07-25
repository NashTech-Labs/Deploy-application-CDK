# Prerequisites
Before getting started we have some steps we need to follow these are:

You must have installed AWS CLI.
You must have configured credentials with AWS.
Install AWS CDK.

## For installing it use the following command:

'''
$ npm install -g aws-cdk

cdk --version

 '''

Make one repository in your github account and clone it on your local.

### Step1: Firstly I will create a folder for the project and inside this I will initialize my project.

'''
$ cd aws-cdk-pipeline 

$ cdk init app --language typescript

'''

### Step2: Now firstly we will create one directory.
In which we will create two files, one is cdk-pipeline.ts and second one cdk-pipeline stack.ts.

Now inside cdk-pipeline-stack.ts define your pipeline.You can change here the pipeline name as per your wish. And don’t forget to change the input inside the function and give your repository name.

### Step3: Push your code to the github.

### Step4: Now we will store our Github Personal Access Token inside the Secrets Manager in AWS.

For this Sign in to your AWS console and move to Secrets Manager. Click on store new secret, select other types of secrets and then paste your github token under plain text. Click on Next and give a secret name as per your wish.

### Step5: Before deploying bootstrap your project. Run the command for bootstrapping.

### Step6: Now it’s time to deploy our project. Run the following command for deploying it. 

If the deployment is successful you can see the completed CloudFormation stack and the pipeline created. It will contain three stages inside the pipeline: Source, Build, Update Pipeline.

These are the stages that you will find inside CDK pipeline:





