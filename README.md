# ☁️ Serverless To-Do API

A fully serverless CRUD (Create, Read, Update, Delete) API for managing to-do items using AWS Lambda, API Gateway, and DynamoDB. Built in Python and deployed via the AWS console.

---

## 🔧 Technologies Used

- **AWS Lambda** – Serverless backend functions
- **Amazon API Gateway** – Public HTTP endpoints for the API
- **Amazon DynamoDB** – NoSQL database for storing tasks
- **Python** – Lambda function runtime
- **AWS CLI + curl** – Used for local testing and deployment

---

## Features

- Add a new to-do task
- View all existing tasks
- Update a task *(coming soon)*
- Delete a task *(coming soon)*

---

## API Endpoints

### `POST /tasks` — Add a New Task
Creates a new task with a unique `id`.

#### Example `curl`:
```bash
curl -X POST https://3ce1acm5mc.execute-api.us-east-2.amazonaws.com/tasks \
-H "Content-Type: application/json" \
-d "{\"task\": \"Finish my cloud resume\"}"
