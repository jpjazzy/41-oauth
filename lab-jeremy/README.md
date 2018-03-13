# General information
_Author_: Jeremy Pearson

_Version_: 1.0.0

_Libraries_ (BACKEND): 

    "dotenv": "^5.0.1",
    "express": "^4.16.3",
    "superagent": "^3.8.2"

_Libraries_ (FRONTEND): 

  NONE

_Last modified_: 3/12/2018

# App use

1. Install with npm i on backend (none needed on front end), and add neccessary .env file and information.

Your env file should contain the following:

```
GOOGLE_OAUTH_ID=[YOUR GOOGLE OAUTH ID GOES HERE]
GOOGLE_OAUTH_SECRET=[YOUR GOOGLE OAUTH SECRET GOES HERE]
PORT=3000
CLIENT_URL=http://localhost:8080
API_URL=http://localhost:3000
```

2. Launch the back end server with nodemon index.js from the backend folder

3. Launch the front end index.html folder with live-server (make sure it's running on port you specify when setting up)

4. Click on the Signup with google href and follow the prompt. See the token on the backend!

# Lab Readme (SPECS)

![cf](http://i.imgur.com/7v5ASc8.png) 41: OAuth
===

## Submission Instructions
  * Work in a fork of this repository
  * Work in a branch on your fork
  * Write all of your code in a directory named `lab-` + `<your name>` **e.g.** `lab-duncan`
  * Submit a pull request to this repository
  * Submit a link to your pull request on canvas
  * Submit a question, observation, and how long you spent on canvas 
  
## Learning Objectives  
* Students will learn to add Google OAuth to an express/mongo app

## Requirements  
#### Configuration  
* make a copy of a previous backend project (not sluggram) that uses authorization in the `/lab-<yourname>/something-backend` directory
* make a copy of a previous frontend project (not sluggram) in the `/lab-<yourname>/something-frontend` directory

#### Feature Tasks  

#### backend
* create an app on the google dev console
 * configure oauth credentials to support a client app on `http://localhost`
 * configure oauth credentials to support a server redirect uri to `http://localhost:3000/oauth/google/code`
* create a backend route `GET /oauth/google/code` for handling google oauth 

#### frontend 
* create an index.html with an anchor tag pointing to the google authorization page 
* configure the query string with correct key value pairs

####  Documentation  
Write a description of the project in your README.md, including detailed instructions for how to build your app. In your frontend README.md add a code block with your frontend .env vars, and in your backend README.md add a code block with your backend .env vars. 