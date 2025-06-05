
# Express.js + PostgreSQL CRUD API

## Setup

1. Install PostgreSQL and create a database:
   ```sql
   CREATE DATABASE myprojectdb;
   ```

2. Run the following SQL to create the users table:
   ```sql
   CREATE TABLE users (
       id SERIAL PRIMARY KEY,
       name VARCHAR(100),
       email VARCHAR(100),
       age INTEGER
   );
   ```

3. Install Node.js dependencies:
   ```bash
   npm install
   ```

4. Start the server:
   ```bash
   node index.js
   ```

## API Endpoints

- `GET /users` - Get all users
- `GET /users/:id` - Get a specific user
- `POST /users` - Create a new user
- `PUT /users/:id` - Update a user
- `DELETE /users/:id` - Delete a user
