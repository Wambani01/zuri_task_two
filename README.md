This is a simple Express API that provides CRUD operations for users using Prisma.

Usage:

# Get a list of all users
GET http://localhost:3003/api

# Create a new user
POST http://localhost:3003/api
Content-Type: application/json

{
  "name": "John Doe"
}

# Get a single user by ID
GET http://localhost:3003/api/1

# Update a user by ID
PUT http://localhost:3003/api/1
Content-Type: application/json

{
  "name": "Jane Doe"
}

# Delete a user by ID
DELETE http://localhost:3003/api/1
Responses:

# Successful responses
GET /api: JSON array of user objects
POST /api: Newly created user object
GET /api/:id: User object with the specified ID
PUT /api/:id: Updated user object
DELETE /api/:id: Deleted user object

# Error responses
400 Bad Request: Request body is invalid
404 Not Found: Requested resource does not exist
500 Internal Server Error: Unexpected error occurred
Running the API:

npm install
npm start
Server will start listening on port 3003.
