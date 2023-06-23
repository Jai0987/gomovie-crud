# Go Movie Web Server

This project focuses on designing a simple web server using the Go programming language, with endpoints to display movies and their details. It utilizes the Postman API tool to interact with the server using HTTP requests and responses on localhost.

## Prerequisites

- Go (version 1.16 or higher) should be installed on your system.
- Postman (version 8.0 or higher) should be installed to test the API endpoints.

## Installation

1. Clone the repository or download the source code.

`git clone https://github.com/your-username/go-movie-web-server.git`

2. Navigate to the project directory

3. Install the required dependencies
`go mod download`


## Usage

1. Start the Go server.

2. By default, the server will run on `http://localhost:8000`.

3. Open Postman and use the following endpoints to interact with the server:

- **GET /movies**: Retrieve all movies.
- **GET /movies/{id}**: Retrieve a specific movie by ID.
- **POST /movies**: Create a new movie. Send a JSON payload with movie details in the request body.
- **PUT /movies/{id}**: Update an existing movie. Send a JSON payload with updated movie details in the request body.
- **DELETE /movies/{id}**: Delete a movie by ID.

### Movie Object

The movie object has the following properties:

- `id` (string): Unique identifier for the movie.
- `ISBN` (string): International Standard Book Number (ISBN) of the movie.
- `title` (string): Title of the movie.
- `director` (object): Director information containing `firstname` and `lastname`.

Example Movie JSON object:

```json
{
  "id": "1",
  "isbn": "438227",
  "title": "Movie One",
  "director": {
    "firstname": "John",
    "lastname": "Doe"
  }
}

# Contributions

Contributions are most welcomed! If you find any issues or want to add new features, feel free to open a pull request.

# Resources and Credits
This project was made from the perspective of a training module in GoLang for beginners. It takes the help of the following video and hence, all the credits for this project goes to the following video owners and contributors -
https://www.youtube.com/watch?v=jFfo23yIWac&t=1061s

# Thank you
