# Dmoney API Testing Project

This repository contains API testing resources for the **Dmoney** application using **Postman**. The project is designed to validate authentication, user management,
and transaction-related APIs with proper assertions and environment handling.

## Files Included

### `Dmoney_API_Testing.postman_collection.json`

**Postman Collection** containing all API test cases.

**Key Coverage:**

* User Authentication (Login)
* User List & Search APIs
* User CRUD Operations (Create, Update – Full & Partial)
* Transaction Information APIs
* Transaction Operations (Deposit, Withdraw, Send Money)

**Features:**

* Automated assertions for status codes and response messages
* Token extraction and reuse using environment variables
* Dynamic data handling (random phone numbers, emails, etc.)

### `ENV_Dmoney.postman_environment.json`

**Postman Environment** file used to manage reusable variables.

**Important Variables:**

* `base_url` – API base URL
* `token` – Authentication token
* `X-AUTH-SECRET-KEY` – Secret key for secured APIs
* `userId`, `userPhone`, `userEmail`
* Transaction-related variables (deposit, withdraw, send money)
* Balance validation variables (before & after transaction)

This environment ensures smooth API chaining and validation.

---

### `Dmoney_API_Testing-2025-12-23-12-49-02-123-0.html`

**Postman HTML Report** generated after executing the collection.

**Purpose:**

* View execution summary
* Analyze passed/failed test cases
* Share test execution results with stakeholders

---

## How to Use This Project

1. Import the **Postman Collection** and **Environment** into Postman
2. Set the correct value for `base_url`
3. Run the Login API to generate token automatically
4. Execute other APIs individually or using **Collection Runner**
5. (Optional) Run using Newman and generate HTML reports


## Tools & Technologies

* Postman
* Newman
* JavaScript (Postman Tests)
* REST API
