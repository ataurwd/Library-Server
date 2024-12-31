# Book Shop - Backend

This is the backend of the Book Shop application. It is built using Node.js, Express.js, and MongoDB to provide a robust and scalable REST API for managing books, users, and borrowing operations.

## Features
- **User Authentication**: JWT-based authentication.
- **CRUD Operations**: Manage books, categories, and user data.
- **Borrowing System**: Track borrowed books with quantity adjustments.
- **Search and Filter**: Search books by location or category.
- **Protected Routes**: API endpoints secured with authentication.

## Technologies Used
- Node.js
- Express.js
- MongoDB (with Mongoose)
- JSON Web Tokens (JWT)
- dotenv (for environment variable management)
- CORS
- bcrypt.js (for password hashing)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/backend-repo.git
   cd backend-repo
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and configure the following environment variables:
   ```env
   PORT=5000
   MONGO_URI=<Your MongoDB Connection String>
   JWT_SECRET=<Your JWT Secret>
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

## API Endpoints

### Public Endpoints
- `POST /auth/register`: Register a new user.
- `POST /auth/login`: Authenticate a user and return a JWT.

### Protected Endpoints
- `GET /books`: Get all books.
- `POST /books`: Add a new book.
- `PUT /books/:id`: Update book details.
- `DELETE /books/:id`: Delete a book.
- `POST /borrow`: Borrow a book.
- `GET /borrowed`: Get all borrowed books by the user.

## Available Scripts
- `npm start`: Starts the server in production mode.
- `npm run dev`: Starts the server in development mode using nodemon.
- `npm test`: Runs test cases (if implemented).

## Folder Structure
```
src/
├── controllers/
├── models/
├── routes/
├── middleware/
├── config/
├── server.js
```

## Deployment
The app is hosted on Render/Heroku. To deploy:
1. Push your code to the repository.
2. Configure environment variables on the hosting platform.
3. Deploy the project using the platform's deployment process.

## License
This project is licensed under the MIT License.
