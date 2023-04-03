# Movies Application
This is a Spring Boot application that provides RESTful APIs for managing movies and their reviews. The application uses MongoDB as the underlying database to store movies and their associated reviews.

## Dependencies

* Spring Boot
* Spring Data MongoDB
* Lombok

## Getting Started
To run the application, first, you need to have a MongoDB instance running on your system or remotely. Then, follow the steps below:

Clone the repository:
```
git clone https://github.com/Kinson99/movies-app.git
```
Navigate to the project directory:
```
cd movies-app
```
Build the application:
```
./mvnw clean package
```
Run the application:
```
./mvnw spring-boot:run
```

The application will start running on port 8080.

## APIs

The application provides the following APIs:

## Movies
GET /api/v1/movies: Gets a list of all movies.

GET /api/v1/movies/{imdbId}: Gets a single movie by its imdbId.

## Reviews

POST /api/v1/reviews: Creates a new review for a movie.

## Code Structure

The application consists of the following packages:


pl.kinast.movies: The root package that contains the main class of the application.

pl.kinast.movies.controllers: Contains the REST controllers for handling movie and review requests.

pl.kinast.movies.models: Contains the models used by the application.

pl.kinast.movies.repositories: Contains the Spring Data repositories used for accessing the MongoDB database.

pl.kinast.movies.services: Contains the services used by the application.

## Configuration

The application can be configured by modifying the application.properties file. By default, the application is configured to connect to a MongoDB instance running on localhost:27017 with the database name movies.

