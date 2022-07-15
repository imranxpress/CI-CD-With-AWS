# CI-CD-With-AWS

![aws01](https://user-images.githubusercontent.com/47071968/179134389-9c56ac7e-01c7-422e-8dcd-531ce5d19986.jpg)


Today I am going to share 3 hard to easy ways to create Continuous Integration and Continuous Delivery [CI/CD] pipelines with Amazon Web Services [AWS].

For those who need to know that CI/CD is a process to create a web or mobile application development and deployment pipeline in different development environments like Dev, Stage, UAT, Production etc with the use of version control systems like Github, CodeCommit etc. 


#    📌 Verify -> Build -> Test -> Deploy

These are the four operations that happens with a complete CI/CD process. I will try to break down all these four steps in next 3 types of heard to easy CI/CD pipelines. 


There are a number of benefits to have such automated CI/CD for any web or mobile application development life cycle. Development verification, Quality assurance on Staging, Server side user experience, traffic load and security check up on UAT and finally Certify for production delivery with a seamless experience for both developer and Server support.


📌 So here comes First way from my list of CI/CD process which can be used for static websites development and deployment with Simple Storage Service [S3] from AWS. We will also use CodeBuild to build the application code and use S3 as the artifact storage. You can use either github or CodeCommit for the code source provider and connect the repository branch with the CI/CD pipeline in such a way that it can detect the code changes every time and deploy the changes to the desired deployment environment. 


⚙ With CodeCommit there is no webhook need to be added in CodeBuild phase but to configure a branch so that it can track that branch and detect new changes on it and automatically start the pipeline to build as per the defined BuildSpec.yaml and deploy accordingly to the S3.


⚙ With Github you can use webhook like "MERGED, PULL REQUEST MERGED, PUSHED" etc to detect the code changes and automateically start the pipeline to verify, build, test and deploy it.

![aws02](https://user-images.githubusercontent.com/47071968/179130079-20ca3f1d-538e-4fd4-834d-5e66d6c41818.jpg)


📌 Now for the Second way to create a CI/CD pipeline is a Serverless way and I love it the most. It's with the service called Amplify. I would highly recommend this CI/CD pipeline to follow if you are building any...


#     Serverless application, Static Web applications, JS framework based web Applications and NoSQL based web applications. 

###  Please follow one of my previous article linked bellow with step by step process to create a super easy CI/CD pipeline for Web or Mobile development.

https://www.linkedin.com/pulse/serverless-development-aws-amplify-partha-sarathi-kundu-he-his-/

📌 With that I am going to share my Third and super easiest CI/CD pipeline creation with a cool service from AWS called "CodeStar" which includes CodeCommit, CodeArtifact, CodeBuild, CodeDeploy and CodePipeline to create an automated and fully agile CI/CD for Web and Mobile application development. It support a variety of types of applications sample to start with. 

###  This is the site AWS codestar documentation:  [AWS Codestar](https://docs.aws.amazon.com/codestar/latest/userguide/welcome.html).

When you create a project, AWS CodeStar quickly sets up a sample application and configures all the AWS resources for the infrastructure to run your application.

You will be amazed by the number of technologies does CodeStar support with sample project template to start with.

### The AWS CodeStar project templates in this category support development in Ruby, Java, ASP.NET, PHP, Node.js, and more.

## 📌 How Do I Get Started with AWS CodeStar?
To get started with AWS CodeStar:

   1. Prepare to use AWS CodeStar by following the steps in [Setting Up AWS CodeStar](https://docs.aws.amazon.com/codestar/latest/userguide/setting-up.html).
   2. Experiment with AWS CodeStar by following the steps in the [Getting Started with AWS CodeStar](https://docs.aws.amazon.com/codestar/latest/userguide/getting-started.html) tutorial. 
   3. Share your project with other developers by following the steps in [Add Team Members to an AWS CodeStar Project](https://docs.aws.amazon.com/codestar/latest/userguide/how-to-add-team-member.html). 
   4. Integrate your favorite IDE by following the steps in [Use an IDE with AWS CodeStar](https://docs.aws.amazon.com/codestar/latest/userguide/setting-up-ide.html). 
   
   ![aws03](https://user-images.githubusercontent.com/47071968/179133256-db508fc9-5e4c-48f0-bbd2-62fa4afc7624.png)
   
 ###  This is the architecture behind the CodeStar CI/CD pipeline to execute. ⤴ For more in depth knowledge please visit this link bellow. ⤵ 
 
 [New- Introducing AWS CodeStar – Quickly Develop, Build, and Deploy Applications on AWS](https://aws.amazon.com/blogs/aws/new-aws-codestar/). 
 
## Stay safe and NEVER STOP LEARNING... 
   


