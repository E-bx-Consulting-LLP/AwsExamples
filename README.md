# AWS Examples

This repo contains a collection of examples and useful information about developing .Net Core v6 solutions that will inform:

- Code, project and solution structure
- Templating tools, so the codebase maintains consitency across the solution
- AWS serverless stacks, so Lambda and Fargate (ECS)
- Deploying to AWS from Azure DevOps, so joining up an end-to-end provision, build, test, deploy (and test again) pipeline

# Areas of focus

## AWS Amplify

Amplify is a 'batteries included' app development toolkit. It contains a lot, so I wont list all the features here. One of the interesting features is the server-side element - GraphQL APIs can be defined declaritively that resolve to other AWS resources (Lambdas, REST APIs in API Gateway, Step Functions etc.).

> **Open question:** can the GraphQL API consume a websockets API exposed via API Gateway?

## AWS Lambda

Lambdas are *just* containers, but small containers. There are quite a few flavours of .Net app that can be hosted as a Lambda - a single function through to a normal ASP.Net WebAPI.

> **Open question 1:** what does an event driven C# codebase look like using Lambdas and SQS?

> **Open question 2:** can the codebase be run as a vanilla app locally on dev machines?


## AWS Serverless Application Model (SAM)

SAM apps target ECS and Fargate. They still look like normal WebAPIs but contain a lot more infrastructure-as-code.
