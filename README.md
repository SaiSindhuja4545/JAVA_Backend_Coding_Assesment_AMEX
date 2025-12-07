# JAVA_Backend_Coding_Assesment_AMEX

This project implements an in-memory user service with CRUD operations, Vert.x HTTP endpoints,
JUnit 5 tests, and a Docker configuration.

## Build

```bash
mvn clean package
```

## Run (locally)

```bash
java -jar target/java-backend-assessment-1.0-SNAPSHOT.jar
```

The service will start on port `8080`.

## Run Tests

```bash
mvn test
```

## Docker

Build the image:

```bash
docker build -t user-service .
```

Run the container:

```bash
**
## API Endpoints (CRUD Operations)**
1.   POST /users
    Request Body (JSON)
        {
        "id": 1,
        "name": "John Doe",
        "email": "john@example.com"
        }

2. Get User by ID

GET /users/{id}

http://localhost:8080/users/1

3. Update User Email

PUT /users/{id}/email

Request Body (JSON)
{
  "email": "new-email@example.com"
}

4. Delete User

DELETE /users/{id}

http://localhost:8080/users/1
docker run -p 8080:8080 user-service
```
