KunochDigiSolvedTask
Completed KunochDigi Assessment 

1. Test Cases for a Registration Form - Includes `name`, `email`, and `password` fields.

 Table of Contents
- [Project Structure](project-structure)
- [Requirements](requirements)
- [Setup Instructions](setup-instructions)
- [Execution Instructions](execution-instructions)
- [Testing Instructions](testing-instructions)


Project Structure

- testCaseAssessment (Manual)-cases.md - Contains the test cases for registration form.
- Regression Test Approach for Code Updates.md - Describes the approach to regression testing on the checkout feature.
- src/test/java/RegistrationFormTest.java - Automated Selenium test script for testing the registration form fields.
- README.md - Instructions to set up, execute, and test the solutions.

Requirements

To run and test these solutions, the following must be installed:

- Java JDK (version 11 or above)
- Maven (for dependency management)
- ChromeDriver** (compatible with the version of Chrome installed)
- IntelliJ IDEA (or any other preferred Java IDE)
- Excel to view the manually designed test cases

Setup Instructions

1. Clone the Repository
   ```bash
   cd repo-name
  

2. Install Dependencies
   - This project uses Maven for dependency management. Ensure Maven is installed, then run:
     ```bash
     mvn clean install
     ```
   - This will download and set up the necessary dependencies, including Selenium WebDriver.

3. Setup ChromeDriver
   - Download the ChromeDriver that matches your Chrome browser version from [ChromeDriver downloads](https://sites.google.com/chromium.org/driver/).
   - Update the path in `src/test/java/RegistrationFormTest.java`:
     ```java
     System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");
     ```

Execution Instructions

1. Run Automated Tests
   - To execute the automated Selenium tests for the registration form, run:
     ```bash
     mvn test
     ```

2. View Test Output
   - Test results will be displayed in the console or can be viewed in your IDE’s test output window.
     

Testing Instructions

1. Test Cases for the Registration Form
   - Test cases are documented in `test-cases.md`.
   - Open `test-cases.md` to review each test case, including the fields for:
     - Name
     - Email
     - Password
   - The document contains detailed scenarios with expected results and steps for manual testing.
   - 

2.  Typical Regression Test approach I employ on checkout feature after a code update

I usually analyze the Code Change to Identify impacted areas, such as pricing, payment, and order confirmation.
I focus on critical checkout steps like product selection, discounts, payment, and confirmation.
I seldomly use existing test cases where applicable and create new ones for modified workflows.
I automate repetitive, high-traffic scenarios while manually testing edge cases.
I perform End-to-End Testing by verifying full checkout flow from cart to payment confirmation to ensure seamless user experience.
I test across various browsers and devices for consistency.
I Implement monitoring to quickly address any live issues in production environment
NB: This approach ensures a thorough, efficient regression test, prioritizing the checkout's critical paths and user experience.


Additional Notes

- Test Environment: Ensure the browser and ChromeDriver versions are compatible. Incompatibility may lead to test failures.
- Customizing the Test: You can adjust the test data for registration fields directly in `RegistrationFormTest.java` if needed.

For any issues or questions, please contact the repository maintainer.


This `README.md` provides a structured guide to understanding and executing the solutions to the QA assessments effectively.
