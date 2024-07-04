# Node.js Apollo Starter Template

Welcome to the Node.js Apollo Starter Template! This template provides a basic setup for a Node.js application using Apollo Server and GraphQL. It's designed to help you get up and running quickly with a simple, yet powerful, server-side application.

## Features

- **Apollo Server**: A fully-featured GraphQL server with a focus on easy setup and performance.
- **GraphQL**: A query language for your API, and a runtime for executing those queries by using a type system you define for your data.
- **Nodemon**: Automatically restarts the server when file changes in the directory are detected.
- **Environment Variables**: Uses `dotenv` to manage environment variables.

## Getting Started

### Prerequisites

- Node.js (v18 or higher recommended)
- npm (v6 or higher recommended)

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Arindam200/node-apollo-starter.git
    cd node-apollo-starter
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Create a `.env` file**:

    Create a `.env` file in the root directory to manage your environment variables.

### Running the Application

To start the server, run the following command:

```bash
npm start
```

This will start the server using `nodemon`, which will watch for any changes in your files and automatically restart the server.

### Example Query

The template includes a basic GraphQL query that responds with "Hello, world!" when accessed:

```graphql
query {
  hello
}
```

## Project Structure

```
node-express-starter/
├── src/
│   └── index.js
├── .gitignore
├── package.json
└── README.md
```

- **src/index.js**: The main entry point of the application. It sets up the Apollo Server and defines a basic GraphQL schema and resolver.
- **.gitignore**: Specifies files and directories to be ignored by Git.
- **package.json**: Contains metadata about the project and lists the dependencies.

### Available Scripts

- **start**: Starts the server using `nodemon`.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.