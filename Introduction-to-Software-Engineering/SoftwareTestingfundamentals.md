# Software Testing Categories

A breakdown of key testing types: Functional, Non-Functional, Regression, and more.

---

## 🧪 Functional Testing
Validates that the system works as per requirements.

| Type                | Description                          | Examples                          | Tools              |
|---------------------|--------------------------------------|-----------------------------------|--------------------|
| **Unit Testing**    | Tests individual components/modules. | Function logic, classes.          | JUnit, NUnit       |
| **Integration**     | Checks interaction between modules.  | API calls, DB connections.        | Postman, TestNG    |
| **System Testing**  | Tests the entire system end-to-end.  | User workflows, full scenarios.   | Selenium, Cypress  |
| **Acceptance (UAT)**| Validates by end-users/clients.      | Business scenarios, sign-off.     | JIRA, FitNesse     |

---

## ⚡ Non-Functional Testing
Evaluates system performance, security, etc.

| Type                | Description                          | Examples                          | Tools              |
|---------------------|--------------------------------------|-----------------------------------|--------------------|
| **Performance**     | Tests speed, scalability.            | Load (1000 users), stress tests.  | JMeter, LoadRunner |
| **Security**        | Identifies vulnerabilities.          | SQL injection, XSS attacks.       | OWASP ZAP, Burp    |
| **Usability**       | Checks user-friendliness.            | UI/UX, navigation flow.           | Hotjar, UserTesting|
| **Compatibility**   | Ensures cross-platform support.      | Browser/device testing.           | BrowserStack       |

---

## 🔄 Regression Testing
Ensures new changes don’t break existing functionality.

| Type                | Description                          | When to Use                       | Tools              |
|---------------------|--------------------------------------|-----------------------------------|--------------------|
| **Full Regression** | Re-tests entire application.         | Major releases.                   | Selenium, QTP      |
| **Partial**         | Tests only impacted modules.         | Small bug fixes.                  | TestNG, Robot      |
| **Automated**       | Script-based repetitive tests.       | CI/CD pipelines.                  | Jenkins, GitLab CI |

---

## 🔗 Integration Testing Types
Focuses on module interactions.

| Type                | Description                          | Approach                          |
|---------------------|--------------------------------------|-----------------------------------|
| **Big Bang**        | Integrates all modules at once.      | High risk, hard to debug.         |
| **Incremental**     | Integrates step-by-step (Top-Down/Bottom-Up). | Easier isolation. |
| **Sandwich**        | Hybrid (Top + Bottom).               | Balanced approach.                |

---

## 🖥️ System vs Acceptance Testing

| Criteria          | System Testing                       | Acceptance Testing (UAT)          |
|-------------------|--------------------------------------|-----------------------------------|
| **Done By**       | QA Team                              | Clients/End-users                 |
| **Environment**   | Staging (Near-production)            | Production-like                   |
| **Goal**          | "Does the system meet specs?"        | "Is this usable for business?"    |

---

## 🛠️ Sample Test Scenario (E-Commerce)
```gherkin
Scenario: User checkout process
  Given I add items to cart
  When I proceed to checkout
  Then I should see payment options
  And my order total must match cart
