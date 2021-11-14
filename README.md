# Vitaleaf Backend Repo

![](https://github.com/melsouthern/Final-Backend-Vitaleaf/blob/main/IMG_0346.PNG)

## Project Overview

Working in a team of 5 people, we worked together for 2 weeks on our project, Vitaleaf, to conclude our time at Northcoders.

Vitaleaf is a plant management application which we developed for plant owners, like ourselves, to manage and look after their plants. The reason why we decided to develop this app is because many of us in the team owned houseplants, and we often faced the same struggles trying to keep them alive!

With Vitaleaf's watering system, you can keep track of your plants watering dates and find out when they are next due for a drink. The search functionality enables users to find out what types of conditions each plant they own likes to grow in. We also developed plant recognition, meaning when users took a photo of a plant, the app would identify the species of plant and provide the user with it's specific care needs.

During this period, we worked really closely on every aspect of the project. Alongside building the front and backend for the project, we've also worked on wireframing, branding and project management, all while following agile practices like kanban and daily standups.

## App Walkthrough

To view our live application demonstration, click on the below video link:
[![](http://img.youtube.com/vi/VH3ZniWAMrA/0.jpg)](https://www.youtube.com/watch?v=VH3ZniWAMrA&t=986s "View the live presentation")

Alternatively, you can take a look at a short app demonstration on the below link:
[![](http://img.youtube.com/vi/gu5F3IX5qL4/0.jpg)](https://www.youtube.com/watch?v=gu5F3IX5qL4 "View the short demo")

## Backend Tech Stack

- Javascript
- Node.js
- Jest
- AWS API Gateway
- AWS Lambda
- AWS DynamoDB
- AWS S3
- AWS Cognito

## Frontend Repo Setup

1. Firstly, you will need to `fork` the repository to your personal GitHub account. To do this, open the GitHub repository at `https://github.com/melsouthern/Final-Frontend-Vitaleaf` and click on the 'Fork' button on the top right hand corner of the repository. From here you can select your personal account where the repository will be accessible.

2. Once the repository has been forked, you will need to `clone` this repository down to your local machine. To do this, make sure you are on the newly forked personal repository `yourUsername/Final-Frontend-Vitaleaf`, click on the 'Code' button and copy the link provided. From here, open up your IDE and use `git clone` in your command line alongside the provided weblink given to clone the repository to your machine.

3. Now you have cloned and opened the repository, you will need to download the `development dependencies` to ensure that the environment is setup correctly. To do this, enter `npm install` into your command line.

4. Please note the following:

- `npm test` - this will run the test suite
- Please note that this repo only holds the API endpoints which have been added to AWS Lambda directly

## Live API Link

https://l81eyc3fja.execute-api.eu-west-2.amazonaws.com/beta/plants

## Endpoints

`GET /plants`\
?category={category}\
?search={filters common and botanical names using regex}

`GET /plants/{commonName}`

`GET /users`

`POST /users`\
input field: { username, email }

`GET /users/{username}`

`PATCH /users/{username}`\
input field: { newUserName }

`GET /users/{username}/plants`

`POST /users/{username}/plants`\
input field: { nickName, commonName }

`GET /users/{username}/plants/{plant_id}`

`DELETE /users/{username}/plants/{plant_id}`

`PATCH /users/{username}/plants/{plant_id}`\
input field: { newNickName }
