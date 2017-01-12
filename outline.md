# Outline

#### Initiating Server:
```
[user@localhost] $ | mongod
```
**mongod** is the primary daemon process for the MongoDB system.

```
[user@localhost] $ | npm start
```
Starts the node server and executes ```index.js``` of the project.

#### index.js:

Mainly performs three tasks in following order:

1. **MongoDb connection**: Mongoose makes a connection to mongoDB.
- **Node server**: Starts the node server and configure port (/config/express.js)


#### MongoDB Models:

All the mongoDB models or schemas are defined under /server/models, namely:
* /server/models/user
* /server/models/vote

#### Express JS:

Express JS contains all the configuration details related to node server. It performs the following tasks:

1. Create and start server.
2. Add different **middleware** namely:
* **bodyParser**: Parse body params and attache them to req.body
* **cookieParser**: Parse Cookie header and populate req.cookies with an object added as key by the cookie names.
* **Compress**: Helps in decreasing the size of the response body and improve the speed of 	the API calls.
* **Passport**: Helps to authenticate different API call.
* **Helmet**: Helps to protect the application from different attacks such as cross-site scripting (XSS), script injection.
* **Cors**: It helps in connecting different domain to the application i.e enable cross origin resource sharing.
* **APIError**: Handles any other error that occurred inside of an API calls such as:
API not found, internal server error, parameter validation error.

3. Api route: Manage various other routes of the application ( /server/routes/index.js )

#### Passport JS:

This module lets you authenticate endpoints using a JSON web token and passport-jwt. A passport middleware is added to all the routes and sockets which will check for authorised token. We can also change the strategy of the passport in the passport-config.js file.

#### Api Routes:

It handles the different routes of the application, namely:

1. **users**: This route contains different routes related to users such as:
  - registration of new user,
  - fetching nearby users,
  - saving vote( like/dislike ) by a user,
  - creating matches as per the request of a user( front-end )
  - updating the user details, etc.

2. **auth**: Manages the login and logout route. This route handles the authentication of the user by 		generating the token.

#### Controllers:

Following are the controllers defined for the above mentioned routes:

1. **user Controller**:
Controls user related tasks, such as:
  - Create new user.
  - Get user details.
  - Update user details, such as, current location etc.

2. **auth Controller**:
Controls user authentication tasks:
  - Login and
  - LogOut.

3. **getNearbyUsers Controller**:
Controls the task of sending nearby users’ details to a particular user as per the preferences( such as gender preferences, the distance within which the user wants to look for a date etc. ) of this user.

4. **saveVote Controller**:
Controls the task of saving a vote, i.e., keeps a record of all the responses of a user while swiping a card( nearby user ), namely, like and dislike.

5. **match Controller**:
Controls the task of creating matches for a particular user as per the responses of this user for other nearby users and also the responses of nearby users for this user, i.e., a match is formed only if two users swipe-right( like ) each other.
