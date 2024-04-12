Movies Website
Description
This project is a Movies website with backend implemented in Spring Boot and frontend in React. It provides functionalities such as user authentication, movie listing, reviewing movies, and adding movies to the watchlist.

Backend
The backend is developed in Spring Boot and includes the following main components:

Authentication: User registration and login functionalities are implemented using Spring Security and JWT tokens.
Controllers: RESTful APIs for user authentication, movie listing, reviewing movies, and managing the watchlist.
Services: Services to handle business logic, including user registration, movie operations, review management, and watchlist management.
Security: JWT token generation and validation are managed using JwtUtils.
Persistence: MongoDB is used as the database to store movie and user-related data.
Dependencies
Spring Boot: Provides the core framework for building the backend application.
Spring Data MongoDB: Simplifies the interaction with MongoDB for data persistence.
Spring Security: Provides authentication and authorization functionalities.
Lombok: Reduces boilerplate code in Java classes.
JUnit: Framework for writing and running tests.
JJWT: Library for JSON Web Tokens.
Frontend
The frontend of the website is implemented in React. It interacts with the backend through RESTful APIs to fetch movie data, manage user authentication, and perform other actions.

Setup Instructions
Backend Setup:

Clone the repository.
Ensure you have MongoDB installed and running locally.
Open the backend project in your preferred IDE.
Configure the MongoDB connection details in application.properties.
Run the Spring Boot application.
Frontend Setup:

Clone the repository.
Navigate to the frontend directory.
Install dependencies using npm install.
Start the development server using npm start.
Accessing the Website:

Once both backend and frontend servers are running, access the website through the provided URL or localhost address.
API Endpoints
Authentication:

POST /auth/register-user: Register a new user.
POST /auth/login: Authenticate a user.
Movie Operations:

GET /api/v1/movies: Get all movies.
GET /api/v1/movies/{imdbId}: Get details of a single movie.
Review Management:

POST /api/v1/reviews: Create a review for a movie.
Watchlist Management:

POST /watchlist/{imdbId}/save: Add a movie to the watchlist.
GET /watchlist/{email}/getByUserEmail: Get movies in the watchlist for a user.
Contributors
Blajan David
