# Movie Review API

A secure and testable backend API built with Node.js, Express, and MongoDB that allows users to browse movies, submit reviews, and fetch movie details with optional embedded review data. The API includes JWT-based authentication, robust validation, and automated testing support.

---

## Project Explanation

The Movie Review API is designed to manage and interact with movie and review data through RESTful endpoints. Authenticated users can submit reviews for movies and retrieve movie details using the optional `?reviews=true` query parameter. It demonstrates secure backend design with token-based authentication, MongoDB relationships, error handling, and integration testing.

---

## Installation and Usage Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-review-api.git
cd movie-review-api
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment

Create a `.env` file in the root directory and add the following:

```env
PORT=8080
MONGODB_URI=mongodb://localhost:27017/movies
JWT_SECRET=your_jwt_secret_key
```

> Replace `your_jwt_secret_key` and `MONGODB_URI` with your actual configuration values.

### 4. Start the Server

```bash
npm start
```

The server will be running at:  
**http://localhost:8080**

You can now use Postman or any API client to interact with the endpoints.

---

## Postman Test Collection

[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://app.getpostman.com/run-collection/41591091-1b2b23e0-30e6-4e72-bb1d-c5095c95f89a?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D41591091-1b2b23e0-30e6-4e72-bb1d-c5095c95f89a%26entityType%3Dcollection%26workspaceId%3D20d203b2-5fa1-4169-876c-f1d6740e5574#?env%5BMoon_HW4%5D=W3sia2V5IjoiSldUIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IkpXVC4uLiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiSldUIGV5SmhiR2NpT2lKSVV6STFOaUlzSW5SNWNDSTZJa3BYVkNKOS5leUpwWkNJNklqWTNaV1E0WkdJeE5UaGlNR1V6TURBMU1qUTBNakk1TXlJc0luVnpaWEp1WVcxbElqb2lZbUYwYldGdU1pSXNJbWxoZENJNk1UYzBNell6TkRVNU0zMC5WY3JSZXNNTEY3ZnMwSFA0RGZ3NHN5SFkyWXdZV3JoYklpbkdHYTZjQmRrIiwic2Vzc2lvbkluZGV4IjowfV0=)

This collection includes:
- JWT login & authentication
- Movie detail requests with/without `?reviews=true`
- Valid and invalid review submission
- Protected review deletion

---

## Project Structure

```
movie-review-api/
├── models/
│   ├── Movie.js
│   └── Review.js
├── routes/
│   └── index.js
├── tests/
│   └── review.test.js
├── .env
├── app.js
├── package.json
└── README.md
```

---
