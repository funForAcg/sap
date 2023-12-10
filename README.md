sap

6、a company is manually deploying its application to production and wants to move to a more mature deployment pattern. 
the company has asked a solutions architect to design a solution that leverages its current chef tools and knowledge. 
the application must be  deployed to a staging environment for testing and verification before being deployed to  production. 
any new deployment must be rolled back in 5 minutes if errors are discovered after a deployment.which aws service and deployment pattern should the solutions  architect use to meet these requirements? 

A.use aws elastic beanstalk and deploy the application using a rolling update deployment  strategy. 
B.use aws codepipeline and deploy the application using a rolling update deployment  strategy. 
C.use aws codebuild and deploy the application using a canary deployment strategy. 
D.use aws opsworks and deploy the application using a blue/green deployment strategy


The requirements mention using Chef tools and knowledge, deploying to a staging environment for testing, and the ability to roll back deployments within 5 minutes if errors are discovered. Based on these requirements, option D is the most suitable:
D. Use AWS OpsWorks and deploy the application using a blue/green deployment strategy.
Here's the breakdown:
Chef Tools and Knowledge: AWS OpsWorks is integrated with Chef, making it a good fit for a company with existing Chef tools and knowledge.
Staging Environment: AWS OpsWorks allows you to set up separate environments, including a staging environment for testing and verification.
Rollback Capability: Blue/green deployment strategy inherently supports quick rollbacks. If issues are discovered after a deployment, you can switch back to the previous (blue) environment rapidly, ensuring a rollback within the 5-minute timeframe.

7, a startup company recently migrated a large ecommerce website to aws the website has experienced a 70% increase in sales.software engineers are using a private github repository to manage code. the devops team is using jenkins for builds and unit testing.the engineers need to receive notifications for bad builds and zero downtime during deployments the engineers also need to ensure any changes to production are seamless for users and can be rolled back in the event of a major issue.the software engineers have decided to use aws codepipeline to manage their build and deployment process. which solution will meet these requirements?

A.	use github websockets to trigger the codepipeline pipeline. use the jenkins plugin for aws codebuild to conduct unit testing. send alerts to an amazon sns topic for any bad builds. deploy in an in-place, all-at once deployment configuration using aws codedeploy
B.	use github webhooks to trigger the codepipeline pipeline. use the jenkins plugin for aws codebuild to conduct unit testing. send alerts to an amazon sns topic for any bad builds. deploy in a blue/green deployment using aws codedeploy.
C.	use github websockets to trigger the codepipeline pipeline. use aws x-ray for unit testing. and static code analysis. send alerts to an amazon sns topic for any bad builds. deploy in a blue/green deployment using aws codedeploy.
D.	use github webhooks to trigger the codepieline pipeline use aws x ray tor unit testing and static code analysis sendalerts to an amazon sns topic for any bad builds. deploy in an in place, ll-at-once deployment configuration using aws codedeploy.



