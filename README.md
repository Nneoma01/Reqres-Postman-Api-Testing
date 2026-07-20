# Reqres API Testing with Postman

This repository contains a comprehensive Postman collection created to practice and demonstrate REST API testing using the Reqres API.

The project covers positive and negative test scenarios, response validation, status code verification, and Postman scripting using JavaScript.


## Project Objective

The goal of this project is to strengthen API testing skills by creating automated validations for common REST API endpoints while following good testing practices.

This collection demonstrates:

- API request creation
- Response validation
- Status code verification
- JSON body validation
- Response time assertions
- Environment variables
- Negative testing
- Test scripting using the Postman Sandbox


## API Used

**Reqres API**

Reqres is a free REST API designed for learning and testing API requests.

Base URL:

```
https://reqres.in
```


## Test Coverage

### Response Code Tests

- Get Users
- Get Single User
- Create User
- Login
- Register User

### Response Body Validation

- Validate response structure
- Validate returned JSON properties
- Validate specific field values

### User Actions

- Create User
- Login
- Register User

### Login Test Scenarios

- Valid email and valid password
- Invalid email and valid password
- Valid email and invalid password
- Missing password
- Missing email


## Assertions Used

The collection contains validations for:

- Status codes
- Response body
- JSON properties
- Response time
- Error messages
- Data types

Example:

```javascript
pm.test("Status code is 200", () => {
    pm.response.to.have.status(200);
});

pm.test("Response time is under 1000ms", () => {
    pm.expect(pm.response.responseTime).to.be.below(1000);
});
```

## Technologies Used

- Postman
- JavaScript
- Postman Test Scripts
- REST API


## Skills Demonstrated

- API Testing
- Functional Testing
- Negative Testing
- Response Validation
- REST API Fundamentals
- Test Automation using Postman
- Test Case Design


## Repository Contents

```
Reqres-Postman-Api-Testing/
│
├── README.md
└── Reqres API Testing.postman_collection.json
```


## Importing the Collection

1. Clone this repository.
2. Open Postman.
3. Click **Import**.
4. Select the collection JSON file.
5. Run the requests individually or using the Collection Runner.


## Author

**Favour Okagbue**

Frontend Developer transitioning into QA Engineering with a focus on API testing, automation, and software quality assurance.
