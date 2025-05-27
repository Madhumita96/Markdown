#  How to Use Postman for API Testing

- [How to Use Postman for API Testing](#how-to-use-postman-for-api-testing)
  - [1. Introduction](#1-introduction)
  - [2. Installing Postman](#2-installing-postman)
  - [3. Understanding the Postman Interface](#3-understanding-the-postman-interface)
  - [4. Creating a Request](#4-creating-a-request)
  - [5. Using Parameters, Headers, and Body](#5-using-parameters-headers-and-body)
  - [6. Sending the Request and Viewing the Response](#6-sending-the-request-and-viewing-the-response)
  - [7. Saving and Organizing Requests in Collections](#7-saving-and-organizing-requests-in-collections)
  - [8. Writing Tests in Postman](#8-writing-tests-in-postman)
  - [9. Environment Variables and Global Variables](#9-environment-variables-and-global-variables)
  - [10. Using Pre-request Scripts](#10-using-pre-request-scripts)
  - [11. Automating Tests with Collection Runner](#11-automating-tests-with-collection-runner)
  - [12. Exporting and Importing Collections](#12-exporting-and-importing-collections)
- [13. Best Practices](#13-best-practices)
  - [14. Troubleshooting Common Issues](#14-troubleshooting-common-issues)
  - [15. Conclusion](#15-conclusion)



## 1. Introduction
Postman is a popular API client that makes it easy to create, share, test, and document APIs. This manual is intended for beginners and intermediate users who want to understand the complete flow of API testing using Postman.

## 2. Installing Postman
- Go to https://www.postman.com/downloads/
- Choose your platform (Windows, macOS, or Linux)
- Download and install the Postman desktop application
- Optionally, sign up or log in to sync your workspace with the cloud

## 3. Understanding the Postman Interface
- Sidebar: Contains tabs like Collections, APIs, Environments
- Request Builder: Where you enter the URL, HTTP method, headers, body, and so on.
- Response Viewer: Displays the API response including status code, response time, headers, and body

## 4. Creating a Request
- Open Postman
- Select the HTTP method (GET, POST, PUT, DELETE)
- com/users)
- Click "Send" to make the request

## 5. Using Parameters, Headers, and Body
•	Params: For query parameters (example, ?id=123)
•	Headers: Add key-value pairs for authentication or content type (e.g., Content-Type: application/json)
•	Body: For POST or PUT requests, use JSON or form-data
Example JSON body:
```
{
  "name": "John Doe",
  "email": "john@example.com"
}
```
## 6. Sending the Request and Viewing the Response
- Click Send
- Postman will display:
  - Status Code (e.g., 200 OK, 404 Not Found)
  - Response Time
  - Response Body in various formats (Pretty, Raw, Preview)

## 7. Saving and Organizing Requests in Collections

- Click Save > Name your request and select a Collection or create a new one.
- Collections allow you to organize requests by project or API.

## 8. Writing Tests in Postman
•	Go to the Tests tab
•	Write JavaScript snippets to test response status, values, headers
Example:
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```
## 9. Environment Variables and Global Variables
•	Define variables like `base_url`, auth_token
•	Click the Environment dropdown > Manage Environments
•	Use variables with `{{variable_name}}` syntax
Example:
```
{{base_url}}/users
```
## 10. Using Pre-request Scripts
•	Located in the Pre-request Script tab
•	Use JavaScript to set headers, tokens, or timestamps dynamically
Example:
```
pm.environment.set("current_time", new Date().toISOString());
```
## 11. Automating Tests with Collection Runner
- Open the Collection > Click **Run**
- Select environment, set iterations, and run all requests in sequence
- View test results, logs, and request/response history

## 12. Exporting and Importing Collections
- Click on a collection > More options (three dots) > **Export**
- To import, click **Import** > Choose file or paste link

# 13. Best Practices
- Use collections and folders to organize tests
- Use environments for different stages (dev, QA, prod)
- Version control collections using Git or cloud sync
- Reuse variables to avoid hard-coding
- 
## 14. Troubleshooting Common Issues
- **Timeouts:** Check your internet or API server
- **Invalid JSON:** Validate your request body
- **401 Unauthorized:** Check API keys or tokens

## 15. Conclusion
Postman is a powerful tool for API testing and automation. By mastering its features, you can improve your testing workflow, reduce errors, and ensure that your APIs are reliable and well-documented.

