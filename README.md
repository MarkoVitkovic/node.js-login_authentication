# Login authentication
> Simple login and register forms, project is based at backend.

## Table of contents
* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## General info
Simple login and register forms, project is based at backend. Demonstration of tehnologies, as I start learn backend. In this project you can create new user, or if you have account then you can login. This project is not demonstration of frontend, just backend.

## Screenshots
Register form <br>
![](https://github.com/MarkoVitkovic/node.js-login_authentication/blob/master/register.png)<br>
Login form<br>
![](https://github.com/MarkoVitkovic/node.js-login_authentication/blob/master/form.png)<br>
Logged<br>
![](https://github.com/MarkoVitkovic/node.js-login_authentication/blob/master/login.png)<br>

## Technologies
* bcrypt - version 4.0.1
* ejs - version 3.0.2
* express - version 4.17.1
* express-flash - version 0.0.2
* express-session - version 1.17.0
* method-override - version 3.0.0
* passport - version 0.4.1


## Setup
1. First create empty folder and open with VSCode. Then create files(you can see them in projcet) <br>
![](https://github.com/MarkoVitkovic/node.js-login_authentication/blob/master/code.png)<br>
2. Open new terminal and install: <br>
![](https://github.com/MarkoVitkovic/node.js-login_authentication/blob/master/term.png)<br>
3. Install following lib:<br>
  * `npm install bcrypt`
  * `npm install ejs`
  * `npm install express express-flash express-session`
  * `npm install passport`
  * `npm install method-override`
4. To start server use npm run devStart. And open localhost/3000.<br>

## Code Examples
Show examples of usage:<br>
`const initializePassport = require('./passport-config')`<br>
  `initializePassport(`<br>
    `passport,`<br>
    `email => users.find(user => user.email === email),`<br>
    `id => users.find(user => user.id === id)`<br>
  `)`<br>
  
  `const users = []`<br>
  
  `app.set('view-engine', 'ejs')`<br>
  `app.use(express.urlencoded({ extended: false }))`<br>
  `app.use(flash())`<br>
  `app.use(session({`<br>
    `secret: process.env.SESSION_SECRET,`<br>
    `resave: false,`<br>
    `saveUninitialized: false`<br>
  `}))`<br>

## Features
List of features ready and TODOs for future development
* Register form
* Login
* After you login with one user, you cant login whit another user. Only if you logout you can.

To-do list:
* Implement in bigger project
* Add better design
* Connect to real database( online, local)


## Status
Project is: _finished_

## Inspiration
Credits: [Web Dev Simplified](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

## Contact
Created by [Marko Vitkovic](https://github.com/MarkoVitkovic) - feel free to contact me!
