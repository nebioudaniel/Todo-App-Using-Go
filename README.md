# ToDo Task App

A simple ToDo Task App built with Go (using the Fiber framework) for the backend and React for the frontend.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Frontend](#frontend)
- [Contributing](#contributing)
- [License](#license)

## Features

- Add, update, delete, and view tasks.
- Mark tasks as completed.
- Responsive UI built with React.
- RESTful API built with Go and Fiber.

## Prerequisites

- [Go](https://golang.org/doc/install) (version 1.16+)
- [Node.js and npm](https://nodejs.org/en/download/) (for the React frontend)
- [Git](https://git-scm.com/)

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/your-username/todo-task-app.git
    cd todo-task-app
    ```

2. **Backend setup:**

    ```sh
    cd backend
    go get ./...
    ```

3. **Frontend setup:**

    ```sh
    cd frontend
    npm install
    ```

## Running the Application

1. **Start the backend server:**

    ```sh
    cd backend
    go run main.go
    ```

    The backend server will start on `http://localhost:4000`.

2. **Start the frontend development server:**

    ```sh
    cd frontend
    npm start
    ```

    The frontend server will start on `http://localhost:3000`.

## API Endpoints

### Get all todos

- **URL:** `/api/todos`
- **Method:** `GET`
- **Success Response:**
    - **Code:** 200
    - **Content:** `[{ "id": 1, "completed": false, "body": "Learn Go" }, ...]`

### Create a new todo

- **URL:** `/api/todos`
- **Method:** `POST`
- **Data Params:** `{ "body": "New Task" }`
- **Success Response:**
    - **Code:** 201
    - **Content:** `{ "id": 1, "completed": false, "body": "New Task" }`

### Update a todo (mark as completed)

- **URL:** `/api/todos/:id`
- **Method:** `PATCH`
- **Success Response:**
    - **Code:** 200
    - **Content:** `{ "id": 1, "completed": true, "body": "New Task" }`

### Delete a todo

- **URL:** `/api/todos/:id`
- **Method:** `DELETE`
- **Success Response:**
    - **Code:** 200
    - **Content:** `{ "success": true }`

## Frontend

The frontend is built with React and uses Axios for making API requests.

### Available Scripts

In the `frontend` directory, you can run:

- `npm start`: Runs the app in the development mode.
- `npm test`: Launches the test runner in the interactive watch mode.
- `npm run build`: Builds the app for production to the `build` folder.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.

### Steps to Contribute

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
# Nebiou Daniel
