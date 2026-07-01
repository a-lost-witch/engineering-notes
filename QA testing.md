# 1. What is QA Testing?
QA (Quality Assurance) testing is the process of checking whether a software product meets required standards and is free of defects before release.

# 2. What is the difference between QA and QC?
- QA (Quality Assurance): Focuses on preventing defects (process-oriented)
- QC (Quality Control): Focuses on finding defects after they occur, before delivering to client (product-oriented testing)

# 3. What is a bug?
A bug is an error or flaw in software that causes incorrect or unexpected results.

# 4. What is SDLC?
SDLC (Software Development Life Cycle) is the process used to design, develop, test, and deploy software.

### Stages:
Requirement → Design → Development → Testing → Deployment → Maintenance

# 5. What is STLC?
STLC (Software Testing Life Cycle) defines the testing process.

Stages:
Requirement Analysis → Test Planning → Test Case Design → Execution → Defect Reporting → Closure

# 6. What is a test case?
A test case is a set of conditions used to check whether a feature works correctly.

Example:

Input: Login credentials
Expected output: User should log in successfully

# 7. What is a test plan?
A document that defines testing scope, strategy, resources, and schedule.

# 8. Difference between verification and validation?
- Verification: “Are we building the product right?”
- Validation: “Are we building the right product?”

# 9. What are levels of testing?
## a) Unit Testing

- What it is: Testing individual components or modules of code.

- Who does it: Developers

- Goal: Ensure each function works correctly in isolation.

- Example: Testing a login function that validates username/password.

---

## b) Integration Testing

- What it is: Testing interaction between multiple modules.

- Who does it: Developers / Testers

- Goal: Ensure combined modules work properly together.

- Example: Login module working with database authentication system.

---
  
## c) System Testing

- What it is: Testing the complete system as a whole.

- Who does it: QA testers

- Goal: Validate full application against requirements.

- Example: Testing entire e-commerce website (login → product → payment → logout).

---

 ## d) Acceptance Testing (UAT)

 - What it is: User Acceptance Testing done by client or end users.
 - Who does it: Customers / Business users
 - Goal: Check if software is ready for real-world use
 - Example: Client verifies if billing system matches business needs

# 10. What is regression testing?
Testing done to ensure new code changes do not affect existing functionality.

# 11. What is smoke testing?
Basic testing to check if the build is stable enough for further testing. It is the Initial verification of critical features before detailed testing. E.g. For a login app, Can user open the app? Can user log out? If smoke testing fails Build is rejected and Sent back to developers.

# 12. What is sanity testing?
Quick testing to verify specific functionality after small changes or bug fixes.

# 13. What is a defect life cycle?
New → Assigned → Open → Fixed → Retest → Verified → Closed (or Rejected/Deferred)

# 14. What is a test strategy?
High-level document describing testing approach for the whole project.

# 15. Differentiate between Manual and automation testing.
Manual: Human executes test cases
Automation: Tools/scripts execute test cases (faster, reusable)

# 16. What is API?
An API (Application Programming Interface) is a set of rules and protocols that allows different software applications to communicate with each other. It takes a request from one system, sends it to another system, and returns the response.

E.g. When weather app is opened, it uses API to Request data from a server and displays the response.

# 17. What is the working principle of API?

APIs operate through a request response cycle between a client and a server

Request: The client sends a request to an API endpoint (URI).
Processing: The API forwards the request to the server.
Response: The server processes and sends back the requested data.
Delivery: The API returns the server’s response to the client.
This communication happens over the HTTP/HTTPS protocol, with additional security via headers, tokens, or cookies.

# 17. What is API testing?
API Testing is a type of software testing where Application Programming Interfaces (APIs) are directly checked to see if they are working correctly, securely, and efficiently. Instead of testing the UI (buttons/screens), communication between systems is tested.

E.g. When logged into an app, UI sends username/password to API → API checks database → API returns success/failure response

# 18. What is checked in API testing?
- Correct response is returned
- Data is accurate
- API handles errors properly
- Response time is good
- Security (authorization, authentication)

