<!-- Please update value in the {}  -->

<h1 align="center">Weather ForeCast app</h1>

<div align="center">
   Solution for a Assignment from  <a href="#" target="_blank">simpluslabs</a>.
</div>

<div align="center">
  <h3>
    <a href="https://newweatherapp1.herokuapp.com/">
      Demo
    </a>
    <span> | </span>
    <a href="https://github.com/rahul9852-dot/mern-weather-app">
      Solution
    </a>
  </h3>
</div>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Overview](#overview)
- [Built With](#built-with)
- [Frameworks](#Frameworks-and-Libraries-used)
- [Features](#features)
- [How to use](#how-to-use) 
- [Contact](#contact)


<!-- OVERVIEW -->

## Overview

![screenshot](https://github.com/rahul9852-dot/mern-weather-app/blob/master/client/src/assets/Fonts/weather.png)

### Built With

- [MongoDB](https://www.mongodb.com/)
- [Express](https://expressjs.com/)
- [React](https://reactjs.org/)
- [Node](https://nodejs.org/en/)

### Frameworks and Libraries used

- MongoDB
- Express
- React
- Node
- Scss
- javascript

## Features

- Users can see city weather as default, preferably my current location
- Users can search for Zipcode to see their current weather and their 10 most recent weather update 
- Users can see the date and location of the weather
- Users can see according to image for each type of weather
- Users can see the min and max degree each day
- Users can see wind status and wind direction
- Users can see humidity percentage
- Users can see a visibility indicator
- Users can see the air pressure number
- Users can request my current location weather
- Users can convert temperature in Celcius to Fahrenheit and vice versa
- Users can also store weather data in local storage, MongoDB to see their recent update in weather.

## How To Use

<!-- Example: -->

To clone and run this application, you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
$ https://github.com/rahul9852-dot/Assignment-Weather-App.git

# Install dependencies
$ npm run setup

# Run the app
$ npm run dev
```

### .env file
Need two creds. Weather API and mongo connection string

#### Mongo
Log into [mongo](https://account.mongodb.com/account/login)

On the left-hand sidebar, you should see **Database Access**. Click on it and make a new user for yourself.  
1. Click on `Add New Database User`
2. Create a new user by filling out `username` and `password`  
(this will be different creds than your actual mongo account. This gives a user access to this particular database.)

On the left-hand sidebar, you should see **Network Access**.  
Make a new access point for your IP address to get permission on using your MongoDB.

Now create a `.env` file in your root directory of `mern-weather-app` and dynamically add this to your `.env`
```javascript
DB=mongodb+srv://<username>:<password>@<cluster-id>.mongodb.net/test?retryWrites=true&w=majority
```
To get the cluster-ID, go to **Clusters** and click on **Connect > Connect your application** to get a more detailed view of how the DB string should look like. 


## Run Locally
**Note:** The mongo connection is commented out in `server.js`. Just uncomment the code block to connect to mongo:
```javascript
// mongoose.connect(process.env.DB, {
//     useNewUrlParser: true,
//     useUnifiedTopology: true
// }).then(() => console.log('MongoDB Connected...')).catch(err => console.log(err));
```

## You can now run your local.  
Go to your root directory and start your web app:
```javascript
npm run dev
```
This is the command will your client and server concurrently. 
- client - localhost:3000
- server - localhost:5000

The service will auto-watch both frontend and backend, so no need to restart to see your changes.  
Once you save your changes, it'll auto-refresh to view your changes.


## Contact

- GitHub [@rahul9852](https://github.com/rahul9852-dot)






















