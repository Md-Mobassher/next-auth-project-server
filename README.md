# Next.Js-Custom-Auth-Server

## Installation:

1. Clone the repository:

```
git clone <repository-url>
```

2. Navigate to the project directory:

```
cd simple-next-authentication-server
```

3. Install dependencies:

```
npm install
```

4. Start the server:

```
npm run dev
```

5. The server will start at `http://localhost:3000` by default.

## Configuration:

- Environment Variables:
  - `PORT`: Port number the server listens on. Default: 3000
  - `MONGODB_URI`: URI for MongoDB database.
  - `JWT_SECRET`: Secret key for JWT token generation.
  - `EXPIRES_IN`: Token expiration time.

## Usage:

- API Endpoints:

  - POST `/api/auth/login`

    - Description: Authenticates user and returns a JWT token.
    - Request:
      ```json
      {
        "email": "example@email.com",
        "password": "password"
      }
      ```
    - Response:
      ```json
      {
        "success": true,
        "message": "User registered successfully"
      }
      ```

  - POST `/api/auth/register`
    - Description: Registers a new user.
    - Request:
      ```json
      {
        "name": "John",
        "email": "example@email.com",
        "password": "password"
      }
      ```

## Dependencies:

- `bcrypt`: Library for hashing passwords.
- `cors`: Express middleware for enabling CORS.
- `dotenv`: Loads environment variables from .env file.
- `express`: Web framework for Node.js.
- `jsonwebtoken`: Library for generating and verifying JWT tokens.
- `mongodb`: MongoDB driver for Node.js.
- `nodemon`: Utility for automatically restarting the server during development.

## Contributing

Contributions are welcome! If you find any bugs or want to suggest improvements, please open an issue or create a pull request.

## License

MIT License