# 19. What are some Common API methods tested?
- GET → fetch data
- POST → send data
- PUT → update data
- DELETE → remove data

# 20. What are some popular SDLC methods?
| Model     | Description                         |
| --------- | ----------------------------------- |
| Waterfall | Sequential approach                 |
| Agile     | Iterative and flexible              |
| Spiral    | Risk-focused model                  |
| V-Model   | Testing at every stage              |
| DevOps    | Continuous integration & deployment |

# 21. What is Jira?
Jira is a project management and issue-tracking tool (like CRM) widely used in software testing, development, Agile, and DevOps teams.

### Testers use Jira to:

- Report bugs
- Track defects
- Assign issues to developers
- Monitor testing progress
- Manage test cases and sprints
- Generate reports

### Example Workflow:
- Tester finds a bug in login page
- Tester creates a Jira ticket
- Developer receives the issue
- Developer fixes the bug
- Tester retests it
- Ticket is closed

# 22. What is Selenium?
Selenium is an open-source automation testing framework used to automate web browsers.

## It is mainly used for:
- Web application testing
- Repetitive browser tasks
- UI automation
- Regression testing

## What Selenium Does
Selenium can automatically:
- Open a browser
- Click buttons
- Enter text
- Submit forms
- Verify webpage content
- Test websites

## Example:
Instead of manually testing login every time:
- Open website
- Enter username/password
- Click login
- Check dashboard

 ## Supported Browsers
Selenium works with:

- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari

## Supported Languages
Selenium scripts can be written using:
- Python
- Java
- C#
- JavaScript
- Ruby

## Example in Python:
```python
from selenium import webdriver

driver = webdriver.Chrome()

driver.get("https://example.com")

driver.find_element("id", "username").send_keys("admin")
driver.find_element("id", "password").send_keys("1234")
driver.find_element("id", "login").click()
```

### This script:
- Opens browser
- Opens website
- Enters login details
- Clicks login

## Selenium Components:
| Component          | Purpose                       |
| ------------------ | ----------------------------- |
| Selenium WebDriver | Main browser automation tool  |
| Selenium IDE       | Record/playback testing       |
| Selenium Grid      | Run tests on multiple systems |
| Selenium RC        | Older deprecated version      |

## Advantages:
- Free and open source
- Supports many browsers
- Supports many languages
- Widely used in QA testing
- Good for automation testinh

## Limitations
- Mainly for web applications
- Cannot directly test desktop apps
- Requires programming knowledge
- Dynamic webpages can be tricky

# 23. What is framework?
A framework is a pre-built structure or foundation that helps developers build software faster and in an organized way.

Instead of creating everything from scratch, a framework provides:
- Ready-made code
- Rules/structure
- Tools and libraries
- Reusable components

# 24. Example Frameworks:
## Web Development:
| Framework        | Language   |
| ---------------- | ---------- |
| Django           | Python     |
| React            | JavaScript |
| Angular          | TypeScript |
| Spring Framework | Java       |
## Testing Framework:
| Framework | Purpose            |
| --------- | ------------------ |
| Selenium  | Browser automation |
| TestNG    | Test execution     |
| PyTest    | Python testing     |

# 25. What is typescript?
TypeScript is a programming language developed by Microsoft that is built on top of JavaScript.
It adds:
- Types
- Better error checking
- Modern coding features
- Easier large-project management

## Example:
In JavaScript,
```javascript
let age = 25;
age = "hello" //allowed;
```

JavaScript allows this because it is dynamically typed. But, this can cause bugs later Because the variable age first stores a number, but later becomes a string.

Say, later in program,
```javascript
let age = 25;
age = "hello";
console.log(age + 5);
```

Instead of 30, output becomes hello5.

But TypeScript catches the mistake early, before running the code,
```ltypescript
let age: number = 25;
age = "hello"; // Error
```

This is because, JavaScript variables do not have fixed types. The variable "age" is just a container that can hold number , string , object , boolean etc.
Whereas, TypeScript adds static type checking to restrict that behavior, giving compile-time error.It either automatically infers age as number from first line or explicit type is needed to be declared.

