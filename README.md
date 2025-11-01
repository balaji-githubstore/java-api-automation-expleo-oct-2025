# 📘 Expleo Solutions API Automation Training - Oct 2025

This repository group is part of the **API Automation Training** using **RestAssured**, **Cucumber**, and **OpenAPI Specification**.

---

## 📂 Repositories Overview

### 🔹 Java API Using restassured.io
**Repository:** [java-api-automation-expleo-oct-2025](https://github.com/balaji-githubstore/java-api-automation-expleo-oct-2025.git)

#### 🧠 Key Topics Covered
- Implementation of REST API methods – **GET**, **POST**, **PUT**, **DELETE**
- Working with **JSON**, `secret.json`, and **OpenAPI Specification**
- Handling **JsonPath**, **JsonNode**, **POJO classes**, and `List<PojoClass>`
- Complete API automation with **OpenAPI Spec validation** in simple `@Test` methods

📁 **Session Details Folder:**  
`Allsessionnotes` – contains `.txt` files with day-wise training notes.

---

## 🧪 Framework 1: Java BDD Framework For API Automation
**Repository:** [java-api-bdd-expleo-oct-2025](https://github.com/balaji-githubstore/java-api-bdd-expleo-oct-2025.git)

### 🔀 Branches
| Branch | Description |
|--------|--------------|
| `master` | ✅ Final Capstone Project – Full BDD implementation completed during the session |

---

### 🧩 Framework Structure

#### 📁 `src/main/java`
| Package | Description |
|----------|--------------|
| `com.expleo.config` | Handles `ConfigReader`, `TokenReader` |
| `com.expleo.helpers` | `GitHubAPIHelper` – Executes actual HTTP method calls and returns responses |
| `com.expleo.model` | Contains POJO classes |
| `com.expleo.utils` | Includes `GitRequestSpecBuilder`, `OpenAPIValidator` – Builds request bodies and validates API specifications |

#### 📁 `src/test/java`
| Package | Description |
|----------|--------------|
| `com.expleo.context` | Manages dependency injection |
| `com.expleo.hooks` | Setup and teardown methods (before/after scenarios) and reporting |
| `com.expleo.runner` | `RunnerTest` with `CucumberOptions` and `TestNG` integration |
| `com.expleo.steps` | Step Definitions for feature files |

#### 📁 `src/test/resources`
| Folder | Description |
|---------|--------------|
| `features/` | Contains `.feature` files |
| `schema/` | Contains `OpenAPISpec.yaml` |
| `config.properties` | Configuration file |
| `secret.json` | Sensitive credentials *(must be added to `.gitignore`)* |

---

### ⚙️ Order of Execution
- Feature File → Step Definition → GitAPIHelper (uses GitRequestSpecBuilder, ConfigReader, TokenReader, OpenAPIValidator) --> Response

## 👤 Author

**Balaji Dinakaran**  
🔗 GitHub: [balaji-githubstore](https://github.com/balaji-githubstore)
---
