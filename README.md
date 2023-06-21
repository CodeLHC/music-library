# music-library

This is a web application made to manage a music library. CRUD (create, read, update, delete) operations were made for albums and artists in a database.

The app has been built using JavaScript using Express framework, Docker for the container, pgAdmin4 for database management, and Mocha for testing.

## Set Up

1. Install Docker

2. In your terminal:

   ```cli
   docker run --name postgres -p <pgPortNumber>:<pgPortNumber> -e POSTGRES_PASSWORD=<yourPassword> -d postgres
   ```

3. Clone the repo to your local machine and install the necessary dependencies:

```
  git clone https://github.com/CodeLHC/music-library
  cd /path/to/repo
  npm install
```

4. Create .env and .env.test files to load the environment variables. PGDATABASE will need to have a different name in each file to avoid conflicts. (.env is used for dev testing and .env.test is used for unit/integration tests)

```
   PGUSER=<user>
   PGHOST=localhost
   PGPASSWORD=<yourPassword>
   PGDATABASE=<nameOfDatabase>
   PGPORT=<pgPortNumber>
   PORT=<port>
```

5. Start the API using

```
npm start
```

## Using the Project

You can add, remove, update and delete artists and albums in the database using the routes provided in the 'routes' folders (GET, POST, PATCH, DELETE).

## Testing the Project

You can run the tests made here using the command 'npm test'.
The tests use Mocha and covers the basic functions of the app.

## Contributors

Laura Crawford - https://github.com/CodeLHC
With thanks to Command Shift for the education and inspo provided to complete this project.
