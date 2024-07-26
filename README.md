# test-API-Github
GitHub API Testing
Project Overview
This project involves testing GitHub's API endpoints using Postman. The objective is to ensure the accuracy and functionality of the API responses. The testing covers the following functionalities:

Retrieving All Repositories: Ensuring the API correctly fetches all repositories of a user on GitHub.
Creating a New Repository: Testing the API's capability to create a new repository.
Renaming a Repository: Validating that the API can successfully rename a repository.
Deleting a Repository: Ensuring the API correctly deletes a repository.
Testing Environment
PC: Intel Core i5-1035G1, RAM 8GB
Operating System: Windows 11, Version 22H2
Browser: Chrome - Version 124.0.6367.201
IDE: Visual Studio Code 2022
Framework: .NET Framework 4.7.2
Libraries:
Selenium.WebDriver – Version 4.20.0
Selenium.WebDriver.ChromeDriver – Version 124.0.6367.6000
Setup Instructions
Postman Setup:

Log in to Postman.
Create a new workspace.
Create a new collection.
GitHub Token Creation:

Log in to GitHub and generate a personal access token.
Follow these steps to configure and generate the token:
Navigate to Settings -> Developer Settings -> Personal Access Tokens.
Create a new token and configure the necessary permissions.
Save the token for use in API requests.
Environment Variables:

Configure environment variables in Postman as needed for the API tests.
Test Cases
1. Retrieve All Repositories
API Endpoint: https://api.github.com/user/repos
Test Cases:
TC1.1: Verify the response status code is 200.
TC1.2: Check if the response format is JSON.
TC1.3: Ensure the number of returned repositories is 17.
2. Create a New Repository
API Endpoint: https://api.github.com/user/repos
Test Cases:
TC2.1: Verify the response status code is 201.
TC2.2: Check if the response format is JSON.
3. Rename a Repository
API Endpoint: https://api.github.com/repos/{owner}/{repo}
Test Cases:
TC3.1: Verify the response status code is 200.
TC3.2: Check if the response format is JSON.
TC3.3: Ensure the repository name has been updated to 'TestSuaName'.
4. Delete a Repository
API Endpoint: https://api.github.com/repos/{owner}/{repo}
Test Cases:
TC4.1: Verify the response status code is 204.
TC4.2: Check if the response data is empty.
Results
The test results for each API functionality are illustrated in the screenshots provided in the report. The results confirm the successful execution of all test cases.

Screenshots:
Retrieve All Repositories
Create a New Repository
Rename a Repository
Delete a Repository
Conclusion
The API testing for GitHub has been successfully conducted using Postman. The tests ensured that all functionalities—retrieving, creating, renaming, and deleting repositories—are working as expected.

For more details on the test cases and results, please refer to the provided screenshots and documentation.
