# 🎬 Movie Review API

A secure and testable backend API built with Node.js, Express, and MongoDB that allows users to browse movies, submit reviews, and fetch movie details with optional embedded review data. The API includes JWT-based authentication, robust validation, and automated testing support.

---

## 📖 Project Explanation

The Movie Review API is designed to manage and interact with movie and review data through RESTful endpoints. Authenticated users can submit reviews for movies and retrieve movie details using the optional `?reviews=true` query parameter. It demonstrates secure backend design with token-based authentication, MongoDB relationships, error handling, and integration testing.

---

## 🛠 Installation and Usage Instructions

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
📍 **http://localhost:8080**

You can now use Postman or any API client to interact with the endpoints.

---

## 🧪 Postman Test Collection

📬 **[Click here to access the Postman collection](https://www.postman.com/your-workspace/collections/your-collection-id)**  
*(Replace the above link with your actual shared collection URL)*

This collection includes:
- JWT login & authentication
- Movie detail requests with/without `?reviews=true`
- Valid and invalid review submission
- Protected review deletion

---

## 🌍 Postman Environment Settings

Create a Postman environment with the following variables:

| Variable   | Example Value           |
|------------|-------------------------|
| `base_url` | `http://localhost:8080` |
| `token`    | (Set after login)       |

Use `{{base_url}}` and `{{token}}` in your collection for dynamic request handling.

---

## 📂 Project Structure

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

## 👤 Author

**Kyungju Moon**  
Backend Development Assignment – 2025  
Instructor: *[Your Instructor's Name]*

---

## 📄 License

This project is for educational use only.
