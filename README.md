# 🚀 FastAPI Todo Items API

A simple RESTful API built with **FastAPI** that allows users to create, list, and retrieve todo items.  
This project demonstrates the use of **Pydantic models**, **response validation**, and basic REST API design.


## 📌 Features

- Create todo items
- List all todo items with optional limit
- Retrieve a todo item by ID
- Input and output validation using Pydantic
- Auto-generated API documentation (Swagger & ReDoc)


## 🛠️ Tech Stack

- **Python 3.9+**
- **FastAPI**
- **Pydantic**
- **Uvicorn**


## 📁 Install dependencies

`pip install fastapi uvicorn`


## 📁  Run the application

`uvicorn main:app --reload`


## The API will be available at:

- localhost/`http://127.0.0.1:8000`
- Swagger UI: `http://127.0.0.1:8000/docs`
- ReDoc: `http://127.0.0.1:8000/redoc`


### 🔀 URL Routing

FastAPI uses **URL routing** to map incoming HTTP requests to Python functions.
-  `/` Root endpoint to verify the API is running 
- `/items` Collection of todo items 
- `/items/{item_id}` Access a specific item by its ID 
Each route is defined using decorators such as `@app.get()` and `@app.post()`.


## 🧠 Significance

- Separation of concerns
  URL routing cleanly separates different functionalities.
- RESTful architecture
  Uses standard HTTP methods and resource-based URLs.
- Data validation
  Pydantic models ensure request and response data is structured and validated.


## 📄 HTTP requests
- GET
   - GET `/items` retrieves all items (with optional limit)
   - GET `/items/{item_id}` retrieves a specific item
   - GET requests are read-only and do not modify data.

- POST — Create a Resource
  - Used to create a new item.

