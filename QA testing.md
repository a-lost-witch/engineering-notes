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

