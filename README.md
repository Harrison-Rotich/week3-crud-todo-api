# Week 3 – CRUD Todo API

A simple REST API built with Node.js and Express.js to manage todo tasks. This project demonstrates CRUD operations, request validation, route parameters, and array filtering.

## Features

- **GET `/todos`** – Retrieve all todos.
- **GET `/todos/:id`** – Retrieve a single todo by ID.
- **GET `/todos/active`** – Retrieve incomplete todos.
- **GET `/todos/completed`** – Retrieve completed todos.
- **POST `/todos`** – Create a todo; the `task` field is required.
- **PATCH `/todos/:id`** – Update an existing todo.
- **DELETE `/todos/:id`** – Delete a todo.

## Technologies

- Node.js
- Express.js
- dotenv
- Nodemon (development)

## Getting Started

1. Clone the repository.
2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file if needed and configure your environment variables.
4. Start the development server:

   ```bash
   npm run dev
   ```

5. The API runs on `http://localhost:3000` by default.

## Example Request

Create a todo using `POST /todos` with a JSON body:

```json
{
  "task": "Practice Express.js",
  "completed": false
}
```

The `task` field is required.

## Notes

Todos are stored in memory, so data resets when the server restarts. Use Postman or Thunder Client to test the endpoints.

## Author

Week 3 learning project.
