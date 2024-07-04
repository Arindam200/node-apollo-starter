# Node Apollo Starter

This is a sample Node.js application that integrates GraphQL with Apollo Server and uses Permit.io for authorization. The application provides a simple task management system with CRUD operations.

## Features

- GraphQL API with Apollo Server
- Permit.io for authorization
- Task management with CRUD operations

## Project Structure

- `src/models/task.js`: Contains the task data model.
- `src/resolvers/taskResolvers.js`: Contains the GraphQL resolvers for task operations.
- `src/index.js`: Entry point of the application.

## GraphQL Schema

The application provides the following GraphQL operations:

### Queries

- `tasks`: Fetch all tasks.
- `task(id: String!)`: Fetch a task by its ID.

### Mutations

- `createTask(title: String!, description: String!)`: Create a new task.
- `updateTask(id: String!, title: String, description: String)`: Update an existing task.
- `deleteTask(id: String!)`: Delete a task by its ID.

## Authorization

The application uses Permit.io for authorization. Each operation checks the user's permissions before proceeding. The permissions are defined as follows:

- `read`: Required to fetch tasks.
- `create`: Required to create a new task.
- `update`: Required to update an existing task.
- `delete`: Required to delete a task.

## Dependencies

- `@apollo/server`: Apollo Server for GraphQL.
- `dotenv`: Loads environment variables from a `.env` file.
- `graphql`: GraphQL library.
- `graphql-tag`: Library for parsing GraphQL queries.
- `nodemon`: Utility that automatically restarts the server on file changes.
- `permitio`: Permit.io library for authorization.

