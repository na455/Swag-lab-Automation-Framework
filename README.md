Swag Labs Automation Framework — Selenium POM

📌 Overview

This repository contains a professional UI automation framework built using Selenium WebDriver, Java, TestNG, and the Page Object Model (POM) design pattern.
The framework automates core user scenarios on the Swag Labs demo application, focusing on maintainability, scalability, and clean test architecture.

The current implementation covers:

- User Login flow
- Add product to cart flow
- Basic navigation validation
- Reusable page objects and test structure

This project is designed to reflect real-world automation best practices and can be easily extended with additional test cases and features.

---

🧱 Framework Design

The project follows the Page Object Model to separate:

- Page locators and actions
- Test logic
- Driver setup and configuration

This improves:

- Code reusability
- Test readability
- Maintenance efficiency
- Scalability for future test coverage

---

🗂 Project Structure

src
 ├── main/java
 │    └── pages
 │         ├── LoginPage.java
 │         └── ProductsPage.java
 │
 └── test/java
      ├── base
      │     └── BaseTest.java
      │
      └── tests
            └── SwagTests.java

---

⚙️ Tech Stack

- Java
- Selenium WebDriver 4
- TestNG
- Maven
- Chrome Browser
- Page Object Model (POM)

---

🚀 Automated Scenarios

✅ Login Test

- Enter valid username and password
- Submit login form
- Verify successful navigation to inventory page

✅ Add To Cart Test

- Add product to cart
- Open cart page
- Validate navigation to cart screen

---

▶️ How To Run

1️⃣ Clone the repository

git clone <your-repo-url>

2️⃣ Open with IntelliJ IDEA or Eclipse

Import as Maven Project

3️⃣ Install dependencies

Maven will automatically download required libraries.

4️⃣ Run tests

Run directly from:

SwagTests.java → Run

or via Maven:

mvn test

---

🔧 Configuration Notes

- Browser driver is managed automatically via Selenium Manager
- Implicit wait is configured in BaseTest
- Browser window is maximized by default
- Test data is currently embedded and can be externalized later

---

📈 Possible Enhancements

- Data-Driven testing (Excel / JSON / CSV)
- PageFactory implementation
- Explicit waits utility layer
- Logging support
- Allure or Extent reporting
- CI/CD pipeline integration
- Cross-browser execution
- Environment configuration files