# 26. What is CI/CD pipeline?
CI/CD pipelines are a way to automate building, testing, and deploying software so developers can release updates faster and more reliably.

### a) Continuous Integration (CI):
Developers frequently merge their code into a shared repository (like GitHub), and every change is automatically tested. Here,
- Code is pushed to GitHub
- Automated build runs
- Automated tests run (unit tests, integration tests)
- If something breaks → developer is notified immediately

### b) Continuous Delivery (CD):
After CI, the tested code is automatically prepared for release. Here,
- Code is built and tested
- Packaged and moved to staging environment
- Ready for manual approval to release

### c) Continuous Deployment:
Every successful code change is automatically deployed to production.

# 27. What is edge case?
An edge case is a situation that occurs at the extreme boundaries of valid input, operating conditions.

**Examples:**

a. Age Input Field If valid age is 1–120:
Normal cases:
25
40
80

Edge cases:
1 (minimum valid value)
120 (maximum valid value)
0 (just below minimum)
121 (just above maximum)

b. Password Length Requirement: Password must be 8–20 characters.

Edge cases:
7 characters
8 characters
20 characters
21 characters

# 28. Explain Characteristics of a Good Test Case.
A good test case is:
- Simple and clear
- Has a unique ID
- Contains defined preconditions
- Specifies test data
- Lists execution steps
- Has expected results
- Covers boundary and error conditions
- Is repeatable and maintainable

### Example:
**Feature:** Login
**Test Case:** Login with valid credentials
**Preconditions:** User account exists.
**Input:** Valid username and password.
**Steps:** Enter credentials → Click Login.
**Expected Result:** User is redirected to dashboard.
**Properties satisfied:** Correct, clear, repeatable, traceable, maintainable.
These are the properties most commonly expected in professional software testing and QA processes.

# 29. What is positive flow and negetive flow?
**Positive flow:** A positive flow (or happy path) is a test scenario where the user performs the expected actions with valid inputs, and the system behaves exactly as intended.
**Negative Flow:** Tests invalid or unexpected inputs.

**Example: Login Feature**
**Requirement:** Users can log in with a valid username and password.
**Positive flow:**
- Open login page.
- Enter valid username.
- Enter valid password.
- Click Login.
- User is successfully redirected
**Expected Result:** Login succeeds

**Negative Flow:**
Tests invalid or unexpected inputs.
**Examples:**
- Wrong password
- Invalid username
- Empty username
- Empty password
**Expected Result:** Appropriate error message is shown.

# 30 What is load testing?
Load testing is a type of **performance testing** used to evaluate how a system behaves under an expected number of users, requests, or transactions. The primary goal is to ensure that the application can handle normal anticipated traffic while maintaining acceptable performance levels.
## Example
Suppose an EV charging application is expected to support **1,000 concurrent users**.
During load testing, 1,000 virtual users are simulated, and the following metrics are monitored:
* Response time
* Throughput (requests per second)
* CPU utilization
* Memory utilization
* Error rates
* Database performance

## Common Use Cases

* 500 users logging into a website simultaneously
* 1,000 customers placing orders on an e-commerce platform
* 10,000 API requests per minute
* Multiple EV charging stations sending status updates concurrently

## Benefits of Load Testing

Load testing helps identify:

* Performance bottlenecks
* Slow response times
* Database issues
* Memory leaks
* Server capacity limitations
* Application instability under expected traffic

## Popular Load Testing Tools

* Apache JMeter
* LoadRunner
* k6
* Gatling

# 31. Stress Testing
Stress testing is a type of **performance testing** used to evaluate how a system behaves when it is subjected to workloads beyond its expected operating capacity.The primary goal is to determine the system's breaking point and assess its ability to recover after failure, i.e. Stress testing is a non-functional testing technique used to evaluate an application's stability, reliability, and recovery capability by subjecting it to workloads beyond its expected operating limits.

## Example

Suppose an EV charging application is designed to support **1,000 concurrent users**.

During stress testing, the load is gradually increased beyond the expected limit, such as:

