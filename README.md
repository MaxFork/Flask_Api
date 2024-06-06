# My Flask DevOps API

This project contains a simple Flask API for managing users. It performs CRUD operations (Create, Read, Update, Delete) using a JSON file as the data store.

## Project Structure

```bash
my_flask_devops_api/
├── app.py
├── requirements.txt
├── users.json
├── .gitignore
└── README.md
```

## Setup Instructions

### 1. Clone the Repository

```sh
git clone https://github.com/arezoomohammadi22/Flask_Api.git
cd Flask_Api
```
create a new user
```bash
curl -X POST http://localhost:5000/users -H "Content-Type: application/json" -d '{"id": 1, "name": "John Doe", "email": "john.doe@example.com"}'
```
Retrieve All Users (GET)
```bash
curl -X GET http://localhost:5000/users
```
Update a Specific User (PUT)
```bash
curl -X PUT http://localhost:5000/users/1 -H "Content-Type: application/json" -d '{"name": "Jane Doe", "email": "jane.doe@example.com"}'
```
Delete a Specific User (DELETE)
```bash
curl -X DELETE http://localhost:5000/users/1
```

