# Backend Graduate Trainee (GT) Skills Assessment

## Overview

Congratulations on progressing to the skills assessment stage.

This assessment is designed to evaluate your **problem-solving ability, backend fundamentals, and coding practices**. The goal is not only to test your ability to write code, but also to understand how you **think through backend problems and design simple APIs**.

The assessment consists of three sections:

1. API Reasoning and Validation  
2. Backend API Implementation  
3. Basic System Thinking  

---

# General Instructions

1. Create a new Git repository for your submission.
2. Complete the tasks described below.
3. Push your solution to GitHub (or any Git platform).
4. Submit the repository link before the deadline.

### Expected Time

The assessment is designed to take approximately **3 to 5 hours**.

### Deadline

**Friday, 13th March 2026**

---

# Allowed Tools

You may use:

- Documentation
- StackOverflow
- AI tools (ChatGPT, Copilot, etc.)

However, you must clearly explain your thinking process in the **EXPLANATION.md** file.

Submissions without explanations may receive a lower score.

---

# Submission Structure

Your repository should follow this structure:

```
backend-gt-assessment/

README.md
EXPLANATION.md

task-1-api-reasoning.md
task-2-api-implementation/
task-3-system-thinking.md
```

---

# Task 1: API Reasoning and Validation

## Objective

This task evaluates your understanding of **API validation, backend logic, and error handling**.

You are given the following API endpoint.

### Create Order

```
POST /orders
```

Example request body:

```json
{
  "userId": 25,
  "items": [
    {
      "productId": 5,
      "quantity": 2
    }
  ]
}
```

---

## Questions

In the file:

```
task-1-api-reasoning.md
```

Answer the following questions.

### 1. Validation

What validations should be performed before creating an order?

Consider both **data validation and business logic validation**.

---

### 2. Possible Errors

List at least **5 possible errors** that could occur when processing this request.

Examples may include:

- Invalid user
- Product not found
- Invalid quantity
- Empty order items
- Database failure

---

### 3. HTTP Responses

What HTTP status codes should be returned for the following scenarios?

- Successful order creation  
- Invalid request body  
- Product not found  
- Server error  

Explain your reasoning.

---

# Task 2: Backend API Implementation

## Objective

Build a simple **Task Management API**.

This task evaluates your ability to:

- Design APIs
- Structure backend code
- Handle errors
- Implement basic backend logic

---

## Requirements

Create a backend service that allows users to manage tasks.

Each task should contain:

- id
- title
- priority
- completed
- createdAt

---

## Required Endpoints

### 1. Create Task

```
POST /tasks
```

Example request:

```json
{
  "title": "Complete assessment",
  "priority": "high"
}
```

Example response:

```json
{
  "id": 1,
  "title": "Complete assessment",
  "priority": "high",
  "completed": false,
  "createdAt": "2026-03-09T12:00:00Z"
}
```

---

### 2. Get All Tasks

```
GET /tasks
```

Return all tasks.

---

### 3. Mark Task as Completed

```
PATCH /tasks/:id/complete
```

This endpoint should update the task status to completed.

---

### 4. Delete Task

```
DELETE /tasks/:id
```

Remove the task.

---

## Implementation Guidelines

You may use any of the following:

- Node.js
- Express
- NestJS
- Fastify

You may use:

- In-memory storage
- Or a simple database

Your implementation should include:

- Input validation
- Proper HTTP status codes
- Clean code structure
- Basic error handling

---

# Task 3: Basic System Thinking

## Objective

This section evaluates your ability to think about **backend systems as they grow**.

In the file:

```
task-3-system-thinking.md
```

Answer the following questions.

---

### 1. Scaling

If this task API starts receiving **thousands of requests per minute**, what problems might occur?

Mention at least **3 possible issues**.

---

### 2. Performance Improvements

What techniques would you use to improve performance?

Examples may include:

- Caching
- Database indexing
- Load balancing

Explain briefly.

---

### 3. Production Monitoring

What metrics would you monitor in production to ensure the API is healthy?

Examples:

- Response time
- Error rate
- CPU or memory usage
- Database performance

---

# Explanation File

Create a file called:

```
EXPLANATION.md
```

Explain the following:

1. How you approached the implementation
2. Why you structured the code the way you did
3. Assumptions you made
4. What you would improve if given more time
5. Any tools or AI assistance used

---

# README File

Your repository must include a **README.md** with:

- Setup instructions
- How to run the project
- Example API requests

---

# Evaluation Criteria

Your submission will be evaluated based on the following:

| Category | Weight |
|--------|--------|
| Code clarity and structure | 30% |
| Problem solving and reasoning | 25% |
| API design and validation | 20% |
| Documentation and explanations | 15% |
| Error handling | 10% |

---

# What We Are Looking For

We are not expecting perfect production systems.

Strong submissions will demonstrate:

- Clear thinking
- Clean and readable code
- Reasonable API design
- Good explanations
- Thoughtful handling of edge cases

Good luck.
