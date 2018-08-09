# Online Judge
A web application for online judge(algorithm questions), built with MEAN stack(MongoDB, Express, Angular and Node.js).

# Function
Solve algorithm questions, submit the solution to see if it passes all of test cases. Currently, three languages are supported, java, javascript and python.

<kbd>![image](/public/questions.png)</kbd>

# Demo
Three available demos:
* `Live Demo on Heroku:` <a href="https://online-judge-mean.herokuapp.com/" target="\_blank">https://online-judge-mean.herokuapp.com/</a>
* `Live Demo on Netlify:` <a href="https://online-judge.netlify.com/" target="\_blank">https://online-judge.netlify.com/</a>
* `Live Demo on Azure:` <a href="https://online-judge.azurewebsites.net/" target="\_blank">https://online-judge.azurewebsites.net/</a>

*Note: The demo websites may be slow when you access them for the first time. Be patient!*

Try it out on any live demo website with the following accounts:
* Regular User: demo / 123456
* Administrator: admin / 123456

# Setup Locally
## 1. Source Files
```bash
git clone https://github.com/jojozhuang/online-judge-mean.git
cd online-judge-mean
npm install
npm run dev
```
Access http://localhost:12080/ in web browser, enjoy!

## 2. Configuration
Notice, four different environments are configured for this app. Edit './server/config/server-config.js' to setup your site, especially the MongoDB connection url.
 Environment  | Command       | Description
--------------|---------------|-----------------------
local         | npm run local | Development environment using local MongoDB
dev           | npm run dev   | Development environment using remote MongoDB hosted on mLab.
stage         | npm run stage | Testing environment using remote MongoDB hosted on mLab.
prod          | npm run prod  | Production environment for deployment, need to set environment variable 'MONGOLAB_URI' for db connection.

## 3. Master Date
When the server is initially started, use admin user 'jojozhuang' and password '111111' to login. Go to 'Database' to import data for 'users' and 'questions'. The data files are located in 'backup_csv' folder.

# Deployment
Follow the tutorial [Deploying Full Stack Angular App to Heroku](https://jojozhuang.github.io/tutorial/angular/deploying-full-stack-angular-app-to-heroku/) to deploy this app to Heroku.

# Portfolio
Read portfolio [Online Judge(MEAN)](https://jojozhuang.github.io/portfolio/online-judge-mean/) to learn the main functions of this MEAN stack app.

# Tutorial
Read tutorial [Building Online Judge Application With Angular and ExpressJS](https://jojozhuang.github.io/tutorial/angular/building-online-judge-application-with-angular-and-expressjs/) to learn how this MEAN stack app is built.