* 2,000 concurrent users
* 5,000 concurrent users
* 10,000 concurrent users

The following metrics are monitored:

* Response time
* Error rates
* CPU utilization
* Memory utilization
* System crashes
* Recovery time after failure

## Common Use Cases

* Simulating traffic spikes during a flash sale
* Testing application behavior during peak usage periods
* Evaluating server stability under excessive load
* Identifying system bottlenecks and failure points
* Assessing recovery mechanisms after a crash

## Benefits of Stress Testing

Stress testing helps identify:

* System breaking points
* Performance bottlenecks
* Resource limitations
* Application crashes
* Data loss risks
* Recovery and failover issues

## Popular Stress Testing Tools

* Apache JMeter
* LoadRunner
* k6
* Gatling


# 32. Compare Load Testing vs Stress Testing

| Load Testing                                 | Stress Testing                           |
| -------------------------------------------- | ---------------------------------------- |
| Tests expected workload                      | Tests beyond expected workload           |
| Evaluates normal system performance          | Determines system breaking point         |
| Focuses on stability under normal conditions | Focuses on recovery and failure behavior |
| Example: 1,000 concurrent users              | Example: 10,000 concurrent users         |

# 33.What is Playright?
Playwright is an open-source browser automation and end-to-end (E2E) testing framework developed by Microsoft Playwright. It allows developers and QA engineers to automate user actions in web browsers such as Chrome, Edge, Firefox, and Safari (WebKit) using a single API.

### Example in Java:

```
const { test, expect } = require('@playwright/test');

test('Check title', async ({ page }) => {
  await page.goto('https://example.com');
  await expect(page).toHaveTitle(/Example/);
});
```

Playright:
- Supports Chromium, Firefox, and WebKit with the same test script.
- Automatically waits for elements to become clickable or visible.
- Runs tests in parallel for faster execution.
- Supports JavaScript, TypeScript, Python, Java, and .NET.
- Includes screenshots, videos, tracing, and debugging tools

# 34. What is Selenium?

# 35. Explain Selenium vs Java.
| Feature         | Playwright              | Selenium                  |
| --------------- | ----------------------- | ------------------------- |
| Setup           | Easier                  | More configuration        |
| Speed           | Faster                  | Usually slower            |
| Auto-wait       | Built-in                | Manual waits often needed |
| Browser Support | Chrome, Firefox, Safari | Almost all browsers       |
| Modern Web Apps | Excellent               | Good                      |

# 36. Explain Playwright Locator.
A locator in Playwright is an object used to find, interact with, and verify web elements on a page. Instead of directly searching for an element once, Playwright locators continuously re-evaluate the element and automatically wait for it to become available, visible, and actionable.
For example: await page.locator('#login-btn').click();
Here, Playwright finds the element with ID login-btn and waits for it to be ready before clicking.


# 37. What is npm?
npm stands for Node Package Manager. It's the tool that comes with Node.js and is used to:
- Install packages/libraries
- Manage project dependencies
- Run scripts and commands

### Common npm Commands
Initialize a project :
```
npm init -y
```
Creates: package.json

# 38. How does Playwright work?
Playwright works by controlling a real browser through its automation APIs. A test script launches a browser, creates an isolated browser context, opens a page, and performs actions such as clicking buttons or entering text. Before interacting with an element, Playwright automatically waits until it is visible, enabled, and ready, making tests more reliable. After each action, it verifies the expected result using assertions. At the end of execution, Playwright can generate reports, screenshots, videos, and traces to help analyze any failures.

# 39. What is Playwright inspector?
The Playwright Inspector is a native, graphical user interface (GUI) tool provided by Microsoft's Playwright framework designed to help developers and QA engineers author, record, and debug automated web tests line by line. It operates alongside a live browser window to display the real-time execution flow of your automation scripts

# 40. What is asynchronous function using Promises?
An asynchronous function using Promises is a JavaScript function that performs a non-blocking operation (like fetching data, reading files, or waiting for a timer) and immediately returns a Promise object instead of the final value. The returned Promise acts as a temporary placeholder representing the future completion or failure of that background task.
