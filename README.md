# MavenConnect-API


## Description

MavenConnect-API is a social network web application API where users can share their thoughts, react to friends’ thoughts, and create a friend list. This API is built using Express.js for routing, a MongoDB database, and the Mongoose ODM.

Table of Contents
- [Installation](#installation)
- [Usage](#usage)
-[APIEndpoints](#API Endpoints)
- [Models](#models)
- [EnvironmentVariables](#environmental variables)
- [Contributing](#contributing)
- [License](liicense)


## Installation
Clone the repository:
git clone https://github.com/gocrushgoals/MavenConnect-API.git

Install the dependencies:
npm install

Set up your environment variables. Create a .env file in the root of the project and add the following to the .env file:
MONGODB_URI=mongodb://localhost:27017/mavenconnect
PORT=3001


## Usage
Start the server with the command: npm start
The API will be running at http://localhost:3001.

## API Endpoints

Users
GET /api/users

Retrieve all users.
GET /api/users/:userId

Retrieve a single user by ID.
POST /api/users

Create a new user.
PUT /api/users/:userId

Update a user by ID.
DELETE /api/users/:userId

Delete a user by ID.
POST /api/users/:userId/friends/:friendId

Add a friend to a user's friend list.
DELETE /api/users/:userId/friends/:friendId

Remove a friend from a user's friend list.
Thoughts
GET /api/thoughts

Retrieve all thoughts.
GET /api/thoughts/:thoughtId

Retrieve a single thought by ID.
POST /api/thoughts

Create a new thought.
PUT /api/thoughts/:thoughtId

Update a thought by ID.
DELETE /api/thoughts/:thoughtId

Delete a thought by ID.
POST /api/thoughts/:thoughtId/reactions

Add a reaction to a thought.
DELETE /api/thoughts/:thoughtId/reactions/:reactionId

Remove a reaction from a thought.


## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any changes.

## License
This project is licensed under the MIT License.