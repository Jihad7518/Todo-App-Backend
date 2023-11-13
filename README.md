# Todo-App-Backend

# Todo App Backend

This is a simple Todo app backend created for the purpose of practicing backend development skills. It provides basic CRUD (Create, Read, Update, Delete) operations for managing a list of tasks.

## Features

- Create a new task
- Read a list of tasks
- Update task details
- Delete a task

## Technologies Used

- **Node.js**: JavaScript runtime for server-side development
- **Express.js**: Web application framework for Node.js
- **MongoDB**: NoSQL database for storing task data
- **Mongoose**: MongoDB object modeling for Node.js
- **RESTful API**: Follows REST principles for API design

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/todo-app-backend.git
Install dependencies:

bash
Copy code
cd todo-app-backend
npm install
Configure the database:

Create a MongoDB database.
Update the database configuration in config/db.js.
Start the server:

bash
Copy code
npm start
API Endpoints
GET /tasks: Get all tasks
GET /tasks/:id: Get a specific task by ID
POST /tasks: Create a new task
PUT /tasks/:id: Update a task by ID
DELETE /tasks/:id: Delete a task by ID
Usage
Make requests to the provided API endpoints using tools like Postman or through your frontend application.

Example request:

http
Copy code
POST /tasks
Content-Type: application/json

{
  "title": "Complete README",
  "description": "Write a comprehensive README.md file for the project."
}
Example response:

http
Copy code
HTTP/1.1 201 Created
Content-Type: application/json

{
  "_id": "some-task-id",
  "title": "Complete README",
  "description": "Write a comprehensive README.md file for the project.",
  "createdAt": "2023-11-14T12:00:00Z",
  "updatedAt": "2023-11-14T12:00:00Z"
}
