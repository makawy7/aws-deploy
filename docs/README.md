# App Documentation

<br />
<br />

## Architecture Diagram

![Architecture Diagram](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/diagram.png)

<br />
<br />

## Deployment Pipeline Process

<br />

![Pipeline Process](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/pipeline.png)

<br />
<br />

### Deployment Pipeline Process
Successful deployment
![circleci1](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/circleci1.png)
![circleci2](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/circleci2.png)
![circleci3](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/circleci3.png)

<br />
<br />

## Environment Variables
All the environment variables are placed in CircleCI project settings

![Pipeline Process](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/env-variables.png)

<br />
<br />

## App Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

<br />
<br />

## Infrastructure description

<br />

### 1. Amazon RDS For Postgress Database
This app uses Amazon RDS for Postgress databasse hosting, the database endpoint is `abdallahdb.cii7jz6iduzf.us-east-1.rds.amazonaws.com`.

![Amazon RDS](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/rds.png)

<br />
<br />

### 2. Amazon Beanstalk For API Hosting
This app uses beanstalk for api hosting, it uses environment named `udagram`  and the  application  name is `udagram-api`.
URL: http://udagram.eba-92ub49im.us-east-1.elasticbeanstalk.com/

![Beanstalk](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/eb.png)

<br />
<br />

### 3. Amazon S3 For Static Front End Web Hosting
This app uses amazon s3 for static front end web hosting, it uses bucket named `randomabdallah45`.
URL: http://randomabdallah45.s3-website-us-east-1.amazonaws.com

![Amazon S3](https://raw.githubusercontent.com/makawy7/aws-deploy/master/screenshots/s3.png)
