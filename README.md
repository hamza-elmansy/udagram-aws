# Hosting a Full-Stack Application

### **The project is part of udacity-fullstack nano-degree and need approvel from udacity to be used**

---

this project was provided as a completed project and my task was to deploy the project and prepare it for deployment and being used.

in this project i used AWS and its' services in order to finish the task, though a workflow. the workflow starts with making and admin account to control the poject and process. second, i needed to make a buscket and database using RDS and S3

After that, i need to use eb to upload, deploy the project. with modified package.json the web is deployed and ready to be used

Using CircleCi connected to repo of the project on github gave circleci the potential to track my changes during the work on the project

## To visit the web site [Site](http://hamza-udagram.s3-website-us-east-1.amazonaws.com) 

This application is provided to you as an alternative starter project if you do not wish to host your own code done in the previous courses of this nanodegree. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

## Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### A way to start this project
1- clone the project
2- add env variables in .env file adding (

| environment variable | describtion |
| POSTGRES_USERNAME | username for database |   
| POSTGRES_PASSWORD | password for database |
| POSTGRES_HOST | link of the database |
| POSTGRES_DB | name of the database |
| AWS_REGION | AWS account region |
| AWS_PROFILE | AWS Access key ID |
| AWS_BUCKET | AWS bucket URL |
| URL | Beanstalk ENV URL |
| SECRET | Database SECRET |
| DB_PORT | Port for DB |

3- CI/CD process 

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
