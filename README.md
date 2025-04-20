# E-Commerce Search and Cart Functionality Testing

This project focuses on testing the **search** and **cart functionality** of an e-commerce platform. It includes test cases, test execution results, defect logs, and API testing using Postman. The project is divided into **4 parts**:

1. **Questions and Answers**: Expected behavior and requirements for the search functionality.
2. **Test Cases**: Detailed test cases for search and cart functionality.
3. **Test Report**: Results of test execution, including defect logs and analysis.
4. **Postman Collection**: API testing for search and cart functionality.

---

## Project Structure

The project is organized into the following files:

1.  **`10 Questions`**:
   - Contains questions and answers related to the expected behavior of the search functionality.
   - Covers topics like handling valid/invalid keywords, search results, response time, and special characters.
    
2. **`Test_case_final.xlsx`**:
   - Contains detailed test cases for the search and cart functionality.
   - Columns include Test Case ID, Test Case Description, Priority, Prerequisites, Test Steps, Expected Result, Actual Result, Status, and Notes.

3. **`Test_report.xlsx`**:
   - Contains the results of test execution, including defect logs and analysis.
   - Columns include Test Case ID, Test Case Description, Expected Result, Actual Result, Status, Severity, URL, Comment, and Screenshots.

4. **`Shopping Cart Test_postman_collection.json`**:
   - A Postman collection for API testing of the search and cart functionality.
   - Includes API requests for searching products, adding products to the cart, and viewing the cart.

---

## How to Use This Project

### 1. Questions and Answers
- Open the `10 Questions.pdf` file to understand the expected behavior of the search functionality.
- This document serves as a reference for validating the test cases and test results.
 
### 2. Test Cases
- Open the `Test_case_final.xlsx` file to view the detailed test cases.
- The test cases cover scenarios like:
  - Searching with valid and invalid keywords.
  - Displaying product details on the search results page.
  - Handling empty search fields.
  - Sorting search results.
  - Adding products to the cart and verifying the cart contents.

### 3. Test Report
- Open the `Test_report.xlsx` file to view the results of test execution.
- The report includes:
  - Passed and failed test cases.
  - Defect logs with details like steps to reproduce, expected result, actual result, severity, and priority.
  - Screenshots and links to evidence for defects.

### 4. Postman Collection
- Import the `Shopping Cart Test_postman_collection.json` file into Postman to execute the API tests.
- The collection includes:
  - A `GET` request to search for products.
  - A `POST` request to add products to the cart.
  - A `GET` request to view the cart contents.

---

## Steps to Replicate the Testing

### 1. Test Case Execution
1. Open the `Test_case_final.xlsx` file.
2. Execute each test case manually or using an automation tool.
3. Record the results in the `Test_report.xlsx` file.

### 2. API Testing with Postman
1. Import the `Shopping Cart Test_postman_collection.json` file into Postman.
2. Execute the API requests:
   - Search for a product using the `GET` request.
   - Add a product to the cart using the `POST` request.
   - View the cart contents using the `GET` request.
3. Verify the API responses against the expected results.

### 3. Defect Logging
1. For any failed test cases or API requests, log the defects in the `Test_report.xlsx` file.
2. Include details like steps to reproduce, expected result, actual result, severity, and priority.
3. Attach screenshots or logs as evidence.

---

## Defect Analysis and Recommendations

### Defects Found
1. **API-001**: API request to add product to cart returned a 500 error.
   - **Severity**: High
   - **Priority**: High
   - **Steps to Reproduce**: Send a `POST` request to add a product to the cart.
   - **Expected Result**: Product should be added to the cart.
   - **Actual Result**: 500 Internal Server Error.

2. **UI-001**: UI did not display the correct product image in the cart.
   - **Severity**: Medium
   - **Priority**: Medium
   - **Steps to Reproduce**: Add a product to the cart and navigate to the cart page.
   - **Expected Result**: Correct product image displayed.
   - **Actual Result**: Placeholder image displayed.

### Recommendations
1. Fix the API endpoint to handle the add to cart request correctly.
2. Ensure the UI displays the correct product images in the cart.
3. Conduct regression testing after fixes are implemented.
