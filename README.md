# API Test Automation with Postman, Newman, and CI/CD Implementation with GitHub Actions

This project demonstrates an automated workflow for API testing using **Postman**, **Newman**, and **GitHub Actions**. It includes a fully automated CI/CD pipeline that runs API tests on every push to the `main` branch and publishes a detailed HTML test report to **GitHub Pages**.

## Features
- Automated API testing with Postman collections.
- CI/CD integration with GitHub Actions.
- Test report generation using Newman and HTML Extra Reporter.
- Test report publication via GitHub Pages.

## Workflow Overview
1. **Postman Collection**: Contains API test cases to validate the functionality of the APIs.
2. **Newman Runner**: Executes the Postman collection and generates a test report.
3. **GitHub Actions CI**:
   - Triggers on every push to the `main` branch.
   - Runs the tests and generates the HTML report.
4. **GitHub Pages Deployment**:
   - The generated report is deployed to the `gh-pages` branch.
   - The report is accessible online via GitHub Pages.

## Prerequisites
- A GitHub repository with a Postman collection (`collection.json`) and environment file (`environment.json`).
- Node.js and npm installed locally (for testing locally).
- Newman and Newman HTML Extra Reporter installed globally.

## Setup and Usage

### 1. **Clone the Repository**
```bash
git clone https://github.com/<your-username>/bookstore-api-test-postman.git
cd bookstore-api-test-postman
```
### 2. **Install dependencies**
```bash
npm install
```
### 3. **Run Tests Locally**
```bash
npm run test
```
### 4. **View Test Report Locally**
Open the generated ```index.html``` in a browser to view the detailed test results.

## How it works

- **Automated Testing**: Every push to the main branch triggers the GitHub Actions workflow to run the API tests.
- **Report Generation**: Newman executes the Postman collection and generates a test report using the HTML Extra Reporter.
- **Report Deployment**: The workflow deploys the report to the gh-pages branch, making it accessible via GitHub Pages.

## Future Enhancements
- Add support for multiple environments (e.g., staging, production).
- Integrate notifications (e.g., Slack, email) for test failures.
- Implement performance testing for API endpoints.
- Generate aggregated reports for multiple test runs.

## License
This project is licensed under the MIT License.

## Author
**M Mohaiminul Islam**  
GitHub: [https://www.github.com/mohaiminul-shovon](https://github.com/mohaiminul-shovon) 
