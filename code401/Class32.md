# Serverless and Amplify

## Serverless

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

Available cloud services:

* AWS Lambda
* Google Cloud Functions
* Azure Functions
* IBM OpenWhisk
* Alibaba Function Compute
* Iron Functions
* Auth0 Webtask
* Oracle Fn Project
* Kubeless

### Traditional vs. Serverless Architecture

* Pricing:One of the major advantages of using Serverless is reduced cost.
* Networking: The downside is that Serverless functions are accessed only as private APIs.
* 3rd Party: DependenciesMost, if not all of your projects have external dependencies, they rely on libraries that are not built into the language or framework you use.
* Environments: Setting up different environments for Serverless is as easy as setting up a single environment.
* Timeout: With Serverless computing, there’s a hard 300-second timeout limit.
* Scale: Scaling process for Serverless is automatic and seamless.

### Functions as a Service (FaaS)

FaaS is an implementation of Serverless architectures where engineers can deploy an individual function or a piece of business logic.

Principles of FaaS:

* Complete management of servers
* Invocation based billing
* Event-driven and instantaneously scalable

## AWS

AWS Amplify is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications, powered by AWS. With Amplify, you can configure app backends and connect your app in minutes, deploy static web apps in a few clicks, and easily manage app content outside the AWS console.

## API (GRAPHQL)

The GraphQL Transform provides a simple to use abstraction that helps you quickly create backends for your web and mobile applications on AWS.

The GraphQL Transform simplifies the process of developing, deploying, and maintaining GraphQL APIs. With it, you define your API using the GraphQL Schema Definition Language (SDL) and can then use automation to transform it into a fully descriptive cloudformation template that implements the spec.
