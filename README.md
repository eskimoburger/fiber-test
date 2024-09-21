# Book API

This is a sample server for a book API built using [Fiber](https://gofiber.io/), a web framework in Go.

## Features

- JWT Authentication
- CRUD operations for books
- File upload
- HTML rendering
- Environment variable configuration
- Swagger documentation

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/fiber-test.git
    cd fiber-test
    ```

2. Install dependencies:
    ```sh
    go mod tidy
    ```

3. Create a `.env` file in the root directory and add your environment variables:
    ```env
    JWT_SECRET=your_jwt_secret
    ```

## Usage

1. Run the application:
    ```sh
    go run main.go
    ```

2. Access the Swagger documentation at:
    ```
    http://localhost:8080/swagger/index.html
    ```

## API Endpoints

### Authentication

- `POST /login`: Authenticate a user and receive a JWT token.

### Books

- `GET /books`: Retrieve a list of books.
- `POST /books`: Create a new book.
- `PUT /books/:id`: Update a book by ID.
- `GET /books/:id`: Retrieve a book by ID.
- `DELETE /books/:id`: Delete a book by ID.

### File Upload

- `POST /upload`: Upload a file.

### HTML Rendering

- `GET /test-html`: Render a sample HTML page.

### Environment Configuration

- `GET /config`: Retrieve environment configuration.

## Middleware

- JWT Authentication middleware to protect routes.
- Custom middleware to check user roles.

## License

This project is licensed under the MIT License.