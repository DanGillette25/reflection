# Explanation of the Directories from Assignment 14.

# Table of Contents:

[Config](#Config)
[Models](#Models)
[Public](#Public)
[Routes](#Routes)
[Diagram](#Diagram)

## Config
This directory contains the code for user authentication.  The passport.js document contains a database call that cross references the user's input with the credentials in the database.  If the creditentials match then the user is let in.  If not then the user receives an error message.  The config.json contains the credentials for the server to access the database.  The is Authenticated.js document determines whether or not a user is logged in.  If they are, they can access the app, if not they are redirected to the login.  Lastly, this directory gets imported into the server.js file which orchestrates all of the files used within this app.

## Models
This directory contains the sequelize schemas for accessing and modifying the relevant SQL tables.  It is imported into the server.js file which orchestrates all of the files used within this app.  It is also imported into the api-routes.js file in the Routes Directory where it is used to architect the necessary API calls.

## Public
This directory contains the front-end code. The javascript files contain the code for gathering the user input and passing it to the authentication mechanisms on the backend.  The HTML files are served via the html-routes.js file in the routes directory.  The CSS files are used to style the HTML files and are linked within the HTML files.

## Routes
This directory contains the routes for making API calls to the database as well as the routes used to serve the HTML files located in the Public Directory.  The api-routes.js file imports the Models directory in order to architect the necessary database calls.  It also imports the Config directory (passport.js) for API calls requiring user authentication.  Like the others, this directory gets imported into the server.js file which orchestrates all of the files used within this app.

## Diagram

  [![Screenshot](https://raw.githubusercontent.com/DanGillette25/reflection/main/screenshot1.JPG)]



