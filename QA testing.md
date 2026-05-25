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
Basic testing to check if the build is stable enough for further testing.

# 12. What is sanity testing?
Quick testing to verify specific functionality after small changes or bug fixes.

# 13. What is a defect life cycle?
New → Assigned → Open → Fixed → Retest → Verified → Closed (or Rejected/Deferred)

# 14. What is a test strategy?
High-level document describing testing approach for the whole project.

# 15. Differentiate between Manual and automation testing.
Manual: Human executes test cases
Automation: Tools/scripts execute test cases (faster, reusable)

# 16. What is API testing?
API Testing is a type of software testing where Application Programming Interfaces (APIs) are directly checked to see if they are working correctly, securely, and efficiently


