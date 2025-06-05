
# Express.js + PostgreSQL CRUD API

## Setup Instructions

1. Install PostgreSQL and create a database:
   ```sql
   CREATE DATABASE myprojectdb;
   ```

2. Create the `users` table:
   ```sql
   CREATE TABLE users (
       id SERIAL PRIMARY KEY,
       name VARCHAR(100),
       email VARCHAR(100),
       age INTEGER
   );
   ```

3. Create a `.env` file with the following:
   ```
   DB_USER=your_pg_user
   DB_HOST=localhost
   DB_NAME=myprojectdb
   DB_PASS=your_pg_password
   DB_PORT=5432
   PORT=3000
   ```

4. Install dependencies:
   ```bash
   npm install
   ```

5. Start the server:
   ```bash
   node index.js
   ```

## API Endpoints

- `GET /users` - List all users
- `GET /users/:id` - Get user by ID
- `POST /users` - Create user
- `PUT /users/:id` - Update user
- `DELETE /users/:id` - Delete user
