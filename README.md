# Docker Fibonacci


[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://weather-react-node.herokuapp.com/)

> A project that runs a Node server and a create-react-app app via two separate containers, using Docker Compose on AWS Elastic Beanstalk.



## App

![Screenshot from 2019-11-02 15-24-55](https://user-images.githubusercontent.com/30200462/68069988-fab6a280-fd8d-11e9-9d5a-56d2634c9ef3.png)

Simple React app to calculate Fibonacci of a number


## Architecture

![Screenshot from 2019-11-02 15-34-18](https://user-images.githubusercontent.com/30200462/68069966-a6132780-fd8d-11e9-8ee0-a7b75f29b943.png)

- The react app is which is deployed on AWS Elastic Beanstalk
- Worker uses AWS ElastiCache for calculating the fibonacci
- Express server uses AWS RDS (Postgres) for storing results
- nginx for routing and deploying 
- Travis use for Continuous integration

## To Build 

In the project directory, you can run:

```
docker-compose up
```

Runs the app in the development mode. 
Open [http://localhost:3000](http://localhost:3050)
