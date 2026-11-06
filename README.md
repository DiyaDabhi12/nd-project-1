"# nd-project-1" 
# Movie Management API

## About Project
This is a Movie Management API built using Node.js, Express.js, and MongoDB. It performs CRUD operations (Create, Read, Update, Delete) on movie data.

## Technologies Used
- Node.js
- Express.js
- MongoDB
- Mongoose
- Postman
- Nodemon

## Installation

First, install all required packages:

```bash
npm install
```

## Run Project

Start the project using:

```bash
npm run dev
```

Server URL:

```text
http://localhost:3000
```

Make sure MongoDB is running before starting the project.

## Database Connection

```text
mongodb://127.0.0.1:27017/movieDB
```

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | / | Check server |
| POST | /addmovie | Add a new movie |
| GET | /getmovies | Get all movies |
| GET | /getmovie | Get a movie by title |
| PUT | /updatemovie | Update movie details |
| DELETE | /deletemovie | Delete a movie |

## Postman Testing

### 1. Add Movie (POST)

URL:
```text
http://localhost:3000/addmovie
```

Body → raw → JSON:

```json
{
  "title": "Jawan",
  "genre": "Action",
  "director": "Atlee"
}
```

### 2. Get All Movies (GET)

URL:
```text
http://localhost:3000/getmovies
```

### 3. Get Movie (GET)

URL:
```text
http://localhost:3000/getmovie
```

### 4. Update Movie (PUT)

URL:
```text
http://localhost:3000/updatemovie
```

Body → raw → JSON:

```json
{
  "id": "YOUR_MOVIE_ID",
  "newData": {
    "title": "Jawan Updated",
    "genre": "Action",
    "director": "Atlee"
  }
}
```

Replace `YOUR_MOVIE_ID` with the actual MongoDB `_id`.

### 5. Delete Movie (DELETE)

URL:
```text
http://localhost:3000/deletemovie
```

Body → raw → JSON:

```json
{
  "id": "YOUR_MOVIE_ID"
}
```

Replace `YOUR_MOVIE_ID` with the actual MongoDB `_id`.

## Features
- Add new movies
- View all movies
- Find a movie
- Update movie details
- Delete movies
- MongoDB database connection

## Author
Movie Management API Project


## Database Screenshot

<img src="./screenshots/Screenshot (201).png" 
     alt="MongoDB Compass Screenshot" 
     width="700">
<img src="./screenshots/Screenshot (202).png" 
     alt="MongoDB Compass Screenshot" 
     width="700">
<img src="./screenshots/Screenshot (203).png" 
     alt="MongoDB Compass Screenshot" 
     width="700">
<img src="./screenshots/Screenshot (204).png" 
     alt="MongoDB Compass Screenshot" 
     width="700">