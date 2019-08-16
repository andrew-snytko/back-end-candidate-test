# Technical assignment, back end developer
There are four tasks described below, please fork this project, complete the assignment and send a pull request so that we can review your work.
Completing all tasks will definitely be optimal, but two or more tasks completed with a high standard will also be considered.
A candidate is free to use any external resources, if calling a friend (or a stranger) is the the only way out, just do it.
The different tasks in the assignment are stand alone, except the final, where the services created should be tied together.
The entire assignment can be completed using open source software and without using any paid services, as it is possible to run all of the services locally (eg. by using virtualization).
Remember to include a description on how to run and test the work (including dependencies).

The assignment will be evaluated based on the following criterias:
- Completed tasks
- Features, does it work like it's expected to
- Coding style
- Tests
- Finding typos in this Readme

## 1. Serverless function and Cloud Storage
Write a serverless function (eg.AWS lambda), in your preferred language, that takes an object as an argument and writes the object into a file on a cloud storage.

### Suggested tools and services
- Docker
- AWS SAM CLI
- MinIO

## 2. GraphQL server
Start a GraphQL server, that has a schema defined with the following types and queries.
- Types: Program, Product, Transaction, User
- Queries: program, programs, product, products, transaction, transactions, user, users

 Fixtures can be found [here](./fixtures.json)
 
### Suggested tools and services
- Docker
- Apollo, apollo-server and graphql

## 3. Web service
Write a simple web service that connects to the graphql server created in the [task above](#2-graphql-server).
The service should be able to present data fetched using grapqhl queries, but no styling needs to be applied (just show raw data, no css needed).

### Suggested tools
- Docker
- reactjs 

## 4. Connect the services
Create an endpoint on the web service that sends a mutation to the GraphQl server. The mutation should call the lambda, that then writes the data sent to a file on the cloud storage (emulated).
Hint! You can run the different services in the same virtual network (also the lambda) to make communication easier.
