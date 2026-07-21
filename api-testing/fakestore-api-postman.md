# REST API Testing – Fake Store API

## Project Overview

This project presents manual REST API testing performed using Postman and the public Fake Store API.

The goal of the project was to test basic product-related endpoints, verify HTTP response status codes, validate JSON response structures and observe API behaviour when incomplete data is submitted.

---

## Tools

- Postman
- REST API
- JSON
- HTTP methods: GET, POST

---

## Tested Endpoints

### GET /products

The endpoint was tested to verify that the API correctly returns a list of available products.

The following elements were verified:

- HTTP status code
- JSON response structure
- Presence of expected product fields
- Product data returned by the API

Expected product fields:

- `id`
- `title`
- `price`
- `category`
- `description`
- `image`

---

### POST /products

The endpoint was tested by sending a request containing data for a new product.

The following elements were verified:

- Request body format
- HTTP response status
- Response body
- Generation of a product ID
- Data returned after submitting the request

### Example Request Body

```json
{
  "title": "Stół kuchenny",
  "price": 99.99,
  "description": "Duży stół drewniany",
  "category": "kitchen",
  "image": "https://example.com/stol.jpg"
}
```



| ID     | Endpoint    | Method | Test Scenario                               | Expected Result                              | Status |
| ------ | ----------- | ------ | ------------------------------------------- | -------------------------------------------- | ------ |
| API-01 | `/products` | GET    | Retrieve the list of products               | Status 200 OK and product list returned      | PASS   |
| API-02 | `/products` | GET    | Verify product response structure           | Products contain expected fields             | PASS   |
| API-03 | `/products` | POST   | Create a product using valid data           | Product data is returned                     | PASS   |
| API-04 | `/products` | POST   | Verify response after creating a product    | Status 201 Created and generated ID returned | PASS   |
| API-05 | `/products` | POST   | Send a request with incomplete product data | API should reject invalid or incomplete data | FAIL   |




Negative Testing

A POST request was sent with incomplete product data to verify how the API handles invalid input.

The API did not provide the expected validation behaviour for incomplete data.

This test was marked as FAIL because the API accepted or processed data that should normally be validated before creating a resource.




Test Results

The tested GET and POST endpoints correctly handled standard requests.

The GET request returned product data with the expected JSON structure, while the POST request returned the submitted product data together with a generated ID.

The negative test identified insufficient validation when incomplete product data was submitted.




Skills Demonstrated
REST API testing
Postman
GET and POST requests
HTTP status code verification
JSON response validation
Positive and negative testing
API test case design
Test result documentation
