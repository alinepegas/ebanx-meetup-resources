# EBANX Meetup - CI/CD com Github, Travis e AWS Elastic Beanstalk

## Concepts

### CI: Continuous Integration
Integrate: merge your code changes into a central repository
- Integrate frequently (daily)
- Keep changes small
- Build and test automatically on every change

### CD: Continuous Deployment
Deploy: release your code to the wild (production)
- Automatically deploy builds that pass the tests to a staging or production environment

## AWS Elastic Beanstalk
- Orchestration service
- Support for Java, .NET, Node.js, PHP, Ruby, Python, Go, and Docker
- Handles autoscaling and load balancing for you
- You have complete control of the underlying resources

## What we will build
- Central repository: Github
- Integration testing: Travis CI
- Deployment tool: Travis CI
- Production Environment: AWS Elastic Beanstalk
- Monitoring: AWS CloudWatch
- Developer Feedback: AWS Lambda and Slack

## Step by step
- Create Beanstalk environment on AWS Console
- Create IAM user access keys with access to the environment just created
- Have a GitHub repository with your code: https://github.com/alinepegas/eb-ruby-sample-app
- Have a Travis CI account connected to your repository
- Set up AWS credentials on Travis settings for the repository
- Create a `.travis.yml` file in your repository with the specifications for Travis
- Make changes to your code and see them getting deployed to your Beanstalk environment
- Create a webhook on Slack
- Create lambda to post Beanstalk events to Slack
