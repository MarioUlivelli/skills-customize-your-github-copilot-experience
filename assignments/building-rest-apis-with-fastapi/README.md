# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI to practice defining endpoints, validating request data, and returning appropriate HTTP responses.

## 📝 Tasks

### 🛠️ Create the API and Read Book Data

#### Description
Create a FastAPI application for an in-memory book catalog. Each book should have an integer `id`, a `title`, and an `author`. Install FastAPI and Uvicorn, run the app locally, and use the automatically generated interactive API documentation at `/docs`.

#### Requirements
Completed program should:

- Define a FastAPI app and a collection of at least two sample books
- Provide `GET /books` to return all books and `GET /books/{book_id}` to return one book
- Return an HTTP 404 response when a requested book ID does not exist


### 🛠️ Add and Update Books

#### Description
Add endpoints that accept book data from a client. Use a Pydantic model to describe and validate the fields sent in the request body.

#### Requirements
Completed program should:

- Define a request model requiring a non-empty `title` and `author`
- Provide `POST /books` to add a book with a unique ID and return the created book
- Provide `PUT /books/{book_id}` to replace an existing book's title and author
- Return an HTTP 404 response when trying to update a book that does not exist


### 🛠️ Delete and Test Books

#### Description
Complete the API by adding a delete operation, then exercise successful and unsuccessful requests using the interactive documentation.

#### Requirements
Completed program should:

- Provide `DELETE /books/{book_id}` to remove an existing book
- Return a clear success response when a book is deleted and HTTP 404 when its ID does not exist
- Use `/docs` to test listing, creating, reading, updating, and deleting books
- Confirm that invalid request data is rejected and that each operation returns the expected status code
