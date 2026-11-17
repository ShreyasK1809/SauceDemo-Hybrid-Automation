# 🛒 E-Commerce Hybrid Test Automation Framework

An enterprise-grade, robust Hybrid Test Automation Framework built from scratch to automate both **UI workflows** (Selenium WebDriver with Java) and **REST API endpoints** (REST Assured). Designed with scalability, parallel execution, and detailed reporting in mind.

---

## 🚀 Tech Stack & Tools

* **Programming Language:** Java (JDK 17)
* **UI Automation:** Selenium WebDriver 4
* **API Automation:** REST Assured
* **Test Runner & Build Tool:** TestNG, Maven
* **Design Patterns:** Page Object Model (POM) with Page Factory & `ThreadLocal` WebDriver
* **Data-Driven Testing:** Apache POI (Excel) & Properties files
* **Logging & Reporting:** ExtentReports, Log4j2, Automated Failure Screenshots
* **Version Control & CI/CD:** Git, GitHub Actions, Maven Surefire Plugin

---

## 📁 Project Architecture

```text
SauceDemo-Hybrid-Automation/
│
├── src/
│   ├── main/java/com/ecommerce/
│   │   ├── base/          # WebDriver initialization & configurations (ThreadLocal)
│   │   ├── pages/         # Page Object Model (POM) classes & element locators
│   │   ├── endpoints/     # API endpoints & payload specifications
│   │   └── utils/         # Config readers, Excel utilities, ExtentManager
│   │
│   └── test/java/com/ecommerce/
│       ├── tests/         # TestNG test scripts (UI E2E & API validation)
│       └── listeners/     # Custom ITestListeners for reporting & screenshots
│
├── src/main/resources/    # config.properties
├── src/test/resources/    # testng suites & log4j2 configs
├── reports/               # Generated ExtentReports & failure screenshots
└── pom.xml                # Maven dependencies & build configurations