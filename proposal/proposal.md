
# FilmFav: Social Cinema Review

## Overview
FilmFav is a streamlined movie rating app that helps users discover great films through trusted opinions. By combining personalized ratings with social features, FilmFav creates an engaging platform where movie lovers can share their views and find their next favorite film.
Key Features:

### Smart Rating System
Rate films with both quick scores and optional mini-reviews, plus mood tags for better recommendations
Personal Watchlist: Keep track of films to watch and organize your viewing history
Quick Find: Easy search with filters for genres, release dates.

### Value Proposition
FilmFav makes it simple to rate movies you've watched and find great recommendations from people whose opinions you trust. Whether you're a casual viewer or film buff, FilmFav helps you discover movies you'll love while connecting with others who share your cinematic interests.

### MVP
- AAU, I want to be able to sign up for account with a username and password.
- AAU, I want to be able to view movies and leave a review.
- AAU,  I would like to see other users reviews and comment on their review.


### Stretch Goals
- AAU, I want to be able to add a favorite to my favorites, prospective movie to my watchlist, and a movies I’ve seen to my movies.
- AAU, I want to be able to see the highest and lowest rated movies on my dashboard.
- AAU, I want to access a preview of the films
- Use API instead of manually inputting the films


# WireFrame

## Landing Page
![alt text](../proposal/A7FBD59B-52C4-4874-8B98-71E3DB974B37_1_201_a.jpeg)

## Sign Up
![alt text](../proposal/0D8F0B47-BDFD-4DBD-B248-7E1A179059BB_1_201_a.jpeg)

## Sign In
![alt text](../proposal/655C6077-D3A9-4DB3-A82E-852D16729CE7_1_201_a.jpeg)

## Dashboard
![alt text](../proposal/3D95F674-852E-45FC-A3AD-774BF8B62811_1_201_a.jpeg)

## WatchList
![alt text](../proposal/0177E0D6-FCED-4189-A6E2-A14AC3B5DE15_1_201_a.jpeg)

## My Movies
![alt text](../proposal/ECDACF34-591E-4537-8334-5DD97B014662_1_201_a.jpeg)

## Favorite Movies
![alt text](../proposal/843D9EC0-946C-42E2-AAAB-04814B901B97_1_201_a.jpeg)

## ERD Diagram
![alt text](../proposal/ED48C00A-3508-43D7-992C-DB6E6FCB8C1C.png)

## Components Diagram
![alt text](<../proposal/image (1).png>)



# Routes

### Sign-up

| Action  | Route       | HTTP Verb |
|---------|-------------|-----------|
| Create  | `/user/sign-up`  | POST      |

### Sign-in

| Action  | Route           | HTTP Verb |
|---------|-----------------|-----------|
| Create  | `/user/sign-in` | POST      |
### My Reviews

| Action | Route               | HTTP Verb |
|--------|---------------------|-----------|
| Index  | `/user/myreviews`   | GET       |

---



---

### My Watchlist

| Action | Route               | HTTP Verb |
|--------|---------------------|-----------|
| Index  | `/user/mywatchlist`   | POST       |
| Index  | `/user/mywatchlist/:movie_id`   | Delete     |

---

### My Movies

| Action | Route               | HTTP Verb |
|--------|---------------------|-----------|
| Index  | `/user/mymovies`    | POST       |
| Index  | `/user/mymovies/:movie_id`    | Delete     |



---

### Movies

| Action  | Route                   | HTTP Verb |
|---------|-------------------------|-----------|
| Index   | `/movies`               | GET       |
| Show    | `/movies/:movieId`      | GET       |

---

### Reviews

| Action  | Route                                | HTTP Verb |
|---------|--------------------------------------|-----------|
| Create  | `/movies/:movieId/reviews`          | POST       |
| Get     | `/movies/:movieId/reviews/:reviewId`| GET        |
|Edit     | `/movies/:moviesId/reviews/:reviewId/edit` | PUT |
| Delete  | `/movies/:movieId/reviews/:reviewId`| DELETE     |

---

### Comments

| Action  | Route                                        | HTTP Verb |
|---------|---------------------------------------------|-----------|
| Create  | `/movies/:movieId/reviews/:reviewId/comments`         | POST      |
| Delete  | `/movies/:movieId/reviews/:reviewId/comments/:commentId` | DELETE    |

# Project Timeline

| Day       | Task                                                | Description                                  |
|-----------|----------------------------------------------------|----------------------------------------------|
| Friday    | Submit and Get Proposal Approved                  | Submit detailed proposal with ERD, wireframes, and user stories. Get approval, set up Git repository, and initialize the project structure. |
| Saturday  | Work on Backend                                   | Set up Express server, MongoDB connection, user authentication routes, JWT tokens, and create a basic user model. |
| Sunday    | Backend Development                               | Create Movie and Review models and routes, set up comments functionality, and test API endpoints with Postman. |
| Monday    | Iterative Improvement and Testing                 | Refine existing features, run integration tests, and address any feedback from previous work. Prepare for deployment tasks. |
| Tuesday   | Presentation Day                                  | Showcase the app's progress, demo key features, and gather feedback for final improvements. |
| Wednesday | Backend Deployment                                | Deploy backend to Heroku (or similar) for early integration testing and feedback. |
| Thursday  | Frontend Deployment                               | Deploy frontend to Netlify (or similar) for user testing as the app continues to be built. |
| Friday    | Core Movie Features                              | Build movie listing page, create individual movie view, implement search and filtering functionality, and add movie details display. |
| Saturday  | User Features                                    | Build user profile sections (MyMovies, MyReviews, MyFavorites), implement watchlist functionality, create a review submission form, and add a commenting system. |
| Sunday    | UI/UX Enhancement                                | Style components with CSS, add responsive design, implement loading states, and improve error handling and user feedback. |
| Monday    | Testing & Bug Fixes                              | Perform comprehensive feature testing, cross-browser testing, mobile responsiveness testing, and fix identified bugs. |
